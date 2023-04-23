# Comparing `tmp/alacorder-79.6.9.tar.gz` & `tmp/alacorder-79.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.6.9.tar", max compression
+gzip compressed data, was "alacorder-79.7.0.tar", max compression
```

## Comparing `alacorder-79.6.9.tar` & `alacorder-79.7.0.tar`

### file list

```diff
@@ -1,2043 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.6.9/LICENSE
--rw-r--r--   0        0        0     9378 2023-04-22 21:04:19.345850 alacorder-79.6.9/README.md
--rw-r--r--   0        0        0      679 2023-04-23 13:49:50.662831 alacorder-79.6.9/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-23 13:50:59.906700 alacorder-79.6.9/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.6.9/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
--rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0       34 2023-03-05 14:00:04.569426 alacorder-79.6.9/src/alacorder/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-03-05 14:01:12.571838 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     1644 2023-03-05 13:59:58.452012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/__init__.data.json
--rw-r--r--   0        0        0     1634 2023-03-05 13:59:58.452197 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/__init__.meta.json
--rw-r--r--   0        0        0     5613 2023-03-05 13:59:58.280947 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/autocall.data.json
--rw-r--r--   0        0        0     1646 2023-03-05 13:59:58.281136 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/autocall.meta.json
--rw-r--r--   0        0        0     8457 2023-03-05 13:59:59.353879 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/compilerop.data.json
--rw-r--r--   0        0        0     1963 2023-03-05 13:59:59.354124 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/compilerop.meta.json
--rw-r--r--   0        0        0     5511 2023-03-05 13:59:58.279859 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/error.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.280044 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/error.meta.json
--rw-r--r--   0        0        0     7827 2023-03-05 13:59:58.278917 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/events.data.json
--rw-r--r--   0        0        0     1679 2023-03-05 13:59:58.279120 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/events.meta.json
--rw-r--r--   0        0        0     2130 2023-03-05 13:59:59.301267 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/excolors.data.json
--rw-r--r--   0        0        0     1717 2023-03-05 13:59:59.301455 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/excolors.meta.json
--rw-r--r--   0        0        0   125581 2023-03-05 13:59:59.283375 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.data.json
--rw-r--r--   0        0        0     2044 2023-03-05 13:59:59.283667 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/guarded_eval.meta.json
--rw-r--r--   0        0        0    40463 2023-03-05 13:59:59.351233 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.data.json
--rw-r--r--   0        0        0     1899 2023-03-05 13:59:59.351509 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/inputtransformer2.meta.json
--rw-r--r--   0        0        0     2147 2023-03-05 13:59:58.056608 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 13:59:58.056811 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/latex_symbols.meta.json
--rw-r--r--   0        0        0     8873 2023-03-05 13:59:59.001609 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/logger.data.json
--rw-r--r--   0        0        0     1857 2023-03-05 13:59:59.001806 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/logger.meta.json
--rw-r--r--   0        0        0     4153 2023-03-05 14:00:01.011324 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/macro.data.json
--rw-r--r--   0        0        0     1829 2023-03-05 14:00:01.011519 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/macro.meta.json
--rw-r--r--   0        0        0    18119 2023-03-05 14:00:02.229094 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.data.json
--rw-r--r--   0        0        0     2048 2023-03-05 14:00:02.229315 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/magic_arguments.meta.json
--rw-r--r--   0        0        0     5662 2023-03-05 13:59:58.454597 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/release.data.json
--rw-r--r--   0        0        0     1709 2023-03-05 13:59:58.454783 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/release.meta.json
--rw-r--r--   0        0        0     6331 2023-03-05 14:00:01.095908 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/splitinput.data.json
--rw-r--r--   0        0        0     1836 2023-03-05 14:00:01.096145 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/splitinput.meta.json
--rw-r--r--   0        0        0     3171 2023-03-05 13:59:58.998590 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/usage.data.json
--rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.998775 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/core/usage.meta.json
--rw-r--r--   0        0        0     1692 2023-03-05 13:59:58.039131 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.data.json
--rw-r--r--   0        0        0     1647 2023-03-05 13:59:58.039362 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/extensions/__init__.meta.json
--rw-r--r--   0        0        0     2227 2023-03-05 13:59:57.904855 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/__init__.data.json
--rw-r--r--   0        0        0     1643 2023-03-05 13:59:57.905037 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/__init__.meta.json
--rw-r--r--   0        0        0     6086 2023-03-05 13:59:59.519735 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/qt_for_kernel.data.json
--rw-r--r--   0        0        0     1796 2023-03-05 13:59:59.519930 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/qt_for_kernel.meta.json
--rw-r--r--   0        0        0    10006 2023-03-05 13:59:59.195867 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/qt_loaders.data.json
--rw-r--r--   0        0        0     2009 2023-03-05 13:59:59.196114 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/external/qt_loaders.meta.json
--rw-r--r--   0        0        0     1636 2023-03-05 13:59:58.442799 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/lib/__init__.data.json
--rw-r--r--   0        0        0     1634 2023-03-05 13:59:58.443014 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/lib/__init__.meta.json
--rw-r--r--   0        0        0    47979 2023-03-05 14:00:01.117977 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/lib/pretty.data.json
--rw-r--r--   0        0        0     2116 2023-03-05 14:00:01.118304 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/lib/pretty.meta.json
--rw-r--r--   0        0        0     1676 2023-03-05 13:59:58.282327 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.data.json
--rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.282506 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/__init__.meta.json
--rw-r--r--   0        0        0     5569 2023-03-05 13:59:59.557973 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.data.json
--rw-r--r--   0        0        0     1928 2023-03-05 13:59:59.558174 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/pt_inputhooks/__init__.meta.json
--rw-r--r--   0        0        0    12623 2023-03-05 14:00:03.783050 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.data.json
--rw-r--r--   0        0        0     2034 2023-03-05 14:00:03.783307 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/terminal/shortcuts/auto_match.meta.json
--rw-r--r--   0        0        0     2023 2023-03-05 13:59:58.245326 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/testing/__init__.data.json
--rw-r--r--   0        0        0     1749 2023-03-05 13:59:58.245538 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/testing/__init__.meta.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.449292 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.data.json
--rw-r--r--   0        0        0     1657 2023-03-05 13:59:58.449470 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/testing/skipdoctest.meta.json
--rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.274389 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/__init__.data.json
--rw-r--r--   0        0        0     1636 2023-03-05 13:59:58.274607 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/__init__.meta.json
--rw-r--r--   0        0        0     3591 2023-03-05 14:00:01.093912 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.data.json
--rw-r--r--   0        0        0     1941 2023-03-05 14:00:01.094186 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_common.meta.json
--rw-r--r--   0        0        0     7627 2023-03-05 14:00:01.659307 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.data.json
--rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.659569 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_process_posix.meta.json
--rw-r--r--   0        0        0     1683 2023-03-05 13:59:58.258635 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.data.json
--rw-r--r--   0        0        0     1646 2023-03-05 13:59:58.258823 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/_sysinfo.meta.json
--rw-r--r--   0        0        0    18814 2023-03-05 13:59:58.891307 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.data.json
--rw-r--r--   0        0        0     1762 2023-03-05 13:59:58.891503 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/coloransi.meta.json
--rw-r--r--   0        0        0     4317 2023-03-05 13:59:59.237241 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/contexts.data.json
--rw-r--r--   0        0        0     1667 2023-03-05 13:59:59.237463 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/contexts.meta.json
--rw-r--r--   0        0        0     1918 2023-03-05 13:59:58.066456 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/data.data.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.066648 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/data.meta.json
--rw-r--r--   0        0        0     3135 2023-03-05 13:59:58.997683 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/decorators.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 13:59:58.997882 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/decorators.meta.json
--rw-r--r--   0        0        0     2353 2023-03-05 13:59:59.556053 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/dir2.data.json
--rw-r--r--   0        0        0     1808 2023-03-05 13:59:59.556242 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/dir2.meta.json
--rw-r--r--   0        0        0     1766 2023-03-05 13:59:58.057380 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/docs.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 13:59:58.057560 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/docs.meta.json
--rw-r--r--   0        0        0     2580 2023-03-05 13:59:59.838183 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/encoding.data.json
--rw-r--r--   0        0        0     1770 2023-03-05 13:59:59.838424 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/encoding.meta.json
--rw-r--r--   0        0        0     2582 2023-03-05 13:59:58.453145 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/frame.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.453326 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/frame.meta.json
--rw-r--r--   0        0        0     4323 2023-03-05 13:59:58.881791 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/generics.data.json
--rw-r--r--   0        0        0     1717 2023-03-05 13:59:58.881975 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/generics.meta.json
--rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.073593 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/importstring.data.json
--rw-r--r--   0        0        0     1692 2023-03-05 13:59:58.073833 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/importstring.meta.json
--rw-r--r--   0        0        0     6937 2023-03-05 13:59:58.277130 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.data.json
--rw-r--r--   0        0        0     1734 2023-03-05 13:59:58.277347 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/ipstruct.meta.json
--rw-r--r--   0        0        0     1898 2023-03-05 13:59:57.949808 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.data.json
--rw-r--r--   0        0        0     1747 2023-03-05 13:59:57.950029 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/module_paths.meta.json
--rw-r--r--   0        0        0     3830 2023-03-05 14:00:01.009760 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/openpy.data.json
--rw-r--r--   0        0        0     1955 2023-03-05 14:00:01.009961 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/openpy.meta.json
--rw-r--r--   0        0        0     8598 2023-03-05 14:00:02.234867 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/path.data.json
--rw-r--r--   0        0        0     2148 2023-03-05 14:00:02.235174 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/path.meta.json
--rw-r--r--   0        0        0     3779 2023-03-05 14:00:01.996773 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/process.data.json
--rw-r--r--   0        0        0     1923 2023-03-05 14:00:01.997030 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/process.meta.json
--rw-r--r--   0        0        0     5466 2023-03-05 14:00:01.068619 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.data.json
--rw-r--r--   0        0        0     1888 2023-03-05 14:00:01.068849 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/py3compat.meta.json
--rw-r--r--   0        0        0     3293 2023-03-05 13:59:58.060565 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.data.json
--rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.060758 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/sentinel.meta.json
--rw-r--r--   0        0        0     3384 2023-03-05 14:00:01.070452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.data.json
--rw-r--r--   0        0        0     2010 2023-03-05 14:00:01.070681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/sysinfo.meta.json
--rw-r--r--   0        0        0     6168 2023-03-05 13:59:59.333192 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:59.333391 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/syspathcontext.meta.json
--rw-r--r--   0        0        0     5308 2023-03-05 13:59:59.300447 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/terminal.data.json
--rw-r--r--   0        0        0     1782 2023-03-05 13:59:59.300650 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/terminal.meta.json
--rw-r--r--   0        0        0    21454 2023-03-05 13:59:58.996542 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/text.data.json
--rw-r--r--   0        0        0     1905 2023-03-05 13:59:58.996788 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/text.meta.json
--rw-r--r--   0        0        0     3340 2023-03-05 13:59:58.685179 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/timing.data.json
--rw-r--r--   0        0        0     1809 2023-03-05 13:59:58.685413 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/timing.meta.json
--rw-r--r--   0        0        0    26574 2023-03-05 13:59:59.225546 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.data.json
--rw-r--r--   0        0        0     1720 2023-03-05 13:59:59.225783 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/tokenutil.meta.json
--rw-r--r--   0        0        0     4244 2023-03-05 13:59:59.786805 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 13:59:59.787065 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/IPython/utils/wildcard.meta.json
--rw-r--r--   0        0        0   128047 2023-03-05 14:01:08.842475 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/Image.data.json
--rw-r--r--   0        0        0     1842 2023-03-05 14:01:08.842682 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/Image.meta.json
--rw-r--r--   0        0        0    52687 2023-03-05 14:01:08.839752 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/ImageFilter.data.json
--rw-r--r--   0        0        0     1730 2023-03-05 14:01:08.839940 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/ImageFilter.meta.json
--rw-r--r--   0        0        0    12596 2023-03-05 14:01:08.838475 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/ImagePalette.data.json
--rw-r--r--   0        0        0     1679 2023-03-05 14:01:08.838688 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/ImagePalette.meta.json
--rw-r--r--   0        0        0    27729 2023-03-05 14:01:08.698509 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/PyAccess.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.698765 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/PyAccess.meta.json
--rw-r--r--   0        0        0     2532 2023-03-05 14:01:08.401402 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/__init__.data.json
--rw-r--r--   0        0        0     1624 2023-03-05 14:01:08.401653 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/__init__.meta.json
--rw-r--r--   0        0        0     6092 2023-03-05 14:01:08.373559 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/_imaging.data.json
--rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.373755 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PIL/_imaging.meta.json
--rw-r--r--   0        0        0     3663 2023-03-05 14:00:03.804381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/__init__.data.json
--rw-r--r--   0        0        0     2032 2023-03-05 14:00:03.804640 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/__init__.meta.json
--rw-r--r--   0        0        0    16555 2023-03-05 14:00:01.802605 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_cmap.data.json
--rw-r--r--   0        0        0     2231 2023-03-05 14:00:01.802873 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_cmap.meta.json
--rw-r--r--   0        0        0     7130 2023-03-05 13:59:58.957796 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/__init__.data.json
--rw-r--r--   0        0        0     1893 2023-03-05 13:59:58.958696 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/__init__.meta.json
--rw-r--r--   0        0        0     2406 2023-03-05 13:59:58.217308 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/adobe_glyphs.data.json
--rw-r--r--   0        0        0     1688 2023-03-05 13:59:58.217624 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/adobe_glyphs.meta.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.991244 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/pdfdoc.data.json
--rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.991435 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/pdfdoc.meta.json
--rw-r--r--   0        0        0     1723 2023-03-05 13:59:57.990191 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/std.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.990386 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/std.meta.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.989154 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/symbol.data.json
--rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.989354 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/symbol.meta.json
--rw-r--r--   0        0        0     1778 2023-03-05 13:59:57.987988 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/zapfding.data.json
--rw-r--r--   0        0        0     1650 2023-03-05 13:59:57.988213 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_codecs/zapfding.meta.json
--rw-r--r--   0        0        0    60542 2023-03-05 14:00:01.856527 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_encryption.data.json
--rw-r--r--   0        0        0     2287 2023-03-05 14:00:01.856829 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_encryption.meta.json
--rw-r--r--   0        0        0    47002 2023-03-05 14:00:03.769631 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_merger.data.json
--rw-r--r--   0        0        0     2431 2023-03-05 14:00:03.769906 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_merger.meta.json
--rw-r--r--   0        0        0   111098 2023-03-05 14:00:02.127558 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_page.data.json
--rw-r--r--   0        0        0     2322 2023-03-05 14:00:02.127913 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_page.meta.json
--rw-r--r--   0        0        0    18237 2023-03-05 13:59:59.620861 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_protocols.data.json
--rw-r--r--   0        0        0     1768 2023-03-05 13:59:59.621055 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_protocols.meta.json
--rw-r--r--   0        0        0   129465 2023-03-05 14:00:02.323210 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_reader.data.json
--rw-r--r--   0        0        0     2400 2023-03-05 14:00:02.323471 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_reader.meta.json
--rw-r--r--   0        0        0     8690 2023-03-05 14:00:01.308344 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_security.data.json
--rw-r--r--   0        0        0     1923 2023-03-05 14:01:09.662038 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_security.meta.json
--rw-r--r--   0        0        0    38598 2023-03-05 13:59:59.430266 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_utils.data.json
--rw-r--r--   0        0        0     2002 2023-03-05 13:59:59.430525 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_utils.meta.json
--rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.466457 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_version.data.json
--rw-r--r--   0        0        0     1632 2023-03-05 13:59:58.466689 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_version.meta.json
--rw-r--r--   0        0        0   157017 2023-03-05 14:00:02.554074 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_writer.data.json
--rw-r--r--   0        0        0     2705 2023-03-05 14:00:02.554375 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/_writer.meta.json
--rw-r--r--   0        0        0   110018 2023-03-05 13:59:58.372482 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/constants.data.json
--rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.372747 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/constants.meta.json
--rw-r--r--   0        0        0    10374 2023-03-05 13:59:58.377723 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/errors.data.json
--rw-r--r--   0        0        0     1629 2023-03-05 13:59:58.377918 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/errors.meta.json
--rw-r--r--   0        0        0    40327 2023-03-05 14:00:01.311286 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/filters.data.json
--rw-r--r--   0        0        0     2137 2023-03-05 14:01:09.664119 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/filters.meta.json
--rw-r--r--   0        0        0    10470 2023-03-05 14:00:01.307705 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/__init__.data.json
--rw-r--r--   0        0        0     2012 2023-03-05 14:01:09.661585 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/__init__.meta.json
--rw-r--r--   0        0        0    17626 2023-03-05 14:00:01.306627 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_annotations.data.json
--rw-r--r--   0        0        0     2033 2023-03-05 14:01:09.660779 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_annotations.meta.json
--rw-r--r--   0        0        0    82838 2023-03-05 14:00:01.300337 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_base.data.json
--rw-r--r--   0        0        0     2076 2023-03-05 14:01:09.655537 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_base.meta.json
--rw-r--r--   0        0        0   137855 2023-03-05 14:00:01.303929 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_data_structures.data.json
--rw-r--r--   0        0        0     2227 2023-03-05 14:01:09.658510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_data_structures.meta.json
--rw-r--r--   0        0        0    17997 2023-03-05 14:00:01.298271 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_fit.data.json
--rw-r--r--   0        0        0     1849 2023-03-05 14:01:09.653675 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_fit.meta.json
--rw-r--r--   0        0        0     6200 2023-03-05 14:00:01.305966 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_outline.data.json
--rw-r--r--   0        0        0     1915 2023-03-05 14:01:09.660232 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_outline.meta.json
--rw-r--r--   0        0        0    67789 2023-03-05 14:00:01.305519 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_rectangle.data.json
--rw-r--r--   0        0        0     1970 2023-03-05 14:01:09.659875 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_rectangle.meta.json
--rw-r--r--   0        0        0     7978 2023-03-05 14:00:01.300868 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_utils.data.json
--rw-r--r--   0        0        0     2000 2023-03-05 14:01:09.655936 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/generic/_utils.meta.json
--rw-r--r--   0        0        0    12082 2023-03-05 13:59:59.060467 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/pagerange.data.json
--rw-r--r--   0        0        0     1786 2023-03-05 13:59:59.060677 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/pagerange.meta.json
--rw-r--r--   0        0        0    28090 2023-03-05 13:59:58.465855 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/papersizes.data.json
--rw-r--r--   0        0        0     1659 2023-03-05 13:59:58.466106 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/papersizes.meta.json
--rw-r--r--   0        0        0     6989 2023-03-05 14:00:01.307091 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/types.data.json
--rw-r--r--   0        0        0     1863 2023-03-05 14:01:09.661130 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/types.meta.json
--rw-r--r--   0        0        0    49070 2023-03-05 14:00:01.309910 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/xmp.data.json
--rw-r--r--   0        0        0     2224 2023-03-05 14:01:09.663164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/PyPDF2/xmp.meta.json
--rw-r--r--   0        0        0     8324 2023-03-05 13:59:58.305693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 13:59:58.305888 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   187134 2023-03-05 13:59:57.831848 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1760 2023-03-05 13:59:57.832039 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    46789 2023-03-05 13:59:57.865471 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_bisect.data.json
--rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.865738 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_bisect.meta.json
--rw-r--r--   0        0        0   118849 2023-03-05 14:01:08.005896 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_cffi_backend/__init__.data.json
--rw-r--r--   0        0        0     1812 2023-03-05 14:01:08.006147 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_cffi_backend/__init__.meta.json
--rw-r--r--   0        0        0    55649 2023-03-05 13:59:57.828560 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1806 2023-03-05 13:59:57.828735 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19484 2023-03-05 13:59:57.827285 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1714 2023-03-05 13:59:57.827448 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    10601 2023-03-05 13:59:58.232432 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_compression.data.json
--rw-r--r--   0        0        0     1769 2023-03-05 13:59:58.232699 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_compression.meta.json
--rw-r--r--   0        0        0     3164 2023-03-05 13:59:57.826656 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1716 2023-03-05 13:59:57.826826 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   229133 2023-03-05 13:59:57.968210 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_curses.data.json
--rw-r--r--   0        0        0     1700 2023-03-05 13:59:57.968444 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_curses.meta.json
--rw-r--r--   0        0        0   179168 2023-03-05 13:59:58.953707 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1760 2023-03-05 13:59:58.954252 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0     7486 2023-03-05 13:59:57.856523 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_heapq.data.json
--rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.856704 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_heapq.meta.json
--rw-r--r--   0        0        0     7846 2023-03-05 14:01:07.967582 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_markupbase.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 14:01:07.967795 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_markupbase.meta.json
--rw-r--r--   0        0        0   118876 2023-03-05 13:59:58.105862 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_operator.data.json
--rw-r--r--   0        0        0     1728 2023-03-05 13:59:58.106095 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_operator.meta.json
--rw-r--r--   0        0        0     6391 2023-03-05 13:59:58.218933 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_random.data.json
--rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.219140 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_random.meta.json
--rw-r--r--   0        0        0    97227 2023-03-05 13:59:58.012662 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_socket.data.json
--rw-r--r--   0        0        0     1790 2023-03-05 13:59:58.012945 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_socket.meta.json
--rw-r--r--   0        0        0    21142 2023-03-05 13:59:58.108166 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_stat.data.json
--rw-r--r--   0        0        0     1677 2023-03-05 13:59:58.108361 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_stat.meta.json
--rw-r--r--   0        0        0    25260 2023-03-05 13:59:58.323974 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1758 2023-03-05 13:59:58.324187 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    24127 2023-03-05 13:59:57.898533 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_tkinter.data.json
--rw-r--r--   0        0        0     1702 2023-03-05 13:59:57.898755 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_tkinter.meta.json
--rw-r--r--   0        0        0    92889 2023-03-05 13:59:57.826277 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1816 2023-03-05 13:59:57.826453 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     5193 2023-03-05 13:59:58.014809 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_typeshed/xml.data.json
--rw-r--r--   0        0        0     1650 2023-03-05 13:59:58.014999 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_typeshed/xml.meta.json
--rw-r--r--   0        0        0    14158 2023-03-05 13:59:58.467877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1643 2023-03-05 13:59:58.468119 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    28348 2023-03-05 13:59:57.999179 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_weakref.data.json
--rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.999473 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_weakref.meta.json
--rw-r--r--   0        0        0    47160 2023-03-05 13:59:57.996138 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_weakrefset.data.json
--rw-r--r--   0        0        0     1720 2023-03-05 13:59:57.996398 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_weakrefset.meta.json
--rw-r--r--   0        0        0  3518265 2023-03-05 14:01:08.336557 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_win32typing/__init__.data.json
--rw-r--r--   0        0        0     1716 2023-03-05 14:01:08.338044 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_win32typing/__init__.meta.json
--rw-r--r--   0        0        0     2474 2023-03-05 13:59:58.018204 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_winapi.data.json
--rw-r--r--   0        0        0     1724 2023-03-05 13:59:58.018402 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/_winapi.meta.json
--rw-r--r--   0        0        0    21701 2023-03-05 13:59:57.824456 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1702 2023-03-05 13:59:57.824620 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0     1603 2023-03-05 13:59:58.496383 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/alacorder/__init__.data.json
--rw-r--r--   0        0        0     1612 2023-03-05 13:59:58.496584 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/alacorder/__init__.meta.json
--rw-r--r--   0        0        0   160642 2023-03-05 13:59:58.089168 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/argparse.data.json
--rw-r--r--   0        0        0     1805 2023-03-05 13:59:58.089405 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/argparse.meta.json
--rw-r--r--   0        0        0    62957 2023-03-05 13:59:57.823739 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1769 2023-03-05 13:59:57.823915 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   143777 2023-03-05 13:59:58.304301 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1824 2023-03-05 13:59:58.304542 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0     2505 2023-03-05 13:59:59.518098 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/__init__.data.json
--rw-r--r--   0        0        0     1742 2023-03-05 14:01:09.924200 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/__init__.meta.json
--rw-r--r--   0        0        0     2629 2023-03-05 13:59:57.867688 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 13:59:57.867994 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/astroid_compat.meta.json
--rw-r--r--   0        0        0    40307 2023-03-05 14:01:09.922135 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/asttokens.data.json
--rw-r--r--   0        0        0     1946 2023-03-05 14:01:09.922417 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/asttokens.meta.json
--rw-r--r--   0        0        0     7295 2023-03-05 13:59:59.117429 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/line_numbers.data.json
--rw-r--r--   0        0        0     1733 2023-03-05 13:59:59.117640 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/line_numbers.meta.json
--rw-r--r--   0        0        0    59837 2023-03-05 14:01:09.923698 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.data.json
--rw-r--r--   0        0        0     1982 2023-03-05 14:01:09.923926 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/mark_tokens.meta.json
--rw-r--r--   0        0        0    64194 2023-03-05 14:01:09.853286 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/util.data.json
--rw-r--r--   0        0        0     1899 2023-03-05 14:01:09.853582 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asttokens/util.meta.json
--rw-r--r--   0        0        0    11557 2023-03-05 14:00:01.723452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2131 2023-03-05 14:00:01.723621 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   106328 2023-03-05 14:00:01.719298 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/base_events.data.json
--rw-r--r--   0        0        0     2078 2023-03-05 14:00:01.719499 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    27410 2023-03-05 13:59:57.972499 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1747 2023-03-05 13:59:57.972738 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   205966 2023-03-05 14:00:01.717080 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/events.data.json
--rw-r--r--   0        0        0     2103 2023-03-05 14:00:01.717296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/events.meta.json
--rw-r--r--   0        0        0     9353 2023-03-05 13:59:57.970739 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 13:59:57.970980 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    35869 2023-03-05 14:00:01.713303 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/futures.data.json
--rw-r--r--   0        0        0     1935 2023-03-05 14:00:01.713480 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/futures.meta.json
--rw-r--r--   0        0        0    28341 2023-03-05 14:00:01.722192 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/locks.data.json
--rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.722368 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/locks.meta.json
--rw-r--r--   0        0        0    17902 2023-03-05 14:00:01.707576 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1839 2023-03-05 14:00:01.707769 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    24473 2023-03-05 14:00:01.721409 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/queues.data.json
--rw-r--r--   0        0        0     1775 2023-03-05 14:00:01.721572 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/queues.meta.json
--rw-r--r--   0        0        0     4869 2023-03-05 14:00:01.720687 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/runners.data.json
--rw-r--r--   0        0        0     1834 2023-03-05 14:00:01.720854 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4031 2023-03-05 14:00:01.706839 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1813 2023-03-05 14:00:01.707081 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36391 2023-03-05 14:00:01.720269 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/streams.data.json
--rw-r--r--   0        0        0     1932 2023-03-05 14:00:01.720454 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/streams.meta.json
--rw-r--r--   0        0        0    25574 2023-03-05 14:00:01.722958 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1955 2023-03-05 14:00:01.723127 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0   107924 2023-03-05 14:00:01.712343 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1936 2023-03-05 14:00:01.712535 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6038 2023-03-05 13:59:57.969160 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/threads.data.json
--rw-r--r--   0        0        0     1706 2023-03-05 13:59:57.969408 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/threads.meta.json
--rw-r--r--   0        0        0    28479 2023-03-05 14:00:01.710003 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/transports.data.json
--rw-r--r--   0        0        0     1802 2023-03-05 14:00:01.710201 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59557 2023-03-05 14:00:01.709114 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.709322 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0     8751 2023-03-05 13:59:58.283327 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/atexit.data.json
--rw-r--r--   0        0        0     1688 2023-03-05 13:59:58.283513 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/atexit.meta.json
--rw-r--r--   0        0        0    17174 2023-03-05 13:59:58.457152 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/base64.data.json
--rw-r--r--   0        0        0     1735 2023-03-05 13:59:58.457346 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/base64.meta.json
--rw-r--r--   0        0        0    52029 2023-03-05 13:59:58.273786 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/bdb.data.json
--rw-r--r--   0        0        0     1731 2023-03-05 13:59:58.274025 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/bdb.meta.json
--rw-r--r--   0        0        0    14694 2023-03-05 13:59:58.451493 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/binascii.data.json
--rw-r--r--   0        0        0     1782 2023-03-05 13:59:58.451703 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/binascii.meta.json
--rw-r--r--   0        0        0    12190 2023-03-05 13:59:58.599840 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/bisect.data.json
--rw-r--r--   0        0        0     1673 2023-03-05 13:59:58.600034 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/bisect.meta.json
--rw-r--r--   0        0        0  1077780 2023-03-05 13:59:57.851144 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1866 2023-03-05 13:59:57.851427 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0    20683 2023-03-05 13:59:58.047211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cProfile.data.json
--rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.047411 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cProfile.meta.json
--rw-r--r--   0        0        0     2485 2023-03-05 13:59:59.304339 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/certifi/__init__.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 13:59:59.304521 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/certifi/__init__.meta.json
--rw-r--r--   0        0        0     3446 2023-03-05 13:59:58.850059 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/certifi/core.data.json
--rw-r--r--   0        0        0     1829 2023-03-05 13:59:58.850253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/certifi/core.meta.json
--rw-r--r--   0        0        0     2991 2023-03-05 14:01:08.767965 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/__init__.data.json
--rw-r--r--   0        0        0     1665 2023-03-05 14:01:08.768157 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/__init__.meta.json
--rw-r--r--   0        0        0    56091 2023-03-05 14:01:08.631782 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/api.data.json
--rw-r--r--   0        0        0     1891 2023-03-05 14:01:08.632022 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/api.meta.json
--rw-r--r--   0        0        0     6206 2023-03-05 14:01:08.015940 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/error.data.json
--rw-r--r--   0        0        0     1630 2023-03-05 14:01:08.016136 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cffi/error.meta.json
--rw-r--r--   0        0        0     8347 2023-03-05 14:00:01.655804 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/__init__.data.json
--rw-r--r--   0        0        0     1887 2023-03-05 14:00:01.656014 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/__init__.meta.json
--rw-r--r--   0        0        0    49662 2023-03-05 14:00:01.032459 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_compat.data.json
--rw-r--r--   0        0        0     1993 2023-03-05 14:00:01.032731 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_compat.meta.json
--rw-r--r--   0        0        0    47515 2023-03-05 14:00:01.642919 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2248 2023-03-05 14:00:01.643116 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5636 2023-03-05 13:59:59.014629 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_textwrap.data.json
--rw-r--r--   0        0        0     1721 2023-03-05 13:59:59.014833 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/_textwrap.meta.json
--rw-r--r--   0        0        0   191965 2023-03-05 14:00:01.652441 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/core.data.json
--rw-r--r--   0        0        0     2284 2023-03-05 14:00:01.652858 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/core.meta.json
--rw-r--r--   0        0        0    60810 2023-03-05 14:00:01.655239 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/decorators.data.json
--rw-r--r--   0        0        0     1974 2023-03-05 14:00:01.655469 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/decorators.meta.json
--rw-r--r--   0        0        0    28813 2023-03-05 14:00:01.641477 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/exceptions.data.json
--rw-r--r--   0        0        0     1888 2023-03-05 14:00:01.641759 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/exceptions.meta.json
--rw-r--r--   0        0        0    18459 2023-03-05 14:00:01.644756 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/formatting.data.json
--rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.645100 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/formatting.meta.json
--rw-r--r--   0        0        0     7446 2023-03-05 14:00:01.639200 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/globals.data.json
--rw-r--r--   0        0        0     1747 2023-03-05 14:00:01.639500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/globals.meta.json
--rw-r--r--   0        0        0    30316 2023-03-05 14:00:01.643880 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/parser.data.json
--rw-r--r--   0        0        0     1920 2023-03-05 14:00:01.644179 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/parser.meta.json
--rw-r--r--   0        0        0    35390 2023-03-05 14:00:01.653759 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/shell_completion.data.json
--rw-r--r--   0        0        0     1979 2023-03-05 14:00:01.654004 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24909 2023-03-05 14:00:01.648012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/termui.data.json
--rw-r--r--   0        0        0     2111 2023-03-05 14:00:01.648211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/termui.meta.json
--rw-r--r--   0        0        0    85218 2023-03-05 14:00:01.647045 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/types.data.json
--rw-r--r--   0        0        0     2133 2023-03-05 14:00:01.647300 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/types.meta.json
--rw-r--r--   0        0        0    33709 2023-03-05 14:00:01.640325 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/utils.data.json
--rw-r--r--   0        0        0     2054 2023-03-05 14:00:01.640513 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/click/utils.meta.json
--rw-r--r--   0        0        0    21484 2023-03-05 13:59:58.017388 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cmd.data.json
--rw-r--r--   0        0        0     1683 2023-03-05 13:59:58.017586 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cmd.meta.json
--rw-r--r--   0        0        0   126779 2023-03-05 13:59:57.822325 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1806 2023-03-05 13:59:57.822511 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0     6009 2023-03-05 13:59:58.068498 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/codeop.data.json
--rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.068675 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/codeop.meta.json
--rw-r--r--   0        0        0   390732 2023-03-05 13:59:57.819770 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1784 2023-03-05 13:59:57.819976 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4026 2023-03-05 13:59:57.813207 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 13:59:57.813377 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0     2641 2023-03-05 14:01:08.704569 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/__init__.data.json
--rw-r--r--   0        0        0     1717 2023-03-05 14:01:08.704770 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/__init__.meta.json
--rw-r--r--   0        0        0    22050 2023-03-05 14:01:08.369752 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/ansi.data.json
--rw-r--r--   0        0        0     1637 2023-03-05 14:01:08.369975 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/ansi.meta.json
--rw-r--r--   0        0        0    24189 2023-03-05 14:01:08.367447 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/ansitowin32.data.json
--rw-r--r--   0        0        0     1762 2023-03-05 14:01:08.367673 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/ansitowin32.meta.json
--rw-r--r--   0        0        0     9594 2023-03-05 14:01:08.523769 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/initialise.data.json
--rw-r--r--   0        0        0     1697 2023-03-05 14:01:08.524034 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorama/initialise.meta.json
--rw-r--r--   0        0        0     8039 2023-03-05 13:59:57.901639 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorsys.data.json
--rw-r--r--   0        0        0     1641 2023-03-05 13:59:57.901828 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/colorsys.meta.json
--rw-r--r--   0        0        0     1649 2023-03-05 13:59:58.025966 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1652 2023-03-05 13:59:58.026146 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4856 2023-03-05 14:00:01.090824 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1860 2023-03-05 14:00:01.091018 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    63653 2023-03-05 13:59:59.171016 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1810 2023-03-05 13:59:59.171238 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    63512 2023-03-05 14:00:00.941072 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     2103 2023-03-05 14:00:00.941334 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    23356 2023-03-05 13:59:59.528953 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1904 2023-03-05 13:59:59.529163 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   127713 2023-03-05 13:59:57.986595 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/configparser.data.json
--rw-r--r--   0        0        0     1760 2023-03-05 13:59:57.986858 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/configparser.meta.json
--rw-r--r--   0        0        0   110453 2023-03-05 13:59:57.812787 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1744 2023-03-05 13:59:57.812965 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    40461 2023-03-05 13:59:57.924454 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/contextvars.data.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:57.924673 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/contextvars.meta.json
--rw-r--r--   0        0        0     5806 2023-03-05 13:59:58.443774 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1632 2023-03-05 13:59:58.443952 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    12928 2023-03-05 13:59:57.858215 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/copyreg.data.json
--rw-r--r--   0        0        0     1710 2023-03-05 13:59:57.858433 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/copyreg.meta.json
--rw-r--r--   0        0        0     2610 2023-03-05 14:01:08.012745 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/__about__.data.json
--rw-r--r--   0        0        0     1647 2023-03-05 14:01:08.012971 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/__about__.meta.json
--rw-r--r--   0        0        0     2805 2023-03-05 14:01:08.861411 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/__init__.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 14:01:08.861596 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/__init__.meta.json
--rw-r--r--   0        0        0    16928 2023-03-05 14:01:09.048476 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/exceptions.data.json
--rw-r--r--   0        0        0     1889 2023-03-05 14:01:09.048685 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/exceptions.meta.json
--rw-r--r--   0        0        0     1700 2023-03-05 14:01:08.018727 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/__init__.data.json
--rw-r--r--   0        0        0     1650 2023-03-05 14:01:08.018942 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/__init__.meta.json
--rw-r--r--   0        0        0    45913 2023-03-05 14:01:09.434895 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/_oid.data.json
--rw-r--r--   0        0        0     1827 2023-03-05 14:01:09.435068 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/_oid.meta.json
--rw-r--r--   0        0        0     2542 2023-03-05 14:01:09.682929 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/__init__.data.json
--rw-r--r--   0        0        0     1769 2023-03-05 14:01:09.683155 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/__init__.meta.json
--rw-r--r--   0        0        0     2430 2023-03-05 14:01:09.473490 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/__init__.data.json
--rw-r--r--   0        0        0     1738 2023-03-05 14:01:09.473662 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/__init__.meta.json
--rw-r--r--   0        0        0    10998 2023-03-05 14:01:09.426640 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/aead.data.json
--rw-r--r--   0        0        0     2190 2023-03-05 14:01:09.426835 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/aead.meta.json
--rw-r--r--   0        0        0   163732 2023-03-05 14:01:09.472136 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/backend.data.json
--rw-r--r--   0        0        0     4610 2023-03-05 14:01:09.472354 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/backend.meta.json
--rw-r--r--   0        0        0    13025 2023-03-05 14:01:09.433928 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ciphers.data.json
--rw-r--r--   0        0        0     2359 2023-03-05 14:01:09.434131 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ciphers.meta.json
--rw-r--r--   0        0        0     8676 2023-03-05 14:01:09.433360 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/cmac.data.json
--rw-r--r--   0        0        0     2221 2023-03-05 14:01:09.433539 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/cmac.meta.json
--rw-r--r--   0        0        0    26433 2023-03-05 14:01:09.467844 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dh.data.json
--rw-r--r--   0        0        0     2232 2023-03-05 14:01:09.468029 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dh.meta.json
--rw-r--r--   0        0        0    25205 2023-03-05 14:01:09.467073 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dsa.data.json
--rw-r--r--   0        0        0     2382 2023-03-05 14:01:09.467260 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/dsa.meta.json
--rw-r--r--   0        0        0    29434 2023-03-05 14:01:09.466334 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ec.data.json
--rw-r--r--   0        0        0     2416 2023-03-05 14:01:09.466518 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ec.meta.json
--rw-r--r--   0        0        0    13578 2023-03-05 14:01:09.465534 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed25519.data.json
--rw-r--r--   0        0        0     2269 2023-03-05 14:01:09.465717 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed25519.meta.json
--rw-r--r--   0        0        0    13642 2023-03-05 14:01:09.465001 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed448.data.json
--rw-r--r--   0        0        0     2263 2023-03-05 14:01:09.465178 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/ed448.meta.json
--rw-r--r--   0        0        0    12027 2023-03-05 14:01:09.432903 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hashes.data.json
--rw-r--r--   0        0        0     2069 2023-03-05 14:01:09.433073 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hashes.meta.json
--rw-r--r--   0        0        0     9895 2023-03-05 14:01:09.432374 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hmac.data.json
--rw-r--r--   0        0        0     2107 2023-03-05 14:01:09.432565 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/hmac.meta.json
--rw-r--r--   0        0        0     7706 2023-03-05 14:01:09.425411 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/poly1305.data.json
--rw-r--r--   0        0        0     2020 2023-03-05 14:01:09.425731 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/poly1305.meta.json
--rw-r--r--   0        0        0    35099 2023-03-05 14:01:09.464445 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/rsa.data.json
--rw-r--r--   0        0        0     2532 2023-03-05 14:01:09.464635 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/rsa.meta.json
--rw-r--r--   0        0        0     4200 2023-03-05 14:01:09.436999 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/utils.data.json
--rw-r--r--   0        0        0     2099 2023-03-05 14:01:09.437167 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/utils.meta.json
--rw-r--r--   0        0        0    12785 2023-03-05 14:01:09.463484 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x25519.data.json
--rw-r--r--   0        0        0     2261 2023-03-05 14:01:09.463712 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x25519.meta.json
--rw-r--r--   0        0        0    12595 2023-03-05 14:01:09.462851 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x448.data.json
--rw-r--r--   0        0        0     2255 2023-03-05 14:01:09.463087 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/backends/openssl/x448.meta.json
--rw-r--r--   0        0        0     1772 2023-03-05 14:01:07.983955 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/__init__.data.json
--rw-r--r--   0        0        0     1668 2023-03-05 14:01:07.984140 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/__init__.meta.json
--rw-r--r--   0        0        0     2336 2023-03-05 14:01:07.976714 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_openssl.data.json
--rw-r--r--   0        0        0     1678 2023-03-05 14:01:07.976898 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_openssl.meta.json
--rw-r--r--   0        0        0    15743 2023-03-05 14:01:08.010886 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/__init__.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.011125 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/__init__.meta.json
--rw-r--r--   0        0        0     6792 2023-03-05 14:01:08.011981 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/asn1.data.json
--rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.012177 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/asn1.meta.json
--rw-r--r--   0        0        0    15180 2023-03-05 14:01:09.450682 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/x509.data.json
--rw-r--r--   0        0        0     2513 2023-03-05 14:01:09.450863 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/_rust/x509.meta.json
--rw-r--r--   0        0        0     1836 2023-03-05 14:01:08.009047 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/__init__.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.009237 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/__init__.meta.json
--rw-r--r--   0        0        0    34261 2023-03-05 14:01:07.983431 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/_conditional.data.json
--rw-r--r--   0        0        0     1703 2023-03-05 14:01:07.983638 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/_conditional.meta.json
--rw-r--r--   0        0        0    38528 2023-03-05 14:01:09.049547 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/binding.data.json
--rw-r--r--   0        0        0     1943 2023-03-05 14:01:09.049734 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/bindings/openssl/binding.meta.json
--rw-r--r--   0        0        0     1788 2023-03-05 14:01:08.019263 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/__init__.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.019449 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/__init__.meta.json
--rw-r--r--   0        0        0     3985 2023-03-05 14:01:08.018142 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_asymmetric.data.json
--rw-r--r--   0        0        0     1687 2023-03-05 14:01:08.018381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_asymmetric.meta.json
--rw-r--r--   0        0        0     9970 2023-03-05 14:01:08.007693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_cipheralgorithm.data.json
--rw-r--r--   0        0        0     1698 2023-03-05 14:01:08.007885 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_cipheralgorithm.meta.json
--rw-r--r--   0        0        0    31769 2023-03-05 14:01:09.435707 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_serialization.data.json
--rw-r--r--   0        0        0     1937 2023-03-05 14:01:09.435887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/_serialization.meta.json
--rw-r--r--   0        0        0     1876 2023-03-05 14:01:08.019767 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/__init__.data.json
--rw-r--r--   0        0        0     1694 2023-03-05 14:01:08.019945 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/__init__.meta.json
--rw-r--r--   0        0        0    50380 2023-03-05 14:01:09.441628 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dh.data.json
--rw-r--r--   0        0        0     2104 2023-03-05 14:01:09.441805 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dh.meta.json
--rw-r--r--   0        0        0    54550 2023-03-05 14:01:09.440514 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dsa.data.json
--rw-r--r--   0        0        0     2267 2023-03-05 14:01:09.440708 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/dsa.meta.json
--rw-r--r--   0        0        0    99258 2023-03-05 14:01:09.444652 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ec.data.json
--rw-r--r--   0        0        0     2432 2023-03-05 14:01:09.444840 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ec.meta.json
--rw-r--r--   0        0        0    18398 2023-03-05 14:01:09.439356 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed25519.data.json
--rw-r--r--   0        0        0     2018 2023-03-05 14:01:09.439535 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed25519.meta.json
--rw-r--r--   0        0        0    17574 2023-03-05 14:01:09.438742 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed448.data.json
--rw-r--r--   0        0        0     2014 2023-03-05 14:01:09.438924 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/ed448.meta.json
--rw-r--r--   0        0        0    16939 2023-03-05 14:01:09.445678 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/padding.data.json
--rw-r--r--   0        0        0     2083 2023-03-05 14:01:09.445856 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/padding.meta.json
--rw-r--r--   0        0        0    57861 2023-03-05 14:01:09.442865 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/rsa.data.json
--rw-r--r--   0        0        0     2338 2023-03-05 14:01:09.443052 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/rsa.meta.json
--rw-r--r--   0        0        0     6470 2023-03-05 14:01:09.445076 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/types.data.json
--rw-r--r--   0        0        0     2206 2023-03-05 14:01:09.445256 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/types.meta.json
--rw-r--r--   0        0        0     7015 2023-03-05 14:01:09.436195 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/utils.data.json
--rw-r--r--   0        0        0     1936 2023-03-05 14:01:09.436389 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/utils.meta.json
--rw-r--r--   0        0        0    16229 2023-03-05 14:01:09.438144 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x25519.data.json
--rw-r--r--   0        0        0     2016 2023-03-05 14:01:09.438319 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x25519.meta.json
--rw-r--r--   0        0        0    15999 2023-03-05 14:01:09.437571 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x448.data.json
--rw-r--r--   0        0        0     2012 2023-03-05 14:01:09.437751 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/asymmetric/x448.meta.json
--rw-r--r--   0        0        0     3339 2023-03-05 14:01:09.429469 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/__init__.data.json
--rw-r--r--   0        0        0     1799 2023-03-05 14:01:09.429656 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/__init__.meta.json
--rw-r--r--   0        0        0    34892 2023-03-05 14:01:09.473106 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/aead.data.json
--rw-r--r--   0        0        0     2129 2023-03-05 14:01:09.473291 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/aead.meta.json
--rw-r--r--   0        0        0    53114 2023-03-05 14:01:09.430611 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/algorithms.data.json
--rw-r--r--   0        0        0     1888 2023-03-05 14:01:09.430791 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/algorithms.meta.json
--rw-r--r--   0        0        0    45452 2023-03-05 14:01:09.427751 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/base.data.json
--rw-r--r--   0        0        0     2102 2023-03-05 14:01:09.427958 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/base.meta.json
--rw-r--r--   0        0        0    60656 2023-03-05 14:01:09.429052 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/modes.data.json
--rw-r--r--   0        0        0     1978 2023-03-05 14:01:09.429246 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/ciphers/modes.meta.json
--rw-r--r--   0        0        0     2344 2023-03-05 14:01:08.466230 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/constant_time.data.json
--rw-r--r--   0        0        0     1815 2023-03-05 14:01:08.466492 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/constant_time.meta.json
--rw-r--r--   0        0        0    59362 2023-03-05 14:01:09.431847 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/hashes.data.json
--rw-r--r--   0        0        0     2034 2023-03-05 14:01:09.432043 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/hashes.meta.json
--rw-r--r--   0        0        0     5920 2023-03-05 14:01:08.008553 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/__init__.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 14:01:08.008735 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/__init__.meta.json
--rw-r--r--   0        0        0     7520 2023-03-05 14:01:09.426074 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/scrypt.data.json
--rw-r--r--   0        0        0     2086 2023-03-05 14:01:09.426274 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/kdf/scrypt.meta.json
--rw-r--r--   0        0        0     4811 2023-03-05 14:01:09.446551 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/__init__.data.json
--rw-r--r--   0        0        0     1875 2023-03-05 14:01:09.446719 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/__init__.meta.json
--rw-r--r--   0        0        0     7669 2023-03-05 14:01:09.446161 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/base.data.json
--rw-r--r--   0        0        0     2409 2023-03-05 14:01:09.446334 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/base.meta.json
--rw-r--r--   0        0        0    29666 2023-03-05 14:01:09.468662 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs12.data.json
--rw-r--r--   0        0        0     2765 2023-03-05 14:01:09.468851 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs12.meta.json
--rw-r--r--   0        0        0    18012 2023-03-05 14:01:09.469291 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs7.data.json
--rw-r--r--   0        0        0     2355 2023-03-05 14:01:09.469468 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/pkcs7.meta.json
--rw-r--r--   0        0        0    58639 2023-03-05 14:01:09.447876 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/ssh.data.json
--rw-r--r--   0        0        0     2731 2023-03-05 14:01:09.448118 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/hazmat/primitives/serialization/ssh.meta.json
--rw-r--r--   0        0        0    19736 2023-03-05 14:01:08.767315 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/utils.data.json
--rw-r--r--   0        0        0     1818 2023-03-05 14:01:08.767545 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/utils.meta.json
--rw-r--r--   0        0        0    32436 2023-03-05 14:01:09.462242 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/__init__.data.json
--rw-r--r--   0        0        0     2026 2023-03-05 14:01:09.462444 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/__init__.meta.json
--rw-r--r--   0        0        0   155738 2023-03-05 14:01:09.461305 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/base.data.json
--rw-r--r--   0        0        0     2926 2023-03-05 14:01:09.461587 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/base.meta.json
--rw-r--r--   0        0        0    21759 2023-03-05 14:01:09.450030 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/certificate_transparency.data.json
--rw-r--r--   0        0        0     2029 2023-03-05 14:01:09.450245 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/certificate_transparency.meta.json
--rw-r--r--   0        0        0   358332 2023-03-05 14:01:09.458363 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/extensions.data.json
--rw-r--r--   0        0        0     3049 2023-03-05 14:01:09.458636 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/extensions.meta.json
--rw-r--r--   0        0        0    50346 2023-03-05 14:01:09.451859 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/general_name.data.json
--rw-r--r--   0        0        0     2009 2023-03-05 14:01:09.452087 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/general_name.meta.json
--rw-r--r--   0        0        0    54874 2023-03-05 14:01:09.449251 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/name.data.json
--rw-r--r--   0        0        0     2145 2023-03-05 14:01:09.449503 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/name.meta.json
--rw-r--r--   0        0        0     3308 2023-03-05 14:01:09.436614 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/oid.data.json
--rw-r--r--   0        0        0     1679 2023-03-05 14:01:09.436779 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/cryptography/x509/oid.meta.json
--rw-r--r--   0        0        0   135879 2023-03-05 13:59:57.810595 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1812 2023-03-05 13:59:57.810785 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     2191 2023-03-05 13:59:57.871488 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/util.data.json
--rw-r--r--   0        0        0     1661 2023-03-05 13:59:57.871675 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/util.meta.json
--rw-r--r--   0        0        0    58772 2023-03-05 13:59:58.031486 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1700 2023-03-05 13:59:58.031722 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0    38052 2023-03-05 13:59:58.887995 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/curses/__init__.data.json
--rw-r--r--   0        0        0     1728 2023-03-05 13:59:58.888181 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/curses/__init__.meta.json
--rw-r--r--   0        0        0    58283 2023-03-05 13:59:58.223995 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1763 2023-03-05 13:59:58.224228 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   147292 2023-03-05 13:59:59.087765 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 13:59:59.088038 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     1618 2023-03-05 14:01:08.338993 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/__init__.data.json
--rw-r--r--   0        0        0     1633 2023-03-05 14:01:08.339181 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/__init__.meta.json
--rw-r--r--   0        0        0     6101 2023-03-05 14:01:08.017356 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/_common.data.json
--rw-r--r--   0        0        0     1669 2023-03-05 14:01:08.017550 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/_common.meta.json
--rw-r--r--   0        0        0    22099 2023-03-05 14:01:08.814783 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/parser/__init__.data.json
--rw-r--r--   0        0        0     1754 2023-03-05 14:01:08.814989 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/parser/__init__.meta.json
--rw-r--r--   0        0        0     8524 2023-03-05 14:01:08.663906 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/parser/isoparser.data.json
--rw-r--r--   0        0        0     1724 2023-03-05 14:01:08.664101 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/parser/isoparser.meta.json
--rw-r--r--   0        0        0    51946 2023-03-05 14:01:08.636450 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/relativedelta.data.json
--rw-r--r--   0        0        0     1725 2023-03-05 14:01:08.636681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/relativedelta.meta.json
--rw-r--r--   0        0        0     2935 2023-03-05 14:01:08.873446 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/__init__.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.873658 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/__init__.meta.json
--rw-r--r--   0        0        0    13570 2023-03-05 14:01:08.638422 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/_common.data.json
--rw-r--r--   0        0        0     1666 2023-03-05 14:01:08.638663 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/_common.meta.json
--rw-r--r--   0        0        0    51080 2023-03-05 14:01:08.779868 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/tz.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 14:01:08.780089 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dateutil/tz/tz.meta.json
--rw-r--r--   0        0        0     5285 2023-03-05 13:59:59.383634 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1706 2023-03-05 13:59:59.383877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    40509 2023-03-05 14:01:08.819735 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/decorator/__init__.data.json
--rw-r--r--   0        0        0     1753 2023-03-05 14:01:08.819935 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/decorator/__init__.meta.json
--rw-r--r--   0        0        0    62436 2023-03-05 13:59:58.312278 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/difflib.data.json
--rw-r--r--   0        0        0     1713 2023-03-05 13:59:58.312482 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/difflib.meta.json
--rw-r--r--   0        0        0    43155 2023-03-05 13:59:59.064110 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dis.data.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:59.064310 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/dis.meta.json
--rw-r--r--   0        0        0     1641 2023-03-05 14:01:08.006489 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/__init__.data.json
--rw-r--r--   0        0        0     1650 2023-03-05 14:01:08.006668 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/__init__.meta.json
--rw-r--r--   0        0        0    27630 2023-03-05 14:01:07.976084 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/cmd.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 14:01:07.976267 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/cmd.meta.json
--rw-r--r--   0        0        0     7954 2023-03-05 14:01:08.473287 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/core.data.json
--rw-r--r--   0        0        0     1754 2023-03-05 14:01:08.473527 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/core.meta.json
--rw-r--r--   0        0        0    34337 2023-03-05 14:01:07.975204 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/dist.data.json
--rw-r--r--   0        0        0     1733 2023-03-05 14:01:07.975416 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/dist.meta.json
--rw-r--r--   0        0        0    10757 2023-03-05 14:01:07.969464 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/extension.data.json
--rw-r--r--   0        0        0     1664 2023-03-05 14:01:07.969697 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/distutils/extension.meta.json
--rw-r--r--   0        0        0    73895 2023-03-05 13:59:59.526681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/doctest.data.json
--rw-r--r--   0        0        0     1843 2023-03-05 13:59:59.526898 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/doctest.meta.json
--rw-r--r--   0        0        0     8108 2023-03-05 13:59:57.807952 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.808113 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12835 2023-03-05 13:59:57.807504 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1677 2023-03-05 13:59:57.807665 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7695 2023-03-05 13:59:57.806939 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1712 2023-03-05 13:59:57.807109 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25479 2023-03-05 13:59:57.806486 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 13:59:57.806658 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9685 2023-03-05 13:59:57.805802 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.805965 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    62343 2023-03-05 13:59:57.805275 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1834 2023-03-05 13:59:57.805454 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0     1649 2023-03-05 14:01:07.968158 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/__init__.data.json
--rw-r--r--   0        0        0     1652 2023-03-05 14:01:07.968360 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/__init__.meta.json
--rw-r--r--   0        0        0     3908 2023-03-05 14:01:07.992693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/base.data.json
--rw-r--r--   0        0        0     1716 2023-03-05 14:01:07.992881 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/base.meta.json
--rw-r--r--   0        0        0     4592 2023-03-05 14:01:08.472100 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/multipart.data.json
--rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.472323 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/multipart.meta.json
--rw-r--r--   0        0        0     2864 2023-03-05 14:01:08.471177 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/nonmultipart.data.json
--rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.471402 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/nonmultipart.meta.json
--rw-r--r--   0        0        0     3898 2023-03-05 14:01:08.623082 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/text.data.json
--rw-r--r--   0        0        0     1760 2023-03-05 14:01:08.623262 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/mime/text.meta.json
--rw-r--r--   0        0        0    32684 2023-03-05 13:59:57.803873 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1770 2023-03-05 13:59:57.804041 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0    23686 2023-03-05 14:01:08.581687 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/utils.data.json
--rw-r--r--   0        0        0     1765 2023-03-05 14:01:08.581929 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/email/utils.meta.json
--rw-r--r--   0        0        0    64237 2023-03-05 13:59:57.802954 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1733 2023-03-05 13:59:57.803122 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    21224 2023-03-05 13:59:58.357164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/errno.data.json
--rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.357363 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/errno.meta.json
--rw-r--r--   0        0        0    23335 2023-03-05 14:00:00.934100 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/__init__.data.json
--rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.934289 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/__init__.meta.json
--rw-r--r--   0        0        0    84326 2023-03-05 13:59:59.725613 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/executing.data.json
--rw-r--r--   0        0        0     2249 2023-03-05 14:01:10.042287 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/executing.meta.json
--rw-r--r--   0        0        0     1658 2023-03-05 13:59:57.866867 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/version.data.json
--rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.867080 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/executing/version.meta.json
--rw-r--r--   0        0        0     7252 2023-03-05 13:59:58.246579 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/faulthandler.data.json
--rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.246806 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/faulthandler.meta.json
--rw-r--r--   0        0        0     6514 2023-03-05 13:59:57.947111 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/fnmatch.data.json
--rw-r--r--   0        0        0     1663 2023-03-05 13:59:57.947347 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/fnmatch.meta.json
--rw-r--r--   0        0        0    92861 2023-03-05 13:59:59.609574 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/fractions.data.json
--rw-r--r--   0        0        0     1830 2023-03-05 13:59:59.609887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/fractions.meta.json
--rw-r--r--   0        0        0   136168 2023-03-05 13:59:58.354722 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1743 2023-03-05 13:59:58.354955 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    16854 2023-03-05 13:59:58.062662 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gc.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 13:59:58.062847 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gc.meta.json
--rw-r--r--   0        0        0    23876 2023-03-05 13:59:57.801500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1731 2023-03-05 13:59:57.801674 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0     6690 2023-03-05 13:59:58.067502 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/getopt.data.json
--rw-r--r--   0        0        0     1637 2023-03-05 13:59:58.067669 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/getopt.meta.json
--rw-r--r--   0        0        0     3943 2023-03-05 13:59:58.307135 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/getpass.data.json
--rw-r--r--   0        0        0     1638 2023-03-05 13:59:58.307304 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/getpass.meta.json
--rw-r--r--   0        0        0    54812 2023-03-05 13:59:58.346430 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gettext.data.json
--rw-r--r--   0        0        0     1737 2023-03-05 13:59:58.346668 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gettext.meta.json
--rw-r--r--   0        0        0    10067 2023-03-05 13:59:58.495045 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/glob.data.json
--rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.495234 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/glob.meta.json
--rw-r--r--   0        0        0    48617 2023-03-05 13:59:59.048012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gzip.data.json
--rw-r--r--   0        0        0     1821 2023-03-05 13:59:59.048253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/gzip.meta.json
--rw-r--r--   0        0        0    28879 2023-03-05 13:59:58.376289 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/hashlib.data.json
--rw-r--r--   0        0        0     1789 2023-03-05 13:59:58.376552 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/hashlib.meta.json
--rw-r--r--   0        0        0     9621 2023-03-05 13:59:58.584792 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/heapq.data.json
--rw-r--r--   0        0        0     1694 2023-03-05 13:59:58.584989 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/heapq.meta.json
--rw-r--r--   0        0        0    17881 2023-03-05 13:59:58.033717 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/hmac.data.json
--rw-r--r--   0        0        0     1798 2023-03-05 13:59:58.033995 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/hmac.meta.json
--rw-r--r--   0        0        0     4481 2023-03-05 13:59:58.448729 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/__init__.data.json
--rw-r--r--   0        0        0     1641 2023-03-05 13:59:58.448910 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/__init__.meta.json
--rw-r--r--   0        0        0     2943 2023-03-05 13:59:57.883399 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/entities.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 13:59:57.883568 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/entities.meta.json
--rw-r--r--   0        0        0    20592 2023-03-05 14:01:08.470431 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/parser.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.470670 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/html/parser.meta.json
--rw-r--r--   0        0        0    20890 2023-03-05 13:59:58.381953 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/__init__.data.json
--rw-r--r--   0        0        0     1718 2023-03-05 13:59:58.382144 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/__init__.meta.json
--rw-r--r--   0        0        0    69551 2023-03-05 13:59:59.627787 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/client.data.json
--rw-r--r--   0        0        0     1949 2023-03-05 13:59:59.628007 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/client.meta.json
--rw-r--r--   0        0        0    60806 2023-03-05 13:59:59.867388 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/cookiejar.data.json
--rw-r--r--   0        0        0     1847 2023-03-05 13:59:59.867618 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/cookiejar.meta.json
--rw-r--r--   0        0        0    42565 2023-03-05 14:01:07.991829 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/cookies.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 14:01:07.992031 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/cookies.meta.json
--rw-r--r--   0        0        0    38023 2023-03-05 14:01:08.758264 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/server.data.json
--rw-r--r--   0        0        0     1829 2023-03-05 14:01:08.758507 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/http/server.meta.json
--rw-r--r--   0        0        0     6502 2023-03-05 13:59:57.800752 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 13:59:57.800927 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73157 2023-03-05 13:59:57.800308 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1863 2023-03-05 13:59:57.800480 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    68131 2023-03-05 13:59:57.798732 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1874 2023-03-05 13:59:57.798919 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    94672 2023-03-05 13:59:57.797237 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1852 2023-03-05 13:59:57.797433 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12472 2023-03-05 13:59:57.795341 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1697 2023-03-05 13:59:57.795510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    11341 2023-03-05 13:59:57.912081 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/resources.data.json
--rw-r--r--   0        0        0     1838 2023-03-05 13:59:57.912285 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/resources.meta.json
--rw-r--r--   0        0        0    22985 2023-03-05 13:59:57.904132 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/util.data.json
--rw-r--r--   0        0        0     1879 2023-03-05 13:59:57.904341 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/importlib/util.meta.json
--rw-r--r--   0        0        0   364855 2023-03-05 13:59:59.484482 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/inspect.data.json
--rw-r--r--   0        0        0     1841 2023-03-05 13:59:59.484779 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/inspect.meta.json
--rw-r--r--   0        0        0    88656 2023-03-05 13:59:57.794721 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1825 2023-03-05 13:59:57.794907 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0   137068 2023-03-05 14:01:07.965983 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipaddress.data.json
--rw-r--r--   0        0        0     1728 2023-03-05 14:01:07.966334 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipaddress.meta.json
--rw-r--r--   0        0        0     7243 2023-03-05 13:59:58.608151 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/_eventloop_macos.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 13:59:58.608350 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/_eventloop_macos.meta.json
--rw-r--r--   0        0        0     3748 2023-03-05 13:59:58.038467 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/_version.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.038724 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/_version.meta.json
--rw-r--r--   0        0        0     4064 2023-03-05 14:00:03.792906 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/control.data.json
--rw-r--r--   0        0        0     1899 2023-03-05 14:00:03.793098 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/control.meta.json
--rw-r--r--   0        0        0     1652 2023-03-05 13:59:57.879119 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/__init__.data.json
--rw-r--r--   0        0        0     1638 2023-03-05 13:59:57.879301 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/__init__.meta.json
--rw-r--r--   0        0        0     5803 2023-03-05 13:59:59.163652 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtk3embed.data.json
--rw-r--r--   0        0        0     1854 2023-03-05 13:59:59.163854 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtk3embed.meta.json
--rw-r--r--   0        0        0     5459 2023-03-05 13:59:59.165063 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtkembed.data.json
--rw-r--r--   0        0        0     1882 2023-03-05 13:59:59.165335 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/gui/gtkembed.meta.json
--rw-r--r--   0        0        0     6733 2023-03-05 14:00:01.135726 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/heartbeat.data.json
--rw-r--r--   0        0        0     2022 2023-03-05 14:00:01.135961 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/heartbeat.meta.json
--rw-r--r--   0        0        0     5254 2023-03-05 13:59:59.222496 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/jsonutil.data.json
--rw-r--r--   0        0        0     1887 2023-03-05 13:59:59.222827 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/jsonutil.meta.json
--rw-r--r--   0        0        0     5290 2023-03-05 13:59:59.331814 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/trio_runner.data.json
--rw-r--r--   0        0        0     1854 2023-03-05 13:59:59.332034 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ipykernel/trio_runner.meta.json
--rw-r--r--   0        0        0   267183 2023-03-05 13:59:58.340980 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/itertools.data.json
--rw-r--r--   0        0        0     1744 2023-03-05 13:59:58.341214 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/itertools.meta.json
--rw-r--r--   0        0        0    16677 2023-03-05 13:59:59.049733 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1730 2023-03-05 13:59:59.049928 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15568 2023-03-05 13:59:58.235753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1674 2023-03-05 13:59:58.236075 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11577 2023-03-05 13:59:58.234077 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1686 2023-03-05 13:59:58.234330 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0     4292 2023-03-05 14:01:08.499292 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/__init__.data.json
--rw-r--r--   0        0        0     1791 2023-03-05 14:01:08.499468 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/__init__.meta.json
--rw-r--r--   0        0        0    29969 2023-03-05 14:01:08.049373 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_format.data.json
--rw-r--r--   0        0        0     1698 2023-03-05 14:01:08.049570 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_format.meta.json
--rw-r--r--   0        0        0    15221 2023-03-05 14:01:08.046373 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_types.data.json
--rw-r--r--   0        0        0     1670 2023-03-05 14:01:08.046620 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_types.meta.json
--rw-r--r--   0        0        0    17667 2023-03-05 14:01:08.022610 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_utils.data.json
--rw-r--r--   0        0        0     1688 2023-03-05 14:01:08.022815 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/_utils.meta.json
--rw-r--r--   0        0        0    36635 2023-03-05 14:01:08.496968 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/exceptions.data.json
--rw-r--r--   0        0        0     1851 2023-03-05 14:01:08.497240 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/exceptions.meta.json
--rw-r--r--   0        0        0    13917 2023-03-05 14:01:08.498874 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/protocols.data.json
--rw-r--r--   0        0        0     1819 2023-03-05 14:01:08.499060 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/protocols.meta.json
--rw-r--r--   0        0        0    47152 2023-03-05 14:01:08.498251 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/validators.data.json
--rw-r--r--   0        0        0     1857 2023-03-05 14:01:08.498467 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jsonschema/validators.meta.json
--rw-r--r--   0        0        0     3959 2023-03-05 13:59:58.035625 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/_version.data.json
--rw-r--r--   0        0        0     1774 2023-03-05 13:59:58.035843 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/_version.meta.json
--rw-r--r--   0        0        0    10411 2023-03-05 13:59:57.919097 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/channelsabc.data.json
--rw-r--r--   0        0        0     1656 2023-03-05 13:59:57.919299 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/channelsabc.meta.json
--rw-r--r--   0        0        0    18522 2023-03-05 13:59:57.917818 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/clientabc.data.json
--rw-r--r--   0        0        0     1653 2023-03-05 13:59:57.918031 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/clientabc.meta.json
--rw-r--r--   0        0        0     5980 2023-03-05 14:01:09.059862 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/jsonutil.data.json
--rw-r--r--   0        0        0     2044 2023-03-05 14:01:09.060152 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/jsonutil.meta.json
--rw-r--r--   0        0        0    11762 2023-03-05 13:59:59.234715 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/localinterfaces.data.json
--rw-r--r--   0        0        0     1834 2023-03-05 13:59:59.234974 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/localinterfaces.meta.json
--rw-r--r--   0        0        0    11677 2023-03-05 13:59:57.916201 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/managerabc.data.json
--rw-r--r--   0        0        0     1654 2023-03-05 13:59:57.916404 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/managerabc.meta.json
--rw-r--r--   0        0        0     2314 2023-03-05 14:00:01.091360 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/__init__.data.json
--rw-r--r--   0        0        0     1731 2023-03-05 14:01:11.363236 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/__init__.meta.json
--rw-r--r--   0        0        0     7663 2023-03-05 13:59:59.530229 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/forward.data.json
--rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.530424 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/forward.meta.json
--rw-r--r--   0        0        0     9253 2023-03-05 14:01:11.166357 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/tunnel.data.json
--rw-r--r--   0        0        0     2201 2023-03-05 14:01:11.166711 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/ssh/tunnel.meta.json
--rw-r--r--   0        0        0     2246 2023-03-05 14:00:02.175819 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/utils.data.json
--rw-r--r--   0        0        0     1957 2023-03-05 14:00:02.176017 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/utils.meta.json
--rw-r--r--   0        0        0     4043 2023-03-05 13:59:57.868686 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/win_interrupt.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 13:59:57.869231 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_client/win_interrupt.meta.json
--rw-r--r--   0        0        0     1868 2023-03-05 13:59:58.875936 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/__init__.data.json
--rw-r--r--   0        0        0     1665 2023-03-05 13:59:58.876119 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/__init__.meta.json
--rw-r--r--   0        0        0    23908 2023-03-05 14:00:02.219317 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/paths.data.json
--rw-r--r--   0        0        0     2193 2023-03-05 14:01:09.876059 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/paths.meta.json
--rw-r--r--   0        0        0    13145 2023-03-05 14:00:01.937099 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/utils/__init__.data.json
--rw-r--r--   0        0        0     2193 2023-03-05 14:00:01.937330 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/utils/__init__.meta.json
--rw-r--r--   0        0        0     2980 2023-03-05 13:59:57.930930 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/version.data.json
--rw-r--r--   0        0        0     1768 2023-03-05 13:59:57.931133 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/jupyter_core/version.meta.json
--rw-r--r--   0        0        0     3743 2023-03-05 13:59:58.065584 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/keyword.data.json
--rw-r--r--   0        0        0     1698 2023-03-05 13:59:58.065764 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/keyword.meta.json
--rw-r--r--   0        0        0     9835 2023-03-05 13:59:58.070122 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/linecache.data.json
--rw-r--r--   0        0        0     1703 2023-03-05 13:59:58.070381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/linecache.meta.json
--rw-r--r--   0        0        0    34120 2023-03-05 13:59:59.553557 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/locale.data.json
--rw-r--r--   0        0        0     1783 2023-03-05 13:59:59.553756 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/locale.meta.json
--rw-r--r--   0        0        0   149635 2023-03-05 13:59:59.032114 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1838 2023-03-05 13:59:59.032388 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0    14995 2023-03-05 13:59:59.303166 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/config.data.json
--rw-r--r--   0        0        0     1794 2023-03-05 13:59:59.303360 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/config.meta.json
--rw-r--r--   0        0        0    80466 2023-03-05 13:59:59.782810 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/handlers.data.json
--rw-r--r--   0        0        0     2007 2023-03-05 13:59:59.783041 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/logging/handlers.meta.json
--rw-r--r--   0        0        0    53989 2023-03-05 13:59:58.493401 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 13:59:58.493632 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    16138 2023-03-05 13:59:58.447957 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/mimetypes.data.json
--rw-r--r--   0        0        0     1714 2023-03-05 13:59:58.448162 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/mimetypes.meta.json
--rw-r--r--   0        0        0    28133 2023-03-05 13:59:57.792831 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2023-03-05 13:59:57.793006 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0     1629 2023-03-05 13:59:58.114296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/msvcrt.data.json
--rw-r--r--   0        0        0     1678 2023-03-05 13:59:58.114485 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/msvcrt.meta.json
--rw-r--r--   0        0        0    34049 2023-03-05 13:59:59.774157 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2172 2023-03-05 13:59:59.774389 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    31566 2023-03-05 13:59:59.123558 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1878 2023-03-05 13:59:59.123753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0   100927 2023-03-05 13:59:59.772819 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2336 2023-03-05 13:59:59.773015 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   154754 2023-03-05 13:59:59.769981 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1969 2023-03-05 13:59:59.770204 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    53330 2023-03-05 13:59:57.863072 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1765 2023-03-05 13:59:57.863408 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9476 2023-03-05 13:59:59.487577 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.487785 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     6015 2023-03-05 13:59:59.764125 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1844 2023-03-05 13:59:59.764323 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6736 2023-03-05 13:59:59.763573 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1846 2023-03-05 13:59:59.763836 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     2122 2023-03-05 13:59:59.485970 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1816 2023-03-05 13:59:59.486320 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    18627 2023-03-05 13:59:57.882714 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1730 2023-03-05 13:59:57.882928 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    20797 2023-03-05 13:59:59.126234 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1734 2023-03-05 13:59:59.126433 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    30807 2023-03-05 13:59:59.765092 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1989 2023-03-05 13:59:59.765273 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29231 2023-03-05 13:59:57.855508 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:57.855717 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    71994 2023-03-05 13:59:59.766780 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1904 2023-03-05 13:59:59.766985 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10341 2023-03-05 13:59:57.880518 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1706 2023-03-05 13:59:57.880697 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    26724 2023-03-05 13:59:59.770837 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1869 2023-03-05 13:59:59.771018 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    24714 2023-03-05 13:59:59.110848 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1773 2023-03-05 13:59:59.111063 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/multiprocessing/util.meta.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:57.941390 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_imports.data.json
--rw-r--r--   0        0        0     1674 2023-03-05 13:59:57.941587 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_imports.meta.json
--rw-r--r--   0        0        0     6775 2023-03-05 13:59:57.944287 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_struct.data.json
--rw-r--r--   0        0        0     1722 2023-03-05 13:59:57.944540 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_struct.meta.json
--rw-r--r--   0        0        0     3211 2023-03-05 13:59:58.042388 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_version.data.json
--rw-r--r--   0        0        0     1852 2023-03-05 13:59:58.042609 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/_version.meta.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:57.883950 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.884168 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/corpus/__init__.meta.json
--rw-r--r--   0        0        0     1790 2023-03-05 13:59:58.673120 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/corpus/words.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 13:59:58.673305 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/corpus/words.meta.json
--rw-r--r--   0        0        0    10248 2023-03-05 14:01:08.680729 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/json_compat.data.json
--rw-r--r--   0        0        0     1868 2023-03-05 14:01:08.681036 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/json_compat.meta.json
--rw-r--r--   0        0        0     3218 2023-03-05 13:59:58.040088 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/sentinel.data.json
--rw-r--r--   0        0        0     1702 2023-03-05 13:59:58.040368 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/sentinel.meta.json
--rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.945938 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v1/convert.data.json
--rw-r--r--   0        0        0     1641 2023-03-05 13:59:57.946173 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v1/convert.meta.json
--rw-r--r--   0        0        0     3946 2023-03-05 13:59:57.887728 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:57.887922 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v1/rwbase.meta.json
--rw-r--r--   0        0        0     2384 2023-03-05 13:59:59.189191 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/convert.data.json
--rw-r--r--   0        0        0     1671 2023-03-05 13:59:59.189380 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/convert.meta.json
--rw-r--r--   0        0        0     4874 2023-03-05 13:59:58.676647 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.data.json
--rw-r--r--   0        0        0     1780 2023-03-05 13:59:58.676894 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbbase.meta.json
--rw-r--r--   0        0        0     2406 2023-03-05 13:59:57.945211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.data.json
--rw-r--r--   0        0        0     1637 2023-03-05 13:59:57.945454 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/nbxml.meta.json
--rw-r--r--   0        0        0     5725 2023-03-05 13:59:58.589761 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.data.json
--rw-r--r--   0        0        0     1722 2023-03-05 13:59:58.589959 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v2/rwbase.meta.json
--rw-r--r--   0        0        0     6240 2023-03-05 13:59:58.587486 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.data.json
--rw-r--r--   0        0        0     1721 2023-03-05 13:59:58.587686 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v3/rwbase.meta.json
--rw-r--r--   0        0        0     5834 2023-03-05 13:59:57.886699 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.data.json
--rw-r--r--   0        0        0     1705 2023-03-05 13:59:57.886908 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/v4/rwbase.meta.json
--rw-r--r--   0        0        0     3081 2023-03-05 13:59:57.937922 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/warnings.data.json
--rw-r--r--   0        0        0     1637 2023-03-05 13:59:57.938130 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/nbformat/warnings.meta.json
--rw-r--r--   0        0        0    77674 2023-03-05 14:01:08.530489 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ntsecuritycon/__init__.data.json
--rw-r--r--   0        0        0     1677 2023-03-05 14:01:08.530690 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ntsecuritycon/__init__.meta.json
--rw-r--r--   0        0        0    84003 2023-03-05 13:59:58.025429 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1638 2023-03-05 13:59:58.025632 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0  2384203 2023-03-05 14:00:00.883866 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3369 2023-03-05 14:00:00.884558 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5239 2023-03-05 13:59:58.463976 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.464164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0    22339 2023-03-05 14:00:00.777296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     2094 2023-03-05 14:00:00.777480 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3910 2023-03-05 14:00:00.922306 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1874 2023-03-05 14:00:00.922492 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    27226 2023-03-05 14:00:00.771301 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1865 2023-03-05 14:00:00.771499 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   277852 2023-03-05 14:00:00.838853 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1905 2023-03-05 14:00:00.839086 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    45396 2023-03-05 13:59:58.290941 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1653 2023-03-05 13:59:58.291135 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    32835 2023-03-05 14:00:00.765570 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1853 2023-03-05 14:00:00.765749 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6215 2023-03-05 14:00:00.833714 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1759 2023-03-05 14:00:00.833889 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    36648 2023-03-05 14:00:00.764024 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1904 2023-03-05 14:00:00.764348 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4746 2023-03-05 13:59:58.306348 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.306533 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    17703 2023-03-05 13:59:59.009120 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1711 2023-03-05 13:59:59.009328 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6364 2023-03-05 14:00:00.764637 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1711 2023-03-05 14:00:00.764847 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2487 2023-03-05 13:59:58.286822 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1642 2023-03-05 13:59:58.287013 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   280489 2023-03-05 14:00:00.928018 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1911 2023-03-05 14:00:00.928306 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     1957 2023-03-05 13:59:59.354577 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1718 2023-03-05 13:59:59.354793 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0     5426 2023-03-05 13:59:58.845346 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 13:59:58.845539 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5986 2023-03-05 13:59:58.097408 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1755 2023-03-05 13:59:58.097610 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    12299 2023-03-05 13:59:57.908006 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1922 2023-03-05 13:59:57.908221 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.463094 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1633 2023-03-05 13:59:58.463271 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    14745 2023-03-05 14:00:00.824038 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1826 2023-03-05 14:00:00.824202 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    23443 2023-03-05 14:00:00.839694 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 14:00:00.839871 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5153 2023-03-05 14:00:00.823464 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 14:00:00.823633 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11857 2023-03-05 14:00:00.823041 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1741 2023-03-05 14:00:00.823211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    30117 2023-03-05 14:00:00.822500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1794 2023-03-05 14:00:00.822681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   180955 2023-03-05 14:00:00.904669 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1847 2023-03-05 14:00:00.904916 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    38950 2023-03-05 14:00:00.821566 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.821764 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   357183 2023-03-05 14:00:00.831811 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1894 2023-03-05 14:00:00.832102 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    53356 2023-03-05 14:00:00.833234 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1853 2023-03-05 14:00:00.833432 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   324101 2023-03-05 14:00:00.820316 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1952 2023-03-05 14:00:00.820644 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   211121 2023-03-05 14:00:00.812837 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1896 2023-03-05 14:00:00.813098 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    48957 2023-03-05 14:00:00.808279 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1962 2023-03-05 14:00:00.808463 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    27023 2023-03-05 13:59:59.006043 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1902 2023-03-05 13:59:59.006249 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    56774 2023-03-05 14:00:00.900555 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1911 2023-03-05 14:00:00.900722 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    56748 2023-03-05 14:00:00.807057 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1871 2023-03-05 14:00:00.807245 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3289 2023-03-05 13:59:59.007242 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 13:59:59.007433 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0   120294 2023-03-05 14:00:00.776554 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1988 2023-03-05 14:00:00.776762 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     4625 2023-03-05 14:00:00.915679 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1766 2023-03-05 14:00:00.915842 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    19981 2023-03-05 14:00:00.896424 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1833 2023-03-05 14:00:00.896590 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    23352 2023-03-05 14:00:00.895738 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1800 2023-03-05 14:00:00.895905 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    26146 2023-03-05 14:00:00.773886 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2400 2023-03-05 14:00:00.774073 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9401 2023-03-05 13:59:58.285037 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1640 2023-03-05 13:59:58.285220 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    19429 2023-03-05 14:00:00.805710 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1805 2023-03-05 14:00:00.805896 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   167194 2023-03-05 14:00:00.804877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1811 2023-03-05 14:00:00.805148 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    27863 2023-03-05 14:00:00.801090 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1797 2023-03-05 14:00:00.801336 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7237 2023-03-05 13:59:58.286146 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1635 2023-03-05 13:59:58.286322 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   240651 2023-03-05 14:00:00.799981 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     2006 2023-03-05 14:00:00.800251 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     9558 2023-03-05 14:00:00.794645 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1817 2023-03-05 14:00:00.794874 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    67811 2023-03-05 14:00:00.794088 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1907 2023-03-05 14:00:00.794287 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    49712 2023-03-05 14:00:00.894997 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 14:00:00.895161 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    97113 2023-03-05 14:00:00.792442 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1921 2023-03-05 14:00:00.792646 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0   103869 2023-03-05 14:00:00.790446 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     2037 2023-03-05 14:00:00.790643 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   103615 2023-03-05 14:00:00.788068 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1810 2023-03-05 14:00:00.788320 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    66510 2023-03-05 14:00:00.893850 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1802 2023-03-05 14:00:00.894035 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    95306 2023-03-05 14:00:00.785688 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1923 2023-03-05 14:00:00.785905 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    25177 2023-03-05 14:00:00.783693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1839 2023-03-05 14:00:00.783862 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    82804 2023-03-05 14:00:00.782912 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1872 2023-03-05 14:00:00.783091 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   104203 2023-03-05 14:00:00.781132 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1871 2023-03-05 14:00:00.781309 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    26752 2023-03-05 14:00:00.778994 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1806 2023-03-05 14:00:00.779182 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    27948 2023-03-05 14:00:00.778188 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1786 2023-03-05 14:00:00.778369 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5678 2023-03-05 14:00:00.899213 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1745 2023-03-05 14:00:00.899378 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   115542 2023-03-05 14:00:00.898801 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1856 2023-03-05 14:00:00.898972 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29854 2023-03-05 14:00:00.773118 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1756 2023-03-05 14:00:00.773300 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   140392 2023-03-05 14:00:00.769468 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1778 2023-03-05 14:00:00.769763 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23680 2023-03-05 14:00:00.770439 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1758 2023-03-05 14:00:00.770629 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14850 2023-03-05 14:00:00.771947 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1744 2023-03-05 14:00:00.772122 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2967 2023-03-05 14:00:00.772333 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1771 2023-03-05 14:00:00.772508 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6637 2023-03-05 14:00:00.766062 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1878 2023-03-05 14:00:00.766233 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4358 2023-03-05 14:00:00.915281 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1936 2023-03-05 14:00:00.915452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27675 2023-03-05 13:59:58.095022 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.095207 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16931 2023-03-05 14:00:00.892428 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 14:00:00.892593 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14576 2023-03-05 14:00:00.891815 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1788 2023-03-05 14:00:00.891979 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14629 2023-03-05 14:00:00.891245 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 14:00:00.891411 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14404 2023-03-05 14:00:00.890659 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1790 2023-03-05 14:00:00.890832 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14404 2023-03-05 14:00:00.890074 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1790 2023-03-05 14:00:00.890244 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13519 2023-03-05 14:00:00.889490 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1794 2023-03-05 14:00:00.889660 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4735 2023-03-05 13:59:58.091725 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.091904 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10544 2023-03-05 14:00:00.921897 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1937 2023-03-05 14:00:00.922063 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   271081 2023-03-05 14:00:00.921316 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1937 2023-03-05 14:00:00.921569 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11101 2023-03-05 14:00:00.914406 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1845 2023-03-05 14:00:00.914573 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16178 2023-03-05 14:00:00.913871 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 14:00:00.914051 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11994 2023-03-05 14:00:00.913252 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1766 2023-03-05 14:00:00.913430 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9431 2023-03-05 14:00:00.912682 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 14:00:00.912866 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    72274 2023-03-05 14:00:00.888879 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1902 2023-03-05 14:00:00.889063 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   347968 2023-03-05 14:00:00.911954 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1906 2023-03-05 14:00:00.912282 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9282 2023-03-05 14:00:00.914871 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1774 2023-03-05 14:00:00.915045 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1724 2023-03-05 13:59:58.090722 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1654 2023-03-05 13:59:58.090918 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   122268 2023-03-05 14:00:00.887254 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     2084 2023-03-05 14:00:00.887457 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     3046 2023-03-05 14:00:00.922721 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1782 2023-03-05 14:00:00.922887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3508 2023-03-05 13:59:59.636465 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 13:59:59.636656 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     6614 2023-03-05 13:59:58.378820 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/opcode.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 13:59:58.379006 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/opcode.meta.json
--rw-r--r--   0        0        0    51024 2023-03-05 13:59:59.011513 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/operator.data.json
--rw-r--r--   0        0        0     1723 2023-03-05 13:59:59.011713 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/operator.meta.json
--rw-r--r--   0        0        0   338829 2023-03-05 13:59:57.791955 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1883 2023-03-05 13:59:57.792149 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5305 2023-03-05 13:59:57.785873 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 13:59:57.786049 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     3451 2023-03-05 13:59:57.878450 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/__init__.data.json
--rw-r--r--   0        0        0     1630 2023-03-05 13:59:57.878681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14453 2023-03-05 13:59:57.877550 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/_structures.data.json
--rw-r--r--   0        0        0     1646 2023-03-05 13:59:57.877834 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/_structures.meta.json
--rw-r--r--   0        0        0    69662 2023-03-05 13:59:58.668662 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/version.data.json
--rw-r--r--   0        0        0     1857 2023-03-05 13:59:58.668918 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/packaging/version.meta.json
--rw-r--r--   0        0        0     6546 2023-03-05 14:01:10.055112 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/__init__.data.json
--rw-r--r--   0        0        0     2291 2023-03-05 14:01:10.055319 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/__init__.meta.json
--rw-r--r--   0        0        0    31892 2023-03-05 14:01:09.826457 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/agent.data.json
--rw-r--r--   0        0        0     1818 2023-03-05 14:01:09.826663 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/agent.meta.json
--rw-r--r--   0        0        0    23965 2023-03-05 14:01:09.736789 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/auth_handler.data.json
--rw-r--r--   0        0        0     1825 2023-03-05 14:01:09.737032 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/auth_handler.meta.json
--rw-r--r--   0        0        0    11969 2023-03-05 14:01:08.484252 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/buffered_pipe.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.484440 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/buffered_pipe.meta.json
--rw-r--r--   0        0        0    49554 2023-03-05 14:01:09.742935 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/channel.data.json
--rw-r--r--   0        0        0     1837 2023-03-05 14:01:09.743112 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/channel.meta.json
--rw-r--r--   0        0        0    24917 2023-03-05 14:01:09.822937 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/client.data.json
--rw-r--r--   0        0        0     1925 2023-03-05 14:01:09.823149 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/client.meta.json
--rw-r--r--   0        0        0    28759 2023-03-05 14:01:08.345324 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/common.data.json
--rw-r--r--   0        0        0     1641 2023-03-05 14:01:08.345522 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/common.meta.json
--rw-r--r--   0        0        0     6323 2023-03-05 14:01:08.482230 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/compress.data.json
--rw-r--r--   0        0        0     1658 2023-03-05 14:01:08.482406 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/compress.meta.json
--rw-r--r--   0        0        0    19702 2023-03-05 14:01:08.781867 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/config.data.json
--rw-r--r--   0        0        0     1736 2023-03-05 14:01:08.782066 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/config.meta.json
--rw-r--r--   0        0        0    14974 2023-03-05 14:01:08.673545 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/dsskey.data.json
--rw-r--r--   0        0        0     1714 2023-03-05 14:01:08.673726 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/dsskey.meta.json
--rw-r--r--   0        0        0    26043 2023-03-05 14:01:09.691458 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ecdsakey.data.json
--rw-r--r--   0        0        0     1965 2023-03-05 14:01:09.691670 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ecdsakey.meta.json
--rw-r--r--   0        0        0     8915 2023-03-05 14:01:08.671720 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ed25519key.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 14:01:08.671913 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ed25519key.meta.json
--rw-r--r--   0        0        0    26482 2023-03-05 14:01:09.055048 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/file.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:09.055237 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/file.meta.json
--rw-r--r--   0        0        0    28415 2023-03-05 14:01:08.670308 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/hostkeys.data.json
--rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.670516 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/hostkeys.meta.json
--rw-r--r--   0        0        0    23353 2023-03-05 14:01:08.343115 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/message.data.json
--rw-r--r--   0        0        0     1706 2023-03-05 14:01:08.343303 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/message.meta.json
--rw-r--r--   0        0        0    24910 2023-03-05 14:01:09.686687 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/packet.data.json
--rw-r--r--   0        0        0     2002 2023-03-05 14:01:09.686897 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/packet.meta.json
--rw-r--r--   0        0        0    30907 2023-03-05 14:01:08.487677 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/pkey.data.json
--rw-r--r--   0        0        0     1701 2023-03-05 14:01:08.487867 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/pkey.meta.json
--rw-r--r--   0        0        0     8240 2023-03-05 14:01:09.052085 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/proxy.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 14:01:09.052273 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/proxy.meta.json
--rw-r--r--   0        0        0    16831 2023-03-05 14:01:09.688702 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/rsakey.data.json
--rw-r--r--   0        0        0     1915 2023-03-05 14:01:09.688898 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/rsakey.meta.json
--rw-r--r--   0        0        0    30724 2023-03-05 14:01:09.741784 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/server.data.json
--rw-r--r--   0        0        0     1788 2023-03-05 14:01:09.741958 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/server.meta.json
--rw-r--r--   0        0        0    13497 2023-03-05 14:01:09.740961 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp.data.json
--rw-r--r--   0        0        0     1704 2023-03-05 14:01:09.741132 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp.meta.json
--rw-r--r--   0        0        0    10648 2023-03-05 14:01:08.340378 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_attr.data.json
--rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.340575 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_attr.meta.json
--rw-r--r--   0        0        0    33946 2023-03-05 14:01:09.740404 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_client.data.json
--rw-r--r--   0        0        0     1921 2023-03-05 14:01:09.740576 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_client.meta.json
--rw-r--r--   0        0        0    16952 2023-03-05 14:01:09.739481 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_file.data.json
--rw-r--r--   0        0        0     1830 2023-03-05 14:01:09.739659 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_file.meta.json
--rw-r--r--   0        0        0     6801 2023-03-05 14:01:09.050907 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_handle.data.json
--rw-r--r--   0        0        0     1701 2023-03-05 14:01:09.051086 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_handle.meta.json
--rw-r--r--   0        0        0    11215 2023-03-05 14:01:09.925511 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_server.data.json
--rw-r--r--   0        0        0     1898 2023-03-05 14:01:09.925718 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_server.meta.json
--rw-r--r--   0        0        0    15086 2023-03-05 14:01:09.820064 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_si.data.json
--rw-r--r--   0        0        0     1749 2023-03-05 14:01:09.820266 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/sftp_si.meta.json
--rw-r--r--   0        0        0    22265 2023-03-05 14:01:08.666861 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ssh_exception.data.json
--rw-r--r--   0        0        0     1720 2023-03-05 14:01:08.667052 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ssh_exception.meta.json
--rw-r--r--   0        0        0    30038 2023-03-05 14:01:08.026118 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ssh_gss.data.json
--rw-r--r--   0        0        0     1642 2023-03-05 14:01:08.026325 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/ssh_gss.meta.json
--rw-r--r--   0        0        0    91286 2023-03-05 14:01:09.738823 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/transport.data.json
--rw-r--r--   0        0        0     2050 2023-03-05 14:01:09.739025 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/transport.meta.json
--rw-r--r--   0        0        0    22713 2023-03-05 14:01:08.864311 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/util.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 14:01:08.864550 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/paramiko/util.meta.json
--rw-r--r--   0        0        0    92975 2023-03-05 13:59:57.785409 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1834 2023-03-05 13:59:57.785601 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    99151 2023-03-05 13:59:59.618853 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pdb.data.json
--rw-r--r--   0        0        0     1871 2023-03-05 13:59:59.619069 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pdb.meta.json
--rw-r--r--   0        0        0    47593 2023-03-05 13:59:57.783487 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1770 2023-03-05 13:59:57.783667 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    33493 2023-03-05 13:59:58.385111 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pkgutil.data.json
--rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.385318 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pkgutil.meta.json
--rw-r--r--   0        0        0    37135 2023-03-05 13:59:58.258093 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platform.data.json
--rw-r--r--   0        0        0     1675 2023-03-05 13:59:58.258299 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platform.meta.json
--rw-r--r--   0        0        0    21800 2023-03-05 13:59:59.549907 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1911 2023-03-05 13:59:59.550105 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    17704 2023-03-05 13:59:59.174094 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/android.data.json
--rw-r--r--   0        0        0     1811 2023-03-05 13:59:59.174315 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/android.meta.json
--rw-r--r--   0        0        0    31813 2023-03-05 13:59:58.672497 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/api.data.json
--rw-r--r--   0        0        0     1738 2023-03-05 13:59:58.672708 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/api.meta.json
--rw-r--r--   0        0        0    14999 2023-03-05 13:59:59.176694 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/macos.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 13:59:59.176954 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/macos.meta.json
--rw-r--r--   0        0        0     2900 2023-03-05 13:59:57.929140 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/version.data.json
--rw-r--r--   0        0        0     1643 2023-03-05 13:59:57.929320 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/platformdirs/version.meta.json
--rw-r--r--   0        0        0    80904 2023-03-05 13:59:57.782301 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:57.782479 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0    12669 2023-03-05 13:59:58.254831 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pprint.data.json
--rw-r--r--   0        0        0     1671 2023-03-05 13:59:58.255021 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pprint.meta.json
--rw-r--r--   0        0        0    19634 2023-03-05 13:59:57.890466 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/profile.data.json
--rw-r--r--   0        0        0     1723 2023-03-05 13:59:57.890681 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/profile.meta.json
--rw-r--r--   0        0        0     3878 2023-03-05 14:00:03.583537 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.data.json
--rw-r--r--   0        0        0     2124 2023-03-05 14:01:11.159370 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/__init__.meta.json
--rw-r--r--   0        0        0     3806 2023-03-05 14:00:03.576593 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.data.json
--rw-r--r--   0        0        0     2050 2023-03-05 14:01:11.153152 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/__init__.meta.json
--rw-r--r--   0        0        0   110705 2023-03-05 14:00:03.574363 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.data.json
--rw-r--r--   0        0        0     4647 2023-03-05 14:01:11.151553 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/application.meta.json
--rw-r--r--   0        0        0    17588 2023-03-05 14:00:03.513758 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.data.json
--rw-r--r--   0        0        0     2245 2023-03-05 14:01:11.101896 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/current.meta.json
--rw-r--r--   0        0        0     9564 2023-03-05 14:00:03.576125 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.data.json
--rw-r--r--   0        0        0     2724 2023-03-05 14:01:11.152877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/dummy.meta.json
--rw-r--r--   0        0        0     6934 2023-03-05 14:00:03.514201 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.data.json
--rw-r--r--   0        0        0     2337 2023-03-05 14:01:11.102262 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/application/run_in_terminal.meta.json
--rw-r--r--   0        0        0    25227 2023-03-05 14:00:03.525841 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.data.json
--rw-r--r--   0        0        0     2234 2023-03-05 14:01:11.111713 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/auto_suggest.meta.json
--rw-r--r--   0        0        0   115144 2023-03-05 14:00:03.554715 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.data.json
--rw-r--r--   0        0        0     3256 2023-03-05 14:01:11.134028 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/buffer.meta.json
--rw-r--r--   0        0        0    21902 2023-03-05 13:59:58.844560 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.data.json
--rw-r--r--   0        0        0     1750 2023-03-05 13:59:58.844787 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cache.meta.json
--rw-r--r--   0        0        0     2966 2023-03-05 13:59:59.726404 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.data.json
--rw-r--r--   0        0        0     1812 2023-03-05 13:59:59.726592 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/__init__.meta.json
--rw-r--r--   0        0        0    19797 2023-03-05 13:59:59.120176 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.data.json
--rw-r--r--   0        0        0     1729 2023-03-05 13:59:59.120391 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/base.meta.json
--rw-r--r--   0        0        0     7335 2023-03-05 13:59:59.489368 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.data.json
--rw-r--r--   0        0        0     1850 2023-03-05 13:59:59.489578 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/clipboard/in_memory.meta.json
--rw-r--r--   0        0        0     4485 2023-03-05 14:00:03.551452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.data.json
--rw-r--r--   0        0        0     2141 2023-03-05 14:01:11.131339 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/__init__.meta.json
--rw-r--r--   0        0        0    45627 2023-03-05 14:00:03.545702 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.data.json
--rw-r--r--   0        0        0     2458 2023-03-05 14:01:11.127226 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/base.meta.json
--rw-r--r--   0        0        0     5921 2023-03-05 14:00:03.547927 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.data.json
--rw-r--r--   0        0        0     1948 2023-03-05 14:01:11.129060 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/deduplicate.meta.json
--rw-r--r--   0        0        0    10558 2023-03-05 14:00:03.550989 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.data.json
--rw-r--r--   0        0        0     2454 2023-03-05 14:01:11.131054 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/filesystem.meta.json
--rw-r--r--   0        0        0    33125 2023-03-05 14:00:03.550396 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.data.json
--rw-r--r--   0        0        0     2596 2023-03-05 14:01:11.130654 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/fuzzy_completer.meta.json
--rw-r--r--   0        0        0    10200 2023-03-05 14:00:03.549396 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.data.json
--rw-r--r--   0        0        0     2533 2023-03-05 14:01:11.129887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/nested.meta.json
--rw-r--r--   0        0        0    10690 2023-03-05 14:00:03.548790 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.data.json
--rw-r--r--   0        0        0     2399 2023-03-05 14:01:11.129479 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/completion/word_completer.meta.json
--rw-r--r--   0        0        0    19855 2023-03-05 14:00:03.510129 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.data.json
--rw-r--r--   0        0        0     2150 2023-03-05 14:01:11.098579 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/cursor_shapes.meta.json
--rw-r--r--   0        0        0    30460 2023-03-05 13:59:58.591476 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.data.json
--rw-r--r--   0        0        0     1682 2023-03-05 13:59:58.591696 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/data_structures.meta.json
--rw-r--r--   0        0        0    87962 2023-03-05 14:00:03.521626 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/document.data.json
--rw-r--r--   0        0        0     2216 2023-03-05 14:01:11.108526 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/document.meta.json
--rw-r--r--   0        0        0     3945 2023-03-05 13:59:58.892010 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.data.json
--rw-r--r--   0        0        0     1677 2023-03-05 13:59:58.892190 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/enums.meta.json
--rw-r--r--   0        0        0     3658 2023-03-05 14:00:02.365510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.data.json
--rw-r--r--   0        0        0     1993 2023-03-05 14:00:02.365710 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/__init__.meta.json
--rw-r--r--   0        0        0    10864 2023-03-05 14:00:02.174624 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.data.json
--rw-r--r--   0        0        0     2025 2023-03-05 14:00:02.174835 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/async_generator.meta.json
--rw-r--r--   0        0        0    19208 2023-03-05 14:00:01.869481 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.data.json
--rw-r--r--   0        0        0     2183 2023-03-05 14:00:01.869725 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/inputhook.meta.json
--rw-r--r--   0        0        0     7927 2023-03-05 14:00:01.864488 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.data.json
--rw-r--r--   0        0        0     1981 2023-03-05 14:00:01.864764 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/eventloop/utils.meta.json
--rw-r--r--   0        0        0    10713 2023-03-05 14:00:03.516480 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.data.json
--rw-r--r--   0        0        0     2007 2023-03-05 14:01:11.104012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/__init__.meta.json
--rw-r--r--   0        0        0    30926 2023-03-05 14:00:03.515056 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.data.json
--rw-r--r--   0        0        0     3161 2023-03-05 14:01:11.103002 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/app.meta.json
--rw-r--r--   0        0        0    33195 2023-03-05 13:59:58.832163 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 13:59:58.832419 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/base.meta.json
--rw-r--r--   0        0        0    21205 2023-03-05 14:00:03.515775 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.data.json
--rw-r--r--   0        0        0     2122 2023-03-05 14:01:11.103589 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/cli.meta.json
--rw-r--r--   0        0        0     5068 2023-03-05 13:59:59.191923 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 13:59:59.192273 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/filters/utils.meta.json
--rw-r--r--   0        0        0     4356 2023-03-05 14:00:03.542170 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.data.json
--rw-r--r--   0        0        0     2100 2023-03-05 14:01:11.124281 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/__init__.meta.json
--rw-r--r--   0        0        0    17413 2023-03-05 14:00:03.541763 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.data.json
--rw-r--r--   0        0        0     2192 2023-03-05 14:01:11.123985 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/ansi.meta.json
--rw-r--r--   0        0        0    17303 2023-03-05 14:00:03.508803 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.data.json
--rw-r--r--   0        0        0     2066 2023-03-05 14:01:11.097449 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/base.meta.json
--rw-r--r--   0        0        0    10370 2023-03-05 14:00:03.511118 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.data.json
--rw-r--r--   0        0        0     2180 2023-03-05 14:01:11.099517 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/html.meta.json
--rw-r--r--   0        0        0     6374 2023-03-05 14:01:11.098887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.data.json
--rw-r--r--   0        0        0     2056 2023-03-05 14:01:11.099111 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/pygments.meta.json
--rw-r--r--   0        0        0     7085 2023-03-05 14:00:03.512562 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.data.json
--rw-r--r--   0        0        0     2033 2023-03-05 14:01:11.100842 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/formatted_text/utils.meta.json
--rw-r--r--   0        0        0    27475 2023-03-05 14:00:01.960642 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/history.data.json
--rw-r--r--   0        0        0     2106 2023-03-05 14:00:01.960961 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/history.meta.json
--rw-r--r--   0        0        0     2881 2023-03-05 14:00:03.539168 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.data.json
--rw-r--r--   0        0        0     1924 2023-03-05 14:01:11.121989 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/__init__.meta.json
--rw-r--r--   0        0        0     4273 2023-03-05 13:59:59.107693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.data.json
--rw-r--r--   0        0        0     1847 2023-03-05 13:59:59.107954 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/ansi_escape_sequences.meta.json
--rw-r--r--   0        0        0    31155 2023-03-05 14:00:03.535376 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.data.json
--rw-r--r--   0        0        0     1958 2023-03-05 14:01:11.119218 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/base.meta.json
--rw-r--r--   0        0        0     4533 2023-03-05 14:00:03.537753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.data.json
--rw-r--r--   0        0        0     2009 2023-03-05 14:01:11.120889 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/defaults.meta.json
--rw-r--r--   0        0        0    18460 2023-03-05 14:00:03.538802 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_pipe.data.json
--rw-r--r--   0        0        0     1987 2023-03-05 14:01:11.121719 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_pipe.meta.json
--rw-r--r--   0        0        0     6081 2023-03-05 13:59:58.581369 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_utils.data.json
--rw-r--r--   0        0        0     1799 2023-03-05 13:59:58.581563 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/posix_utils.meta.json
--rw-r--r--   0        0        0     5412 2023-03-05 14:00:03.537081 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.data.json
--rw-r--r--   0        0        0     2029 2023-03-05 14:01:11.120590 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/typeahead.meta.json
--rw-r--r--   0        0        0    30618 2023-03-05 14:00:03.536660 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100.data.json
--rw-r--r--   0        0        0     2212 2023-03-05 14:01:11.120263 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100.meta.json
--rw-r--r--   0        0        0    17493 2023-03-05 14:00:03.527259 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.data.json
--rw-r--r--   0        0        0     2208 2023-03-05 14:01:11.112698 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/input/vt100_parser.meta.json
--rw-r--r--   0        0        0     3319 2023-03-05 14:00:03.533123 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.data.json
--rw-r--r--   0        0        0     1962 2023-03-05 14:01:11.117377 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/__init__.meta.json
--rw-r--r--   0        0        0     1828 2023-03-05 13:59:57.973215 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 13:59:57.973441 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/__init__.meta.json
--rw-r--r--   0        0        0     4097 2023-03-05 14:00:03.530822 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.data.json
--rw-r--r--   0        0        0     2424 2023-03-05 14:01:11.115574 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/auto_suggest.meta.json
--rw-r--r--   0        0        0     5644 2023-03-05 14:00:03.561022 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.data.json
--rw-r--r--   0        0        0     2547 2023-03-05 14:01:11.139572 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/basic.meta.json
--rw-r--r--   0        0        0     8035 2023-03-05 14:00:03.552032 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.data.json
--rw-r--r--   0        0        0     3601 2023-03-05 14:01:11.131710 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/completion.meta.json
--rw-r--r--   0        0        0     3577 2023-03-05 14:00:03.528756 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.data.json
--rw-r--r--   0        0        0     2345 2023-03-05 14:01:11.113821 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/cpr.meta.json
--rw-r--r--   0        0        0     8228 2023-03-05 14:00:03.560614 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.data.json
--rw-r--r--   0        0        0     2850 2023-03-05 14:01:11.139253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/emacs.meta.json
--rw-r--r--   0        0        0     4040 2023-03-05 14:00:03.529641 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.data.json
--rw-r--r--   0        0        0     2109 2023-03-05 14:01:11.114482 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/focus.meta.json
--rw-r--r--   0        0        0    13631 2023-03-05 14:00:03.528353 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.data.json
--rw-r--r--   0        0        0     2531 2023-03-05 14:01:11.113528 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/mouse.meta.json
--rw-r--r--   0        0        0    78608 2023-03-05 14:00:03.559305 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.data.json
--rw-r--r--   0        0        0     3170 2023-03-05 14:01:11.138100 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/named_commands.meta.json
--rw-r--r--   0        0        0     5555 2023-03-05 14:00:03.561420 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.data.json
--rw-r--r--   0        0        0     2214 2023-03-05 14:01:11.139894 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/open_in_editor.meta.json
--rw-r--r--   0        0        0     6935 2023-03-05 14:00:03.533578 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.data.json
--rw-r--r--   0        0        0     2209 2023-03-05 14:01:11.117715 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/page_navigation.meta.json
--rw-r--r--   0        0        0     8523 2023-03-05 14:00:03.527776 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.data.json
--rw-r--r--   0        0        0     2352 2023-03-05 14:01:11.113082 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/scroll.meta.json
--rw-r--r--   0        0        0    11950 2023-03-05 14:00:03.526520 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/search.data.json
--rw-r--r--   0        0        0     2458 2023-03-05 14:01:11.112155 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/search.meta.json
--rw-r--r--   0        0        0    31790 2023-03-05 14:00:03.560166 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.data.json
--rw-r--r--   0        0        0     3266 2023-03-05 14:01:11.138884 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/bindings/vi.meta.json
--rw-r--r--   0        0        0     4865 2023-03-05 14:00:03.565383 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.data.json
--rw-r--r--   0        0        0     2330 2023-03-05 14:01:11.143655 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/defaults.meta.json
--rw-r--r--   0        0        0     2898 2023-03-05 13:59:58.579433 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.data.json
--rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.579686 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/digraphs.meta.json
--rw-r--r--   0        0        0     8419 2023-03-05 14:00:03.529248 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.data.json
--rw-r--r--   0        0        0     1926 2023-03-05 14:01:11.114191 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/emacs_state.meta.json
--rw-r--r--   0        0        0    63950 2023-03-05 14:00:03.518054 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.data.json
--rw-r--r--   0        0        0     2393 2023-03-05 14:01:11.105335 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_bindings.meta.json
--rw-r--r--   0        0        0    41469 2023-03-05 14:00:03.524415 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.data.json
--rw-r--r--   0        0        0     2768 2023-03-05 14:01:11.110718 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/key_processor.meta.json
--rw-r--r--   0        0        0    18190 2023-03-05 14:00:03.509475 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.data.json
--rw-r--r--   0        0        0     2127 2023-03-05 14:01:11.098012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/key_binding/vi_state.meta.json
--rw-r--r--   0        0        0    70984 2023-03-05 13:59:58.605526 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.data.json
--rw-r--r--   0        0        0     1740 2023-03-05 13:59:58.605737 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/keys.meta.json
--rw-r--r--   0        0        0     7543 2023-03-05 14:00:03.571697 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.data.json
--rw-r--r--   0        0        0     2145 2023-03-05 14:01:11.149160 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/__init__.meta.json
--rw-r--r--   0        0        0   185167 2023-03-05 14:00:03.564905 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.data.json
--rw-r--r--   0        0        0     3079 2023-03-05 14:01:11.143294 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/containers.meta.json
--rw-r--r--   0        0        0   101505 2023-03-05 14:00:03.556850 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.data.json
--rw-r--r--   0        0        0     3148 2023-03-05 14:01:11.135918 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/controls.meta.json
--rw-r--r--   0        0        0    17147 2023-03-05 13:59:58.598937 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.data.json
--rw-r--r--   0        0        0     1799 2023-03-05 13:59:58.599164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dimension.meta.json
--rw-r--r--   0        0        0     4023 2023-03-05 14:00:03.571262 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.data.json
--rw-r--r--   0        0        0     2658 2023-03-05 14:01:11.148815 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/dummy.meta.json
--rw-r--r--   0        0        0    35286 2023-03-05 14:00:03.568999 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.data.json
--rw-r--r--   0        0        0     2810 2023-03-05 14:01:11.146826 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/layout.meta.json
--rw-r--r--   0        0        0    28065 2023-03-05 14:00:03.557669 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.data.json
--rw-r--r--   0        0        0     2407 2023-03-05 14:01:11.136628 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/margins.meta.json
--rw-r--r--   0        0        0    41688 2023-03-05 14:00:03.568023 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.data.json
--rw-r--r--   0        0        0     3168 2023-03-05 14:01:11.145985 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/menus.meta.json
--rw-r--r--   0        0        0     6947 2023-03-05 14:00:03.508100 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.data.json
--rw-r--r--   0        0        0     2029 2023-03-05 14:01:11.096881 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/mouse_handlers.meta.json
--rw-r--r--   0        0        0    80241 2023-03-05 14:00:03.547414 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.data.json
--rw-r--r--   0        0        0     3173 2023-03-05 14:01:11.128714 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/processors.meta.json
--rw-r--r--   0        0        0    26873 2023-03-05 14:00:03.507434 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.data.json
--rw-r--r--   0        0        0     2098 2023-03-05 14:01:11.096386 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/screen.meta.json
--rw-r--r--   0        0        0    24465 2023-03-05 14:00:03.567022 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.data.json
--rw-r--r--   0        0        0     2708 2023-03-05 14:01:11.145064 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/scrollable_pane.meta.json
--rw-r--r--   0        0        0    37663 2023-03-05 14:00:03.512077 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.data.json
--rw-r--r--   0        0        0     1981 2023-03-05 14:01:11.100444 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/layout/utils.meta.json
--rw-r--r--   0        0        0     3133 2023-03-05 14:00:03.535778 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.data.json
--rw-r--r--   0        0        0     1928 2023-03-05 14:01:11.119505 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/__init__.meta.json
--rw-r--r--   0        0        0    14260 2023-03-05 14:00:03.522261 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.data.json
--rw-r--r--   0        0        0     1968 2023-03-05 14:01:11.109047 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/base.meta.json
--rw-r--r--   0        0        0    23666 2023-03-05 14:01:11.115063 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.data.json
--rw-r--r--   0        0        0     2335 2023-03-05 14:01:11.115276 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/lexers/pygments.meta.json
--rw-r--r--   0        0        0    14038 2023-03-05 13:59:59.135212 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.data.json
--rw-r--r--   0        0        0     1735 2023-03-05 13:59:59.135487 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/mouse_events.meta.json
--rw-r--r--   0        0        0     2777 2023-03-05 14:00:03.539520 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.data.json
--rw-r--r--   0        0        0     1971 2023-03-05 14:01:11.122252 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/__init__.meta.json
--rw-r--r--   0        0        0    78156 2023-03-05 14:00:03.532689 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.data.json
--rw-r--r--   0        0        0     2124 2023-03-05 14:01:11.117090 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/base.meta.json
--rw-r--r--   0        0        0    10286 2023-03-05 14:00:03.513069 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.data.json
--rw-r--r--   0        0        0     2025 2023-03-05 14:01:11.101293 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/color_depth.meta.json
--rw-r--r--   0        0        0     4358 2023-03-05 14:00:03.538159 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.data.json
--rw-r--r--   0        0        0     2230 2023-03-05 14:01:11.121182 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/defaults.meta.json
--rw-r--r--   0        0        0     5097 2023-03-05 13:59:58.583627 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.data.json
--rw-r--r--   0        0        0     1754 2023-03-05 13:59:58.583829 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/flush_stdout.meta.json
--rw-r--r--   0        0        0    31425 2023-03-05 14:00:03.534472 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.data.json
--rw-r--r--   0        0        0     2216 2023-03-05 14:01:11.118456 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/plain_text.meta.json
--rw-r--r--   0        0        0    55786 2023-03-05 14:00:03.541081 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.data.json
--rw-r--r--   0        0        0     2366 2023-03-05 14:01:11.123435 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/output/vt100.meta.json
--rw-r--r--   0        0        0    23377 2023-03-05 14:00:03.582292 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.data.json
--rw-r--r--   0        0        0     2310 2023-03-05 14:01:11.158109 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/patch_stdout.meta.json
--rw-r--r--   0        0        0    42172 2023-03-05 14:00:03.543253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.data.json
--rw-r--r--   0        0        0     2974 2023-03-05 14:01:11.125217 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/renderer.meta.json
--rw-r--r--   0        0        0    13392 2023-03-05 14:00:03.519722 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/search.data.json
--rw-r--r--   0        0        0     2713 2023-03-05 14:01:11.106749 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/search.meta.json
--rw-r--r--   0        0        0     9949 2023-03-05 13:59:58.601265 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.data.json
--rw-r--r--   0        0        0     1686 2023-03-05 13:59:58.601458 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/selection.meta.json
--rw-r--r--   0        0        0     4761 2023-03-05 14:00:03.583148 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.data.json
--rw-r--r--   0        0        0     2031 2023-03-05 14:01:11.158956 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/__init__.meta.json
--rw-r--r--   0        0        0    22151 2023-03-05 14:00:03.579243 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.data.json
--rw-r--r--   0        0        0     3893 2023-03-05 14:01:11.155439 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/dialogs.meta.json
--rw-r--r--   0        0        0     4211 2023-03-05 14:00:03.582741 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.data.json
--rw-r--r--   0        0        0     1994 2023-03-05 14:01:11.158447 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/__init__.meta.json
--rw-r--r--   0        0        0    51945 2023-03-05 14:00:03.577848 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.data.json
--rw-r--r--   0        0        0     3590 2023-03-05 14:01:11.154271 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/base.meta.json
--rw-r--r--   0        0        0    49462 2023-03-05 14:00:03.544527 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.data.json
--rw-r--r--   0        0        0     2456 2023-03-05 14:01:11.126233 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/progress_bar/formatters.meta.json
--rw-r--r--   0        0        0   103285 2023-03-05 14:00:03.581359 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.data.json
--rw-r--r--   0        0        0     4315 2023-03-05 14:01:11.157391 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/prompt.meta.json
--rw-r--r--   0        0        0    10977 2023-03-05 14:00:03.578474 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.data.json
--rw-r--r--   0        0        0     3245 2023-03-05 14:01:11.154749 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/shortcuts/utils.meta.json
--rw-r--r--   0        0        0     5819 2023-03-05 14:00:03.525016 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.data.json
--rw-r--r--   0        0        0     2107 2023-03-05 14:01:11.111048 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/__init__.meta.json
--rw-r--r--   0        0        0    52830 2023-03-05 13:59:58.825893 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.data.json
--rw-r--r--   0        0        0     1701 2023-03-05 13:59:58.826108 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/base.meta.json
--rw-r--r--   0        0        0     7461 2023-03-05 13:59:59.540204 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.data.json
--rw-r--r--   0        0        0     1896 2023-03-05 13:59:59.540393 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/defaults.meta.json
--rw-r--r--   0        0        0     2547 2023-03-05 13:59:58.820538 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.data.json
--rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.820746 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/named_colors.meta.json
--rw-r--r--   0        0        0     5208 2023-03-05 14:01:08.821870 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.data.json
--rw-r--r--   0        0        0     1922 2023-03-05 14:01:08.822152 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/pygments.meta.json
--rw-r--r--   0        0        0    28427 2023-03-05 13:59:59.216223 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.data.json
--rw-r--r--   0        0        0     1913 2023-03-05 13:59:59.216445 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style.meta.json
--rw-r--r--   0        0        0    43235 2023-03-05 14:00:03.519116 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.data.json
--rw-r--r--   0        0        0     2334 2023-03-05 14:01:11.106259 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/styles/style_transformation.meta.json
--rw-r--r--   0        0        0    33097 2023-03-05 13:59:58.840698 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.data.json
--rw-r--r--   0        0        0     1914 2023-03-05 13:59:58.840966 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/utils.meta.json
--rw-r--r--   0        0        0    28835 2023-03-05 14:00:03.523097 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.data.json
--rw-r--r--   0        0        0     2113 2023-03-05 14:01:11.109783 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/validation.meta.json
--rw-r--r--   0        0        0     4794 2023-03-05 14:00:03.575562 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.data.json
--rw-r--r--   0        0        0     2015 2023-03-05 14:01:11.152484 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/__init__.meta.json
--rw-r--r--   0        0        0    88345 2023-03-05 14:00:03.570849 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.data.json
--rw-r--r--   0        0        0     3384 2023-03-05 14:01:11.148510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/base.meta.json
--rw-r--r--   0        0        0     8559 2023-03-05 14:00:03.572183 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.data.json
--rw-r--r--   0        0        0     2599 2023-03-05 14:01:11.149540 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/dialogs.meta.json
--rw-r--r--   0        0        0    20393 2023-03-05 14:00:03.575101 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.data.json
--rw-r--r--   0        0        0     2878 2023-03-05 14:01:11.152174 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/menus.meta.json
--rw-r--r--   0        0        0    29788 2023-03-05 14:00:03.566267 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.data.json
--rw-r--r--   0        0        0     3364 2023-03-05 14:01:11.144407 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/prompt_toolkit/widgets/toolbars.meta.json
--rw-r--r--   0        0        0    42144 2023-03-05 13:59:58.683257 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pstats.data.json
--rw-r--r--   0        0        0     1806 2023-03-05 13:59:58.683502 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pstats.meta.json
--rw-r--r--   0        0        0    69566 2023-03-05 14:01:08.872765 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/__init__.data.json
--rw-r--r--   0        0        0     1817 2023-03-05 14:01:08.873013 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/__init__.meta.json
--rw-r--r--   0        0        0   459802 2023-03-05 14:01:08.659690 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/_common.data.json
--rw-r--r--   0        0        0     1753 2023-03-05 14:01:08.659947 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/_common.meta.json
--rw-r--r--   0        0        0   106929 2023-03-05 14:01:08.773963 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/_psosx.data.json
--rw-r--r--   0        0        0     1679 2023-03-05 14:01:08.774170 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/psutil/_psosx.meta.json
--rw-r--r--   0        0        0     2307 2023-03-05 14:00:01.656772 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/__init__.data.json
--rw-r--r--   0        0        0     1767 2023-03-05 14:00:01.657005 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/__init__.meta.json
--rw-r--r--   0        0        0    17272 2023-03-05 14:00:01.089774 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/core.data.json
--rw-r--r--   0        0        0     2009 2023-03-05 14:00:01.090032 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/core.meta.json
--rw-r--r--   0        0        0     7726 2023-03-05 14:00:00.931825 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.data.json
--rw-r--r--   0        0        0     1833 2023-03-05 14:00:00.932028 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/my_getattr_static.meta.json
--rw-r--r--   0        0        0    14265 2023-03-05 13:59:59.650997 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/utils.data.json
--rw-r--r--   0        0        0     1995 2023-03-05 13:59:59.651237 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/utils.meta.json
--rw-r--r--   0        0        0     1658 2023-03-05 13:59:57.866253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/version.data.json
--rw-r--r--   0        0        0     1636 2023-03-05 13:59:57.866489 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pure_eval/version.meta.json
--rw-r--r--   0        0        0   109208 2023-03-05 13:59:58.903390 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pydoc.data.json
--rw-r--r--   0        0        0     1752 2023-03-05 13:59:58.903602 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pydoc.meta.json
--rw-r--r--   0        0        0    38603 2023-03-05 13:59:58.848848 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/__init__.data.json
--rw-r--r--   0        0        0     1833 2023-03-05 13:59:58.849050 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/__init__.meta.json
--rw-r--r--   0        0        0    11077 2023-03-05 13:59:57.909966 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/errors.data.json
--rw-r--r--   0        0        0     1688 2023-03-05 13:59:57.910157 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/errors.meta.json
--rw-r--r--   0        0        0     3512 2023-03-05 13:59:57.908745 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/model.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 13:59:57.908933 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pyexpat/model.meta.json
--rw-r--r--   0        0        0    15061 2023-03-05 14:01:08.569581 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/__init__.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.569795 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/__init__.meta.json
--rw-r--r--   0        0        0    12596 2023-03-05 14:01:08.405329 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatter.data.json
--rw-r--r--   0        0        0     1645 2023-03-05 14:01:08.405519 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatter.meta.json
--rw-r--r--   0        0        0     6802 2023-03-05 14:01:08.847511 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/__init__.data.json
--rw-r--r--   0        0        0     2110 2023-03-05 14:01:08.847755 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/__init__.meta.json
--rw-r--r--   0        0        0     5938 2023-03-05 14:01:08.557698 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/bbcode.data.json
--rw-r--r--   0        0        0     1689 2023-03-05 14:01:08.557896 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/bbcode.meta.json
--rw-r--r--   0        0        0    17954 2023-03-05 14:01:08.556823 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/html.data.json
--rw-r--r--   0        0        0     1705 2023-03-05 14:01:08.557015 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/html.meta.json
--rw-r--r--   0        0        0    26743 2023-03-05 14:01:08.555019 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/img.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.555233 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/img.meta.json
--rw-r--r--   0        0        0     6457 2023-03-05 14:01:08.552601 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/irc.data.json
--rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.552782 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/irc.meta.json
--rw-r--r--   0        0        0    14567 2023-03-05 14:01:08.708006 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/latex.data.json
--rw-r--r--   0        0        0     1711 2023-03-05 14:01:08.708197 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/latex.meta.json
--rw-r--r--   0        0        0    13276 2023-03-05 14:01:08.551691 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/other.data.json
--rw-r--r--   0        0        0     1687 2023-03-05 14:01:08.551893 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/other.meta.json
--rw-r--r--   0        0        0     6133 2023-03-05 14:01:08.549981 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/pangomarkup.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.550172 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/pangomarkup.meta.json
--rw-r--r--   0        0        0     6142 2023-03-05 14:01:08.549117 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/rtf.data.json
--rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.549296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/rtf.meta.json
--rw-r--r--   0        0        0     8986 2023-03-05 14:01:08.548241 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/svg.data.json
--rw-r--r--   0        0        0     1683 2023-03-05 14:01:08.548444 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/svg.meta.json
--rw-r--r--   0        0        0     6969 2023-03-05 14:01:08.547226 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.547431 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal.meta.json
--rw-r--r--   0        0        0    15695 2023-03-05 14:01:08.546168 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal256.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 14:01:08.546412 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/formatters/terminal256.meta.json
--rw-r--r--   0        0        0    43182 2023-03-05 14:01:08.562689 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/lexer.data.json
--rw-r--r--   0        0        0     1729 2023-03-05 14:01:08.562915 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/lexer.meta.json
--rw-r--r--   0        0        0    11933 2023-03-05 14:01:08.738330 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/lexers/__init__.data.json
--rw-r--r--   0        0        0     1767 2023-03-05 14:01:08.738589 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/lexers/__init__.meta.json
--rw-r--r--   0        0        0    11959 2023-03-05 14:01:08.535060 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/style.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 14:01:08.535256 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/style.meta.json
--rw-r--r--   0        0        0     4682 2023-03-05 14:01:08.705469 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/styles/__init__.data.json
--rw-r--r--   0        0        0     1777 2023-03-05 14:01:08.705656 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/styles/__init__.meta.json
--rw-r--r--   0        0        0    11861 2023-03-05 14:01:08.393198 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/token.data.json
--rw-r--r--   0        0        0     1689 2023-03-05 14:01:08.393434 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/token.meta.json
--rw-r--r--   0        0        0    15519 2023-03-05 14:01:08.385877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/util.data.json
--rw-r--r--   0        0        0     1667 2023-03-05 14:01:08.386074 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/pygments/util.meta.json
--rw-r--r--   0        0        0    32155 2023-03-05 13:59:58.879428 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/queue.data.json
--rw-r--r--   0        0        0     1703 2023-03-05 13:59:58.879625 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/queue.meta.json
--rw-r--r--   0        0        0    44133 2023-03-05 13:59:59.843167 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/random.data.json
--rw-r--r--   0        0        0     1799 2023-03-05 13:59:59.843414 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/random.meta.json
--rw-r--r--   0        0        0   151207 2023-03-05 13:59:57.780628 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1855 2023-03-05 13:59:57.780826 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    17427 2023-03-05 13:59:58.064688 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/reprlib.data.json
--rw-r--r--   0        0        0     1727 2023-03-05 13:59:58.064875 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/reprlib.meta.json
--rw-r--r--   0        0        0    43927 2023-03-05 13:59:57.894462 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/resource.data.json
--rw-r--r--   0        0        0     1701 2023-03-05 13:59:57.894677 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/resource.meta.json
--rw-r--r--   0        0        0    11069 2023-03-05 13:59:58.268268 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/runpy.data.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.268457 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/runpy.meta.json
--rw-r--r--   0        0        0    25728 2023-03-05 13:59:57.927952 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/select.data.json
--rw-r--r--   0        0        0     1737 2023-03-05 13:59:57.928161 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/select.meta.json
--rw-r--r--   0        0        0    58547 2023-03-05 13:59:57.937087 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selectors.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 13:59:57.937305 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selectors.meta.json
--rw-r--r--   0        0        0     1844 2023-03-05 13:59:58.480737 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/__init__.data.json
--rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.480934 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/__init__.meta.json
--rw-r--r--   0        0        0     6903 2023-03-05 13:59:59.002365 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/common/__init__.data.json
--rw-r--r--   0        0        0     1680 2023-03-05 13:59:59.002544 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/common/__init__.meta.json
--rw-r--r--   0        0        0    37581 2023-03-05 13:59:58.462559 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/common/exceptions.data.json
--rw-r--r--   0        0        0     1656 2023-03-05 13:59:58.462770 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/common/exceptions.meta.json
--rw-r--r--   0        0        0     2578 2023-03-05 13:59:58.458282 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/types.data.json
--rw-r--r--   0        0        0     1633 2023-03-05 13:59:58.458458 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/types.meta.json
--rw-r--r--   0        0        0     4859 2023-03-05 14:00:03.770536 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.data.json
--rw-r--r--   0        0        0     2704 2023-03-05 14:00:03.770741 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/__init__.meta.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.477153 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.data.json
--rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.477376 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/__init__.meta.json
--rw-r--r--   0        0        0     5742 2023-03-05 13:59:59.639120 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.data.json
--rw-r--r--   0        0        0     1940 2023-03-05 13:59:59.639342 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/options.meta.json
--rw-r--r--   0        0        0     4143 2023-03-05 14:00:02.030949 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.data.json
--rw-r--r--   0        0        0     2015 2023-03-05 14:00:02.031189 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/service.meta.json
--rw-r--r--   0        0        0     5832 2023-03-05 14:00:02.561027 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.data.json
--rw-r--r--   0        0        0     2402 2023-03-05 14:00:02.561377 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chrome/webdriver.meta.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.457669 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.data.json
--rw-r--r--   0        0        0     1666 2023-03-05 13:59:58.457841 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/__init__.meta.json
--rw-r--r--   0        0        0    24423 2023-03-05 13:59:59.465110 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.data.json
--rw-r--r--   0        0        0     1987 2023-03-05 13:59:59.465353 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/options.meta.json
--rw-r--r--   0        0        0     3914 2023-03-05 13:59:59.846450 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.data.json
--rw-r--r--   0        0        0     1834 2023-03-05 14:01:09.707289 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/remote_connection.meta.json
--rw-r--r--   0        0        0     5123 2023-03-05 14:00:01.728428 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.data.json
--rw-r--r--   0        0        0     1806 2023-03-05 14:00:01.728644 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/service.meta.json
--rw-r--r--   0        0        0    17717 2023-03-05 14:00:02.245859 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.data.json
--rw-r--r--   0        0        0     2395 2023-03-05 14:01:09.882553 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/chromium/webdriver.meta.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.479874 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.data.json
--rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.480235 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/__init__.meta.json
--rw-r--r--   0        0        0    13594 2023-03-05 14:00:02.559460 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.data.json
--rw-r--r--   0        0        0     2279 2023-03-05 14:00:02.559702 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/action_chains.meta.json
--rw-r--r--   0        0        0     1812 2023-03-05 13:59:58.230822 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.data.json
--rw-r--r--   0        0        0     1678 2023-03-05 13:59:58.231048 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/__init__.meta.json
--rw-r--r--   0        0        0    21140 2023-03-05 14:00:02.240410 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.data.json
--rw-r--r--   0        0        0     2479 2023-03-05 14:00:02.240641 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/action_builder.meta.json
--rw-r--r--   0        0        0     4359 2023-03-05 13:59:58.986060 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.data.json
--rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.986263 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/input_device.meta.json
--rw-r--r--   0        0        0     9216 2023-03-05 13:59:58.230235 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.data.json
--rw-r--r--   0        0        0     1808 2023-03-05 13:59:58.230476 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/interaction.meta.json
--rw-r--r--   0        0        0     4805 2023-03-05 14:00:01.120893 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.data.json
--rw-r--r--   0        0        0     1952 2023-03-05 14:00:01.121091 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_actions.meta.json
--rw-r--r--   0        0        0    11074 2023-03-05 13:59:59.307061 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.data.json
--rw-r--r--   0        0        0     1897 2023-03-05 13:59:59.307264 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/key_input.meta.json
--rw-r--r--   0        0        0     3890 2023-03-05 13:59:58.013797 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.data.json
--rw-r--r--   0        0        0     1695 2023-03-05 13:59:58.013992 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/mouse_button.meta.json
--rw-r--r--   0        0        0     8252 2023-03-05 14:00:01.965347 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.data.json
--rw-r--r--   0        0        0     2349 2023-03-05 14:00:01.965546 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_actions.meta.json
--rw-r--r--   0        0        0     7552 2023-03-05 14:00:01.726869 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.data.json
--rw-r--r--   0        0        0     2147 2023-03-05 14:00:01.727092 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/pointer_input.meta.json
--rw-r--r--   0        0        0     4270 2023-03-05 14:00:01.963113 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.data.json
--rw-r--r--   0        0        0     2045 2023-03-05 14:00:01.963335 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_actions.meta.json
--rw-r--r--   0        0        0    17775 2023-03-05 14:00:01.820500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.data.json
--rw-r--r--   0        0        0     2227 2023-03-05 14:00:01.820753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/actions/wheel_input.meta.json
--rw-r--r--   0        0        0     4852 2023-03-05 14:00:01.119604 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.data.json
--rw-r--r--   0        0        0     1837 2023-03-05 14:00:01.119821 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/alert.meta.json
--rw-r--r--   0        0        0     4382 2023-03-05 13:59:58.495870 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 13:59:58.496060 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/by.meta.json
--rw-r--r--   0        0        0     6606 2023-03-05 13:59:58.476553 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 13:59:58.476789 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/desired_capabilities.meta.json
--rw-r--r--   0        0        0     1796 2023-03-05 13:59:58.227666 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.data.json
--rw-r--r--   0        0        0     1674 2023-03-05 13:59:58.227892 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/__init__.meta.json
--rw-r--r--   0        0        0     6289 2023-03-05 13:59:59.445296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.data.json
--rw-r--r--   0        0        0     1871 2023-03-05 13:59:59.445493 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/html5/application_cache.meta.json
--rw-r--r--   0        0        0    19713 2023-03-05 13:59:58.475277 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.data.json
--rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.475501 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/keys.meta.json
--rw-r--r--   0        0        0    43425 2023-03-05 13:59:59.054328 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.data.json
--rw-r--r--   0        0        0     1777 2023-03-05 13:59:59.054544 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/options.meta.json
--rw-r--r--   0        0        0    46958 2023-03-05 13:59:58.398912 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.data.json
--rw-r--r--   0        0        0     1820 2023-03-05 13:59:58.399164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/print_page_options.meta.json
--rw-r--r--   0        0        0    41912 2023-03-05 13:59:58.473632 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.data.json
--rw-r--r--   0        0        0     1752 2023-03-05 13:59:58.473894 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/proxy.meta.json
--rw-r--r--   0        0        0     7869 2023-03-05 13:59:59.219877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.data.json
--rw-r--r--   0        0        0     1931 2023-03-05 13:59:59.220107 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/selenium_manager.meta.json
--rw-r--r--   0        0        0    16679 2023-03-05 14:00:01.133259 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.data.json
--rw-r--r--   0        0        0     2273 2023-03-05 14:00:01.133512 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/service.meta.json
--rw-r--r--   0        0        0    15320 2023-03-05 13:59:58.390831 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.data.json
--rw-r--r--   0        0        0     1800 2023-03-05 13:59:58.391093 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/timeouts.meta.json
--rw-r--r--   0        0        0    10986 2023-03-05 14:00:01.039296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.data.json
--rw-r--r--   0        0        0     2005 2023-03-05 14:00:01.039586 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/utils.meta.json
--rw-r--r--   0        0        0    34270 2023-03-05 13:59:59.042615 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.data.json
--rw-r--r--   0        0        0     1865 2023-03-05 13:59:59.042892 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/common/virtual_authenticator.meta.json
--rw-r--r--   0        0        0     1732 2023-03-05 13:59:58.427753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.data.json
--rw-r--r--   0        0        0     1658 2023-03-05 13:59:58.427937 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/__init__.meta.json
--rw-r--r--   0        0        0     9581 2023-03-05 13:59:59.638037 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.data.json
--rw-r--r--   0        0        0     1936 2023-03-05 13:59:59.638271 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/options.meta.json
--rw-r--r--   0        0        0     4244 2023-03-05 14:00:02.029970 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.data.json
--rw-r--r--   0        0        0     2032 2023-03-05 14:00:02.030205 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/service.meta.json
--rw-r--r--   0        0        0     6213 2023-03-05 14:00:02.556215 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.data.json
--rw-r--r--   0        0        0     2394 2023-03-05 14:00:02.556578 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/edge/webdriver.meta.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.427243 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.data.json
--rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.427435 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/__init__.meta.json
--rw-r--r--   0        0        0     9555 2023-03-05 14:00:01.316839 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.data.json
--rw-r--r--   0        0        0     2077 2023-03-05 14:00:01.317040 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_binary.meta.json
--rw-r--r--   0        0        0    21852 2023-03-05 14:00:01.340092 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.data.json
--rw-r--r--   0        0        0     2327 2023-03-05 14:00:01.340400 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/firefox_profile.meta.json
--rw-r--r--   0        0        0    26663 2023-03-05 14:00:01.861506 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.data.json
--rw-r--r--   0        0        0     2255 2023-03-05 14:00:01.861745 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/options.meta.json
--rw-r--r--   0        0        0     4316 2023-03-05 13:59:59.847547 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.data.json
--rw-r--r--   0        0        0     1924 2023-03-05 14:01:09.709165 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/remote_connection.meta.json
--rw-r--r--   0        0        0     5364 2023-03-05 14:00:01.816861 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.data.json
--rw-r--r--   0        0        0     1988 2023-03-05 14:00:01.817084 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/service.meta.json
--rw-r--r--   0        0        0    17781 2023-03-05 14:00:02.336923 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.data.json
--rw-r--r--   0        0        0     2675 2023-03-05 14:01:09.894607 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/firefox/webdriver.meta.json
--rw-r--r--   0        0        0     1716 2023-03-05 13:59:58.400110 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.data.json
--rw-r--r--   0        0        0     1654 2023-03-05 13:59:58.400332 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/__init__.meta.json
--rw-r--r--   0        0        0    70437 2023-03-05 13:59:59.459397 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.data.json
--rw-r--r--   0        0        0     1977 2023-03-05 13:59:59.459674 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/options.meta.json
--rw-r--r--   0        0        0     5028 2023-03-05 14:00:01.815292 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.data.json
--rw-r--r--   0        0        0     1922 2023-03-05 14:00:01.815533 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/service.meta.json
--rw-r--r--   0        0        0     8894 2023-03-05 14:00:02.330586 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.data.json
--rw-r--r--   0        0        0     2195 2023-03-05 14:00:02.330815 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/ie/webdriver.meta.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.399530 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.data.json
--rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.399758 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/__init__.meta.json
--rw-r--r--   0        0        0     4438 2023-03-05 13:59:58.387843 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.data.json
--rw-r--r--   0        0        0     1685 2023-03-05 13:59:58.388030 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/bidi_connection.meta.json
--rw-r--r--   0        0        0    25487 2023-03-05 13:59:58.387110 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.data.json
--rw-r--r--   0        0        0     1670 2023-03-05 13:59:58.387296 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/command.meta.json
--rw-r--r--   0        0        0    22349 2023-03-05 13:59:59.444269 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.data.json
--rw-r--r--   0        0        0     1946 2023-03-05 13:59:59.444505 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/errorhandler.meta.json
--rw-r--r--   0        0        0     8366 2023-03-05 14:00:01.313122 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.data.json
--rw-r--r--   0        0        0     1870 2023-03-05 14:00:01.313325 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/file_detector.meta.json
--rw-r--r--   0        0        0    13913 2023-03-05 13:59:59.435452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.data.json
--rw-r--r--   0        0        0     1799 2023-03-05 13:59:59.435654 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/mobile.meta.json
--rw-r--r--   0        0        0    17637 2023-03-05 14:01:09.671857 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.data.json
--rw-r--r--   0        0        0     2303 2023-03-05 14:01:09.672163 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/remote_connection.meta.json
--rw-r--r--   0        0        0     4936 2023-03-05 13:59:59.036999 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.data.json
--rw-r--r--   0        0        0     1692 2023-03-05 13:59:59.037211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/script_key.meta.json
--rw-r--r--   0        0        0     8313 2023-03-05 13:59:59.035798 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.data.json
--rw-r--r--   0        0        0     1926 2023-03-05 13:59:59.036042 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/shadowroot.meta.json
--rw-r--r--   0        0        0    10787 2023-03-05 14:00:01.810133 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.data.json
--rw-r--r--   0        0        0     2226 2023-03-05 14:00:01.810446 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/switch_to.meta.json
--rw-r--r--   0        0        0     3211 2023-03-05 13:59:59.305088 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.data.json
--rw-r--r--   0        0        0     1776 2023-03-05 13:59:59.305269 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/utils.meta.json
--rw-r--r--   0        0        0    91970 2023-03-05 14:00:02.158329 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.data.json
--rw-r--r--   0        0        0     3414 2023-03-05 14:01:09.818020 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webdriver.meta.json
--rw-r--r--   0        0        0    40435 2023-03-05 14:00:01.332392 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.data.json
--rw-r--r--   0        0        0     2291 2023-03-05 14:00:01.332692 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/remote/webelement.meta.json
--rw-r--r--   0        0        0     1748 2023-03-05 13:59:58.382463 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.data.json
--rw-r--r--   0        0        0     1662 2023-03-05 13:59:58.382647 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/__init__.meta.json
--rw-r--r--   0        0        0    22656 2023-03-05 13:59:59.433543 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.data.json
--rw-r--r--   0        0        0     1877 2023-03-05 13:59:59.433770 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/options.meta.json
--rw-r--r--   0        0        0     4073 2023-03-05 13:59:59.844344 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.data.json
--rw-r--r--   0        0        0     1922 2023-03-05 14:01:09.704850 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/remote_connection.meta.json
--rw-r--r--   0        0        0     8421 2023-03-05 14:00:01.807872 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.data.json
--rw-r--r--   0        0        0     1989 2023-03-05 14:00:01.808073 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/service.meta.json
--rw-r--r--   0        0        0     7381 2023-03-05 14:00:02.327877 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.data.json
--rw-r--r--   0        0        0     2450 2023-03-05 14:01:09.887455 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/safari/webdriver.meta.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.477751 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.data.json
--rw-r--r--   0        0        0     1664 2023-03-05 13:59:58.477991 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/__init__.meta.json
--rw-r--r--   0        0        0    13107 2023-03-05 14:00:01.813306 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.data.json
--rw-r--r--   0        0        0     2089 2023-03-05 14:00:01.813550 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/relative_locator.meta.json
--rw-r--r--   0        0        0    13030 2023-03-05 13:59:59.071510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.data.json
--rw-r--r--   0        0        0     1901 2023-03-05 13:59:59.071756 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/select.meta.json
--rw-r--r--   0        0        0     1741 2023-03-05 13:59:59.485193 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.data.json
--rw-r--r--   0        0        0     1796 2023-03-05 13:59:59.485395 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/ui.meta.json
--rw-r--r--   0        0        0     7966 2023-03-05 13:59:59.066790 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.data.json
--rw-r--r--   0        0        0     1884 2023-03-05 13:59:59.067008 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/support/wait.meta.json
--rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.379850 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.data.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.380038 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/__init__.meta.json
--rw-r--r--   0        0        0    11454 2023-03-05 13:59:59.450822 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.data.json
--rw-r--r--   0        0        0     1862 2023-03-05 13:59:59.451012 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/options.meta.json
--rw-r--r--   0        0        0     5211 2023-03-05 14:00:01.805852 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.data.json
--rw-r--r--   0        0        0     1950 2023-03-05 14:00:01.806083 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/service.meta.json
--rw-r--r--   0        0        0     4048 2023-03-05 14:00:02.325486 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.data.json
--rw-r--r--   0        0        0     2197 2023-03-05 14:00:02.325674 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/webkitgtk/webdriver.meta.json
--rw-r--r--   0        0        0     1772 2023-03-05 13:59:58.379343 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.data.json
--rw-r--r--   0        0        0     1668 2023-03-05 13:59:58.379536 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/__init__.meta.json
--rw-r--r--   0        0        0     9242 2023-03-05 13:59:59.449381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.data.json
--rw-r--r--   0        0        0     1862 2023-03-05 13:59:59.449583 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/options.meta.json
--rw-r--r--   0        0        0     5211 2023-03-05 14:00:01.804332 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.data.json
--rw-r--r--   0        0        0     1950 2023-03-05 14:00:01.804576 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/service.meta.json
--rw-r--r--   0        0        0     4065 2023-03-05 14:00:02.324511 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.data.json
--rw-r--r--   0        0        0     2163 2023-03-05 14:00:02.324702 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/selenium/webdriver/wpewebkit/webdriver.meta.json
--rw-r--r--   0        0        0    17092 2023-03-05 13:59:58.314564 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/shlex.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.314747 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/shlex.meta.json
--rw-r--r--   0        0        0    75994 2023-03-05 13:59:58.426675 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/shutil.data.json
--rw-r--r--   0        0        0     1735 2023-03-05 13:59:58.426889 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/shutil.meta.json
--rw-r--r--   0        0        0    33917 2023-03-05 13:59:58.251165 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/signal.data.json
--rw-r--r--   0        0        0     1751 2023-03-05 13:59:58.251396 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/signal.meta.json
--rw-r--r--   0        0        0    16136 2023-03-05 13:59:58.260551 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/site.data.json
--rw-r--r--   0        0        0     1691 2023-03-05 13:59:58.260741 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/site.meta.json
--rw-r--r--   0        0        0    65683 2023-03-05 14:01:09.716253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/__init__.data.json
--rw-r--r--   0        0        0     1931 2023-03-05 14:01:09.716470 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/__init__.meta.json
--rw-r--r--   0        0        0     2064 2023-03-05 14:01:08.860692 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/BaseHTTPServer.data.json
--rw-r--r--   0        0        0     1678 2023-03-05 14:01:08.860871 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/BaseHTTPServer.meta.json
--rw-r--r--   0        0        0     2057 2023-03-05 14:01:08.860213 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/CGIHTTPServer.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.860400 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/CGIHTTPServer.meta.json
--rw-r--r--   0        0        0     2078 2023-03-05 14:01:08.859711 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/SimpleHTTPServer.data.json
--rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.859911 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/SimpleHTTPServer.meta.json
--rw-r--r--   0        0        0     8164 2023-03-05 14:01:09.683840 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/__init__.data.json
--rw-r--r--   0        0        0     2932 2023-03-05 14:01:09.684044 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/__init__.meta.json
--rw-r--r--   0        0        0     2552 2023-03-05 14:01:08.481099 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/_dummy_thread.data.json
--rw-r--r--   0        0        0     1707 2023-03-05 14:01:08.481275 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/_dummy_thread.meta.json
--rw-r--r--   0        0        0     2389 2023-03-05 14:01:08.480404 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/_thread.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.480583 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/_thread.meta.json
--rw-r--r--   0        0        0    15901 2023-03-05 14:01:08.014732 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/builtins.data.json
--rw-r--r--   0        0        0     1645 2023-03-05 14:01:08.014936 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/builtins.meta.json
--rw-r--r--   0        0        0     8791 2023-03-05 14:01:08.013676 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/cPickle.data.json
--rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.013915 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/cPickle.meta.json
--rw-r--r--   0        0        0     4004 2023-03-05 14:01:08.479822 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/configparser.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.480054 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/configparser.meta.json
--rw-r--r--   0        0        0     1937 2023-03-05 14:01:08.479019 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/copyreg.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.479331 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/copyreg.meta.json
--rw-r--r--   0        0        0     1579 2023-03-05 14:01:08.478031 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_base.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.478273 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_base.meta.json
--rw-r--r--   0        0        0     1629 2023-03-05 14:01:08.626865 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_multipart.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.627075 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_multipart.meta.json
--rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.626329 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_nonmultipart.data.json
--rw-r--r--   0        0        0     1708 2023-03-05 14:01:08.626548 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_nonmultipart.meta.json
--rw-r--r--   0        0        0     1579 2023-03-05 14:01:08.761338 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_text.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.761510 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/email_mime_text.meta.json
--rw-r--r--   0        0        0     1879 2023-03-05 14:01:08.477365 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/html_entities.data.json
--rw-r--r--   0        0        0     1678 2023-03-05 14:01:08.477625 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/html_entities.meta.json
--rw-r--r--   0        0        0     1551 2023-03-05 14:01:08.625785 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/html_parser.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.626000 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/html_parser.meta.json
--rw-r--r--   0        0        0     9807 2023-03-05 14:01:08.859213 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_client.data.json
--rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.859397 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_client.meta.json
--rw-r--r--   0        0        0     2328 2023-03-05 14:01:09.042354 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_cookiejar.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:09.042539 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_cookiejar.meta.json
--rw-r--r--   0        0        0     1860 2023-03-05 14:01:08.476775 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_cookies.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.476978 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/http_cookies.meta.json
--rw-r--r--   0        0        0     1947 2023-03-05 14:01:08.625233 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/queue.data.json
--rw-r--r--   0        0        0     1654 2023-03-05 14:01:08.625456 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/queue.meta.json
--rw-r--r--   0        0        0     1695 2023-03-05 14:01:08.476257 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/reprlib.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.476466 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/reprlib.meta.json
--rw-r--r--   0        0        0     3290 2023-03-05 14:01:08.760873 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/socketserver.data.json
--rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.761057 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/socketserver.meta.json
--rw-r--r--   0        0        0    13745 2023-03-05 14:01:08.624657 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter.data.json
--rw-r--r--   0        0        0     1660 2023-03-05 14:01:08.624893 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter.meta.json
--rw-r--r--   0        0        0     1615 2023-03-05 14:01:08.475724 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_commondialog.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 14:01:08.475947 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_commondialog.meta.json
--rw-r--r--   0        0        0     8903 2023-03-05 14:01:08.475179 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_constants.data.json
--rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.475408 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_constants.meta.json
--rw-r--r--   0        0        0     1567 2023-03-05 14:01:08.760391 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_dialog.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.760557 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_dialog.meta.json
--rw-r--r--   0        0        0     2937 2023-03-05 14:01:08.759938 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_filedialog.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.760115 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_filedialog.meta.json
--rw-r--r--   0        0        0     2951 2023-03-05 14:01:08.759439 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_tkfiledialog.data.json
--rw-r--r--   0        0        0     1697 2023-03-05 14:01:08.759625 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_tkfiledialog.meta.json
--rw-r--r--   0        0        0     3891 2023-03-05 14:01:08.758918 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_ttk.data.json
--rw-r--r--   0        0        0     1672 2023-03-05 14:01:08.759108 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/tkinter_ttk.meta.json
--rw-r--r--   0        0        0     2179 2023-03-05 14:01:09.071858 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/__init__.data.json
--rw-r--r--   0        0        0     1827 2023-03-05 14:01:09.072082 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/__init__.meta.json
--rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.582253 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/error.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.582452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/error.meta.json
--rw-r--r--   0        0        0     3575 2023-03-05 14:01:08.467841 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/parse.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.468008 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/parse.meta.json
--rw-r--r--   0        0        0     5326 2023-03-05 14:01:09.041831 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/request.data.json
--rw-r--r--   0        0        0     1683 2023-03-05 14:01:09.042020 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/request.meta.json
--rw-r--r--   0        0        0     1583 2023-03-05 14:01:08.467319 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/response.data.json
--rw-r--r--   0        0        0     1685 2023-03-05 14:01:08.467505 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/response.meta.json
--rw-r--r--   0        0        0     1617 2023-03-05 14:01:08.466847 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/robotparser.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.467031 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib/robotparser.meta.json
--rw-r--r--   0        0        0     1775 2023-03-05 14:01:08.623777 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_error.data.json
--rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.624014 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_error.meta.json
--rw-r--r--   0        0        0     3613 2023-03-05 14:01:08.474479 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_parse.data.json
--rw-r--r--   0        0        0     1675 2023-03-05 14:01:08.474695 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_parse.meta.json
--rw-r--r--   0        0        0     1617 2023-03-05 14:01:08.473868 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_robotparser.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 14:01:08.474094 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/six/moves/urllib_robotparser.meta.json
--rw-r--r--   0        0        0    86759 2023-03-05 13:59:58.984945 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/socket.data.json
--rw-r--r--   0        0        0     1843 2023-03-05 13:59:58.985175 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/socket.meta.json
--rw-r--r--   0        0        0    65585 2023-03-05 13:59:59.133392 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/socketserver.data.json
--rw-r--r--   0        0        0     1848 2023-03-05 13:59:59.133607 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/socketserver.meta.json
--rw-r--r--   0        0        0    10113 2023-03-05 13:59:59.298601 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sqlite3/__init__.data.json
--rw-r--r--   0        0        0     1671 2023-03-05 13:59:59.298782 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sqlite3/__init__.meta.json
--rw-r--r--   0        0        0   128383 2023-03-05 13:59:59.298040 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.data.json
--rw-r--r--   0        0        0     1868 2023-03-05 13:59:59.298273 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sqlite3/dbapi2.meta.json
--rw-r--r--   0        0        0    15087 2023-03-05 13:59:57.777717 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1700 2023-03-05 13:59:57.777888 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    29752 2023-03-05 13:59:57.777156 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 13:59:57.777327 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    52521 2023-03-05 13:59:57.776302 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:57.776497 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   197333 2023-03-05 13:59:59.327668 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ssl.data.json
--rw-r--r--   0        0        0     1894 2023-03-05 13:59:59.327914 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/ssl.meta.json
--rw-r--r--   0        0        0     3342 2023-03-05 14:00:02.195008 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/__init__.data.json
--rw-r--r--   0        0        0     1926 2023-03-05 14:01:11.397050 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/__init__.meta.json
--rw-r--r--   0        0        0   109628 2023-03-05 14:00:01.911180 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/core.data.json
--rw-r--r--   0        0        0     2231 2023-03-05 14:01:11.362148 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/core.meta.json
--rw-r--r--   0        0        0    19167 2023-03-05 14:00:02.194559 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/formatting.data.json
--rw-r--r--   0        0        0     2169 2023-03-05 14:01:11.396750 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/formatting.meta.json
--rw-r--r--   0        0        0    18775 2023-03-05 14:00:02.193660 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/serializing.data.json
--rw-r--r--   0        0        0     2256 2023-03-05 14:01:11.396116 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/serializing.meta.json
--rw-r--r--   0        0        0    18281 2023-03-05 13:59:59.738055 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/utils.data.json
--rw-r--r--   0        0        0     1893 2023-03-05 14:01:10.054463 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/utils.meta.json
--rw-r--r--   0        0        0     1666 2023-03-05 13:59:57.973823 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/version.data.json
--rw-r--r--   0        0        0     1638 2023-03-05 13:59:57.974678 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stack_data/version.meta.json
--rw-r--r--   0        0        0     7079 2023-03-05 13:59:59.012156 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stat.data.json
--rw-r--r--   0        0        0     1647 2023-03-05 13:59:59.012326 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/stat.meta.json
--rw-r--r--   0        0        0    28271 2023-03-05 13:59:58.227007 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1749 2023-03-05 13:59:58.227251 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0    16134 2023-03-05 13:59:58.445777 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/struct.data.json
--rw-r--r--   0        0        0     1746 2023-03-05 13:59:58.445965 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/struct.meta.json
--rw-r--r--   0        0        0   170345 2023-03-05 13:59:57.775023 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1824 2023-03-05 13:59:57.775212 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   147982 2023-03-05 13:59:57.771706 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1803 2023-03-05 13:59:57.771904 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   118973 2023-03-05 13:59:58.420881 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tempfile.data.json
--rw-r--r--   0        0        0     1768 2023-03-05 13:59:58.421132 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tempfile.meta.json
--rw-r--r--   0        0        0    51601 2023-03-05 13:59:58.112567 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/termios.data.json
--rw-r--r--   0        0        0     1699 2023-03-05 13:59:58.112777 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/termios.meta.json
--rw-r--r--   0        0        0    20620 2023-03-05 13:59:58.120113 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1679 2023-03-05 13:59:58.120312 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    67623 2023-03-05 13:59:58.325619 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1734 2023-03-05 13:59:58.325856 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    45246 2023-03-05 13:59:58.486404 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1693 2023-03-05 13:59:58.486643 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0    12783 2023-03-05 13:59:57.948922 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/timeit.data.json
--rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.949145 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/timeit.meta.json
--rw-r--r--   0        0        0  1132743 2023-03-05 13:59:58.816870 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/__init__.data.json
--rw-r--r--   0        0        0     1911 2023-03-05 13:59:58.817181 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/__init__.meta.json
--rw-r--r--   0        0        0     5838 2023-03-05 14:01:07.987231 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/commondialog.data.json
--rw-r--r--   0        0        0     1722 2023-03-05 14:01:07.987421 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/commondialog.meta.json
--rw-r--r--   0        0        0    20007 2023-03-05 13:59:57.900380 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/constants.data.json
--rw-r--r--   0        0        0     1687 2023-03-05 13:59:57.900604 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/constants.meta.json
--rw-r--r--   0        0        0     5652 2023-03-05 14:01:08.622277 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/dialog.data.json
--rw-r--r--   0        0        0     1727 2023-03-05 14:01:08.622489 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/dialog.meta.json
--rw-r--r--   0        0        0    42762 2023-03-05 14:01:08.621195 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/filedialog.data.json
--rw-r--r--   0        0        0     1807 2023-03-05 14:01:08.621417 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/filedialog.meta.json
--rw-r--r--   0        0        0    46653 2023-03-05 13:59:58.794883 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/font.data.json
--rw-r--r--   0        0        0     1747 2023-03-05 13:59:58.795151 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/font.meta.json
--rw-r--r--   0        0        0   414945 2023-03-05 14:01:08.616570 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/ttk.data.json
--rw-r--r--   0        0        0     1792 2023-03-05 14:01:08.616848 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tkinter/ttk.meta.json
--rw-r--r--   0        0        0    16221 2023-03-05 13:59:58.059713 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/token.data.json
--rw-r--r--   0        0        0     1670 2023-03-05 13:59:58.059900 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/token.meta.json
--rw-r--r--   0        0        0    52823 2023-03-05 13:59:58.886341 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tokenize.data.json
--rw-r--r--   0        0        0     1766 2023-03-05 13:59:58.886540 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tokenize.meta.json
--rw-r--r--   0        0        0     2322 2023-03-05 13:59:58.247211 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/__init__.data.json
--rw-r--r--   0        0        0     1627 2023-03-05 13:59:58.247407 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/__init__.meta.json
--rw-r--r--   0        0        0    27215 2023-03-05 14:00:03.725587 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/concurrent.data.json
--rw-r--r--   0        0        0     2085 2023-03-05 14:01:11.316802 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/concurrent.meta.json
--rw-r--r--   0        0        0    32193 2023-03-05 14:00:02.171811 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/escape.data.json
--rw-r--r--   0        0        0     2105 2023-03-05 14:00:02.172051 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/escape.meta.json
--rw-r--r--   0        0        0    58686 2023-03-05 14:00:03.729865 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/gen.data.json
--rw-r--r--   0        0        0     2291 2023-03-05 14:01:11.320794 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/gen.meta.json
--rw-r--r--   0        0        0    69509 2023-03-05 14:00:03.727405 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/ioloop.data.json
--rw-r--r--   0        0        0     2637 2023-03-05 14:01:11.318549 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/ioloop.meta.json
--rw-r--r--   0        0        0    79926 2023-03-05 14:00:03.731684 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/iostream.data.json
--rw-r--r--   0        0        0     2502 2023-03-05 14:01:11.322505 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/iostream.meta.json
--rw-r--r--   0        0        0    35943 2023-03-05 14:00:03.779546 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/locks.data.json
--rw-r--r--   0        0        0     2214 2023-03-05 14:00:03.779820 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/locks.meta.json
--rw-r--r--   0        0        0     9760 2023-03-05 14:01:09.954166 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/log.data.json
--rw-r--r--   0        0        0     2041 2023-03-05 14:01:09.954484 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/log.meta.json
--rw-r--r--   0        0        0    36166 2023-03-05 14:00:03.728451 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/netutil.data.json
--rw-r--r--   0        0        0     2303 2023-03-05 14:01:11.319484 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/netutil.meta.json
--rw-r--r--   0        0        0    42399 2023-03-05 14:00:02.364748 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/options.data.json
--rw-r--r--   0        0        0     2159 2023-03-05 14:01:09.955589 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/options.meta.json
--rw-r--r--   0        0        0     1676 2023-03-05 13:59:57.928546 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/platform/__init__.data.json
--rw-r--r--   0        0        0     1642 2023-03-05 13:59:57.928735 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/platform/__init__.meta.json
--rw-r--r--   0        0        0    57261 2023-03-05 14:00:03.733022 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/platform/asyncio.data.json
--rw-r--r--   0        0        0     2350 2023-03-05 14:01:11.323753 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/platform/asyncio.meta.json
--rw-r--r--   0        0        0    20538 2023-03-05 14:00:03.733762 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/process.data.json
--rw-r--r--   0        0        0     2406 2023-03-05 14:01:11.324391 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/process.meta.json
--rw-r--r--   0        0        0    40269 2023-03-05 14:00:03.812585 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/queues.data.json
--rw-r--r--   0        0        0     2301 2023-03-05 14:00:03.812881 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/queues.meta.json
--rw-r--r--   0        0        0    42511 2023-03-05 14:00:01.932095 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/util.data.json
--rw-r--r--   0        0        0     2201 2023-03-05 14:00:01.932340 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tornado/util.meta.json
--rw-r--r--   0        0        0     5659 2023-03-05 14:01:08.917555 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/__init__.data.json
--rw-r--r--   0        0        0     1818 2023-03-05 14:01:08.917788 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/__init__.meta.json
--rw-r--r--   0        0        0     7167 2023-03-05 14:01:08.571896 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/_monitor.data.json
--rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.572093 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/_monitor.meta.json
--rw-r--r--   0        0        0     2675 2023-03-05 14:01:08.438395 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/_tqdm_pandas.data.json
--rw-r--r--   0        0        0     1643 2023-03-05 14:01:08.438567 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/_tqdm_pandas.meta.json
--rw-r--r--   0        0        0    66131 2023-03-05 14:01:08.858250 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/asyncio.data.json
--rw-r--r--   0        0        0     1744 2023-03-05 14:01:08.858458 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/asyncio.meta.json
--rw-r--r--   0        0        0     1965 2023-03-05 14:01:09.041109 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/auto.data.json
--rw-r--r--   0        0        0     1649 2023-03-05 14:01:09.041406 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/auto.meta.json
--rw-r--r--   0        0        0     2733 2023-03-05 14:01:08.437828 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/cli.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.438003 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/cli.meta.json
--rw-r--r--   0        0        0    27887 2023-03-05 14:01:08.853500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/gui.data.json
--rw-r--r--   0        0        0     1709 2023-03-05 14:01:08.853697 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/gui.meta.json
--rw-r--r--   0        0        0    40061 2023-03-05 14:01:08.851002 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/notebook.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 14:01:08.851214 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/notebook.meta.json
--rw-r--r--   0        0        0   104587 2023-03-05 14:01:08.746596 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/std.data.json
--rw-r--r--   0        0        0     1796 2023-03-05 14:01:08.746826 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/std.meta.json
--rw-r--r--   0        0        0    30940 2023-03-05 14:01:08.414127 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/utils.data.json
--rw-r--r--   0        0        0     1713 2023-03-05 14:01:08.414342 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/utils.meta.json
--rw-r--r--   0        0        0     1587 2023-03-05 14:01:08.437123 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/version.data.json
--rw-r--r--   0        0        0     1633 2023-03-05 14:01:08.437343 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tqdm/version.meta.json
--rw-r--r--   0        0        0    54443 2023-03-05 13:59:58.266744 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traceback.data.json
--rw-r--r--   0        0        0     1743 2023-03-05 13:59:58.266961 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traceback.meta.json
--rw-r--r--   0        0        0    11487 2023-03-05 14:00:01.136847 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/__init__.data.json
--rw-r--r--   0        0        0     1940 2023-03-05 14:00:01.137062 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/__init__.meta.json
--rw-r--r--   0        0        0     2956 2023-03-05 13:59:58.071651 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/_version.data.json
--rw-r--r--   0        0        0     1764 2023-03-05 13:59:58.071887 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/_version.meta.json
--rw-r--r--   0        0        0    10223 2023-03-05 13:59:58.909113 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.data.json
--rw-r--r--   0        0        0     1839 2023-03-05 13:59:58.909336 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/config/argcomplete_config.meta.json
--rw-r--r--   0        0        0   174172 2023-03-05 13:59:59.836772 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/traitlets.data.json
--rw-r--r--   0        0        0     2291 2023-03-05 13:59:59.837128 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/traitlets.meta.json
--rw-r--r--   0        0        0     2592 2023-03-05 13:59:58.252655 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.data.json
--rw-r--r--   0        0        0     1809 2023-03-05 13:59:58.252884 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/__init__.meta.json
--rw-r--r--   0        0        0     3280 2023-03-05 13:59:58.072713 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.data.json
--rw-r--r--   0        0        0     1645 2023-03-05 13:59:58.072957 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/bunch.meta.json
--rw-r--r--   0        0        0     3960 2023-03-05 14:00:00.949052 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.data.json
--rw-r--r--   0        0        0     1831 2023-03-05 14:00:00.949251 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/decorators.meta.json
--rw-r--r--   0        0        0     3084 2023-03-05 13:59:59.545834 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.data.json
--rw-r--r--   0        0        0     1849 2023-03-05 13:59:59.546029 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/descriptions.meta.json
--rw-r--r--   0        0        0     1911 2023-03-05 13:59:59.543824 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.data.json
--rw-r--r--   0        0        0     1835 2023-03-05 13:59:59.544019 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/getargspec.meta.json
--rw-r--r--   0        0        0     1756 2023-03-05 13:59:58.281826 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.data.json
--rw-r--r--   0        0        0     1761 2023-03-05 13:59:58.282007 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/importstring.meta.json
--rw-r--r--   0        0        0     1781 2023-03-05 13:59:58.090164 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 13:59:58.090352 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/nested_update.meta.json
--rw-r--r--   0        0        0     3862 2023-03-05 13:59:58.019287 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.data.json
--rw-r--r--   0        0        0     1716 2023-03-05 13:59:58.019470 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/sentinel.meta.json
--rw-r--r--   0        0        0     2832 2023-03-05 13:59:58.910459 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/text.data.json
--rw-r--r--   0        0        0     1689 2023-03-05 13:59:58.910652 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/traitlets/utils/text.meta.json
--rw-r--r--   0        0        0     5215 2023-03-05 13:59:58.113689 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tty.data.json
--rw-r--r--   0        0        0     1671 2023-03-05 13:59:58.113898 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/tty.meta.json
--rw-r--r--   0        0        0   242405 2023-03-05 13:59:57.768979 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1775 2023-03-05 13:59:57.769191 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   430606 2023-03-05 13:59:57.764584 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1842 2023-03-05 13:59:57.764833 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    71533 2023-03-05 13:59:57.755998 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1765 2023-03-05 13:59:57.756331 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    25457 2023-03-05 13:59:58.050448 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unicodedata.data.json
--rw-r--r--   0        0        0     1707 2023-03-05 13:59:58.050655 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unicodedata.meta.json
--rw-r--r--   0        0        0     6387 2023-03-05 13:59:59.382990 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1941 2023-03-05 13:59:59.383193 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    25783 2023-03-05 13:59:59.374580 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1789 2023-03-05 13:59:59.374767 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8109 2023-03-05 13:59:59.379451 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1820 2023-03-05 13:59:59.379631 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   221008 2023-03-05 13:59:59.378920 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1940 2023-03-05 13:59:59.379146 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15471 2023-03-05 13:59:59.381827 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1851 2023-03-05 13:59:59.382059 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12425 2023-03-05 13:59:59.382484 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1860 2023-03-05 13:59:59.382701 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    21795 2023-03-05 13:59:59.373746 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1807 2023-03-05 13:59:59.373974 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11341 2023-03-05 13:59:59.381170 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1850 2023-03-05 13:59:59.381383 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12147 2023-03-05 13:59:59.380559 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1802 2023-03-05 13:59:59.380784 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    11760 2023-03-05 13:59:59.379987 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1823 2023-03-05 13:59:59.380161 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0     1617 2023-03-05 13:59:58.240199 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/__init__.data.json
--rw-r--r--   0        0        0     1644 2023-03-05 13:59:58.240409 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/__init__.meta.json
--rw-r--r--   0        0        0    11137 2023-03-05 13:59:58.988694 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/error.data.json
--rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.988933 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/error.meta.json
--rw-r--r--   0        0        0   152232 2023-03-05 13:59:58.442114 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/parse.data.json
--rw-r--r--   0        0        0     1723 2023-03-05 13:59:58.442386 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/parse.meta.json
--rw-r--r--   0        0        0   159266 2023-03-05 13:59:59.870660 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/request.data.json
--rw-r--r--   0        0        0     2041 2023-03-05 13:59:59.870878 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/request.meta.json
--rw-r--r--   0        0        0    29584 2023-03-05 13:59:58.239627 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/response.data.json
--rw-r--r--   0        0        0     1832 2023-03-05 13:59:58.239854 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/response.meta.json
--rw-r--r--   0        0        0    24428 2023-03-05 14:01:07.986173 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/robotparser.data.json
--rw-r--r--   0        0        0     1719 2023-03-05 14:01:07.986364 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib/robotparser.meta.json
--rw-r--r--   0        0        0    12146 2023-03-05 14:01:08.908762 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/__init__.data.json
--rw-r--r--   0        0        0     2053 2023-03-05 14:01:08.908979 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/__init__.meta.json
--rw-r--r--   0        0        0    25682 2023-03-05 14:01:08.377381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/_collections.data.json
--rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.377576 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/_collections.meta.json
--rw-r--r--   0        0        0    21622 2023-03-05 14:01:08.905784 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/connection.data.json
--rw-r--r--   0        0        0     1917 2023-03-05 14:01:08.905970 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/connection.meta.json
--rw-r--r--   0        0        0    34741 2023-03-05 14:01:08.909756 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/connectionpool.data.json
--rw-r--r--   0        0        0     2239 2023-03-05 14:01:08.909988 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/connectionpool.meta.json
--rw-r--r--   0        0        0     1674 2023-03-05 14:01:08.381426 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/contrib/__init__.data.json
--rw-r--r--   0        0        0     1647 2023-03-05 14:01:08.381594 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/contrib/__init__.meta.json
--rw-r--r--   0        0        0    13461 2023-03-05 14:01:09.061711 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/contrib/socks.data.json
--rw-r--r--   0        0        0     1856 2023-03-05 14:01:09.061908 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/contrib/socks.meta.json
--rw-r--r--   0        0        0    46021 2023-03-05 14:01:08.913260 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/exceptions.data.json
--rw-r--r--   0        0        0     1843 2023-03-05 14:01:08.913492 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/exceptions.meta.json
--rw-r--r--   0        0        0    13505 2023-03-05 14:01:08.378923 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/fields.data.json
--rw-r--r--   0        0        0     1690 2023-03-05 14:01:08.379115 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/fields.meta.json
--rw-r--r--   0        0        0     3293 2023-03-05 14:01:08.904525 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/filepost.data.json
--rw-r--r--   0        0        0     1684 2023-03-05 14:01:08.904757 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/filepost.meta.json
--rw-r--r--   0        0        0     1682 2023-03-05 14:01:08.379440 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/packages/__init__.data.json
--rw-r--r--   0        0        0     1649 2023-03-05 14:01:08.379621 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/packages/__init__.meta.json
--rw-r--r--   0        0        0     2952 2023-03-05 14:01:08.815767 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/packages/ssl_match_hostname/__init__.data.json
--rw-r--r--   0        0        0     1702 2023-03-05 14:01:08.815959 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/packages/ssl_match_hostname/__init__.meta.json
--rw-r--r--   0        0        0    10966 2023-03-05 14:01:08.541195 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/poolmanager.data.json
--rw-r--r--   0        0        0     1715 2023-03-05 14:01:08.541450 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/poolmanager.meta.json
--rw-r--r--   0        0        0     4744 2023-03-05 14:01:08.380339 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/request.data.json
--rw-r--r--   0        0        0     1639 2023-03-05 14:01:08.380524 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/request.meta.json
--rw-r--r--   0        0        0    42034 2023-03-05 14:01:08.910915 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/response.data.json
--rw-r--r--   0        0        0     1970 2023-03-05 14:01:08.911136 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/response.meta.json
--rw-r--r--   0        0        0    13666 2023-03-05 14:01:08.906366 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/__init__.data.json
--rw-r--r--   0        0        0     1869 2023-03-05 14:01:08.906544 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/__init__.meta.json
--rw-r--r--   0        0        0     2948 2023-03-05 14:01:08.380948 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/connection.data.json
--rw-r--r--   0        0        0     1655 2023-03-05 14:01:08.381129 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/connection.meta.json
--rw-r--r--   0        0        0     2526 2023-03-05 14:01:08.699260 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/queue.data.json
--rw-r--r--   0        0        0     1659 2023-03-05 14:01:08.699467 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/queue.meta.json
--rw-r--r--   0        0        0     2227 2023-03-05 14:01:08.403337 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/request.data.json
--rw-r--r--   0        0        0     1649 2023-03-05 14:01:08.403582 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/request.meta.json
--rw-r--r--   0        0        0     1708 2023-03-05 14:01:08.374452 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/response.data.json
--rw-r--r--   0        0        0     1651 2023-03-05 14:01:08.374639 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/response.meta.json
--rw-r--r--   0        0        0    47266 2023-03-05 14:01:08.912150 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/retry.data.json
--rw-r--r--   0        0        0     1849 2023-03-05 14:01:08.912374 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/retry.meta.json
--rw-r--r--   0        0        0     5838 2023-03-05 14:01:08.905048 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/ssl_.data.json
--rw-r--r--   0        0        0     1704 2023-03-05 14:01:08.905229 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/ssl_.meta.json
--rw-r--r--   0        0        0     8569 2023-03-05 14:01:08.908153 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/timeout.data.json
--rw-r--r--   0        0        0     1696 2023-03-05 14:01:08.908359 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/timeout.meta.json
--rw-r--r--   0        0        0    44985 2023-03-05 14:01:08.907590 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/url.data.json
--rw-r--r--   0        0        0     1688 2023-03-05 14:01:08.907803 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/urllib3/util/url.meta.json
--rw-r--r--   0        0        0    35323 2023-03-05 13:59:58.362832 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/uuid.data.json
--rw-r--r--   0        0        0     1760 2023-03-05 13:59:58.363039 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/uuid.meta.json
--rw-r--r--   0        0        0    23606 2023-03-05 13:59:59.074351 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1761 2023-03-05 13:59:59.074594 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    56221 2023-03-05 13:59:58.432763 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/wave.data.json
--rw-r--r--   0        0        0     1758 2023-03-05 13:59:58.433004 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/wave.meta.json
--rw-r--r--   0        0        0   129763 2023-03-05 13:59:58.974457 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/weakref.data.json
--rw-r--r--   0        0        0     1767 2023-03-05 13:59:58.974692 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/weakref.meta.json
--rw-r--r--   0        0        0    28219 2023-03-05 13:59:58.117751 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/webbrowser.data.json
--rw-r--r--   0        0        0     1711 2023-03-05 13:59:58.117974 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/webbrowser.meta.json
--rw-r--r--   0        0        0     1594 2023-03-05 14:01:08.338502 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/__init__.data.json
--rw-r--r--   0        0        0     1627 2023-03-05 14:01:08.338693 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/__init__.meta.json
--rw-r--r--   0        0        0     1626 2023-03-05 14:01:08.051448 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/__init__.data.json
--rw-r--r--   0        0        0     1635 2023-03-05 14:01:08.051639 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/__init__.meta.json
--rw-r--r--   0        0        0   139485 2023-03-05 14:01:08.359031 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/ntsecuritycon.data.json
--rw-r--r--   0        0        0     1685 2023-03-05 14:01:08.359268 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/ntsecuritycon.meta.json
--rw-r--r--   0        0        0    18511 2023-03-05 14:01:08.662627 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/pywintypes.data.json
--rw-r--r--   0        0        0     1738 2023-03-05 14:01:08.662831 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/lib/pywintypes.meta.json
--rw-r--r--   0        0        0   152994 2023-03-05 14:01:08.812178 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32api.data.json
--rw-r--r--   0        0        0     1784 2023-03-05 14:01:08.812399 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32api.meta.json
--rw-r--r--   0        0        0    15962 2023-03-05 14:01:08.783715 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32clipboard.data.json
--rw-r--r--   0        0        0     1681 2023-03-05 14:01:08.783906 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32clipboard.meta.json
--rw-r--r--   0        0        0   168289 2023-03-05 14:01:08.797648 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32security.data.json
--rw-r--r--   0        0        0     1742 2023-03-05 14:01:08.797883 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32/win32security.meta.json
--rw-r--r--   0        0        0    30155 2023-03-05 14:01:08.884498 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32api/__init__.data.json
--rw-r--r--   0        0        0     1658 2023-03-05 14:01:08.884685 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32api/__init__.meta.json
--rw-r--r--   0        0        0     6929 2023-03-05 14:01:08.881569 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32clipboard/__init__.data.json
--rw-r--r--   0        0        0     1676 2023-03-05 14:01:08.881773 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32clipboard/__init__.meta.json
--rw-r--r--   0        0        0    65049 2023-03-05 14:01:08.883381 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32security/__init__.data.json
--rw-r--r--   0        0        0     1673 2023-03-05 14:01:08.883578 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/win32security/__init__.meta.json
--rw-r--r--   0        0        0     2320 2023-03-05 13:59:58.228375 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/winreg.data.json
--rw-r--r--   0        0        0     1712 2023-03-05 13:59:58.228565 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/winreg.meta.json
--rw-r--r--   0        0        0     1679 2023-03-05 13:59:59.787437 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/__init__.data.json
--rw-r--r--   0        0        0     1710 2023-03-05 13:59:59.787667 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/__init__.meta.json
--rw-r--r--   0        0        0    26139 2023-03-05 13:59:59.447948 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/__init__.data.json
--rw-r--r--   0        0        0     1721 2023-03-05 13:59:59.448143 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/__init__.meta.json
--rw-r--r--   0        0        0     5029 2023-03-05 13:59:58.986959 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/domreg.data.json
--rw-r--r--   0        0        0     1721 2023-03-05 13:59:58.987213 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/domreg.meta.json
--rw-r--r--   0        0        0    65369 2023-03-05 14:00:01.062328 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.data.json
--rw-r--r--   0        0        0     1851 2023-03-05 14:00:01.062598 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/expatbuilder.meta.json
--rw-r--r--   0        0        0   158529 2023-03-05 14:00:01.066721 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/minidom.data.json
--rw-r--r--   0        0        0     1936 2023-03-05 14:00:01.066932 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/minidom.meta.json
--rw-r--r--   0        0        0    35261 2023-03-05 14:00:01.063373 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.data.json
--rw-r--r--   0        0        0     1852 2023-03-05 14:00:01.063576 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/dom/xmlbuilder.meta.json
--rw-r--r--   0        0        0     1747 2023-03-05 13:59:59.540738 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/parsers/__init__.data.json
--rw-r--r--   0        0        0     1732 2023-03-05 13:59:59.540924 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/parsers/__init__.meta.json
--rw-r--r--   0        0        0     3195 2023-03-05 13:59:59.303774 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.data.json
--rw-r--r--   0        0        0     1733 2023-03-05 13:59:59.303959 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/parsers/expat/__init__.meta.json
--rw-r--r--   0        0        0    18310 2023-03-05 13:59:58.852394 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/__init__.data.json
--rw-r--r--   0        0        0     1823 2023-03-05 13:59:58.852582 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/__init__.meta.json
--rw-r--r--   0        0        0    19177 2023-03-05 13:59:57.914888 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/handler.data.json
--rw-r--r--   0        0        0     1689 2023-03-05 13:59:57.915089 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/handler.meta.json
--rw-r--r--   0        0        0    24582 2023-03-05 13:59:58.243941 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.data.json
--rw-r--r--   0        0        0     1685 2023-03-05 13:59:58.244178 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/xml/sax/xmlreader.meta.json
--rw-r--r--   0        0        0    72877 2023-03-05 13:59:58.408739 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1829 2023-03-05 13:59:58.408945 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    13835 2023-03-05 13:59:58.044500 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zipimport.data.json
--rw-r--r--   0        0        0     1777 2023-03-05 13:59:58.044736 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zipimport.meta.json
--rw-r--r--   0        0        0    18083 2023-03-05 13:59:58.359414 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zlib.data.json
--rw-r--r--   0        0        0     1759 2023-03-05 13:59:58.359609 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zlib.meta.json
--rw-r--r--   0        0        0    33030 2023-03-05 14:00:01.007795 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/__init__.data.json
--rw-r--r--   0        0        0     1751 2023-03-05 14:00:01.007967 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/__init__.meta.json
--rw-r--r--   0        0        0    69457 2023-03-05 14:00:01.951668 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/_future.data.json
--rw-r--r--   0        0        0     2277 2023-03-05 14:00:01.951940 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/_future.meta.json
--rw-r--r--   0        0        0     1795 2023-03-05 13:59:58.036894 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/_typing.data.json
--rw-r--r--   0        0        0     1658 2023-03-05 13:59:58.037124 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/_typing.meta.json
--rw-r--r--   0        0        0    17089 2023-03-05 14:00:03.788290 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/asyncio.data.json
--rw-r--r--   0        0        0     2334 2023-03-05 14:00:03.788515 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/asyncio.meta.json
--rw-r--r--   0        0        0    38399 2023-03-05 14:00:01.000376 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/backend/__init__.data.json
--rw-r--r--   0        0        0     1978 2023-03-05 14:00:01.000634 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/backend/__init__.meta.json
--rw-r--r--   0        0        0     2757 2023-03-05 13:59:57.920517 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/backend/select.data.json
--rw-r--r--   0        0        0     1673 2023-03-05 13:59:57.920717 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/backend/select.meta.json
--rw-r--r--   0        0        0   177007 2023-03-05 13:59:58.875313 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/constants.data.json
--rw-r--r--   0        0        0     1803 2023-03-05 13:59:58.875567 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/constants.meta.json
--rw-r--r--   0        0        0    17018 2023-03-05 14:00:00.998965 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/error.data.json
--rw-r--r--   0        0        0     1908 2023-03-05 14:00:00.999151 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/error.meta.json
--rw-r--r--   0        0        0     2191 2023-03-05 14:00:03.788948 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/eventloop/__init__.data.json
--rw-r--r--   0        0        0     1840 2023-03-05 14:00:03.789227 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/eventloop/__init__.meta.json
--rw-r--r--   0        0        0    65591 2023-03-05 14:00:03.803470 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/eventloop/zmqstream.data.json
--rw-r--r--   0        0        0     2509 2023-03-05 14:01:11.376379 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/eventloop/zmqstream.meta.json
--rw-r--r--   0        0        0     4243 2023-03-05 14:00:01.006876 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/__init__.data.json
--rw-r--r--   0        0        0     1883 2023-03-05 14:00:01.007061 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/__init__.meta.json
--rw-r--r--   0        0        0    10283 2023-03-05 14:00:00.998176 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/attrsettr.data.json
--rw-r--r--   0        0        0     1782 2023-03-05 14:00:00.998453 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/attrsettr.meta.json
--rw-r--r--   0        0        0    50766 2023-03-05 14:00:01.006420 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/context.data.json
--rw-r--r--   0        0        0     2174 2023-03-05 14:00:01.006628 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/context.meta.json
--rw-r--r--   0        0        0     7720 2023-03-05 14:00:01.002413 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/frame.data.json
--rw-r--r--   0        0        0     1767 2023-03-05 14:00:01.002579 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/frame.meta.json
--rw-r--r--   0        0        0    10246 2023-03-05 14:00:01.001953 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/poll.data.json
--rw-r--r--   0        0        0     1837 2023-03-05 14:00:01.002121 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/poll.meta.json
--rw-r--r--   0        0        0    93213 2023-03-05 14:00:01.004930 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/socket.data.json
--rw-r--r--   0        0        0     2247 2023-03-05 14:00:01.005216 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/socket.meta.json
--rw-r--r--   0        0        0     7030 2023-03-05 14:00:01.001442 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/tracker.data.json
--rw-r--r--   0        0        0     1762 2023-03-05 14:00:01.001613 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/tracker.meta.json
--rw-r--r--   0        0        0     8454 2023-03-05 14:00:01.000975 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/version.data.json
--rw-r--r--   0        0        0     1833 2023-03-05 14:00:01.001154 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/sugar/version.meta.json
--rw-r--r--   0        0        0     1620 2023-03-05 13:59:58.036201 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/__init__.data.json
--rw-r--r--   0        0        0     1628 2023-03-05 13:59:58.036407 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/__init__.meta.json
--rw-r--r--   0        0        0     2190 2023-03-05 13:59:57.870736 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/interop.data.json
--rw-r--r--   0        0        0     1824 2023-03-05 14:01:08.865530 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/interop.meta.json
--rw-r--r--   0        0        0     4472 2023-03-05 13:59:59.236169 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/jsonapi.data.json
--rw-r--r--   0        0        0     1809 2023-03-05 13:59:59.236385 alacorder-79.6.9/src/alacorder/.mypy_cache/3.10/zmq/utils/jsonapi.meta.json
--rw-r--r--   0        0        0      190 2023-03-05 14:00:04.569522 alacorder-79.6.9/src/alacorder/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.6.9/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.6.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   140423 2023-04-23 13:49:18.357735 alacorder-79.6.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   140423 2023-04-23 13:49:11.638569 alacorder-79.6.9/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.6.9/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10268 1970-01-01 00:00:00.000000 alacorder-79.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.7.0/LICENSE
+-rw-r--r--   0        0        0     9378 2023-04-22 21:04:19.345850 alacorder-79.7.0/README.md
+-rw-r--r--   0        0        0      679 2023-04-23 16:40:28.032022 alacorder-79.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9208 2023-04-21 18:06:44.921207 alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb
+-rw-r--r--   0        0        0   138382 2023-04-21 18:24:49.412475 alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.7.0/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.7.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   139978 2023-04-23 16:40:07.746618 alacorder-79.7.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   139978 2023-04-23 16:40:14.007977 alacorder-79.7.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.7.0/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10268 1970-01-01 00:00:00.000000 alacorder-79.7.0/PKG-INFO
```

### Comparing `alacorder-79.6.9/LICENSE` & `alacorder-79.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.9/README.md` & `alacorder-79.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.9/pyproject.toml` & `alacorder-79.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.6.9"
+version = "79.7.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.6.9/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb` & `alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/AlacorderMessinAround-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-79.7.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.9/src/alacorder/__init__.py` & `alacorder-79.7.0/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.6.9/src/alacorder/__main__.py` & `alacorder-79.7.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.9"
+version = "79.7.0"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -48,26 +48,24 @@
 
 prt = print
 
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
-        if cf == None:
-            prt(msg)
-        elif type(cf) == bool and cf:
-            prt(msg)
-        elif type(cf) != bool:
+        if isinstance(cf, pl.dataframe.frame.DataFrame):
             try:
-                bl = cf["LOG"]
-                print(bl)
-                if bl:
+                if cf['LOG']:
                     prt(msg)
             except:
-                pass
+                prt(msg)
+        elif cf == None:
+            prt(msg)
+        elif type(cf) == bool and cf:
+            prt(msg)
     elif len(msg) > 1:
         for m in msg:
             if cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
             elif type(cf) != bool:
@@ -525,14 +523,15 @@
                     count = 0
                 try:
                     cf = set(
                         window["TB-INPUTPATH"].get(),
                         window["TB-OUTPUTPATH"].get(),
                         count=count,
                         table=tabl,
+                        log=True,
                         overwrite=window["TB-OVERWRITE"].get(),
                         no_prompt=True,
                         debug=False,
                         archive=False,
                         window=window,
                     )
                 except:
@@ -560,14 +559,15 @@
                 count = 0
             try:
                 cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
+                    log=True,
                     overwrite=window["MA-OVERWRITE"].get(),
                     append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
@@ -840,51 +840,59 @@
     "--no-prompt",
     "-s",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+    )
+@click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
-    input_path, output_path, count, table, overwrite, no_write, no_prompt, debug
+    input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write data tables to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to table output
         count (int): Total cases to pull from input
         table (str): Table (all, cases, fees, charges, settings, witnesses, attorneys, case_action_summaries, images)
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
+    log = not no_log
     if os.path.splitext(output_path)[1] in (".xls", ".xlsx") and not bool(table):
         table = "all"
     elif os.path.splitext(output_path)[1] not in (".xls", ".xlsx") and not bool(table):
         table = click.prompt(
             "Table export choice (cases, fees, charges, disposition, filing, attorneys, witnesses, images, case-action-summary, settings)"
         )
     cf = set(
         input_path,
         output_path,
         count=count,
         table=table,
         overwrite=overwrite,
         no_write=no_write,
+        log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf, debug=debug)
     return o
@@ -927,48 +935,56 @@
     is_flag=True,
     help="Attempt to append to existing file at output path",
 )
 @click.option(
     "--no-write", "-n", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+    )
+@click.option(
     "--no-prompt",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def cli_archive(
-    input_path, output_path, count, overwrite, append, no_write, no_prompt, debug
+    input_path, output_path, count, overwrite, append, no_write, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
         overwrite (bool): Overwrite existing files at output path
         append (bool): Attempt to append to existing file at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console for developers
     """
+    log = not no_log
     cf = set(
         input_path,
         output_path,
         archive=True,
         count=count,
         overwrite=overwrite,
         no_write=no_write,
+        log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if debug:
         click.echo(cf)
     o = archive(cf, debug=debug)
     return o
@@ -1532,15 +1548,15 @@
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
     }
     dlog(out, cf=debug)
     if now:
-        return init(out, window=window, debug=debug)
+        return init(out, debug=debug)
     return out
 
 
 def read(cf=""):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
@@ -1853,15 +1869,17 @@
             )
             .str.replace_all("Case Number:", "", literal=True)
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(SSN)(.+)(Alias)", group_index=2)
-            .str.replace_all(r"(SSN|Alias)", "")
+            .str.replace(r"(SSN)", "")
+            .str.replace(r"Alias","")
+            .str.replace(r"\:","")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
             .alias("DOB"),
@@ -2649,28 +2667,23 @@
             .arr.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
             pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
             pl.col("SPACE_SEP").arr.get(5).alias("Code"),
             pl.col("SPACE_SEP").arr.get(6).alias("Payor2"),
             pl.col("SPACE_SEP").arr.get(7).alias("Payee2"),
-            # pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", "").alias("Balance"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
             pl.when(pl.col("AdminFee1") != "ACTIVE")
             .then(True)
             .otherwise(False)
             .alias("Total"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
-            .then("")
-            .otherwise(pl.col("AdminFee1"))
-            .alias("AdminFee"),
             pl.when(pl.col("Payor2").str.contains(r"[^R0-9]\d{3}").is_not())
             .then(pl.lit(""))
             .otherwise(pl.col("Payor2"))
             .alias("Payor1"),
             pl.when(pl.col("Payor2").str.contains(r"[^R0-9]\d{3}").is_not())
             .then(pl.col("Payor2"))
             .otherwise(pl.col("Payee2"))
@@ -2685,47 +2698,34 @@
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
         pl.when(pl.col("Total")==True)
         .then(pl.col("FEE_SEP").arr.get(-1))
         .otherwise(pl.col("AmtHold2"))
-        .alias("AmtHold"),
-        pl.when(pl.col("Total")==True)
-        .then(pl.col("AmtHold2"))
-        .otherwise(pl.col("FEE_SEP").arr.get(-1))
-        .alias("Balance")
+        .alias("AmtHold")
         )
     dlog(out.columns, out.shape, cf=debug)
-    out = out.with_columns(
+    out = out.select(
         [
             pl.col("CaseNumber"),
             pl.col("Total"),
-            pl.col("AdminFee"),
-            pl.when(pl.col("FeeStatus2").str.contains("$", literal=True))
-            .then(pl.lit(None))
-            .otherwise(pl.col("FeeStatus2"))
-            .alias("FeeStatus"),
             pl.col("Code"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
-            .then("")
-            .otherwise(pl.col("Payor1"))
-            .alias("Payor"),
-            pl.when(pl.col("Payee1").str.contains(r"\$"))
-            .then("")
-            .otherwise(pl.col("Payee1"))
-            .alias("Payee"),
             pl.col("AmtDue").str.strip().cast(pl.Float64, strict=False),
             pl.col("AmtPaid").str.strip().cast(pl.Float64, strict=False),
-            pl.col("Balance").str.strip().cast(pl.Float64, strict=False),
-            pl.col("AmtHold").str.replace("$","",literal=True).str.strip().cast(pl.Float64, strict=False),
+        ]
+    )
+    out = out.with_columns(
+        [
+            pl.col("AmtDue").sub(pl.col("AmtPaid")).alias("Balance")
         ]
     )
     dlog(out.columns, out.shape, cf=debug)
-    out = out.drop_nulls("Balance")
+    out = out.fill_null('')
+    out = out.drop_nulls('AmtDue')
     return out
 
 
 def explode_images(df, debug=False):
     images = df.select(
         [
             pl.concat_str(
@@ -2788,17 +2788,18 @@
             .alias("CASChunk"),
         ]
     )
     cas = cas.select(
         [
             pl.col("CaseNumber"),
             pl.col("CASChunk")
-            .str.replace_all(
+            .str.replace(
                 r"© Alacourt\.com|Date: Description Doc# Title|Operator", ""
             )
+            .str.replace(r'Date\: Time Code CommentsCase Action Summary','')
             .str.strip()
             .str.rstrip()
             .str.split("\n")
             .alias("CaseActionSummary"),
         ]
     )
     cas = cas.explode("CaseActionSummary")
```

### Comparing `alacorder-79.6.9/src/alacorder/alac.py` & `alacorder-79.7.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tqdm, 
     xlsxwriter, 
     xlsx2csv
 
 """
 
 name = "ALACORDER"
-version = "79.6.9"
+version = "79.7.0"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 if autoload_graphical_user_interface:
     import PySimpleGUI as sg
 
@@ -48,26 +48,24 @@
 
 prt = print
 
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
-        if cf == None:
-            prt(msg)
-        elif type(cf) == bool and cf:
-            prt(msg)
-        elif type(cf) != bool:
+        if isinstance(cf, pl.dataframe.frame.DataFrame):
             try:
-                bl = cf["LOG"]
-                print(bl)
-                if bl:
+                if cf['LOG']:
                     prt(msg)
             except:
-                pass
+                prt(msg)
+        elif cf == None:
+            prt(msg)
+        elif type(cf) == bool and cf:
+            prt(msg)
     elif len(msg) > 1:
         for m in msg:
             if cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
             elif type(cf) != bool:
@@ -525,14 +523,15 @@
                     count = 0
                 try:
                     cf = set(
                         window["TB-INPUTPATH"].get(),
                         window["TB-OUTPUTPATH"].get(),
                         count=count,
                         table=tabl,
+                        log=True,
                         overwrite=window["TB-OVERWRITE"].get(),
                         no_prompt=True,
                         debug=False,
                         archive=False,
                         window=window,
                     )
                 except:
@@ -560,14 +559,15 @@
                 count = 0
             try:
                 cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
+                    log=True,
                     overwrite=window["MA-OVERWRITE"].get(),
                     append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
@@ -840,51 +840,59 @@
     "--no-prompt",
     "-s",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+    )
+@click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
-    input_path, output_path, count, table, overwrite, no_write, no_prompt, debug
+    input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write data tables to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to table output
         count (int): Total cases to pull from input
         table (str): Table (all, cases, fees, charges, settings, witnesses, attorneys, case_action_summaries, images)
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
+    log = not no_log
     if os.path.splitext(output_path)[1] in (".xls", ".xlsx") and not bool(table):
         table = "all"
     elif os.path.splitext(output_path)[1] not in (".xls", ".xlsx") and not bool(table):
         table = click.prompt(
             "Table export choice (cases, fees, charges, disposition, filing, attorneys, witnesses, images, case-action-summary, settings)"
         )
     cf = set(
         input_path,
         output_path,
         count=count,
         table=table,
         overwrite=overwrite,
         no_write=no_write,
+        log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf, debug=debug)
     return o
@@ -927,48 +935,56 @@
     is_flag=True,
     help="Attempt to append to existing file at output path",
 )
 @click.option(
     "--no-write", "-n", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+    )
+@click.option(
     "--no-prompt",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def cli_archive(
-    input_path, output_path, count, overwrite, append, no_write, no_prompt, debug
+    input_path, output_path, count, overwrite, append, no_write, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
         overwrite (bool): Overwrite existing files at output path
         append (bool): Attempt to append to existing file at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console for developers
     """
+    log = not no_log
     cf = set(
         input_path,
         output_path,
         archive=True,
         count=count,
         overwrite=overwrite,
         no_write=no_write,
+        log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if debug:
         click.echo(cf)
     o = archive(cf, debug=debug)
     return o
@@ -1532,15 +1548,15 @@
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
     }
     dlog(out, cf=debug)
     if now:
-        return init(out, window=window, debug=debug)
+        return init(out, debug=debug)
     return out
 
 
 def read(cf=""):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
@@ -1853,15 +1869,17 @@
             )
             .str.replace_all("Case Number:", "", literal=True)
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(SSN)(.+)(Alias)", group_index=2)
-            .str.replace_all(r"(SSN|Alias)", "")
+            .str.replace(r"(SSN)", "")
+            .str.replace(r"Alias","")
+            .str.replace(r"\:","")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
             .alias("DOB"),
@@ -2649,28 +2667,23 @@
             .arr.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
             pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
             pl.col("SPACE_SEP").arr.get(5).alias("Code"),
             pl.col("SPACE_SEP").arr.get(6).alias("Payor2"),
             pl.col("SPACE_SEP").arr.get(7).alias("Payee2"),
-            # pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", "").alias("Balance"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
             pl.when(pl.col("AdminFee1") != "ACTIVE")
             .then(True)
             .otherwise(False)
             .alias("Total"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
-            .then("")
-            .otherwise(pl.col("AdminFee1"))
-            .alias("AdminFee"),
             pl.when(pl.col("Payor2").str.contains(r"[^R0-9]\d{3}").is_not())
             .then(pl.lit(""))
             .otherwise(pl.col("Payor2"))
             .alias("Payor1"),
             pl.when(pl.col("Payor2").str.contains(r"[^R0-9]\d{3}").is_not())
             .then(pl.col("Payor2"))
             .otherwise(pl.col("Payee2"))
@@ -2685,47 +2698,34 @@
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
         pl.when(pl.col("Total")==True)
         .then(pl.col("FEE_SEP").arr.get(-1))
         .otherwise(pl.col("AmtHold2"))
-        .alias("AmtHold"),
-        pl.when(pl.col("Total")==True)
-        .then(pl.col("AmtHold2"))
-        .otherwise(pl.col("FEE_SEP").arr.get(-1))
-        .alias("Balance")
+        .alias("AmtHold")
         )
     dlog(out.columns, out.shape, cf=debug)
-    out = out.with_columns(
+    out = out.select(
         [
             pl.col("CaseNumber"),
             pl.col("Total"),
-            pl.col("AdminFee"),
-            pl.when(pl.col("FeeStatus2").str.contains("$", literal=True))
-            .then(pl.lit(None))
-            .otherwise(pl.col("FeeStatus2"))
-            .alias("FeeStatus"),
             pl.col("Code"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
-            .then("")
-            .otherwise(pl.col("Payor1"))
-            .alias("Payor"),
-            pl.when(pl.col("Payee1").str.contains(r"\$"))
-            .then("")
-            .otherwise(pl.col("Payee1"))
-            .alias("Payee"),
             pl.col("AmtDue").str.strip().cast(pl.Float64, strict=False),
             pl.col("AmtPaid").str.strip().cast(pl.Float64, strict=False),
-            pl.col("Balance").str.strip().cast(pl.Float64, strict=False),
-            pl.col("AmtHold").str.replace("$","",literal=True).str.strip().cast(pl.Float64, strict=False),
+        ]
+    )
+    out = out.with_columns(
+        [
+            pl.col("AmtDue").sub(pl.col("AmtPaid")).alias("Balance")
         ]
     )
     dlog(out.columns, out.shape, cf=debug)
-    out = out.drop_nulls("Balance")
+    out = out.fill_null('')
+    out = out.drop_nulls('AmtDue')
     return out
 
 
 def explode_images(df, debug=False):
     images = df.select(
         [
             pl.concat_str(
@@ -2788,17 +2788,18 @@
             .alias("CASChunk"),
         ]
     )
     cas = cas.select(
         [
             pl.col("CaseNumber"),
             pl.col("CASChunk")
-            .str.replace_all(
+            .str.replace(
                 r"© Alacourt\.com|Date: Description Doc# Title|Operator", ""
             )
+            .str.replace(r'Date\: Time Code CommentsCase Action Summary','')
             .str.strip()
             .str.rstrip()
             .str.split("\n")
             .alias("CaseActionSummary"),
         ]
     )
     cas = cas.explode("CaseActionSummary")
```

### Comparing `alacorder-79.6.9/PKG-INFO` & `alacorder-79.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.6.9
+Version: 79.7.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

