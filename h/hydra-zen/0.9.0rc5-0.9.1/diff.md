# Comparing `tmp/hydra_zen-0.9.0rc5.tar.gz` & `tmp/hydra_zen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_zen-0.9.0rc5.tar", last modified: Fri Dec  9 19:36:46 2022, max compression
+gzip compressed data, was "hydra_zen-0.9.1.tar", last modified: Fri Jan 13 14:27:58 2023, max compression
```

## Comparing `hydra_zen-0.9.0rc5.tar` & `hydra_zen-0.9.1.tar`

### file list

```diff
@@ -1,131 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.095935 hydra_zen-0.9.0rc5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.099935 hydra_zen-0.9.0rc5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/workflows/test_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.github/workflows/tox_run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/SPDX.spdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.099935 hydra_zen-0.9.0rc5/brand/
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen - favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   217449 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full.png
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full.svg
--rw-r--r--   0 runner    (1001) docker     (123)   143262 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd.png
--rw-r--r--   0 runner    (1001) docker     (123)    29376 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd_smaller.png
--rw-r--r--   0 runner    (1001) docker     (123)   140126 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_light_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_light_blue_smaller.png
--rw-r--r--   0 runner    (1001) docker     (123)   170855 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_blue.svg
--rw-r--r--   0 runner    (1001) docker     (123)   186684 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_border.png
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_border.svg
--rw-r--r--   0 runner    (1001) docker     (123)   143698 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_transparent.png
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/HydraZen_logo_transparent.svg
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/hydra_zen_favicon_32x32.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/brand/hydra_zen_favicon_64x64.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.103935 hydra_zen-0.9.0rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.103935 hydra_zen-0.9.0rc5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.103935 hydra_zen-0.9.0rc5/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/_static/gtag.js
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/_static/hydra_zen_favicon_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/_static/hydra_zen_favicon_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36125 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.103935 hydra_zen-0.9.0rc5/docs/source/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/explanation/dont_repeat_yourself.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/explanation/hydrated_dataclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/explanation/type_refinement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/explanation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.ZenField.rst
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.ZenStore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.builds.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.get_target.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.hydrated_dataclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.instantiate.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.is_partial_builds.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.just.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.launch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.load_from_yaml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.make_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.make_custom_builds_fn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.save_as_yaml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.third_party.beartype.validates_with_beartype.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.third_party.pydantic.validates_with_pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.to_yaml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.typing.ZenConvert.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.uses_zen_processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.wrapper.Zen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.wrapper.default_to_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.zen.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/docs/source/how_to/
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/how_to/beartype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/how_to/partial_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/how_to/pytorch_lightning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/how_tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials/add_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials/basic_app.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials/config_groups.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials/hierarchy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials/inject_wrapper.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/docs/source/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.095935 hydra_zen-0.9.0rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/src/hydra_zen/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_hydra_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/src/hydra_zen/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_utils/coerce.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-09 19:36:45.000000 hydra_zen-0.9.0rc5/src/hydra_zen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    79189 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_implementations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_just.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_make_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_make_custom_builds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_value_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/src/hydra_zen/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/third_party/beartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/third_party/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/src/hydra_zen/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16569 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/typing/_builds_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/typing/_implementations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.111935 hydra_zen-0.9.0rc5/src/hydra_zen/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51513 2022-12-09 19:36:30.000000 hydra_zen-0.9.0rc5/src/hydra_zen/wrapper/_implementations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 19:36:46.107935 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-09 19:36:46.000000 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2022-12-09 19:36:46.000000 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 19:36:46.000000 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-09 19:36:46.000000 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-09 19:36:46.000000 hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.156278 hydra_zen-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.156278 hydra_zen-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.github/workflows/tox_run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/SPDX.spdx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/brand/
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen - favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   217449 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   143262 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29376 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd_smaller.png
+-rw-r--r--   0 runner    (1001) docker     (123)   140126 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_light_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_light_blue_smaller.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170855 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_blue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   186684 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_border.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_border.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   143698 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/HydraZen_logo_transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/hydra_zen_favicon_32x32.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/brand/hydra_zen_favicon_64x64.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/deps/requirements-pyright.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/_static/gtag.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/_static/hydra_zen_favicon_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/_static/hydra_zen_favicon_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    41902 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.160278 hydra_zen-0.9.1/docs/source/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/explanation/dont_repeat_yourself.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/explanation/hydrated_dataclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/explanation/type_refinement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/explanation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.ZenField.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.ZenStore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.builds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.get_target.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.hydrated_dataclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.instantiate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.is_partial_builds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.just.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.launch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.load_from_yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.make_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.make_custom_builds_fn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.save_as_yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.third_party.beartype.validates_with_beartype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.third_party.pydantic.validates_with_pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.to_yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.typing.DataclassOptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.typing.ZenConvert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.uses_zen_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.wrapper.Zen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.wrapper.default_to_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/generated/hydra_zen.zen.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/docs/source/how_to/
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/how_to/beartype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/how_to/partial_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/how_to/pytorch_lightning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/how_tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials/add_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials/basic_app.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials/config_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials/hierarchy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials/inject_wrapper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/docs/source/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.152278 hydra_zen-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/src/hydra_zen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/_hydra_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/_launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/src/hydra_zen/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/_utils/coerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/src/hydra_zen/structured_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88010 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_just.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_make_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_make_custom_builds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23334 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/structured_configs/_value_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/src/hydra_zen/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/third_party/beartype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/third_party/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/src/hydra_zen/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/typing/_builds_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/typing/_implementations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.168278 hydra_zen-0.9.1/src/hydra_zen/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54024 2023-01-13 14:27:42.000000 hydra_zen-0.9.1/src/hydra_zen/wrapper/_implementations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 14:27:58.164278 hydra_zen-0.9.1/src/hydra_zen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-13 14:27:58.000000 hydra_zen-0.9.1/src/hydra_zen.egg-info/top_level.txt
```

### Comparing `hydra_zen-0.9.0rc5/.github/workflows/publish_docs.yml` & `hydra_zen-0.9.1/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/.github/workflows/pypi_publish.yml` & `hydra_zen-0.9.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/.github/workflows/test_docs.yml` & `hydra_zen-0.9.1/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/.github/workflows/tox_run.yml` & `hydra_zen-0.9.1/.github/workflows/tox_run.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 jobs:
   tests:
     runs-on: ubuntu-latest
 
     strategy:
       max-parallel: 5
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.7, 3.8, 3.9, "3.10", 3.11]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
@@ -51,18 +51,18 @@
     - name: Test with tox
       run: tox -e py38
 
   coverage:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.8
+    - name: Set up Python 3.10
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox
     - name: Measure coverage
       run: tox -e coverage
   
@@ -79,15 +79,15 @@
         python -m pip install --upgrade pip
         pip install tox
     - name: Cache tox environments
       id: cache-third-party
       uses: actions/cache@v3
       with:
         path: .tox
-        key: tox-pyright-docs-${{ hashFiles('setup.cfg') }}-${{ hashFiles('setup.py') }}-${{ hashFiles('tests/conftest.py') }}-${{ hashFiles('.github/workflows/tox.yml') }}
+        key: tox-pyright-docs-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('deps/requirements-pyright.txt') }}-${{ hashFiles('.github/workflows/tox.yml') }}
     - name: Scan docs with pyright
       run: tox -e pyright-scan-docs
 
   test-third-party:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
@@ -100,15 +100,15 @@
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Cache tox environments
       id: cache-third-party
       uses: actions/cache@v3
       with:
         path: .tox
-        key: tox-third-party-${{ hashFiles('setup.cfg') }}-${{ hashFiles('setup.py') }}-${{ hashFiles('tests/conftest.py') }}-${{ hashFiles('.github/workflows/tox.yml') }}
+        key: tox-third-party-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('tests/conftest.py') }}-${{ hashFiles('.github/workflows/tox.yml') }}
     - name: Test with tox
       run: tox -e third-party
 
   test-minimum-dependencies:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
@@ -124,109 +124,84 @@
       run: tox -e min-deps
 
 
   test-against-pre-releases-of-dependencies:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
       run: tox -e pre-release
 
-  test-against-hydra-1_1_2dev:
+  test-against-omegaconf-2p2p2:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
         python-version: 3.8
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
-      run: tox -e hydra-1p1p2-pre-release
+      run: tox -e omegaconf-2p2p2
 
-  test-against-omegaconf-2p2p2:
+  check-repo-format:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
-      run: tox -e omegaconf-2p2p2
+      run: tox -e enforce-format
 
-  check-repo-format:
+  run-pyright:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
-      run: tox -e enforce-format
+      run: tox -e pyright
 
-  run-pyright:
+  test-docs-builds:
     runs-on: ubuntu-latest
-
     steps:
     - uses: actions/checkout@v3
-
-    - uses: actions/setup-node@v3.5.1
-      with:
-        node-version: ${{ env.NODE_VERSION }}
-
-    - name: Cache node modules
-      id: cache-npm
-      uses: actions/cache@v3
-      env:
-        cache-name: cache-node-modules
-      with:
-        # npm cache files are stored in `~/.npm` on Linux/macOS
-        path: ~/.npm
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/package-lock.json') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
-
-    - name: Install pyright
-      run: sudo npm install -g pyright@"<1.1.283"
-    - uses: actions/checkout@v3
-    - name: Set up Python
+    - name: Set up Python 3.9
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .
-    - name: Run pyright basic on src
-      run: pyright --lib tests/annotations/ src/
-    - name: (pyright) verify type completeness
-      run: pyright --ignoreexternal --verifytypes hydra_zen
+        pip install tox tox-gh-actions
+    - name: Test with tox
+      run: tox -e docs
 
   run-mypy:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
```

### Comparing `hydra_zen-0.9.0rc5/.gitignore` & `hydra_zen-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/CONTRIBUTING.md` & `hydra_zen-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/LICENSE.txt` & `hydra_zen-0.9.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Massachusetts Institute of Technology
+Copyright (c) 2023 Massachusetts Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hydra_zen-0.9.0rc5/PKG-INFO` & `hydra_zen-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra_zen
-Version: 0.9.0rc5
+Version: 0.9.1
 Summary: Configurable, reproducible, and scalable workflows in Python, via Hydra
 Author-email: Ryan Soklaski <ryan.soklaski@ll.mit.edu>, Justin Goodwin <jgoodwin@ll.mit.edu>
 Maintainer-email: Ryan Soklaski <ryan.soklaski@ll.mit.edu>
 License: MIT
 Project-URL: Homepage, https://mit-ll-responsible-ai.github.io/hydra-zen/
 Project-URL: Bug Reports, https://github.com/mit-ll-responsible-ai/hydra-zen/issues
 Project-URL: Source, https://github.com/mit-ll-responsible-ai/hydra-zen
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: pydantic
 Provides-Extra: beartype
@@ -31,15 +32,15 @@
 
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/hydra-zen">
     <img src="https://img.shields.io/pypi/v/hydra-zen.svg" alt="PyPI" />
   </a>
   <a>
-    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.10-blue.svg" alt="Python version support" />
+    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.11-blue.svg" alt="Python version support" />
   </a>
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://github.com/mit-ll-responsible-ai/hydra-zen/workflows/Tests/badge.svg" alt="GitHub Actions" />
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://img.shields.io/badge/coverage-100%25-green.svg" alt="Code Coverage" />
   <a href="https://github.com/microsoft/pyright/blob/92b4028cd5fd483efcf3f1cdb8597b2d4edd8866/docs/typed-libraries.md#verifying-type-completeness">
     <img src="https://img.shields.io/badge/type%20completeness-100%25-green.svg" alt="Type-Completeness Score" />
@@ -109,15 +110,15 @@
 }
 ```
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
-© 2022 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+© 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
     
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: MIT
     
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: hydra_zen Version: 0.9.0rc5 Summary: Configurable,
+Metadata-Version: 2.1 Name: hydra_zen Version: 0.9.1 Summary: Configurable,
 reproducible, and scalable workflows in Python, via Hydra Author-email: Ryan
 Soklaski
 soklaski@ll.mit.edu>, Justin Goodwin
 ll.mit.edu> Maintainer-email: Ryan Soklaski
 soklaski@ll.mit.edu> License: MIT Project-URL: Homepage, https://mit-ll-
 responsible-ai.github.io/hydra-zen/ Project-URL: Bug Reports, https://
 github.com/mit-ll-responsible-ai/hydra-zen/issues Project-URL: Source, https://
 github.com/mit-ll-responsible-ai/hydra-zen Keywords: machine
 learning,research,configuration,scalable,reproducible,yaml,Hydra,dataclass
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering Classifier:
-Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: test Provides-Extra: pydantic
-Provides-Extra: beartype License-File: LICENSE.txt # hydra-zen ![image](brand/
-Hydra-Zen_logo_full_filled_bkgrnd_small.png)
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering Classifier: Programming Language :: Python :: 3
+:: Only Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: pydantic Provides-Extra: beartype License-
+File: LICENSE.txt # hydra-zen ![image](brand/Hydra-
+Zen_logo_full_filled_bkgrnd_small.png)
                        [PyPI] [Python version support]
                                [GitHub_Actions]
                                [Code_Coverage]
          [Type-Completeness_Score]_[Tested_with_Hypothesis]_[Cite_Us]
 A_library_that_facilitates_configurable,_reproducible,_and_scalable_workflows,
                                  using_Hydra.
                Check_out_our_documentation_for_more_information.
@@ -51,15 +52,15 @@
 the Discussion Share ideas, ask questions, and chat with us over at [hydra-
 zen's discussion board](https://github.com/mit-ll-responsible-ai/hydra-zen/
 discussions). ## Citation Using `hydra-zen` for your research? Please cite the
 following publication: ``` @article{soklaski2022tools, title={Tools and
 Practices for Responsible AI Engineering}, author={Soklaski, Ryan and Goodwin,
 Justin and Brown, Olivia and Yee, Michael and Matterer, Jason}, journal={arXiv
 preprint arXiv:2201.05647}, year={2022} } ``` ## Disclaimer DISTRIBUTION
-STATEMENT A. Approved for public release: distribution unlimited. Â© 2022
+STATEMENT A. Approved for public release: distribution unlimited. Â© 2023
 MASSACHUSETTS INSTITUTE OF TECHNOLOGY Subject to FAR 52.227-11 â Patent
 Rights â Ownership by the Contractor (May 2014) SPDX-License-Identifier: MIT
 This material is based upon work supported by the Under Secretary of Defense
 for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any
 opinions, findings, conclusions or recommendations expressed in this material
 are those of the author(s) and do not necessarily reflect the views of the
 Under Secretary of Defense for Research and Engineering. A portion of this
```

### Comparing `hydra_zen-0.9.0rc5/README.md` & `hydra_zen-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/hydra-zen">
     <img src="https://img.shields.io/pypi/v/hydra-zen.svg" alt="PyPI" />
   </a>
   <a>
-    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.10-blue.svg" alt="Python version support" />
+    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.11-blue.svg" alt="Python version support" />
   </a>
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://github.com/mit-ll-responsible-ai/hydra-zen/workflows/Tests/badge.svg" alt="GitHub Actions" />
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://img.shields.io/badge/coverage-100%25-green.svg" alt="Code Coverage" />
   <a href="https://github.com/microsoft/pyright/blob/92b4028cd5fd483efcf3f1cdb8597b2d4edd8866/docs/typed-libraries.md#verifying-type-completeness">
     <img src="https://img.shields.io/badge/type%20completeness-100%25-green.svg" alt="Type-Completeness Score" />
@@ -81,15 +81,15 @@
 }
 ```
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
-© 2022 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+© 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
     
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: MIT
     
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
```

#### html2text {}

```diff
@@ -32,15 +32,15 @@
 the Discussion Share ideas, ask questions, and chat with us over at [hydra-
 zen's discussion board](https://github.com/mit-ll-responsible-ai/hydra-zen/
 discussions). ## Citation Using `hydra-zen` for your research? Please cite the
 following publication: ``` @article{soklaski2022tools, title={Tools and
 Practices for Responsible AI Engineering}, author={Soklaski, Ryan and Goodwin,
 Justin and Brown, Olivia and Yee, Michael and Matterer, Jason}, journal={arXiv
 preprint arXiv:2201.05647}, year={2022} } ``` ## Disclaimer DISTRIBUTION
-STATEMENT A. Approved for public release: distribution unlimited. Â© 2022
+STATEMENT A. Approved for public release: distribution unlimited. Â© 2023
 MASSACHUSETTS INSTITUTE OF TECHNOLOGY Subject to FAR 52.227-11 â Patent
 Rights â Ownership by the Contractor (May 2014) SPDX-License-Identifier: MIT
 This material is based upon work supported by the Under Secretary of Defense
 for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any
 opinions, findings, conclusions or recommendations expressed in this material
 are those of the author(s) and do not necessarily reflect the views of the
 Under Secretary of Defense for Research and Engineering. A portion of this
```

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen - favicon.png` & `hydra_zen-0.9.1/brand/Hydra-Zen - favicon.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full.svg` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full.svg`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd_small.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd_small.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_filled_bkgrnd_smaller.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_filled_bkgrnd_smaller.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_light_blue.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_light_blue.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/Hydra-Zen_logo_full_light_blue_smaller.png` & `hydra_zen-0.9.1/brand/Hydra-Zen_logo_full_light_blue_smaller.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_blue.png` & `hydra_zen-0.9.1/brand/HydraZen_logo_blue.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_blue.svg` & `hydra_zen-0.9.1/brand/HydraZen_logo_blue.svg`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_border.png` & `hydra_zen-0.9.1/brand/HydraZen_logo_border.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_border.svg` & `hydra_zen-0.9.1/brand/HydraZen_logo_border.svg`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_transparent.png` & `hydra_zen-0.9.1/brand/HydraZen_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/HydraZen_logo_transparent.svg` & `hydra_zen-0.9.1/brand/HydraZen_logo_transparent.svg`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/hydra_zen_favicon_32x32.ico` & `hydra_zen-0.9.1/brand/hydra_zen_favicon_32x32.ico`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/brand/hydra_zen_favicon_64x64.ico` & `hydra_zen-0.9.1/brand/hydra_zen_favicon_64x64.ico`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/Makefile` & `hydra_zen-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/make.bat` & `hydra_zen-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/_static/hydra_zen_favicon_32x32.png` & `hydra_zen-0.9.1/docs/source/_static/hydra_zen_favicon_32x32.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/_static/hydra_zen_favicon_64x64.png` & `hydra_zen-0.9.1/docs/source/_static/hydra_zen_favicon_64x64.png`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/api_reference.rst` & `hydra_zen-0.9.1/docs/source/api_reference.rst`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 ****************
 .. currentmodule:: hydra_zen.typing
 
 .. autosummary::
    :toctree: generated/
 
 
+   DataclassOptions
    ZenConvert
 
 
 .. _valid-types:
 
 **********************************************************
 Configuration-Value Types Supported by Hydra and hydra-zen
@@ -147,16 +148,18 @@
 .. _additional-types:
 
 Auto-Config Support for Additional Types via hydra-zen
 ******************************************************
 
 Values of additional types can be specified directly via hydra-zen's 
 :ref:`config-creation functions <create-config>` (and other utility functions like :func:`~hydra_zen.to_yaml`) and those functions will automatically 
-create targeted configs to represent those values in a way that is compatible 
-with Hydra. For example, a :py:class:`complex` value can be specified directly via :func:`~hydra_zen.make_config`, and a targeted config will be created for that value.
+create dataclass instances to represent those values in a way that is compatible 
+with Hydra. For example, a :py:class:`complex` value can be passed directly to 
+:func:`~hydra_zen.make_config`, and hydra-zen will generate a dataclass instance that 
+represents that complex value in a Hydra-compatible way.
 
 .. code-block:: pycon
    :caption: Demonstrating auto-config support for `complex`, `functools.partial` and `dataclasses.dataclass`
 
    >>> from hydra_zen import builds, just, make_config, to_yaml, instantiate
    >>> def print_yaml(x): print(to_yaml(x))
 
@@ -209,28 +212,29 @@
 hydra-zen provides specialized auto-config support for values of the following types:
 
 - :py:class:`bytes` (*support provided for OmegaConf < 2.2.0*)
 - :py:class:`bytearray`
 - :py:class:`complex`
 - :py:class:`collections.Counter`
 - :py:class:`collections.deque`
-- :py:func:`functools.partial`
+- :py:func:`functools.partial` (note: not compatible with pickling)
 - :py:class:`pathlib.Path` (*support provided for OmegaConf < 2.2.1*)
 - :py:class:`pathlib.PosixPath`
 - :py:class:`pathlib.WindowsPath`
 - :py:class:`range`
 - :py:class:`set`
 - :py:class:`frozenset`
-- :py:func:`dataclasses.dataclass`
+- :py:func:`dataclasses.dataclass` (note: not compatible with pickling)
 
 hydra-zen also provides auto-config support for some third-pary libraries:
 
 - `pydantic.dataclasses.dataclass`
 - `pydantic.Field`
-
+- `pydantic.Field`
+- `torch.optim.optimizer.required` (i.e. the default parameter for `lr` in `Optimizer`)
 
 
 *********************
 Third-Party Utilities
 *********************
 
 .. _data-val:
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/changes.rst` & `hydra_zen-0.9.1/docs/source/changes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,43 @@
 =========
 Changelog
 =========
 
 This is a record of all past hydra-zen releases and what went into them, in reverse 
 chronological order. All previous releases should still be available on pip.
 
-.. _v0.9.0:
+.. _v0.9.1:
+
+------------------
+0.9.1 - 2023-01-13
+------------------
+
 
----------------------
-0.9.0rc5 - 2022-12-09
----------------------
+Improvements
+------------
+- :func:`hydra_zen.zen` now returns pickle-compatible wrapped functions. See :pull:`384`.
 
-.. note:: This is documentation for an unreleased version of hydra-zen. You can try out this pre-release version using `pip install --pre hydra-zen`
+Bug Fixes
+---------
+- :func:`hydra_zen.zen`'s `hydra_main` method now handles string `config_path` entries properly (only for Hydra 1.3.0+). Previously Hydra could not find the path to the wrapped task function. hydra-zen will warn users that a string `config_path` is not supported via :func:`hydra_zen.zen` for Hydra 1.2 and earlier. See :pull:`384`.
 
+.. _v0.9.0:
+
+------------------
+0.9.0 - 2022-12-30
+------------------
 
 Release Highlights
 ------------------
 This release introduces :func:`~hydra_zen.zen` and :class:`~hydra_zen.ZenStore`, which enable hydra-zen users to eliminate Hydra-specific boilerplate code from their projects and to utilize new patterns and best practices for working with config stores.
 
-The :func:`~hydra_zen.zen` decorator enables of use Hydra-agnostic task functions in Hydra apps; the decorator will automatically extract, resolve, and instantiate fields from an input config based on the function's signature. This encourages users to eliminate Hydra-specific boilerplate code from their projects and to instead opt for task functions with explicit signatures, which can include functions from third parties.
-
-E.g., :func:`~hydra_zen.zen` enables us to replace the following Hydra-specific task function:
+The wrapper `~hydra_zen.zen` will automatically extract, resolve, and instantiate 
+fields from a config in order to call the function that it has wrapped, thus saving the 
+user from writing repetitive, hydra-specific boilerplate code in their function.
+Thus this wrapper enables users to replace the following Hydra-specific task function:
 
 .. code-block:: python
    :caption: The "old school" way of designing a task function for a Hydra app
 
    import hydra
    from hydra.utils import instantiate
    
@@ -63,18 +76,41 @@
        # config and pass it to `trainer_task_fn`
        zen(trainer_task_fn).hydra_main(config_name="my_app", config_path=None)
 
 
 There are plenty more bells and whistles to :func:`~hydra_zen.zen`, refer to :pull:`310` and its reference documentation for more details.
 
 :class:`~hydra_zen.ZenStore` is an abstraction over Hydra's config store.
-It enables users to maintain multiple, isolated store instances before populating Hydra's global config store.
-It also protects users from accidentally overwriting  entries in Hydra's global store
+It enables users to maintain multiple, isolated store instances before populating 
+Hydra's global config store. It also protects users from accidentally overwriting  
+entries in Hydra's global store. :class:`~hydra_zen.ZenStore` possesses auto-config 
+capabilities: it will automatically apply :func:`~hyda_zen.builds` and 
+:func:`~hyda_zen.just` in intuitive ways on inputs to generate the stored configs.
 
-This enables objects to be stored using a decorator pattern, e.g.
+.. code-block:: python
+   :caption: Using `hydra_zen.store` auto-generate and store configs
+
+   from hydra_zen import ZenStore
+   from torch.optim import Adam, AdamW, RMSprop
+
+   torch_store = ZenStore("torch_store")
+
+   # Specify defaults for storing entries (group=optim)
+   # and for generating configs (_partial_=True and lr=1e-3)
+   optim_store = torch_store(group="optim", zen_partial=True, lr=0.001)
+
+   # Automatically applies `builds(<obj>, zen_partial=True, lr=0.001)` 
+   # to create and then store configs under the "optim" group
+   optim_store(Adam, name="adam", amsgrad=True)
+   optim_store(AdamW, name="adamw", betas=(0.1, 0.999))
+   optim_store(RMSprop, name="rmsprop")
+
+   torch_store.add_to_hydra_store()  # populate Hydra's global store
+
+The store can also be populated using a decorator pattern [1]_, e.g.
 
 .. code-block:: python
    :caption: Using `hydra_zen.store` as a decorator to auto-configure and store objects.
 
    from dataclasses import dataclass
    from hydra_zen import store
 
@@ -86,55 +122,125 @@
    @profile_store(name="basic", has_root=False)
    @dataclass
    class Profile:
        username: str
        schema: str
        has_root: bool
 
-:class:`~hydra_zen.ZenStore` also possesses auto-config capabilities: it will automatically apply :func:`~hyda_zen.builds` and :func:`~hyda_zen.just` in intuitive ways on inputs to generate the stored configs.
-
-.. code-block:: python
-   :caption: Using `hydra_zen.store` auto-generate and store configs
-
-   from hydra_zen import ZenStore
-   from torch.optim import Adam, AdamW, RMSprop
-
-   torch_store = ZenStore("torch_store")
+   
+   db_store = store(group="database")
 
-   # Specify defaults for storing entries (group=optim)
-   # and for generating configs (_partial_=True and lr=1e-3)
-   optim_store = torch_store(group="optim", zen_partial=True, lr=0.001)
+   # calls `builds(profile_database, [...])` under the hood and
+   # adds the config to the store under the "profile" group
+   @db_store(name="database")
+   @db_store(name="test_database", size=1)
+   def profile_database(size):
+       ...
 
-   # Automatically applies `builds(<obj>, zen_partial=True, lr=0.001)` 
-   # to create and then store configs under the "optim" group
-   optim_store(Adam, name="adam", amsgrad=True)
-   optim_store(AdamW, name="adamw", betas=(0.1, 0.999))
-   optim_store(RMSprop, name="rmsprop")
 
 New Features
 ------------
+- hydra-zen now supports Python 3.11
 - Adds the :func:`~hydra_zen.zen` decorator (see :pull:`310`)
 - Adds the :func:`~hydra_zen.wrapper.Zen` decorator-class (see :pull:`310`)
 - Adds the :class:`~hydra_zen.ZenStore` class (see :pull:`331`)
 - Adds `hyda_zen.store`, which is a pre-initialized instance of :class:`~hydra_zen.ZenStore` (see :pull:`331`)
-
+- The option `hydra_convert='object'` is now supported by all of hydra-zen's config-creation functions. So that an instantiated structured config can be converted to an instance of its backing dataclass. This feature was added by `Hydra 1.3.0 <https://github.com/facebookresearch/hydra/issues/1719>`_.
+- Adds auto-config support for `torch.optim.optimizer.required` so that the common pattern `builds(<torch_optimizer_type>, populate_full_signature=True, zen_partial=True)` works and exposes `lr` as a required configurable parameter. Thanks to @addisonklinke for requesting this in :issue:`257`.
+- :ref:`builds([...], zen_wrapper=...) <zen-wrapper>` can now accept a partial'd function as a wrapper.
 
 Improvements
 ------------
+- Updated the :ref:`Tutorials <tutorials>` and :ref:`How-To Guides <hydra-zen-how-to>` to reflect idomatic usage of :class:`~hydra_zen.ZenStore` and :func:`~hydra_zen.zen`.
 - :func:`~hydra_zen.hydrated_dataclass` will now produce a pickle-compatible dataclass type. See :pull:`338`.
+- hydra-zen's :ref:`auto-config support <additional-types>` has been enhanced so that it produces pickle-compatible configs. This excludes auto-config support for :py:func:`functools.partial` and :py:func:`dataclasses.dataclass`. See :pull:`360`.
+- All options available to :func:`dataclasses.dataclass` are now exposed by :func:`~hydra_zen.hydrated_dataclass`, :func:`~hydra_zen.builds`, :func:`~hydra_zen.make_custom_builds_fn`, :func:`~hydra_zen.make_config`, and :func:`~hydra_zen.just` via the :class:`hydra_zen.typing.DataclassOptions` API. See :pull:`360`.
 - All documentation code blocks are scanned by pyright as part of our CI process. Several errors in the documentation were fixed. See :pull:`343` and :pull:`344`.
+- Updated the `hydra_zen.typing.Partial` protocol to match against the output of `functools.partial` more reliably in the eyes of pyright (:pull:`354`).
 
 Bug Fixes
 ---------
 - :pull:`355` fixes an issue where the parameterized generic `hydra_zen.typing.Partial[<...>]` would return `None` for Python versions 3.9+. This prevented this annotation from being used by runtime type checkers.
 
+Deprecations
+------------
+- Specifying `frozen=True` via :func:`~hydra_zen.builds` or :func:`~hydra_zen.make_config` is deprecated in favor of `zen_dataclass={'frozen': True}`. See :pull:`360`.
+- Specifying `config_name=<str>` via :func:`~hydra_zen.builds` or :func:`~hydra_zen.make_config` is deprecated in favor of `zen_dataclass={'cls_name': True}`. See :pull:`360`.
+
 Compatibility-Breaking Changes
 ------------------------------
+- Calling :func:`~hydra_zen.just` on a class-object or function will now return a frozen instance of a statically-defined dataclass. Previously it returned a dynamically-defined dataclass type. This change was made to improve pickle-compatibility and hashability of configs that are automatically generated by hydra-zen. This is unlikely to cause any issues for users.
 - Previously, any class decorated by :func:`~hydra_zen.hydrated_dataclass` would have a `__module__` attribute set to `typing`. Now the class's `__module__` will reflect the module where its static definition resides. This enables pickle-compatibility  (:pull:`338`). This is unlikely to cause any issues for users.
-- Improved the `hydra_zen.typing.Partial` protocol to match against the output of `functools.partial` more reliably in the eyes of pyright (:pull:`354`).
+
+Mutable Default Values for Dataclasses
+======================================
+Beginning in Python 3.11 :func:`dataclasses.dataclass` `checks for mutable default values <https://docs.python.org/3/library/dataclasses.html#mutable-default-values>`_ by assessing if an object possesses a `__hash__` attribute. Previously it only considered `set`, `dict`, and `list` types to be mutable. Accordingly, dataclass instances are now considered to be mutable unless they are frozen or if `unsafe_hash=True` was specified.
+
+.. code-block:: python
+   :caption: Demonstrating change in mutability rules for dataclasses starting in Python 3.11
+
+   from dataclasses import dataclass, field
+   
+   @dataclass
+   class A:
+      ...
+   
+   @dataclass
+   class NoLongerValid:
+      number: int = 1
+      nested: A = A()  # will raise at runtime due to mutable default
+
+   @dataclass
+   class IsOK:
+      number: int = 1
+      nested: A = field(default_factory=lambda: A())
+
+A ramification of the use of a default-factory in this example is that the field `nested` can only be accessed from an *instance* of ``IsOK``, whereas non-factory defaults can be accessed from the dataclass type itself.
+
+.. code-block:: pycon
+   :caption: Default factories require access from dataclass instances; they cannot be accessed from the dataclass type.
+
+   >>> hasattr(IsOK, "number")
+   True
+   >>> hasattr(IsOK, "nested")
+   False
+   >>> hasattr(IsOK(), "nested")
+   True
+
+Because hydra-zen users frequently nest dataclasses, hydra-zen's dataclass-creation functions (`builds` et al.) now specify `unsafe_hash=True` by default. Thus the following pattern is still valid:
+
+.. code-block:: python
+   :caption: The dataclasses produced by hydra-zen 0.9.0 are hashable by default so that existing patterns do not break in Python 3.11.
+
+   from dataclasses import dataclass, field
+   from typing import Any
+   
+   from hydra_zen import builds
+   from hydra_zen.typing import Builds
+
+   @dataclass
+   class Config:
+       # This is still OK
+       builds_dict: Builds[type[dict[Any, Any]]] = builds(dict)()
+
+That being said, hydra-zen will now treat dataclass instances whose `__hash__` attribute is `None` as mutable – *regardless of the Python version* – in order to ensure consistent behaviors across all supported Python versions. Thus the following pattern will now break
+
+.. code-block:: python
+   
+   @dataclass
+   class A:
+       ...
+
+   Conf = builds(dict, y=A(), zen_convert={'dataclass': False})
+   
+   Conf.y  # this will raise in hydra_zen 0.9.0+
+   Conf().y  # this is OK
+
+In general it is recommended that config fields be accessed from dataclass instances, not types. This will avoid all such default value/factory issues.
+
 
 .. _v0.8.0:
 
 ------------------
 0.8.0 - 2022-09-13
 ------------------
 
@@ -198,15 +304,15 @@
 
 Big thanks to `Jasha10 <https://github.com/Jasha10>`_ for proposing and prototyping the crux of this new capability.
 
 Compatibility-Breaking Changes
 ------------------------------
 This release drops support for Python 3.6. If you require Python 3.6, please restrict your hydra-zen installation dependency as `hydra-zen<0.8.0`.
 
-Specifing `make_custom_builds_fn([...], builds_bases=<...>)` was deprecated in 
+Specifying `make_custom_builds_fn([...], builds_bases=<...>)` was deprecated in 
 hydra-zen 0.7.0 (:pull:`263`). Accordingly, this option has now been removed from
 :func:`hydra_zen.make_custom_builds_fn`.
 
 The addition of auto-config support for dataclasses (:pull:`301`) changes the default 
 behaviors of :func:`~hydra_zen.just` and :func:`~hydra_zen.builds`. Previously, all 
 dataclass types and instances lacking a `_target_` field would be left unprocessed by 
 these functions, and omegaconf would convert dataclass types and instances alike to 
@@ -689,7 +795,14 @@
 This is hydra-zen's first stable release on PyPI!
 Although we have not yet released version `v1.0.0`, it should be noted that hydra-zen's codebase is thoroughly tested.
 Its test suite makes keen use of the property-based testing library `Hypothesis <https://hypothesis.readthedocs.io/en/latest/>`_.
 Furthermore, 100% code coverage is enforced on all commits into `main`.
 
 We plan to have an aggressive release schedule for compatibility-preserving patches of bug-fixes and quality-of-life improvements (e.g. improved type annotations).
 hydra-zen will maintain a wide window of compatibility with Hydra versions; we test against pre-releases of Hydra and will maintain compatibility with its future releases.
+
+
+---------
+Footnotes
+---------
+.. [1] The config creation process associated with the decorator is deferred until 
+   the config is actually accessed by the store. Thus this decorator pattern does not add substantial runtime overhead to library code until Hydra capabilities are actually utilized.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/conf.py` & `hydra_zen-0.9.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 import hydra_zen
 
 # -- Project information -----------------------------------------------------
 
 project = "hydra-zen"
-copyright = "2022 Massachusetts Institute of Technology"
+copyright = "2023 Massachusetts Institute of Technology"
 author = "Ryan Soklaski, Justin Goodwin"
 
 # The short X.Y version
 version = ""
 # The full version, including alpha/beta/rc tags
 release = ""
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/explanation/dont_repeat_yourself.rst` & `hydra_zen-0.9.1/docs/source/explanation/dont_repeat_yourself.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
            pass
 
 We'll compare the processes of configuring :class:`DNN` using a YAML-file, using a hand-written dataclass, and using :func:`hydra_zen.builds`.
 
 Statically-Defined Configs are WET
 ==================================
 
-Manually writing a structured config for ``DNN`` entails hard-coding its current import-path as a string as wll as explicitly mirroring its signature:
+Manually writing a structured config for ``DNN`` entails hard-coding its current import-path as a string as well as explicitly mirroring its signature:
 
 
 .. tab-set::
 
    .. tab-item:: dataclass-based config
 
       .. code-block:: python
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/explanation/hydrated_dataclass.rst` & `hydra_zen-0.9.1/docs/source/explanation/hydrated_dataclass.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/explanation/type_refinement.rst` & `hydra_zen-0.9.1/docs/source/explanation/type_refinement.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/generated/hydra_zen.typing.ZenConvert.rst` & `hydra_zen-0.9.1/docs/source/generated/hydra_zen.typing.ZenConvert.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/how_to/beartype.rst` & `hydra_zen-0.9.1/docs/source/how_to/beartype.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/how_to/partial_config.rst` & `hydra_zen-0.9.1/docs/source/how_to/partial_config.rst`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 has launched.
 
 
 In this How-To we will write a config that only partially configures a target object.
 We will
 
 1. Define toy examples of a class and a function, respectively.
-2. Use ``builds(<target>, zen_partial=True)`` to create their partial configurations.
+2. Use ``builds(<target>, zen_partial=True)`` and ``just(functools.partial(<target>))`` to create their partial configurations.
 3. Check that :func:`~hydra_zen.instantiate` only partially-instantiates the targets of these two configs.
 4. Examine the YAML-config for one of these partial configs.
 
 
 Let's define toy examples of a class and a function; we'll create partial configs for 
 both of these.
 
@@ -38,24 +38,27 @@
            self.lr = learning_rate
 
    def logger(message: str, format_spec: str) -> str:
        return format_spec.format(message)
 
 Suppose that the ``model_weights`` parameter in :class:`Optimizer`, and the ``message`` parameter in :func:`logger` ought not be configured by our app's interface. 
 :func:`~hydra_zen.builds` provides the ``zen_partial`` feature, which makes it trivial 
-to partially-configure a target. Let's create configs for our toy class and toy 
-function.
+to partially-configure a target. We can also apply :func:`~hydra_zen.just` to a instance of :py:class:`functools.partial` Let's create configs for our toy class and 
+toy function.
 
 .. code-block:: python
    :caption: 2: Creating partial configs.
    
-   from hydra_zen import builds, instantiate
+   from functools import partial
+   from hydra_zen import builds, instantiate, just
    
    OptimConf = builds(Optimizer, learning_rate=0.1, zen_partial=True)
-   LogConf = builds(logger, format_spec='{0:>8s}', zen_partial=True)
+   
+   partial_logger = partial(logger, format_spec='{0:>8s}')
+   LogConf = just(partial_logger)
 
 Instantiating these configs will apply :func:`functools.partial` to the config's target.
 
 .. code-block:: pycon
    :caption: 3: Instantiating the configs
    
    >>> partiald_optim = instantiate(OptimConf)
@@ -70,18 +73,23 @@
    functools.partial(<function logger at 0x0000018998D1E040>, format_spec='{0:>8s}')
    
    >>> partiald_logger("hello")
    '   hello'
    >>> partiald_logger("goodbye")
    ' goodbye'
 
-Lastly, let's inspect the YAML-serialized config for :class:`OptimConf`.
+Lastly, let's inspect the YAML-serialized config for :class:`OptimConf` and :class:`LongConf`.
 
 .. code-block:: pycon
    :caption: 4: Examining a YAML-serialized partial config.
 
    >>> from hydra_zen import to_yaml
 
    >>> print(to_yaml(OptimConf))
    _target_: __main__.Optimizer
    _partial_: true
    learning_rate: 0.1
+
+   >>> print(to_yaml(LogConf))
+   _target_: __main__.logger
+   _partial_: true
+   format_spec: '{0:>8s}'
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/how_to/pytorch_lightning.rst` & `hydra_zen-0.9.1/docs/source/how_to/pytorch_lightning.rst`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,16 @@
    import torch.nn as nn
    import torch.nn.functional as F
    from torch.optim import Optimizer
    from torch.utils.data import DataLoader, TensorDataset
    
    from hydra_zen.typing import Partial
    
+   __all__ = ["UniversalFuncModule", "single_layer_nn", "train_and_eval"]
+   
    
    def single_layer_nn(num_neurons: int) -> nn.Module:
        """y = sum(V sigmoid(X W + b))"""
        return nn.Sequential(
            nn.Linear(1, num_neurons),
            nn.Sigmoid(),
            nn.Linear(num_neurons, 1, bias=False),
@@ -98,14 +100,45 @@
        def train_dataloader(self):
            # generate dataset: x, cos(x)
            x = self.training_domain.reshape(-1, 1)
            y = self.target_fn(x)
            return self.dataloader(TensorDataset(x, y))
 
 
+   def train_and_eval(
+       model: tr.nn.Module,
+       optim: Partial[Optimizer],
+       dataloader: Type[DataLoader],
+       target_fn: Callable[[tr.Tensor], tr.Tensor],
+       training_domain: tr.Tensor,
+       lit_module: Type[UniversalFuncModule],
+       trainer: pl.Trainer,
+   ):
+   
+       
+       lit = lit_module(
+           model=model,
+           optim=optim,
+           dataloader=dataloader,
+           target_fn=target_fn,
+           training_domain=training_domain,
+       )
+   
+       # train the model
+       trainer.fit(lit)
+   
+       # evaluate the model over the domain to assess the fit
+       final_eval = lit(training_domain.reshape(-1, 1))
+       final_eval = final_eval.detach().cpu().numpy().ravel()
+   
+       # return the final evaluation of our model:
+       # a shape-(N,) numpy-array
+       return final_eval
+
+
 .. attention::
 
    :plymi:`Type-annotations <Module5_OddsAndEnds/Writing_Good_Code.html#Type-Hinting>` are **not** required by hydra-zen. However, they do enable :ref:`runtime type-checking of configured values <type-support>` for our app.
 
 
 Creating Our Configs and Task Function
 ======================================
@@ -114,77 +147,61 @@
 Here, we will create the configs for our optimizer, model, data-loader, lightning module,
 and trainer. We'll also define the task function that trains and tests our model.
 
 
 .. code-block:: python
    :caption: Contents of ``experiment.py``
 
-   import math
+   from math import pi
    
+   import pytorch_lightning as pl
+   from hydra_zen import builds, make_config, make_custom_builds_fn, zen
    import torch as tr
    from torch.optim import Adam
    from torch.utils.data import DataLoader
-   from zen_model import UniversalFuncModule, single_layer_nn
    
-   import pytorch_lightning as pl
-   from hydra_zen import builds, make_config, make_custom_builds_fn, instantiate
+   from zen_model import UniversalFuncModule, train_and_eval, single_layer_nn
    
    pbuilds = make_custom_builds_fn(zen_partial=True, populate_full_signature=True)
    
-   OptimConf = pbuilds(Adam)
-   
-   LoaderConf = pbuilds(DataLoader, batch_size=25, shuffle=True, drop_last=True)
-   
-   ModelConf = builds(single_layer_nn, num_neurons=10)
-
-   # configure our lightning module
-   LitConf = pbuilds(
-       UniversalFuncModule,
-       model=ModelConf,
-       target_fn=tr.cos,
-       training_domain=builds(
-           tr.linspace, start=-2 * math.pi, end=2 * math.pi, steps=1000
-       ),
-   )
-   
-   TrainerConf = builds(pl.Trainer, max_epochs=100)
    
    ExperimentConfig = make_config(
-       optim=OptimConf,
-       dataloader=LoaderConf,
-       lit_module=LitConf,
-       trainer=TrainerConf,
        seed=1,
+       lit_module=UniversalFuncModule,
+       trainer=builds(pl.Trainer, max_epochs=100),
+       model=builds(single_layer_nn, num_neurons=10),
+       optim=pbuilds(Adam),
+       dataloader=pbuilds(DataLoader, batch_size=25, shuffle=True, drop_last=True),
+       target_fn=tr.cos,
+       training_domain=builds(tr.linspace, start=-2 * pi, end=2 * pi, steps=1000),
    )
    
-   
-   def task_function(cfg):
-       # cfg: ExperimentConfig
-       pl.seed_everything(cfg.seed)
-   
-       obj = instantiate(cfg)
-       
-       # finish instantiating the lightning module, data-loader, and optimizer
-       lit_module = obj.lit_module(dataloader=obj.dataloader, optim=obj.optim)
-   
-       # train the model
-       obj.trainer.fit(lit_module)
-   
-       # evaluate the model over the domain to assess the fit
-       data = lit_module.training_domain
-       final_eval = lit_module.forward(data.reshape(-1, 1))
-       final_eval = final_eval.detach().cpu().numpy().ravel()
-       
-       # return the final evaluation of our model:
-       # a shape-(N,) numpy-array
-       return final_eval
+   # Wrapping `train_and_eval` with `zen` makes it compatible with Hydra as a task function
+   #
+   # We must specify `pre_call` to ensure that pytorch lightning seeds everything
+   # *before* any of our configs are instantiated (which will initialize the pytorch
+   # model whose weights depend on the seed)
+   task_function = zen(train_and_eval, pre_call=zen(lambda seed: pl.seed_everything(seed)))
+   
+   if __name__ == "__main__":
+       # enables us to call 
+       from hydra_zen import ZenStore
+   
+       store = ZenStore(deferred_hydra_store=False)
+       store(ExperimentConfig, name="lit_app")
+   
+       task_function.hydra_main(
+           config_name="lit_app",
+           version_base="1.1",
+           config_path=".",
+       )
 
 .. admonition:: Be Mindful of What Your Task Function Returns
 
-   We *could* make this task-function return our trained neural network, which would enable
+   We *could* make this `train_and_eval` return our trained neural network, which would enable
    convenient access to it, in-memory, after our Hydra job completes. However, launching this
    task function in a multirun fashion will train multiple models and thus would keep *all* of
    those models in-memory (and perhaps on-GPU) simultaneously! 
    
    By not returning the model from our task function, we avoid the risk of hitting out-of-memory
    errors when training multiple large models.
 
@@ -197,36 +214,49 @@
 - a batch-size of 20 and 200
 - a model with 10 and 100 neurons
 
 Open a Python console (or Jupyter notebook) in the same directory as ``experiment.py`` 
 and run the following code.
 
 .. code-block:: pycon
-   :caption: Launching four jobs
+   :caption: Launching four jobs from a Python console.
 
    >>> from hydra_zen import launch
    >>> from experiment import ExperimentConfig, task_function
    >>> (jobs,) = launch(  # type: ignore
    ...     ExperimentConfig,
    ...     task_function,
    ...     overrides=[
    ...         "dataloader.batch_size=20,200",
-   ...         "lit_module.model.num_neurons=10,100",
+   ...         "model.num_neurons=10,100",
    ...     ],
    ...     multirun=True,
    ... )
    [2021-10-24 21:23:32,556][HYDRA] Launching 4 jobs locally
-   [2021-10-24 21:23:32,558][HYDRA] 	#0 : dataloader.batch_size=20 lit_module.model.num_neurons=10
-   [2021-10-24 21:23:45,809][HYDRA] 	#1 : dataloader.batch_size=20 lit_module.model.num_neurons=100
-   [2021-10-24 21:23:58,656][HYDRA] 	#2 : dataloader.batch_size=200 lit_module.model.num_neurons=10
-   [2021-10-24 21:24:01,796][HYDRA] 	#3 : dataloader.batch_size=200 lit_module.model.num_neurons=100
+   [2021-10-24 21:23:32,558][HYDRA] 	#0 : dataloader.batch_size=20 model.num_neurons=10
+   [2021-10-24 21:23:45,809][HYDRA] 	#1 : dataloader.batch_size=20 model.num_neurons=100
+   [2021-10-24 21:23:58,656][HYDRA] 	#2 : dataloader.batch_size=200 model.num_neurons=10
+   [2021-10-24 21:24:01,796][HYDRA] 	#3 : dataloader.batch_size=200 model.num_neurons=100
 
 Keep this Python console open; we will be making use of ``jobs`` in order to inspect 
 our results.
 
+Note that this is equivalent to running the following from the CLI:
+
+.. code-block:: console
+   :caption: Launching four jobs from the CLI.
+
+   $ python experiment.py dataloader.batch_size=20,200 model.num_neurons=10,100 -m
+   [2021-10-24 21:23:32,556][HYDRA] Launching 4 jobs locally
+   [2021-10-24 21:23:32,558][HYDRA] 	#0 : dataloader.batch_size=20 model.num_neurons=10
+   [2021-10-24 21:23:45,809][HYDRA] 	#1 : dataloader.batch_size=20 model.num_neurons=100
+   [2021-10-24 21:23:58,656][HYDRA] 	#2 : dataloader.batch_size=200 model.num_neurons=10
+   [2021-10-24 21:24:01,796][HYDRA] 	#3 : dataloader.batch_size=200 model.num_neurons=100
+
+
 Inspecting Our Results
 =======================
 
 Visualizing Our Results
 -----------------------
 
 Let's begin inspecting our results by plotting our four models on :math:`x \in [-2\pi, 2\pi]`, alongside the
@@ -235,16 +265,16 @@
 
 .. code-block:: pycon
    :caption: Plotting our models
 
    >>> from hydra_zen import instantiate
    >>> import matplotlib.pyplot as plt
    
-   >>> x = instantiate(ExperimentConfig.lit_module.training_domain)
-   >>> target_fn = instantiate(ExperimentConfig.lit_module.target_fn)
+   >>> x = instantiate(ExperimentConfig.training_domain)
+   >>> target_fn = instantiate(ExperimentConfig.target_fn)
    
    >>> fig, ax = plt.subplots()
    >>> ax.plot(x, target_fn(x), ls="--", label="Target")
 
    >>> for j in jobs:
    ...     out = j.return_value
    ...     ax.plot(x, out, label=",".join(s.split(".")[-1] for s in j.overrides))
@@ -269,15 +299,15 @@
 
 .. code-block:: pycon
    :caption: Job 1 corresponds to the 100-neuron model trained with batch-size 20.
    
    >>> best = jobs[1]
    >>> best.cfg.dataloader.batch_size
    20
-   >>> best.cfg.lit_module.model.num_neurons
+   >>> best.cfg.model.num_neurons
    100
 
 Next, we'll load the config for this job. Recall that Hydra saves a ``.hydra/config.yaml`` file, which contains the complete configuration of this job -- we can reproduce 
 all aspects of it from this YAML. 
 
 .. code-block:: pycon
    :caption: Loading the complete config for this job
@@ -290,83 +320,88 @@
 
 It is worth printing our this config to appreciate all of the exhaustive details that 
 it captures about this job.
 
 .. code-block:: pycon
    
    >>> print(to_yaml(cfg))  # fully details this job's config
+   seed: 1
+   lit_module:
+     path: zen_model.UniversalFuncModule
+     _target_: hydra_zen.funcs.get_obj
+   trainer:
+     _target_: pytorch_lightning.trainer.trainer.Trainer
+     max_epochs: 100
+   model:
+     _target_: zen_model.single_layer_nn
+     num_neurons: 100
    optim:
-     _target_: hydra_zen.funcs.zen_processing
-     _zen_target: torch.optim.adam.Adam
-     _zen_partial: true
+     _target_: torch.optim.adam.Adam
+     _partial_: true
      lr: 0.001
      betas:
      - 0.9
      - 0.999
      eps: 1.0e-08
      weight_decay: 0
      amsgrad: false
    dataloader:
-     _target_: hydra_zen.funcs.zen_processing
-     _zen_target: torch.utils.data.dataloader.DataLoader
-     _zen_partial: true
+     _target_: torch.utils.data.dataloader.DataLoader
+     _partial_: true
      batch_size: 20
      shuffle: true
+     sampler: null
+     batch_sampler: null
+     num_workers: 0
+     collate_fn: null
+     pin_memory: false
      drop_last: true
-   lit_module:
-     _target_: hydra_zen.funcs.zen_processing
-     _zen_target: zen_model.UniversalFuncModule
-     _zen_partial: true
-     model:
-       _target_: zen_model.single_layer_nn
-       num_neurons: 100
-     target_fn:
-       _target_: hydra_zen.funcs.get_obj
-       path: torch.cos
-     training_domain:
-       _target_: torch.linspace
-       start: -6.283185307179586
-       end: 6.283185307179586
-       steps: 1000
-   trainer:
-     _target_: pytorch_lightning.trainer.trainer.Trainer
-     max_epochs: 100
-     progress_bar_refresh_rate: 0
-   seed: 1
+     timeout: 0.0
+     worker_init_fn: null
+     multiprocessing_context: null
+     generator: null
+     prefetch_factor: 2
+     persistent_workers: false
+   target_fn:
+     path: torch.cos
+     _target_: hydra_zen.funcs.get_obj
+   training_domain:
+     _target_: torch.linspace
+     start: -6.283185307179586
+     end: 6.283185307179586
+     steps: 1000
 
 PyTorch Lightning saved the model's trained weights as a ``.ckpt`` file in this job's 
 working directory. Let's load these weights and use them to instantiate our lighting 
 module.
 
 .. code-block:: pycon
    :caption: Loading our lighting module with trained weights
 
+   >>> from hydra_zen import zen
+   >>> from functools import partial
    >>> *_, last_ckpt = sorted(outdir.glob("**/*.ckpt"))
    >>> LitModule = get_target(cfg.lit_module)
 
-   >>> loaded = LitModule.load_from_checkpoint(
-   ...     last_ckpt,
-   ...     model=instantiate(cfg.lit_module.model),
-   ...     target_fn=instantiate(cfg.lit_module.target_fn),
-   ...     training_domain=instantiate(cfg.lit_module.training_domain),
-   ...     optim=instantiate(cfg.optim),
-   ...     dataloader=instantiate(cfg.dataloader),
-   ... )
+   >>> pload = partial(LitModule.load_from_checkpoint, last_ckpt)
+   >>> # extract top-level fields from `cfg`, instantiate them, and pass to `load_from_checkpoint`
+   >>> loaded = zen(pload, unpack_kwargs=True)(cfg)  # type: ignore
 
 Finally, let's double check that this loaded model behaves as-expected. Evaluating it 
 at :math:`-\pi/2`, :math:`0`, and :math:`\pi/2` should return, approximately, :math:`0`, :math:`1`, and :math:`0`, respectively.
 
 .. code-block:: pycon
    :caption: Checkout our loaded model's behavior
    
    >>> import torch as tr
    >>> loaded(tr.tensor([-3.1415 / 2, 0.0, 3.1415 / 2]).reshape(-1, 1))
-   tensor([[0.0218],
-           [0.9526],
-           [0.0125]], grad_fn=<MmBackward>
+   tensor([[0.0110],
+           [0.9633],
+           [0.0364]], grad_fn=<MmBackward>)
+
 
 
 
 .. admonition:: Math Details
 
    For the interested reader... In this toy-problem we are optimizing `arbitrary-width universal function approximators    <https://en.wikipedia.org/wiki/Universal_approximation_theorem#Arbitrary-width_case>`_ to fit :math:`\cos{x}`
    on :math:`x \in [-2\pi, 2\pi]`.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/index.rst` & `hydra_zen-0.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials/add_cli.rst` & `hydra_zen-0.9.1/docs/source/tutorials/add_cli.rst`

 * *Files 16% similar despite different names*

```diff
@@ -12,61 +12,57 @@
 .. _cli-app:
 
 ===============================================
 Add a Command Line Interface to Our Application
 ===============================================
 
 In this tutorial we will update our project so that it can be configured and launched 
-from a command line interface, using Hydra.
+from a command line interface (CLI), using Hydra.
 
 
 Modifying Our Project
 =====================
 
 Open ``my_app.py`` in your editor. We will make the following modifications to it:
 
-1. Register our config in Hydra's "config store".
-2. Decorate our task function to tell Hydra what config to use to define its interface.
-3. Add a ``__main__`` clause to our ``my_app.py`` script so that the script runs our task function.
+1. User :func:`hydra_zen.store` to generate for our task function and to store it in Hydra's global config store.
+2. Add a ``__main__`` clause to our ``my_app.py`` script so that the script runs our task function.
+3. Use :func:`hydra_zen.zen` to wrap the task function and to generate the CLI.
 
 Modify your script to match this:
 
 .. code-block:: python
    :caption: Contents of my_app.py:
 
-   import hydra
-   from hydra.core.config_store import ConfigStore
-   
-   from hydra_zen import instantiate, make_config
-   
-   Config = make_config("player1", "player2")
-   
-   # 1) Register our config with Hydra's config store
-   cs = ConfigStore.instance()
-   cs.store(name="my_app", node=Config)
-   
-   
-   # 2) Tell Hydra what config to use for our task-function.
-   #    The name specified here - 'config' - must match the
-   #    name that we provided to `cs.store(name=<...>, node=Config)`
-   @hydra.main(config_path=None, config_name="my_app")
-   def task_function(cfg):
-       # cfg: Config
-       obj = instantiate(cfg)
-       p1 = obj.player1
-       p2 = obj.player2
+   from hydra_zen import store, zen
    
+   # 1) `hydra_zen.store generates a config for our task function
+   #    and stores it locally under the entry-name "my_app"
+   @store(name="my_app")
+   def task_function(player1, player2):
+       # write the log with the names
        with open("player_log.txt", "w") as f:
            f.write("Game session log:\n")
-           f.write(f"Player 1: {p1}\n" f"Player 2: {p2}")
-   
-   
-   # 3) Executing `python my_app.py [...]` will run our task function
+           f.write(f"Player 1: {player1}\n" f"Player 2: {player2}")
+
+       return player1, player2
+      
+   # 2) Executing `python my_app.py [...]` will run our task function
    if __name__ == "__main__":
-       task_function()
+       # 3) We need to add the configs from our local store to Hydra's
+       #    global config store 
+       store.add_to_hydra_store()
+       
+       # 4) Our zen-wrapped task function is used to generate
+       #    the CLI, and to specify which config we want to use
+       #    to configure the app by default
+       zen(task_function).hydra_main(config_name="my_app", 
+                                     version_base="1.1",
+                                     config_path=None,
+                                     )
 
 
 Launching Our Application from the Command Line
 ===============================================
 
 With the above modifications to ``my_app.py`` complete, we can launch our application 
 from the command line. The following will launch a job with ``mario`` and ``luigi`` as 
@@ -141,15 +137,15 @@
 
 Reference Documentation
 =======================
 Want a deeper understanding of how hydra-zen and Hydra work?
 The following reference materials are especially relevant to this
 tutorial section.
 
-- `~hydra_zen.make_config`
+- `~hydra_zen.store`
 - :hydra:`Hydra's Config Store API <tutorials/structured_config/config_store>`
 - :hydra:`Hydra's command line override syntax <advanced/override_grammar/basic>`
 
 
 .. attention:: **Cleaning Up**:
    To clean up after this tutorial, delete the ``outputs`` directory that Hydra created 
    upon launching our application.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials/basic_app.rst` & `hydra_zen-0.9.1/docs/source/tutorials/basic_app.rst`

 * *Files 15% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
 Our program will consist of two components, which comprises the structure of any 
 Hydra-based application:
 
 1. A "config", which defines the configurable interface of our application.
 2. A task function, which accepts the populated config, and whose body specifies the code that will be executed when our application is launched.
 
+Once we create this typical Hydra app, we will iterate on it and simplify things by using how hydra-zen's :func:`hydra_zen.zen` wrapper.
 
 Writing the Application
 -----------------------
 
 In ``my_app.py`` we'll define a config and task function for this application. We will 
 use :func:`~hydra_zen.make_config` to create the config. Write the following code in 
 this file.
@@ -121,20 +122,22 @@
 .. code-block:: pycon
     
     >>> from hydra_zen import launch
 
 Next, we will launch our application by providing the :func:`~hydra_zen.launch` 
 function with: our config, our task function, and specific configured values for the 
 player's names. Here, we will use the names ``link`` and ``zelda`` for the names of 
-player 1 and player 2, respectively.
+player 1 and player 2, respectively. The ``version_base`` parameter controls some of the default behaviors of Hydra [1]_.
+
 
 .. code-block:: pycon
    :caption: Launching our application
 
-   >>> job = launch(Config, task_function, overrides=["player1=link", "player2=zelda"])
+   >>> job = launch(Config, task_function, overrides=["player1=link", "player2=zelda"], version_base="1.1")
+
 
 Let's inspect the completion status of this job by inspecting ``job.status``; it should
 indicate ``COMPLETED``.
 
 .. code:: pycon
 
    >>> job.status
@@ -220,22 +223,84 @@
    >>> print_file(job_dir / ".hydra" / "config.yaml")
    player1: link
    player2: zelda
 
 We successfully designed, configured, and launched an application using hydra-zen and 
 Hydra! In the next tutorial, we will add a command line interface to this app.
 
+In the final section, let's see how we can simplify some of our code using special features provided by hydra-zen.
+
+Simplifying Things with :func:`hydra_zen.zen`
+---------------------------------------------
+
+.. note:: This part of the tutorial requires ``hydra-zen v0.9.0`` or later to be installed.
+
+We can simplify our task function, removing Hydra-specific logic from it, by using :func:`hydra_zen.zen`. 
+
+Let's update our task function in `my_app.py` to be a simple function whose signature determines the fields that will be extracted and instantiated from our config.
+Then we can use :func:`hydra_zen.builds`, instead of :func:`hydra_zen.make_config`, to generate our config based off of the task function's signature.
+
+
+.. code-block:: python
+   :caption: Simplified contents of my_app.py:
+    
+   from hydra_zen import builds
+    
+   def new_task_function(player1, player2):
+       # write the log with the names
+       with open("player_log.txt", "w") as f:
+           f.write("Game session log:\n")
+           f.write(f"Player 1: {player1}\n" f"Player 2: {player2}")
+
+       return player1, player2
+
+   # auto-populates the fields of our configs based on the signature of
+   # `task_function`
+   Config = builds(new_task_function, populate_full_signature=True)
+
+
+Wrapping this function as
+
+.. code-block:: python
+   :caption: Simplified contents of my_app.py:
+    
+   from hydra_zen import zen
+
+   hydra_compat_task_fn = zen(task_function)
+
+returns a Hydra-compatible task function, which accepts a single input config just like our original task function did. However, the `zen` wrapper adds the logic of extracting
+and instantiating the `player1` and `player2` fields from our config for us.
+
+Now we will supply a zen-wrapped version of our task function to :func:`hydra_zen.launch`; all other aspects of launching our app and inspecting its results are unchanged.
+
+.. code-block:: pycon
+   :caption: Launching our application
+
+   >>> from my_app import Config, new_task_function
+   >>> from hydra_zen import zen, launch
+   >>> wrapped_fn = zen(new_task_function)
+   >>> job = launch(Config, wrapped_fn, overrides=["player1=link", "player2=zelda"], version_base="1.1")
+
+See that we were able to launch the same app as before, but with some additional benefits:
+
+- Our task function does not have any Hydra-specific logic and can be used for other purposes.
+- We can utilize :func:`hydra_zen.builds` to auto-populate our config instead of hand-specifying the fields.
 
 Reference Documentation
 =======================
 Want a deeper understanding of how hydra-zen and Hydra work?
 The following reference materials are especially relevant to this
 tutorial section.
 
 - :func:`~hydra_zen.make_config`
 - :func:`~hydra_zen.launch`
+- `Hydra's version_base <https://hydra.cc/docs/upgrades/version_base/#internaldocs-banner>`_
 
 
 .. attention:: **Cleaning Up**:
    To clean up after this tutorial, delete the ``outputs`` directory that Hydra created 
    upon launching our application. You can find this in the same directory as your 
    ``my_app.py`` file.
+
+Footnotes
+==========
+.. [1] Specifically, we want to ensure that Hydra will `change its working directory to its "jobdir" <https://hydra.cc/docs/upgrades/1.1_to_1.2/changes_to_job_working_dir/>`_ when we launch our app.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials/config_groups.rst` & `hydra_zen-0.9.1/docs/source/tutorials/config_groups.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,78 +7,79 @@
 
 .. _config-groups-tutorial:
 
 ======================================
 Provide Swappable Configuration Groups
 ======================================
 
-In this tutorial we will create swappable configuration groups for our application; 
-this will enable us to create specific player profiles and inventory load-outs. These 
-config groups can then be specified by name when we launch our application.
+In this tutorial we will create swappable configuration groups for our application: we 
+will pre-configure specific player profiles and inventory load-outs. By storing these 
+configs in a config store, we will be able to load them and swap them out by group & 
+name from the command line.
 
 Modifying Our Application
 =========================
 
 We will need to make three modifications to our code in ``my_app.py``:
 
 1. Create additional inventory configs and player-profile configs.
-2. Register these configs - by name - in Hydra's config store, under the appropriate respective groups.
-3. Update our application's top-level config to include a "defaults" list, which is a special field that Hydra uses to define the interface to our application.
+2. Register these configs - by group and name - in a config store.
+3. Update our application's top-level config to include a "Hydra defaults" list, which is a special field that Hydra uses to define the default inputs to our application.
 
 
 Creating Inventory-Config Groups
 --------------------------------
 
 In the previous tutorial, we created a config that represented an inventory of "starter gear". Let's simply create some other inventory "load-outs" that we can pick from. We 
 will use the following code in ``my_app.py``.
 
 .. attention:: 
 
    The ``game_library`` code used below comes from a script that we, the 
    tutorial-readers, created ourselves. See :ref:`game-library` for details.
 
 .. code-block:: python
-   :caption: Creating configs for new inventory load-outs
+   :caption: Creating configs for new inventory load-outs.
 
    from hydra_zen import make_custom_builds_fn
 
    from game_library import inventory
 
    builds = make_custom_builds_fn(populate_full_signature=True)
 
    InventoryConf = builds(inventory)
    starter_gear = InventoryConf(gold=10, weapon="stick", costume="tunic")
    advanced_gear = InventoryConf(gold=500, weapon="wand", costume="magic robe")
    hard_mode_gear = InventoryConf(gold=0, weapon="inner thoughts", costume="rags")
 
-Now we will register each of these configs in Hydra's config store. Each of these will 
-be stored with a distinct name, but under the same group: ``player/inventory``.
+Now we will register each of these configs using :class:`~hydra_zen.ZenStore`. Each of 
+these will be stored with a distinct name, but under the same group: 
+``player/inventory``.
 
 .. code-block:: python
-   :caption: Adding configs to the ``player/inventory`` group in Hydra's config store
+   :caption: Adding configs to the ``player/inventory`` group in hydra-zen's config store.
 
-   from hydra.core.config_store import ConfigStore
+   from hydra_zen import store
 
+   # pre-set the group name
+   inv_store = store(group="player/inventory")
 
-   cs = ConfigStore.instance()
-
-   cs.store(group="player/inventory", name="starter", node=starter_gear)
-   cs.store(group="player/inventory", name="advanced", node=advanced_gear)
-   cs.store(group="player/inventory", name="hard_mode", node=hard_mode_gear)
-
+   inv_store(starter_gear, name="starter")
+   inv_store(advanced_gear, name="advanced")
+   inv_store(hard_mode_gear, name="hard_mode")
 
 Creating Player-Config Groups
 -----------------------------
 
 Suppose that we have a couple of players who have saved their player profiles, so that 
 they can resume progress when they play our game. Let's mock-up these player configs 
 and then add them to the config store.
 
 .. code-block:: python
-   :caption: Creating player-profile configs
+   :caption: Creating player-profile configs.
    
    from game_library import Character
 
    CharConf = builds(Character, inventory=starter_gear)
    
    brinda_conf = CharConf(
        name="brinda",
@@ -88,40 +89,45 @@
    
    rakesh_conf = CharConf(
        name="rakesh",
        level=300,
        inventory=InventoryConf(costume="PJs", weapon="pillow", gold=41),
    )
 
-We will add these to Hydra's config store under the ``player`` group, so that these 
-particular player-profiles can be used by-name when we launch our application.
+We will add these to the same config store, but under the ``player`` group. This will 
+enable us to load these particular player-profiles by-name when we launch our 
+application.
 
 
 .. code-block:: python
-   :caption: Adding configs to the ``player`` group in Hydra's config store
+   :caption: Adding configs to the ``player`` group in hydra-zen's config store.
+
+   # pre-set the group name
+   player_store = store(group="player")
 
-   cs.store(group="player", name="base", node=CharConf)
-   cs.store(group="player", name="brinda", node=brinda_conf)
-   cs.store(group="player", name="rakesh", node=rakesh_conf)
+   player_store(CharConf, name="base")
+   player_store(brinda_conf, name="brinda")
+   player_store(rakesh_conf, name="rakesh")
 
 
 Updating Our Top-Level Config 
 -----------------------------
 
 With these groups specified, we can tell Hydra to use a particular group-entry as a 
-default config for that group. Let's specify the ``CharConf`` config, which we named ``base`` in the config store, as the default player-profile.
+default config for that group by specifying a `hydra_defaults` in our task function's 
+config. For this example, let's specify the ``CharConf`` config, which we named 
+``base`` in the config store, as the default player-profile.
 
 
 .. code-block:: python
-   :caption: Specifying the player-group item named ``base`` as the default player-profile
+   :caption: Specifying the player-group item named ``base`` as the default player-profile.
 
-   from hydra_zen import make_config
-
-   Config = make_config("player", hydra_defaults=["_self_", {"player": "base"}])
-   cs.store(name="my_app", node=Config)
+   @store(name="my_app",  hydra_defaults=["_self_", {"player": "base"}])
+   def task_function(player: Character):
+       ...
 
 .. note:: 
 
    The ``hydra-defaults`` field in our top-level config has special meaning in the 
    context of Hydra: it specifies a list that instructs Hydra how to build the 
    resulting config, and the list itself is not included in the config. You can read 
    about the Defaults List in :hydra:`this tutorial <tutorials/structured_config/
@@ -133,77 +139,83 @@
 
 Let's update the contents of ``my_app.py`` to reflect the changes that we just went 
 over. Modify your ``my_app.py`` script to match the following code.
 
 .. code-block:: python
    :caption: Contents of ``my_app.py``
 
-   import hydra
-   from hydra.core.config_store import ConfigStore
-   
-   from hydra_zen import instantiate, make_config, make_custom_builds_fn
+   from hydra_zen import store, make_custom_builds_fn, zen
    
    from game_library import inventory, Character
    
    builds = make_custom_builds_fn(populate_full_signature=True)
    
-   cs = ConfigStore.instance()
-
    # Create inventory configs
    InventoryConf = builds(inventory)
    starter_gear = InventoryConf(gold=10, weapon="stick", costume="tunic")
    advanced_gear = InventoryConf(gold=500, weapon="wand", costume="magic robe")
    hard_mode_gear = InventoryConf(gold=0, weapon="inner thoughts", costume="rags")
    
    # Register inventory configs under group: player/inventory
-   cs.store(group="player/inventory", name="starter", node=starter_gear)
-   cs.store(group="player/inventory", name="advanced", node=advanced_gear)
-   cs.store(group="player/inventory", name="hard_mode", node=hard_mode_gear)
+   inv_store = store(group="player/inventory")
+   
+   inv_store(starter_gear, name="starter")
+   inv_store(advanced_gear, name="advanced")
+   inv_store(hard_mode_gear, name="hard_mode")
    
    # Create player-profile configs
    CharConf = builds(Character, inventory=starter_gear)
-
+   
    brinda_conf = CharConf(
        name="brinda",
        level=47,
        inventory=InventoryConf(costume="cape", weapon="flute", gold=52),
    )
    
    rakesh_conf = CharConf(
        name="rakesh",
        level=300,
        inventory=InventoryConf(costume="PJs", weapon="pillow", gold=41),
    )
    
    # Register player-profile configs under group: player
-   cs.store(group="player", name="base", node=CharConf)
-   cs.store(group="player", name="brinda", node=brinda_conf)
-   cs.store(group="player", name="rakesh", node=rakesh_conf)
-   
-   # Specify default group for player to be: base
-   Config = make_config("player", hydra_defaults=["_self_", {"player": "base"}])
+   player_store = store(group="player")
+
+   player_store(CharConf, name="base")
+   player_store(brinda_conf, name="brinda")
+   player_store(rakesh_conf, name="rakesh")
    
-   cs.store(name="my_app", node=Config)
    
+   # The `hydra_defaults` field is specified in our task function's config.
+   # It instructs Hydra to use the player config that named 'base' in our 
+   # config store as the default config for our app.
+   @store(name="my_app",  hydra_defaults=["_self_", {"player": "base"}])
+   def task_function(player: Character):
    
-   @hydra.main(config_path=None, config_name="my_app")
-   def task_function(cfg):
-       # cfg: Config
-       player = instantiate(cfg.player)
        print(player)
    
-       with open("player_log.txt", "w") as f:
+       with open("player_log.txt", "a") as f:
            f.write("Game session log:\n")
            f.write(f"Player: {player}\n")
    
        return player
    
    
    if __name__ == "__main__":
-       task_function()
+       # We need to add the configs from our local store to Hydra's
+       # global config store
+       store.add_to_hydra_store()
+   
+       # Our zen-wrapped task function is used to generate
+       # the CLI, and to specify which config we want to use
+       # to configure the app by default
+       zen(task_function).hydra_main(config_name="my_app",
+                                     version_base="1.1",
+                                     config_path=".",
+                                     )
 
 .. tip::
 
    **A matter of housekeeping**: our configs need not be defined in the same file as
    ``task_function``. They can be defined - and added to the config store - in a 
    separate file in our library, e.g. ``configs.py``, or across multiple files. This is 
    nice from an organizational perspective, plus it enables to use these configs
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials/hierarchy.rst` & `hydra_zen-0.9.1/docs/source/tutorials/hierarchy.rst`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 .. code-block:: python
    :caption: Contents of ``game_library.py``
    
    # Should be in same directory as `my_app.py`
    
    # Note: type annotations are *not* required by hydra-zen
 
+   __all__ = ["inventory", "Character"]
+
+
    class Character:
        def __init__(self, name: str, level: int = 1, inventory=None):
            self.name = name
            self.level = level
            self.inventory = inventory
  
        def __repr__(self):
@@ -151,104 +154,77 @@
    starter_gear = InventoryConf(gold=10, weapon="stick", costume="tunic")
    
    # note: 
    # We are nesting the config for `inventory` within the 
    # config for `Character`.
    CharConf = builds(Character, inventory=starter_gear)
 
-Finally, the top-level config for our application will simply specify that ``player`` 
-is described by this character config:
-
-.. code-block:: python
-   :caption: The top-level config for our application
-
-   from hydra_zen import make_config
-
-   Config = make_config(player=CharConf)
-
 
 Updating the Task Function
 --------------------------
 
 We'll make some modifications to our task function.
 
 - We're only dealing with one player now, not two, so we adjust accordingly.
-- We need to make use of the :func:`~hydra_zen.instantiate` function to create the ``Character``-instance based on our config. 
 - Let's print ``Character``-instance for ``player`` so that we get instant feedback when we run our application from the CLI.
 
 .. code-block:: python
    :caption: A revised task function (single-player only)
 
-   def task_function(cfg):      
-       # `instantiate(cfg.player)` calls:
-       #
-       # Character(
-       #    name=cfg.player.name,
-       #    level=cfg.player.level,
-       #    inventory=inventory(gold=cfg.player.inventory.gold,
-       #                        weapon=cfg.player.inventory.weapon,
-       #                        costume=cfg.player.inventory.costume                        
-       # )
-       player = instantiate(cfg.player) # an instance of `Character`
-       print(player)
+   def task_function(player: Character):
 
-       with open("player_log.txt", "w") as f:
-           f.write("Game session log:\n")
-           f.write(f"Player: {player}\n")
-       
-       return player
+      print(player)
+
+      with open("player_log.txt", "a") as f:
+         f.write("Game session log:\n")
+         f.write(f"Player: {player}\n")
+
+      return player
 
 
 Piecing It All Together
 -----------------------
 
 Combining these configs and task function together - along with the boilerplate code 
 needed to :ref:`create a command line interface <cli-app>` - our updated ``my_app.py`` 
 script is as follows.
 
 .. code-block:: python
-    :caption: Contents of my_app.py:
+   :caption: Contents of my_app.py:
 
-    import hydra
-    from hydra.core.config_store import ConfigStore
-    
-    from hydra_zen import instantiate, make_config, make_custom_builds_fn
-    
-    from game_library import inventory, Character
-    
-    builds = make_custom_builds_fn(populate_full_signature=True)
-    
-    # generating configs
-    InventoryConf = builds(inventory)
-    starter_gear = InventoryConf(gold=10, weapon="stick", costume="tunic")
-    
-    CharConf = builds(Character, inventory=starter_gear)
-    
-    # creating the top-level config for our application
-    Config = make_config(player=CharConf)
-    
-    cs = ConfigStore.instance()
-    cs.store(name="my_app", node=Config)
-    
-    
-    @hydra.main(config_path=None, config_name="my_app")
-    def task_function(cfg):
-
-        player = instantiate(cfg.player) # an instance of `Character`
-
-        print(player)
-        
-        with open("player_log.txt", "w") as f:
-            f.write("Game session log:\n")
-            f.write(f"Player: {player}\n")
-
-        return player
-    
-    if __name__ == "__main__":
-        task_function()
+   from hydra_zen import make_custom_builds_fn, store, zen
+   
+   from game_library import inventory, Character
+   
+   builds = make_custom_builds_fn(populate_full_signature=True)
+   
+   # generating configs
+   starter_gear = builds(inventory, gold=10, weapon="stick", costume="tunic")
+   
+   CharConf = builds(Character, inventory=starter_gear)
+   
+   # Generate and store a top-level config specifying `CharConf` as the
+   # default config for `player`
+   @store(name="my_app", player=CharConf)
+   def task_function(player: Character):
+   
+       print(player)
+   
+       with open("player_log.txt", "a") as f:
+           f.write("Game session log:\n")
+           f.write(f"Player: {player}\n")
+   
+       return player
+   
+   if __name__ == "__main__":
+       store.add_to_hydra_store()
+       zen(task_function).hydra_main(config_name="my_app", 
+                                     version_base="1.1",
+                                     config_path=".",
+                                     )
 
 
 Running Our Application
 =======================
 
 We can now configure any aspect of the player when launching our application; let's try 
 a few examples in order to get a feel for the syntax.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials/inject_wrapper.rst` & `hydra_zen-0.9.1/docs/source/tutorials/inject_wrapper.rst`

 * *Files 6% similar despite different names*

```diff
@@ -94,66 +94,66 @@
 -----------------------------------
 
 Incorporating this wrapper into our application simply involves specifying it as a 
 "zen-wrapper" in our config for :class:`game_library.Character`. I.e. we will update:
 
 .. code:: python 
    
-   CharConf = builds(Character, inventory=starter_gear)
+   CharConf = builds(Character, ...)
 
 to be
 
 .. code:: python 
    
-   CharConf = builds(Character, inventory=starter_gear, zen_wrappers=halloween_update)
+   CharConf = builds(Character, ..., zen_wrappers=halloween_update)
 
 
 Putting It All Together
 -----------------------
 
 Let's update the contents of ``my_app.py`` to reflect the changes that we just went 
 over. Modify your ``my_app.py`` script to match the following code.
 
 .. code-block:: python
    :caption: Contents of ``my_app.py``
 
-   import hydra
-   from hydra.core.config_store import ConfigStore
-   
-   from hydra_zen import instantiate, make_config, make_custom_builds_fn
+   from hydra_zen import store, make_custom_builds_fn, zen
    
    from game_library import inventory, Character
    
+   builds = make_custom_builds_fn(populate_full_signature=True)
+   
+   
    # 1. Added our wrapper
    def halloween_update(CharClass):
        def wrapper(*args, **kwargs):
            # instantiate the Character
            char = CharClass(*args, **kwargs)
    
            costume = char.inventory["costume"]
            if costume:
                # update the costume
                char.inventory["costume"] = f"spooky {costume}"
            return char
    
        return wrapper
    
-   
-   builds = make_custom_builds_fn(populate_full_signature=True)
-   
-   cs = ConfigStore.instance()
-   
+
+   # Create inventory configs
    InventoryConf = builds(inventory)
    starter_gear = InventoryConf(gold=10, weapon="stick", costume="tunic")
    advanced_gear = InventoryConf(gold=500, weapon="wand", costume="magic robe")
    hard_mode_gear = InventoryConf(gold=0, weapon="inner thoughts", costume="rags")
    
-   cs.store(group="player/inventory", name="starter", node=starter_gear)
-   cs.store(group="player/inventory", name="advanced", node=advanced_gear)
-   cs.store(group="player/inventory", name="hard_mode", node=hard_mode_gear)
+   # Register inventory configs under group: player/inventory
+   inv_store = store(group="player/inventory")
+   
+   inv_store(starter_gear, name="starter")
+   inv_store(advanced_gear, name="advanced")
+   inv_store(hard_mode_gear, name="hard_mode")
    
    # 2. Included the wrapper in our config for `Character`
    CharConf = builds(Character, inventory=starter_gear, zen_wrappers=halloween_update)
    
    brinda_conf = CharConf(
        name="brinda",
        level=47,
@@ -162,39 +162,49 @@
    
    rakesh_conf = CharConf(
        name="rakesh",
        level=300,
        inventory=InventoryConf(costume="PJs", weapon="pillow", gold=41),
    )
    
-   cs.store(group="player", name="base", node=CharConf)
-   cs.store(group="player", name="brinda", node=brinda_conf)
-   cs.store(group="player", name="rakesh", node=rakesh_conf)
-   
-   
-   Config = make_config("player", hydra_defaults=["_self_", {"player": "base"}])
+   # Register player-profile configs under group: player
+   player_store = store(group="player")
+
+   player_store(CharConf, name="base")
+   player_store(brinda_conf, name="brinda")
+   player_store(rakesh_conf, name="rakesh")
    
-   cs.store(name="my_app", node=Config)
    
+   # The `hydra_defaults` field is specified in our task function's config.
+   # It instructs Hydra to use the player config that named 'base' in our
+   # config store as the default config for our app.
+   @store(name="my_app",  hydra_defaults=["_self_", {"player": "base"}])
+   def task_function(player: Character):
    
-   @hydra.main(config_path=None, config_name="my_app")
-   def task_function(cfg):
-       # cfg: Config
-       player = instantiate(cfg.player)
        print(player)
    
-       with open("player_log.txt", "w") as f:
+       with open("player_log.txt", "a") as f:
            f.write("Game session log:\n")
            f.write(f"Player: {player}\n")
    
        return player
    
    
    if __name__ == "__main__":
-       task_function()
+       # We need to add the configs from our local store to Hydra's
+       # global config store
+       store.add_to_hydra_store()
+   
+       # Our zen-wrapped task function is used to generate
+       # the CLI, and to specify which config we want to use
+       # to configure the app by default
+       zen(task_function).hydra_main(config_name="my_app",
+                                     version_base="1.1",
+                                     config_path=".",
+                                     )
 
 Running Our Application
 =======================
 
 We can configure and launch our application exactly as we had before, but now all of 
 the player's costumes will automatically become 👻 spooky 👻.
```

### Comparing `hydra_zen-0.9.0rc5/docs/source/tutorials.rst` & `hydra_zen-0.9.1/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/__init__.py` & `hydra_zen-0.9.1/src/hydra_zen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 from typing import TYPE_CHECKING
 
 from ._hydra_overloads import (
     MISSING,
     instantiate,
     load_from_yaml,
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/_compatibility.py` & `hydra_zen-0.9.1/src/hydra_zen/_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 from collections import Counter, deque
 from enum import Enum
 from functools import partial
 from pathlib import Path, PosixPath, WindowsPath
 from typing import NamedTuple, Set
 
@@ -85,7 +85,9 @@
 if HYDRA_SUPPORTS_Path:  # pragma: no cover
     HYDRA_SUPPORTED_PRIMITIVES.update(_path_types)
     HYDRA_SUPPORTED_PRIMITIVE_TYPES.add(Path)
 else:  # pragma: no cover
     ZEN_SUPPORTED_PRIMITIVES.update(_path_types)
 
 del _path_types
+
+HYDRA_SUPPORTS_OBJECT_CONVERT = HYDRA_VERSION >= Version(1, 3, 0)
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/_hydra_overloads.py` & `hydra_zen-0.9.1/src/hydra_zen/_hydra_overloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 """
 Provides annotation overloads for various hydra functions, using the types defined in `hydra_zen.typing`.
 This enables tools like IDEs to be more incisive during static analysis and to provide users with additional
 context about their code.
 
 E.g.
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/_launch.py` & `hydra_zen-0.9.1/src/hydra_zen/_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import warnings
 from dataclasses import fields, is_dataclass
 from typing import Any, Callable, List, Mapping, Optional, Type, Union
 
 from hydra import initialize
 from hydra._internal.callbacks import Callbacks
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/_utils/coerce.py` & `hydra_zen-0.9.1/src/hydra_zen/_utils/coerce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) 2023 Massachusetts Institute of Technology
+# SPDX-License-Identifier: MIT
+
 import sys
 
 if sys.version_info < (3, 7):  # pragma: no cover
     raise NotImplementedError(
         "Features that utilize `hydra_zen._utils.coerce` "
         "(e.g. beartype-validation) require Python 3.7 or greater."
     )
@@ -77,15 +80,15 @@
     -------
     wrapped_obj
 
     Notes
     -----
     The supported non-string sequence types are:
     - tuples
-    - deques
+    - dequeues
     - lists
     - named-tuples
 
     The only Union-based types that are supported are of the form
     ``Optional[<sequence-type>]``.
 
     Examples
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/errors.py` & `hydra_zen-0.9.1/src/hydra_zen/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 
 
 class HydraZenException(Exception):
     """Generic parent class for exceptions thrown by hydra-zen."""
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/funcs.py` & `hydra_zen-0.9.1/src/hydra_zen/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 
 """
 Simple helper functions used to implement `just` and `builds`. This module is designed specifically so
 that these functions have a legible module-path when they appear in configuration files.
 """
 import functools as _functools
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_globals.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 # pyright: strict
 from typing import FrozenSet
 
 from typing_extensions import Final
 
 from hydra_zen._compatibility import HYDRA_SUPPORTS_PARTIAL
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_implementations.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_implementations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import functools
 import inspect
 import sys
 import warnings
 from dataclasses import (  # use this for runtime checks
     MISSING,
@@ -38,21 +38,26 @@
 
 from hydra_zen._compatibility import (
     HYDRA_SUPPORTED_PRIMITIVES,
     HYDRA_SUPPORTS_PARTIAL,
     PATCH_OMEGACONF_830,
     ZEN_SUPPORTED_PRIMITIVES,
 )
-from hydra_zen.errors import HydraZenUnsupportedPrimitiveError, HydraZenValidationError
+from hydra_zen.errors import (
+    HydraZenDeprecationWarning,
+    HydraZenUnsupportedPrimitiveError,
+    HydraZenValidationError,
+)
 from hydra_zen.funcs import get_obj
 from hydra_zen.structured_configs import _utils
+from hydra_zen.structured_configs._type_guards import safe_getattr
 from hydra_zen.typing import (
     Builds,
+    DataclassOptions,
     Importable,
-    Just,
     PartialBuilds,
     SupportedPrimitive,
     ZenWrappers,
 )
 from hydra_zen.typing._implementations import (
     AllConvert,
     BuildsWithSig,
@@ -63,28 +68,33 @@
     InstOrType,
     ZenConvert,
 )
 
 from ._globals import (
     CONVERT_FIELD_NAME,
     DEFAULTS_LIST_FIELD_NAME,
-    GET_OBJ_LOCATION,
     HYDRA_FIELD_NAMES,
     JUST_FIELD_NAME,
     META_FIELD_NAME,
     PARTIAL_FIELD_NAME,
     POS_ARG_FIELD_NAME,
     RECURSIVE_FIELD_NAME,
     TARGET_FIELD_NAME,
     ZEN_PARTIAL_FIELD_NAME,
     ZEN_PROCESSING_LOCATION,
     ZEN_TARGET_FIELD_NAME,
     ZEN_WRAPPERS_FIELD_NAME,
 )
-from ._type_guards import is_builds, is_just, is_old_partial_builds, uses_zen_processing
+from ._type_guards import (
+    is_builds,
+    is_just,
+    is_old_partial_builds,
+    safe_getattr,
+    uses_zen_processing,
+)
 
 _T = TypeVar("_T")
 
 P = ParamSpec("P")
 R = TypeVar("R")
 Field_Entry: TypeAlias = Tuple[str, type, Field[Any]]
 
@@ -170,30 +180,42 @@
     >>> x
     HasMutableDefault(a_list=[1, 2, 3, -1])
     >>> HasMutableDefault()
     HasMutableDefault(a_list=[1, 2, 3])"""
     cast = type(x)  # ensure that we return a copy of the default value
     settings = _utils.merge_settings(zen_convert, _BUILDS_CONVERT_SETTINGS)
     del zen_convert
-    x = sanitize_collection(x, convert_dataclass=settings["dataclass"])
-    return field(default_factory=lambda: cast(x))
+
+    if cast in {list, tuple, dict}:
+        x = sanitize_collection(x, convert_dataclass=settings["dataclass"])
+        return field(default_factory=lambda: cast(x))
+    return field(default_factory=lambda: x)
 
 
 @dataclass_transform()
 def hydrated_dataclass(
     target: Callable[..., Any],
     *pos_args: SupportedPrimitive,
     zen_partial: Optional[bool] = None,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = tuple(),
     zen_meta: Optional[Mapping[str, Any]] = None,
     populate_full_signature: bool = False,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
-    frozen: bool = False,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
     zen_convert: Optional[ZenConvert] = None,
+    init: bool = True,
+    repr: bool = True,
+    eq: bool = True,
+    order: bool = False,
+    unsafe_hash: bool = True,
+    frozen: bool = False,
+    match_args: bool = True,
+    kw_only: bool = False,
+    slots: bool = False,
+    weakref_slot: bool = False,
 ) -> Callable[[Type[_T]], Type[_T]]:
     """A decorator that uses `builds` to create a dataclass with the appropriate
     Hydra-specific fields for specifying a targeted config [1]_.
 
     This provides similar functionality to `builds`, but enables a user to define
     a config explicitly using the :func:`dataclasses.dataclass` syntax, which can
     enable enhanced static analysis of the resulting config.
@@ -262,18 +284,88 @@
         - ``"none"``: No conversion occurs; omegaconf containers are passed through (Default)
         - ``"partial"``: ``DictConfig`` and ``ListConfig`` objects converted to ``dict`` and
           ``list``, respectively. Structured configs and their fields are passed without conversion.
         - ``"all"``: All passed objects are converted to dicts, lists, and primitives, without a trace of OmegaConf containers.
 
         If ``None``, the ``_convert_`` attribute is not set on the resulting config.
 
+    hydra_convert : Optional[Literal["none", "partial", "all", "object"]], optional (default="none")
+        Determines how Hydra treats the non-primitive, omegaconf-specific objects
+        during instantiateion [3]_.
+
+        - ``"none"``: No conversion occurs; omegaconf containers are passed through (Default)
+        - ``"partial"``: ``DictConfig`` and ``ListConfig`` objects converted to ``dict`` and
+          ``list``, respectively. Structured configs and their fields are passed without conversion.
+        - ``"all"``: All passed objects are converted to dicts, lists, and primitives, without
+          a trace of OmegaConf containers.
+        - ``"object"``: Passed objects are converted to dict and list. Structured Configs are converted to instances of the backing dataclass / attr class.
+
+        If ``None``, the ``_convert_`` attribute is not set on the resulting config.
+
+    init : bool, optional (default=True)
+        If true (the default), a __init__() method will be generated. If the class
+        already defines __init__(), this parameter is ignored.
+
+    repr : bool, optional (default=True)
+        If true (the default), a `__repr__()` method will be generated. The generated
+        repr string will have the class name and the name and repr of each field, in
+        the order they are defined in the class. Fields that are marked as being
+        excluded from the repr are not included. For example:
+        `InventoryItem(name='widget', unit_price=3.0, quantity_on_hand=10)`.
+
+    eq : bool, optional (default=True)
+        If true (the default), an __eq__() method will be generated. This method
+        compares the class as if it were a tuple of its fields, in order. Both
+        instances in the comparison must be of the identical type.
+
+    order : bool, optional (default=False)
+        If true (the default is `False`), `__lt__()`, `__le__()`, `__gt__()`, and
+        `__ge__()` methods will be generated. These compare the class as if it were a
+        tuple of its fields, in order. Both instances in the comparison must be of the
+        identical type. If order is true and eq is false, a ValueError is raised.
+
+        If the class already defines any of `__lt__()`, `__le__()`, `__gt__()`, or
+        `__ge__()`, then `TypeError` is raised.
+
+    unsafe_hash : bool, optional (default=False)
+        If `False` (the default), a `__hash__()` method is generated according to how
+        `eq` and `frozen` are set.
+
+        If `eq` and `frozen` are both true, by default `dataclass()` will generate a
+        `__hash__()` method for you. If `eq` is true and `frozen` is false, `__hash__()
+        ` will be set to `None`, marking it unhashable. If `eq` is false, `__hash__()`
+        will be left untouched meaning the `__hash__()` method of the superclass will
+        be used (if the superclass is object, this means it will fall back to id-based
+        hashing).
+
     frozen : bool, optional (default=False)
-        If ``True``, the resulting config will create frozen (i.e. immutable) instances.
-        I.e. setting/deleting an attribute of an instance will raise
-        :py:class:`dataclasses.FrozenInstanceError` at runtime.
+        If true (the default is `False`), assigning to fields will generate an
+        exception. This emulates read-only frozen instances.
+
+    match_args : bool, optional (default=True)
+        (*New in version 3.10*) If true (the default is `True`), the `__match_args__`
+        tuple will be created from the list of parameters to the generated `__init__()`
+        method (even if `__init__()` is not generated, see above). If false, or if
+        `__match_args__` is already defined in the class, then `__match_args__` will
+        not be generated.
+
+    kw_only : bool, optional (default=False)
+        (*New in version 3.10*) If true (the default value is `False`), then all fields
+        will be marked as keyword-only.
+
+    slots : bool, optional (default=False)
+        (*New in version 3.10*) If true (the default is `False`), `__slots__` attribute
+        will be generated and new class will be returned instead of the original one.
+        If `__slots__` is already defined in the class, then `TypeError` is raised.
+
+    weakref_slot : bool, optional (default=False)
+        (*New in version 3.11*) If true (the default is `False`), add a slot named
+        “__weakref__”, which is required to make an instance weakref-able. It is an
+        error to specify `weakref_slot=True` without also specifying `slots=True`.
+
 
     See Also
     --------
     builds : Create a targeted structured config designed to "build" a particular object.
 
     Raises
     ------
@@ -302,22 +394,28 @@
     **Basic usage**
 
     >>> from hydra_zen import hydrated_dataclass, instantiate
 
     Here, we specify a config that is designed to "build" a dictionary
     upon instantiation
 
-    >>> @hydrated_dataclass(target=dict)
+    >>> @hydrated_dataclass(target=dict, frozen=True)
     ... class DictConf:
     ...     x: int = 2
     ...     y: str = 'hello'
 
     >>> instantiate(DictConf(x=10))  # override default `x`
     {'x': 10, 'y': 'hello'}
 
+    >>> d = DictConf()
+    >>> # Static type checker marks the following as
+    >>> # an error because `d` is frozen.
+    >>> d.x = 3  # type: ignore
+    FrozenInstanceError: cannot assign to field 'x'
+
     For more detailed examples, refer to `builds`.
     """
 
     def wrapper(decorated_obj: Any) -> Any:
 
         if not isinstance(decorated_obj, type):
             raise NotImplementedError(
@@ -325,16 +423,29 @@
             )
 
         # TODO: We should mutate `decorated_obj` directly like @dataclass does.
         #       Presently, we create an intermediate dataclass that we inherit
         #       from, which gets the job done for the most part but there are
         #       practical differences. E.g. you cannot delete an attribute that
         #       was declared in the definition of `decorated_obj`.
-        decorated_obj = cast(Any, decorated_obj)
-        decorated_obj = dataclass(frozen=frozen)(decorated_obj)
+        dc_options = _utils.parse_dataclass_options(
+            {
+                "init": init,
+                "repr": repr,
+                "eq": eq,
+                "order": order,
+                "unsafe_hash": unsafe_hash,
+                "frozen": frozen,
+                "match_args": match_args,
+                "kw_only": kw_only,
+                "slots": slots,
+                "weakref_slot": weakref_slot,
+            }
+        )
+        decorated_obj = dataclass(**dc_options)(decorated_obj)  # type: ignore
 
         if PATCH_OMEGACONF_830 and 2 < len(decorated_obj.__mro__):  # pragma: no cover
             parents = decorated_obj.__mro__[1:-1]
             # this class inherits from a parent
             for field_ in fields(decorated_obj):
                 if field_.default_factory is not MISSING and any(
                     hasattr(p, field_.name) for p in parents
@@ -368,49 +479,46 @@
             populate_full_signature=populate_full_signature,
             hydra_recursive=hydra_recursive,
             hydra_convert=hydra_convert,
             zen_wrappers=zen_wrappers,
             zen_partial=zen_partial,
             zen_meta=zen_meta,
             builds_bases=(decorated_obj,),
-            dataclass_name=decorated_obj.__name__,
-            frozen=frozen,
+            zen_dataclass={
+                "cls_name": decorated_obj.__name__,
+                "module": decorated_obj.__module__,
+                "init": init,
+                "repr": repr,
+                "eq": eq,
+                "order": order,
+                "unsafe_hash": unsafe_hash,
+                "frozen": frozen,
+                "match_args": match_args,
+                "kw_only": kw_only,
+                "slots": slots,
+                "weakref_slot": weakref_slot,
+            },
             zen_convert=zen_convert,
         )
-        out.__module__ = decorated_obj.__module__
+
         return out
 
     return wrapper
 
 
-def _just(obj: Importable) -> Type[Just[Importable]]:
-    obj_path = _utils.get_obj_path(obj)
+@dataclass(frozen=True)
+class Just:
+    """Just[T] is a config that returns T when instantiated."""
 
-    entry: List[Tuple[Any, Any, Field[Any]]] = [
-        (
-            TARGET_FIELD_NAME,
-            str,
-            _utils.field(default=GET_OBJ_LOCATION, init=False),
-        ),
-        (
-            JUST_FIELD_NAME,
-            str,
-            _utils.field(
-                default=obj_path,
-                init=False,
-            ),
-        ),
-    ]
+    path: str
+    _target_: str = field(default="hydra_zen.funcs.get_obj", init=False, repr=False)
 
-    out_class = make_dataclass(("Just_" + _utils.safe_name(obj)), entry)
-    out_class.__doc__ = (
-        f"A structured config designed to return {obj} when it is instantiated by hydra"
-    )
 
-    return cast(Type[Just[Importable]], out_class)
+def _just(obj: Any) -> Just:
+    return Just(path=_utils.get_obj_path(obj))
 
 
 def _is_ufunc(value: Any) -> bool:
     # checks without importing numpy
     numpy = sys.modules.get("numpy")
     if numpy is None:  # pragma: no cover
         # we do actually cover this branch some runs of our CI,
@@ -429,14 +537,27 @@
     try:
         CompiledFunction = getattr(jaxlib_xla_extension, "CompiledFunction")
         return isinstance(value, CompiledFunction)
     except AttributeError:
         return False
 
 
+def _is_torch_optim_required(value: Any) -> bool:  # pragma: no cover
+    torch_optim_optimizer = sys.modules.get("torch.optim.optimizer")
+
+    if torch_optim_optimizer is None:
+        return False
+
+    try:
+        required = getattr(torch_optim_optimizer, "required")
+        return value is required
+    except AttributeError:
+        return False
+
+
 def _check_for_dynamically_defined_dataclass_type(target_path: str, value: Any) -> None:
     if target_path.startswith("types."):
         raise HydraZenUnsupportedPrimitiveError(
             f"Configuring {value}: Cannot auto-config an instance of a "
             f"dynamically-generated dataclass type (e.g. one created from "
             f"`hydra_zen.make_config` or `dataclasses.make_dataclass`). "
             f"Consider disabling auto-config support for dataclasses here."
@@ -448,15 +569,16 @@
     allow_zen_conversion: bool = True,
     *,
     error_prefix: str = "",
     field_name: str = "",
     structured_conf_permitted: bool = True,
     convert_dataclass: bool,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
+    zen_dataclass: Optional[DataclassOptions] = None,
 ) -> Any:
     """Converts `value` to Hydra-supported type if necessary and possible. Otherwise
     raises `HydraZenUnsupportedPrimitiveError`"""
     # Common primitives supported by Hydra.
     # We check exhaustively for all Hydra-supported primitives below but seek to
     # speedup checks for common types here.
     if value is None or type(value) in {str, int, bool, float}:
@@ -467,14 +589,17 @@
         value = sanitize_collection(
             value,
             convert_dataclass=convert_dataclass,
             hydra_convert=hydra_convert,
             hydra_recursive=hydra_recursive,
         )
 
+    if zen_dataclass is None:
+        zen_dataclass = {}
+
     # non-targeted dataclass instance
     if (
         structured_conf_permitted
         and convert_dataclass
         and not is_builds(value)
         and (is_dataclass(value) and not isinstance(value, type))
     ):
@@ -489,30 +614,31 @@
                 f"type has an Init-only field. Consider using "
                 f"`builds({type(value).__name__}, ...)` instead."
             )
 
         converted_fields = {}
         for _field in _val_fields:
             if _field.init and hasattr(value, _field.name):
-                _val = getattr(value, _field.name)
+                _val = safe_getattr(value, _field.name)
                 converted_fields[_field.name] = sanitized_default_value(
                     _val,
                     allow_zen_conversion=allow_zen_conversion,
                     field_name=_field.name,
                     convert_dataclass=convert_dataclass,
                 )
 
         out = builds(
             type(value),
             **converted_fields,
             hydra_recursive=hydra_recursive,
             hydra_convert=hydra_convert,
+            zen_dataclass=zen_dataclass,
         )
         _check_for_dynamically_defined_dataclass_type(
-            getattr(out, TARGET_FIELD_NAME), value
+            safe_getattr(out, TARGET_FIELD_NAME), value
         )
         return out
 
     # importable callable (function, type, or method)
     if (
         structured_conf_permitted
         and callable(value)
@@ -529,18 +655,18 @@
             or isinstance(value, _BUILTIN_TYPES)
             or _is_ufunc(value)
             or _is_jax_compiled_func(value)
         )
     ):
         # `value` is importable callable -- create config that will import
         # `value` upon instantiation
-        out = _just(value)  # type: ignore
+        out = _just(value)
         if convert_dataclass and is_dataclass(value):
             _check_for_dynamically_defined_dataclass_type(
-                getattr(out, JUST_FIELD_NAME), value
+                safe_getattr(out, JUST_FIELD_NAME), value
             )
         return out
 
     resolved_value = value
     type_of_value = type(resolved_value)
 
     # hydra-zen supported primitives from stdlib
@@ -589,14 +715,18 @@
         # Supports pydantic.AnyURL
         _v = str(value)
         if type(_v) is str:  # pragma: no branch
             return _v
         else:  # pragma: no cover
             del _v
 
+    # support for torch objects
+    if _is_torch_optim_required(value):  # pragma: no cover
+        return MISSING
+
     # `value` could no be converted to Hydra-compatible representation.
     # Raise error
     if field_name:
         field_name = f", for field `{field_name}`,"
 
     err_msg = (
         error_prefix
@@ -614,15 +744,15 @@
 
 
 def sanitize_collection(
     x: _T,
     *,
     convert_dataclass: bool,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
 ) -> _T:
     """Pass contents of lists, tuples, or dicts through sanitized_default_values"""
     type_x = type(x)
     if type_x in {list, tuple}:
         return type_x(sanitized_default_value(_x, convert_dataclass=convert_dataclass, hydra_convert=hydra_convert, hydra_recursive=hydra_recursive) for _x in x)  # type: ignore
     elif type_x is dict:
         return {
@@ -666,14 +796,16 @@
         convert_dataclass=convert_dataclass,
     )
 
     type_value = type(value)
     if (
         type_value in _utils.KNOWN_MUTABLE_TYPES
         and type_value in HYDRA_SUPPORTED_PRIMITIVES
+    ) or (
+        is_dataclass(value) and not isinstance(value, type) and value.__hash__ is None
     ):
         if _mutable_default_permitted:
             return cast(
                 Field[Any],
                 mutable_value(value, zen_convert={"dataclass": convert_dataclass}),
             )
         else:  # pragma: no cover
@@ -690,18 +822,19 @@
     __hydra_target: Callable[P, R],
     *,
     zen_partial: Literal[False, None] = ...,
     populate_full_signature: Literal[True],
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
     hydra_defaults: Optional[DefaultsList] = ...,
     dataclass_name: Optional[str] = ...,
     builds_bases: Tuple[()] = ...,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> Type[BuildsWithSig[Type[R], P]]:
     ...
 
 
 # partial=False, pop-sig=bool
@@ -710,18 +843,19 @@
     __hydra_target: Importable,
     *pos_args: SupportedPrimitive,
     zen_partial: Literal[False, None] = ...,
     populate_full_signature: bool = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
     hydra_defaults: Optional[DefaultsList] = ...,
     dataclass_name: Optional[str] = ...,
     builds_bases: Tuple[Type[DataClass_], ...] = ...,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
     **kwargs_for_target: SupportedPrimitive,
 ) -> Type[Builds[Importable]]:
     ...
 
 
@@ -731,18 +865,19 @@
     __hydra_target: Importable,
     *pos_args: SupportedPrimitive,
     zen_partial: Literal[True] = ...,
     populate_full_signature: bool = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
     hydra_defaults: Optional[DefaultsList] = ...,
     dataclass_name: Optional[str] = ...,
     builds_bases: Tuple[Type[DataClass_], ...] = ...,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
     **kwargs_for_target: SupportedPrimitive,
 ) -> Type[PartialBuilds[Importable]]:
     ...
 
 
@@ -752,18 +887,19 @@
     __hydra_target: Importable,
     *pos_args: SupportedPrimitive,
     zen_partial: Optional[bool] = ...,
     populate_full_signature: Literal[False] = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
     hydra_defaults: Optional[DefaultsList] = ...,
     dataclass_name: Optional[str] = ...,
     builds_bases: Tuple[Type[DataClass_], ...] = ...,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
     **kwargs_for_target: SupportedPrimitive,
 ) -> Union[Type[Builds[Importable]], Type[PartialBuilds[Importable]],]:
     ...
 
 
@@ -773,18 +909,19 @@
     __hydra_target: Union[Callable[P, R], Importable],
     *pos_args: SupportedPrimitive,
     zen_partial: Optional[bool],
     populate_full_signature: bool = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
     hydra_defaults: Optional[DefaultsList] = ...,
     dataclass_name: Optional[str] = ...,
     builds_bases: Tuple[Type[DataClass_], ...] = ...,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
     **kwargs_for_target: SupportedPrimitive,
 ) -> Union[
     Type[Builds[Importable]],
     Type[PartialBuilds[Importable]],
     Type[BuildsWithSig[Type[R], P]],
@@ -796,19 +933,18 @@
     *pos_args: Union[Importable, Callable[P, R], SupportedPrimitive],
     zen_partial: Optional[bool] = None,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = tuple(),
     zen_meta: Optional[Mapping[str, SupportedPrimitive]] = None,
     populate_full_signature: bool = False,
     zen_convert: Optional[ZenConvert] = None,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
     hydra_defaults: Optional[DefaultsList] = None,
-    frozen: bool = False,
     builds_bases: Tuple[Type[DataClass_], ...] = (),
-    dataclass_name: Optional[str] = None,
+    zen_dataclass: Optional[DataclassOptions] = None,
     **kwargs_for_target: SupportedPrimitive,
 ) -> Union[
     Type[Builds[Importable]],
     Type[PartialBuilds[Importable]],
     Type[BuildsWithSig[Type[R], P]],
 ]:
     """builds(hydra_target, /, *pos_args, zen_partial=None, zen_wrappers=(), zen_meta=None, populate_full_signature=False, hydra_recursive=None, hydra_convert=None, hydra_defaults=None, frozen=False, dataclass_name=None, builds_bases=(), **kwargs_for_target)
@@ -893,38 +1029,54 @@
 
     hydra_recursive : Optional[bool], optional (default=True)
         If ``True``, then Hydra will recursively instantiate all other
         hydra-config objects nested within this config [3]_.
 
         If ``None``, the ``_recursive_`` attribute is not set on the resulting config.
 
-    hydra_convert : Optional[Literal["none", "partial", "all"]], optional (default="none")
+    hydra_convert : Optional[Literal["none", "partial", "all", "object"]], optional (default="none")
         Determines how Hydra handles the non-primitive, omegaconf-specific objects passed to
         ``<hydra_target>`` [4]_.
 
         - ``"none"``: No conversion occurs; omegaconf containers are passed through (Default)
         - ``"partial"``: ``DictConfig`` and ``ListConfig`` objects converted to ``dict`` and
           ``list``, respectively. Structured configs and their fields are passed without conversion.
         - ``"all"``: All passed objects are converted to dicts, lists, and primitives, without
           a trace of OmegaConf containers.
+        - ``"object"``: Passed objects are converted to dict and list. Structured Configs are converted to instances of the backing dataclass / attr class.
 
         If ``None``, the ``_convert_`` attribute is not set on the resulting config.
 
     hydra_defaults : None | list[str | dict[str, str | list[str] | None ]], optional (default = None)
         A list in an input config that instructs Hydra how to build the output config
         [6]_ [7]_. Each input config can have a Defaults List as a top level element. The
         Defaults List itself is not a part of output config.
 
+    zen_dataclass : Optional[DataclassOptions]
+        A dictionary that can specify any option that is supported by
+        :py:func:`dataclasses.make_dataclass` other than `fields`.
+        The default value for `unsafe_hash` is `True`.
+
+        Additionally, the `module` field can be specified to enable pickle
+        compatibility. See `hydra_zen.typing.DataclassOptions` for details.
+
     frozen : bool, optional (default=False)
+        .. deprecated:: 0.9.0
+            `frozen` will be removed in hydra-zen 0.10.0. It is replaced by
+            `zen_dataclass={'frozen': <bool>}`.
+
         If ``True``, the resulting config will create frozen (i.e. immutable) instances.
         I.e. setting/deleting an attribute of an instance will raise
         :py:class:`dataclasses.FrozenInstanceError` at runtime.
 
-
     dataclass_name : Optional[str]
+        .. deprecated:: 0.9.0
+            `dataclass_name` will be removed in hydra-zen 0.10.0. It is replaced by
+            `zen_dataclass={'cls_name': <str>}`.
+
         If specified, determines the name of the returned class object.
 
     Returns
     -------
     Config : Type[Builds[Type[T]]] | Type[PartialBuilds[Type[T]]]
         A dynamically-generated structured config (i.e. a dataclass type) that
         describes how to build ``hydra_target``.
@@ -970,16 +1122,16 @@
                for hint, (field_name, v) in zip(type_annots, kw.items())
            ]
 
            Config = make_dataclass(f"Builds_{target}", fields)
            return Config
 
     The resulting "config" is a dynamically-generated dataclass type [5]_ with
-    Hydra-specific attributes attached to it [1]_. It posseses a `_target_` attribute
-    that indicates the import path to the configured target as a string.
+    Hydra-specific attributes attached to it [1]_. It possesses a `_target_`
+    attribute that indicates the import path to the configured target as a string.
 
     Using any of the ``zen_xx`` features will result in a config that depends
     explicitly on hydra-zen. I.e. hydra-zen must be installed in order to
     instantiate the resulting config, including its yaml version.
 
     For details of the annotation `SupportedPrimitive`, see :ref:`valid-types`.
 
@@ -1011,24 +1163,27 @@
     just: Produces a config that, when instantiated by Hydra, "just" returns the un-instantiated target-object.
     to_yaml: Serialize a config as a yaml-formatted string.
 
     Examples
     --------
     These examples describe:
 
-    - Basic usage of `builds`
+    - Basic usage
     - Creating a partial config
     - Auto-populating parameters
     - Composing configs via inheritance
-    - Runtime validation performed by `builds`
+    - Runtime validation performed by builds
     - Using meta-fields
     - Using zen-wrappers
+    - Creating a pickle-compatible config
     - Creating a frozen config
     - Support for partial'd targets
 
+    A helpful utility for printing examples
+
     >>> from hydra_zen import builds, instantiate, to_yaml
     >>> def pyaml(x):
     ...     # for pretty printing configs
     ...     print(to_yaml(x))
 
     **Basic Usage**
 
@@ -1127,15 +1282,15 @@
     >>> instantiate(ChildConf)
     {'a': 1, 'b': -2, 'c': -3}
     >>> issubclass(ChildConf, ParentConf)
     True
 
     .. _builds-validation:
 
-    **Runtime validation perfomed by builds**
+    **Runtime validation performed by builds**
 
     Misspelled parameter names and other invalid configurations for the target’s
     signature will be caught by `builds` so that such errors are caught prior to
     instantiation.
 
     >>> def func(a_number: int): pass
 
@@ -1174,17 +1329,17 @@
 
     **Using zen-wrappers**
 
     Zen-wrappers enables us to make arbitrary changes to ``<hydra_target>``, its inputs,
     and/or its outputs during the instantiation process.
 
     Let's use a wrapper to add a unit-conversion step to a config. We'll modify a
-    config that builds a function, which converts a temperature in Farenheit to
-    Celcius, and add a wrapper to it so that it will convert from Farenheit to Kelvin
-    instead.
+    config that builds a function, which converts a temperature in Fahrenheit to
+    Celsius, and add a wrapper to it so that it will convert from Fahrenheit to
+    Kelvin instead.
 
     >>> def faren_to_celsius(temp_f):  # our target
     ...     return ((temp_f - 32) * 5) / 9
 
     >>> def change_celcius_to_kelvin(celc_func):  # our wrapper
     ...     def wraps(*args, **kwargs):
     ...         return 273.15 + celc_func(*args, **kwargs)
@@ -1193,19 +1348,37 @@
     >>> AsCelcius = builds(faren_to_celsius)
     >>> AsKelvin = builds(faren_to_celsius, zen_wrappers=change_celcius_to_kelvin)
     >>> instantiate(AsCelcius, temp_f=32)
     0.0
     >>> instantiate(AsKelvin, temp_f=32)
     273.15
 
+    **Creating a pickle-compatible config**
+
+    The dynamically-generated classes created by `builds` can be made pickle-compatible
+    by specifying the name of the symbol that it is assigned to and the module in which
+    it was defined.
+
+    .. code-block:: python
+
+       # contents of mylib/foo.py
+       from pickle import dumps, loads
+
+       DictConf = builds(dict,
+                         zen_dataclass={'module': 'mylib.foo',
+                                        'cls_name': 'DictConf'})
+
+       assert DictConf is loads(dumps(DictConf))
+
+
     **Creating a frozen config**
 
     Let's create a config object whose instances will by "frozen" (i.e., immutable).
 
-    >>> RouterConfig = builds(dict, ip_address=None, frozen=True)
+    >>> RouterConfig = builds(dict, ip_address=None, zen_dataclass={'frozen': True})
     >>> my_router = RouterConfig(ip_address="192.168.56.1")  # an immutable instance
 
     Attempting to overwrite the attributes of ``my_router`` will raise.
 
     >>> my_router.ip_address = "148.109.37.2"
     FrozenInstanceError: cannot assign to field 'ip_address'
 
@@ -1218,16 +1391,47 @@
     >>> partiald_dict = functools.partial(dict, a=1, b=2)
     >>> Conf = builds(partiald_dict)  # signature: (a = 1, b = 2)
     >>> instantiate(Conf)  # equivalent to calling: `partiald_dict()`
     {'a': 1, 'b': 2}
     >>> instantiate(Conf(a=-4))  # equivalent to calling: `partiald_dict(a=-4)`
     {'a': -4, 'b': 2}
     """
-
     zen_convert_settings = _utils.merge_settings(zen_convert, _BUILDS_CONVERT_SETTINGS)
+    if zen_dataclass is None:
+        zen_dataclass = {}
+
+    # initial validation
+    _utils.parse_dataclass_options(zen_dataclass)
+
+    if "frozen" in kwargs_for_target:
+        warnings.warn(
+            HydraZenDeprecationWarning(
+                "Specifying `builds(..., frozen=<...>)` is deprecated. Instead, "
+                "specify `builds(..., zen_dataclass={'frozen': <...>})"
+            ),
+            stacklevel=2,
+        )
+        zen_dataclass["frozen"] = kwargs_for_target.pop("frozen")  # type: ignore
+
+    if "dataclass_name" in kwargs_for_target:
+        warnings.warn(
+            HydraZenDeprecationWarning(
+                "Specifying `builds(..., dataclass_name=<...>)` is deprecated. "
+                "Instead specify `builds(..., zen_dataclass={'cls_name': <...>})"
+            ),
+            stacklevel=2,
+        )
+        zen_dataclass["cls_name"] = kwargs_for_target.pop("dataclass_name")  # type: ignore
+    if not builds_bases:
+        builds_bases = zen_dataclass.get("bases", ())
+
+    dataclass_options = _utils.parse_dataclass_options(zen_dataclass)
+    dataclass_name = dataclass_options.pop("cls_name", None)
+    module = dataclass_options.pop("module", None)
+
     del zen_convert
 
     if not pos_args and not kwargs_for_target:
         # `builds()`
         raise TypeError(
             "builds() missing 1 required positional argument: 'hydra_target'"
         )
@@ -1266,22 +1470,14 @@
     if zen_partial is not None and not isinstance(zen_partial, bool):
         raise TypeError(f"`zen_partial` must be a boolean type, got: {zen_partial}")
 
     _utils.validate_hydra_options(
         hydra_recursive=hydra_recursive, hydra_convert=hydra_convert
     )
 
-    if not isinstance(frozen, bool):
-        raise TypeError(f"frozen must be a bool, got: {frozen}")
-
-    if dataclass_name is not None and not isinstance(dataclass_name, str):
-        raise TypeError(
-            f"`dataclass_name` must be a string or None, got: {dataclass_name}"
-        )
-
     if any(not (is_dataclass(_b) and isinstance(_b, type)) for _b in builds_bases):
         raise TypeError("All `build_bases` must be a tuple of dataclass types")
 
     if zen_meta is None:
         zen_meta = {}
 
     if not isinstance(zen_meta, Mapping):
@@ -1301,23 +1497,26 @@
 
         validated_wrappers: Sequence[Union[str, Builds[Any]]] = []
         for wrapper in zen_wrappers:
             if wrapper is None:
                 continue
             # We are intentionally keeping each condition branched
             # so that test-coverage will be checked for each one
+            if isinstance(wrapper, functools.partial):
+                wrapper = ZEN_VALUE_CONVERSION[functools.partial](wrapper)
+
             if is_builds(wrapper):
                 # If Hydra's locate function starts supporting importing literals
                 # – or if we decide to ship our own locate function –
                 # then we should get the target of `wrapper` and make sure it is callable
                 if is_just(wrapper):
                     # `zen_wrappers` handles importing string; we can
-                    # elimintate the indirection of Just and "flatten" this
+                    # eliminate the indirection of Just and "flatten" this
                     # config
-                    validated_wrappers.append(getattr(wrapper, JUST_FIELD_NAME))
+                    validated_wrappers.append(safe_getattr(wrapper, JUST_FIELD_NAME))
                 else:
                     if hydra_recursive is False:
                         warnings.warn(
                             "A structured config was supplied for `zen_wrappers`. Its parent config has "
                             "`hydra_recursive=False`.\n If this value is not toggled to `True`, the config's "
                             "instantiation will result in an error"
                         )
@@ -1380,21 +1579,21 @@
 
     # reflects state of closest parent that has partial field specified
     parent_partial: Optional[bool] = None
 
     for base in builds_bases:
         _set_this_iteration = False
         if HYDRA_SUPPORTS_PARTIAL and base_hydra_partial is None:
-            base_hydra_partial = getattr(base, PARTIAL_FIELD_NAME, None)
+            base_hydra_partial = safe_getattr(base, PARTIAL_FIELD_NAME, None)
             if parent_partial is None:
                 parent_partial = base_hydra_partial
                 _set_this_iteration = True
 
         if base_zen_partial is None:
-            base_zen_partial = getattr(base, ZEN_PARTIAL_FIELD_NAME, None)
+            base_zen_partial = safe_getattr(base, ZEN_PARTIAL_FIELD_NAME, None)
             if parent_partial is None or (
                 _set_this_iteration and base_zen_partial is not None
             ):
                 parent_partial = parent_partial or base_zen_partial
 
         del _set_this_iteration
 
@@ -1414,16 +1613,15 @@
     )
 
     if base_zen_partial:
         assert requires_zen_processing
 
     del base_zen_partial
 
-    if not requires_zen_processing and requires_partial_field:  # pragma: no cover
-        # TODO: require test-coverage once Hydra publishes nightly builds
+    if not requires_zen_processing and requires_partial_field:
         target_field = [
             (
                 TARGET_FIELD_NAME,
                 str,
                 _utils.field(default=target_path, init=False),
             ),
             (
@@ -1695,15 +1893,15 @@
         p.name
         for p in chain(sig_by_kind[_POSITIONAL_OR_KEYWORD], sig_by_kind[_KEYWORD_ONLY])
     }
 
     if not _pos_args and builds_bases:
         # pos_args is potentially inherited
         for _base in builds_bases:
-            _pos_args = getattr(_base, POS_ARG_FIELD_NAME, ())
+            _pos_args = safe_getattr(_base, POS_ARG_FIELD_NAME, ())
 
             # validates
             _pos_args = tuple(
                 sanitized_default_value(
                     x, allow_zen_conversion=False, convert_dataclass=False
                 )
                 for x in _pos_args
@@ -1964,49 +2162,54 @@
                     convert_dataclass=zen_convert_settings["dataclass"],
                 )
             else:
                 _field = value
 
             # If `.default` is not set, then `value` is a Hydra-supported mutable
             # value, and thus it is "sanitized"
-            sanitized_value = getattr(_field, "default", value)
+            sanitized_value = safe_getattr(_field, "default", value)
             sanitized_type = (
                 _utils.sanitized_type(type_, wrap_optional=sanitized_value is None)
                 if _retain_type_info(
                     type_=type_, value=sanitized_value, hydra_recursive=hydra_recursive
                 )
                 else Any
             )
             sanitized_base_fields.append((name, sanitized_type, _field))
             del value
             del _field
             del sanitized_value
 
-    out = make_dataclass(
-        dataclass_name, fields=sanitized_base_fields, bases=builds_bases, frozen=frozen
-    )
+    dataclass_options["cls_name"] = dataclass_name
+    dataclass_options["bases"] = builds_bases
+    assert _utils.parse_strict_dataclass_options(dataclass_options)
+
+    out = make_dataclass(fields=sanitized_base_fields, **dataclass_options)
+
+    if module is not None:
+        out.__module__ = module
 
     out.__doc__ = (
-        f"A structured config designed to {'partially ' if zen_partial else ''}initialize/call "
-        f"`{target_path}` upon instantiation by hydra."
+        f"A structured config designed to {'partially ' if zen_partial else ''}"
+        f"initialize/call `{target_path}` upon instantiation by hydra."
     )
     if hasattr(target, "__doc__"):  # pragma: no branch
         target_doc = target.__doc__
         if target_doc:
             out.__doc__ += (
                 f"\n\nThe docstring for {_utils.safe_name(target)} :\n\n" + target_doc
             )
 
     assert requires_zen_processing is uses_zen_processing(out)
 
     # _partial_=True should never be relied on when zen-processing is being used.
     assert not (
         HYDRA_SUPPORTS_PARTIAL
         and requires_zen_processing
-        and getattr(out, PARTIAL_FIELD_NAME, False)
+        and safe_getattr(out, PARTIAL_FIELD_NAME, False)
     )
 
     return cast(Union[Type[Builds[Importable]], Type[BuildsWithSig[Type[R], P]]], out)
 
 
 @overload
 def get_target(obj: InstOrType[Builds[_T]]) -> _T:
@@ -2087,15 +2290,15 @@
         field_name = TARGET_FIELD_NAME
     else:
         raise TypeError(
             f"`obj` must specify a target; i.e. it must have an attribute named"
             f" {TARGET_FIELD_NAME} or named {ZEN_PARTIAL_FIELD_NAME} that"
             f" points to a target-object or target-string"
         )
-    target = getattr(obj, field_name)
+    target = safe_getattr(obj, field_name)
 
     if isinstance(target, str):
         target = get_obj(path=target)
     else:
         # Hydra 1.1.0 permits objects-as-_target_ instead of strings
         # https://github.com/facebookresearch/hydra/issues/1017
         pass  # makes sure we cover this branch in tests
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_just.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_just.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 from typing import Any, Callable, FrozenSet, Optional, Type, TypeVar, Union, overload
 
 from typing_extensions import Literal
 
 from hydra_zen.structured_configs import _utils
-from hydra_zen.typing import Builds, Just
+from hydra_zen.typing import Builds, DataclassOptions, Just
 from hydra_zen.typing._implementations import _HydraPrimitive  # type: ignore
 from hydra_zen.typing._implementations import _SupportedViaBuilds  # type: ignore
 from hydra_zen.typing._implementations import AllConvert, DataClass_, ZenConvert
 
 from ._implementations import sanitized_default_value
 from ._utils import merge_settings
 from ._value_conversion import ConfigComplex
@@ -29,102 +29,111 @@
 
 @overload
 def just(
     obj: TP,
     *,
     zen_convert: Optional[ZenConvert] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> TP:
     ...
 
 
 @overload
 def just(
     obj: complex,
     *,
     zen_convert: Optional[ZenConvert] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> ConfigComplex:
     ...
 
 
 @overload
 def just(
     obj: TC,
     *,
     zen_convert: Optional[ZenConvert] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
-) -> Type[Just[TC]]:
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
+) -> Just[TC]:
     ...
 
 
 @overload
 def just(
     obj: TB,
     *,
     zen_convert: Optional[ZenConvert] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> Builds[Type[TB]]:
     ...
 
 
 @overload
 def just(
     obj: TD,
     *,
     zen_convert: Literal[None] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> Type[Builds[Type[TD]]]:
     ...
 
 
 @overload
 def just(
     obj: DataClass_,
     *,
     zen_convert: ZenConvert,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> Any:
     ...
 
 
 @overload
 def just(
     obj: Any,
     *,
     zen_convert: Optional[ZenConvert] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
 ) -> Any:
     ...
 
 
 def just(
     obj: Any,
     *,
     zen_convert: Optional[ZenConvert] = None,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
+    zen_dataclass: Optional[DataclassOptions] = None,
 ) -> Any:
     """`just(obj)` returns a config that, when instantiated, just returns `obj`.
 
     I.e., `instantiate(just(obj)) == obj`
 
-    `just` is designed to be idempotent: `just(obj) == just(just(obj))`
+    `just` is designed to be idempotent. I.e., `just(obj) == just(just(obj))`
 
     Parameters
     ----------
     obj : Callable[..., Any] | HydraSupportedPrimitive | ZenSupportedPrimitive
-        A value, type (e.g. a class-object), or function-object that is either supported by Hydra or has auto-config support via hydra-zen.
+        A type (e.g. a class-object), function-object, or a value that is either
+        supported by Hydra or has auto-config support via hydra-zen.
 
     zen_convert : Optional[ZenConvert]
         A dictionary that modifies hydra-zen's value and type conversion behavior.
         Consists of the following optional key-value pairs (:ref:`zen-convert`):
 
         - `dataclass` : `bool` (default=True):
             If `True` any dataclass type/instance without a
@@ -135,26 +144,38 @@
 
     hydra_recursive : Optional[bool], optional (default=True)
         If ``True``, then Hydra will recursively instantiate all other
         hydra-config objects nested within this config [2]_.
 
         If ``None``, the ``_recursive_`` attribute is not set on the resulting config.
 
-    hydra_convert : Optional[Literal["none", "partial", "all"]], optional (default="none")
+    hydra_convert : Optional[Literal["none", "partial", "all", "object"]], optional (default="none")
         Determines how Hydra treats the non-primitive, omegaconf-specific objects
         during instantiateion [3]_.
 
         - ``"none"``: No conversion occurs; omegaconf containers are passed through (Default)
         - ``"partial"``: ``DictConfig`` and ``ListConfig`` objects converted to ``dict`` and
           ``list``, respectively. Structured configs and their fields are passed without conversion.
         - ``"all"``: All passed objects are converted to dicts, lists, and primitives, without
           a trace of OmegaConf containers.
+        - ``"object"``: Passed objects are converted to dict and list. Structured Configs are converted to instances of the backing dataclass / attr class.
 
         If ``None``, the ``_convert_`` attribute is not set on the resulting config.
 
+    zen_dataclass : Optional[DataclassOptions]
+        A dictionary that can specify any option that is supported by
+        :py:func:`dataclasses.make_dataclass` other than `fields`.
+        The default value for `unsafe_hash` is `True`.
+
+        These options are only relevant when the input to `just` is a dataclass
+        instance. Otherwise, `just` does not utilize these options when auto-generating
+        configs.
+
+        Additionally, the `module` field can be specified to enable pickle
+        compatibility. See `hydra_zen.typing.DataclassOptions` for details.
 
     Returns
     -------
     out : HydraSupportedPrimitive | Builds[Type[obj]]
         ``out`` is ``obj`` unchanged if ``obj`` is supported natively by Hydra, otherwise ``out`` is a dynamically-generated dataclass type or instance.
 
     Raises
@@ -283,18 +304,21 @@
     (3+5j)
     """
     convert_settings = merge_settings(zen_convert, _JUST_CONVERT_SETTINGS)
     del zen_convert
     _utils.validate_hydra_options(
         hydra_recursive=hydra_recursive, hydra_convert=hydra_convert
     )
+    if zen_dataclass is None:
+        zen_dataclass = {}
 
     return sanitized_default_value(
         obj,
         allow_zen_conversion=True,
         structured_conf_permitted=True,
         field_name="",
         error_prefix="",
         convert_dataclass=convert_settings["dataclass"],
         hydra_convert=hydra_convert,
         hydra_recursive=hydra_recursive,
+        zen_dataclass=_utils.parse_dataclass_options(zen_dataclass),
     )
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_make_config.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_make_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
+import warnings
 from collections import Counter
 from dataclasses import (  # use this for runtime checks
     MISSING,
     Field as _Field,
     InitVar,
     dataclass,
     make_dataclass,
 )
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
 from typing_extensions import Literal
 
 from hydra_zen._compatibility import PATCH_OMEGACONF_830
+from hydra_zen.errors import HydraZenDeprecationWarning
 from hydra_zen.structured_configs import _utils
 from hydra_zen.structured_configs._implementations import (
     _BUILDS_CONVERT_SETTINGS,
     sanitize_collection,
 )
-from hydra_zen.typing import SupportedPrimitive
+from hydra_zen.typing import DataclassOptions, SupportedPrimitive
 from hydra_zen.typing._implementations import (
     AllConvert,
     DataClass,
     DataClass_,
     DefaultsList,
     Field,
     ZenConvert,
@@ -34,25 +36,25 @@
     DEFAULTS_LIST_FIELD_NAME,
     PARTIAL_FIELD_NAME,
     RECURSIVE_FIELD_NAME,
     ZEN_PARTIAL_FIELD_NAME,
     ZEN_TARGET_FIELD_NAME,
 )
 from ._implementations import _retain_type_info, builds, sanitized_field
-from ._type_guards import uses_zen_processing
+from ._type_guards import safe_getattr, uses_zen_processing
 
 __all__ = ["ZenField", "make_config"]
 
 
 class NOTHING:
     def __init__(self) -> None:
         raise TypeError("`NOTHING` cannot be instantiated")
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class ZenField:
     """
     ZenField(hint=Any, default=<class 'NOTHING'>, name=<class 'NOTHING'>)
 
     Specifies a field's name and/or type-annotation and/or default value.
     Designed to specify fields in `make_config`.
 
@@ -136,18 +138,17 @@
 
 _MAKE_CONFIG_SETTINGS = AllConvert(dataclass=False)
 
 
 def make_config(
     *fields_as_args: Union[str, ZenField],
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
     hydra_defaults: Optional[DefaultsList] = None,
-    config_name: str = "Config",
-    frozen: bool = False,
+    zen_dataclass: Optional[DataclassOptions] = None,
     bases: Tuple[Type[DataClass_], ...] = (),
     zen_convert: Optional[ZenConvert] = None,
     **fields_as_kwargs: Union[SupportedPrimitive, ZenField],
 ) -> Type[DataClass]:
     """
     Returns a config with user-defined field names and, optionally,
     associated default values and/or type annotations.
@@ -184,35 +185,50 @@
 
     hydra_recursive : Optional[bool], optional (default=True)
         If ``True``, then Hydra will recursively instantiate all other
         hydra-config objects nested within this dataclass [2]_.
 
         If ``None``, the ``_recursive_`` attribute is not set on the resulting config.
 
-    hydra_convert : Optional[Literal["none", "partial", "all"]], optional (default="none")
+    hydra_convert : Optional[Literal["none", "partial", "all", "object"]], optional (default="none")
         Determines how Hydra handles the non-primitive objects passed to configuration [3]_.
 
         - ``"none"``: Passed objects are DictConfig and ListConfig, default
         - ``"partial"``: Passed objects are converted to dict and list, with the exception of Structured Configs (and their fields).
         - ``"all"``: Passed objects are dicts, lists and primitives without a trace of OmegaConf containers
+        - ``"object"``: Passed objects are converted to dict and list. Structured Configs are converted to instances of the backing dataclass / attr class.
 
         If ``None``, the ``_convert_`` attribute is not set on the resulting config.
 
-
     hydra_defaults : None | list[str | dict[str, str | list[str] | None ]], optional (default = None)
         A list in an input config that instructs Hydra how to build the output config
         [7]_ [8]_. Each input config can have a Defaults List as a top level element. The
         Defaults List itself is not a part of output config.
 
+    zen_dataclass : Optional[DataclassOptions]
+        A dictionary can specify any option that is supported by
+        :py:func:`dataclasses.make_dataclass` other than `fields`.
+
+        Additionally, a ``'module': <str>`` entry can be specified to enable pickle
+        compatibility. See `hydra_zen.typing.DataclassOptions` for details.
+
     frozen : bool, optional (default=False)
-        If ``True``, the resulting config class will produce 'frozen' (i.e. immutable) instances.
-        I.e. setting/deleting an attribute of an instance of the config will raise
-        :py:class:`dataclasses.FrozenInstanceError` at runtime.
+        .. deprecated:: 0.9.0
+            `frozen` will be removed in hydra-zen 0.10.0. It is replaced by
+            ``zen_dataclass={'frozen': <bool>}``.
+
+        If ``True``, the resulting config class will produce 'frozen' (i.e. immutable)
+        instances. I.e. setting/deleting an attribute of an instance of the config will
+        raise :py:class:`dataclasses.FrozenInstanceError` at runtime.
 
     config_name : str, optional (default="Config")
+        .. deprecated:: 0.9.0
+            `config_name` will be removed in hydra-zen 0.10.0. It is replaced by
+            ``zen_dataclass={'cls_name': <str>}``.
+
         The class name of the resulting config class.
 
     Returns
     -------
     Config : Type[DataClass]
         The resulting config class; a dataclass that possess the user-specified fields.
 
@@ -222,15 +238,16 @@
         The provided configured value cannot be serialized by Hydra, nor does hydra-zen
         provide specialized support for it. See :ref:`valid-types` for more details.
 
     Notes
     -----
     The resulting "config" is a dataclass-object [4]_ with Hydra-specific attributes
     attached to it, along with the attributes specified via ``fields_as_args`` and
-    ``fields_as_kwargs``.
+    ``fields_as_kwargs``. **Unlike std-lib dataclasses, the default value for
+    unsafe_hash is True.**
 
     Any field specified without a type-annotation is automatically annotated with
     :py:class:`typing.Any`. Hydra only supports a narrow subset of types [5]_;
     `make_config` will automatically 'broaden' any user-specified annotations so that
     they are compatible with Hydra.
 
     `make_config` will automatically manipulate certain types of default values to
@@ -368,14 +385,46 @@
 
     See :ref:`data-val` for more general data validation capabilities via hydra-zen.
     """
     convert_settings = _utils.merge_settings(zen_convert, _MAKE_CONFIG_SETTINGS)
     convert_settings = cast(ZenConvert, convert_settings)
     del zen_convert
 
+    if zen_dataclass is None:
+        zen_dataclass = {}
+
+    # initial validation
+    _utils.parse_dataclass_options(zen_dataclass)
+
+    if "frozen" in fields_as_kwargs:
+        warnings.warn(
+            HydraZenDeprecationWarning(
+                "Specifying `builds(frozen=<...>)` is deprecated. Instead, "
+                "specify `builds(zen_dataclass={'frozen': <...>})"
+            ),
+            stacklevel=2,
+        )
+        zen_dataclass["frozen"] = fields_as_kwargs.pop("frozen")  # type: ignore
+
+    if "config_name" in fields_as_kwargs:
+        warnings.warn(
+            HydraZenDeprecationWarning(
+                "Specifying `make_config(config_name=<...>)` is deprecated. "
+                "Instead specify `make_config(zen_dataclass={'cls_name': <...>})"
+            ),
+            stacklevel=2,
+        )
+        zen_dataclass["cls_name"] = fields_as_kwargs.pop("config_name")  # type: ignore
+
+    if not bases:
+        bases = zen_dataclass.get("bases", ())
+
+    zen_dataclass.setdefault("cls_name", "Config")
+    dataclass_options = _utils.parse_dataclass_options(zen_dataclass)
+
     for _field in fields_as_args:
         if not isinstance(_field, (str, ZenField)):
             raise TypeError(
                 f"`fields_as_args` can only consist of field-names (i.e. strings) or "
                 f"`ZenField` instances. Got: "
                 f"{', '.join(str(x) for x in fields_as_args if not isinstance(x, (str, ZenField)))}"
             )
@@ -512,26 +561,32 @@
             (
                 DEFAULTS_LIST_FIELD_NAME,
                 List[Any],
                 _utils.field(default_factory=lambda: list(hydra_defaults), init=False),
             )
         )
 
-    out = make_dataclass(
-        cls_name=config_name, fields=config_fields, frozen=frozen, bases=bases
-    )
+    dataclass_options["bases"] = bases
+    module = dataclass_options.pop("module", None)
+    assert _utils.parse_strict_dataclass_options(dataclass_options), dataclass_options
+
+    out = make_dataclass(fields=config_fields, **dataclass_options)
+
+    if module is not None:
+        out.__module__ = module
+
     if hasattr(out, ZEN_TARGET_FIELD_NAME) and not uses_zen_processing(out):
         raise ValueError(
             f"{out.__name__} inherits from base classes that overwrite some fields "
             f"associated with zen-processing features. As a result, this config will "
             f"not instantiate correctly."
         )
     if (
         HYDRA_SUPPORTS_PARTIAL
-        and getattr(out, PARTIAL_FIELD_NAME, False)
+        and safe_getattr(out, PARTIAL_FIELD_NAME, False)
         and uses_zen_processing(out)
     ):
         raise ValueError(
             f"{out.__name__} specifies both `{PARTIAL_FIELD_NAME}=True` and `"
             f"{ZEN_PARTIAL_FIELD_NAME}=True`. This config will not instantiate "
             f"correctly. This is typically caused by inheriting from multiple, "
             f"conflicting configs."
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_make_custom_builds.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_make_custom_builds.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 # pyright: strict
 import inspect
+import warnings
 from functools import wraps
 from typing import Any, Callable, Dict, Mapping, Optional, Union, cast, overload
 
 from typing_extensions import Final, Literal
 
-from hydra_zen.typing import ZenWrappers
+from hydra_zen.errors import HydraZenDeprecationWarning
+from hydra_zen.typing import DataclassOptions, ZenWrappers
 from hydra_zen.typing._builds_overloads import FullBuilds, PBuilds, StdBuilds
 from hydra_zen.typing._implementations import ZenConvert
 
 from ._implementations import builds
+from ._utils import parse_dataclass_options
 
 __all__ = ["make_custom_builds_fn"]
 
 
 _builds_sig = inspect.signature(builds)
 __BUILDS_DEFAULTS: Final[Dict[str, Any]] = {
     name: p.default
     for name, p in _builds_sig.parameters.items()
     if p.kind is p.KEYWORD_ONLY
 }
+# TODO: Remove deprecated options once they are phased out
+__BUILDS_DEFAULTS["frozen"] = False
+__BUILDS_DEFAULTS["dataclass_name"] = None
 del _builds_sig
 
 
 # partial=False, pop-sig=True
 @overload
 def make_custom_builds_fn(
     *,
     zen_partial: Literal[False, None] = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     populate_full_signature: Literal[True],
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> FullBuilds:
     ...
 
 
 # partial=True, pop-sig=bool
@@ -46,15 +53,16 @@
 def make_custom_builds_fn(
     *,
     zen_partial: Literal[True],
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     populate_full_signature: bool = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> PBuilds:
     ...
 
 
 # partial=False, pop-sig=False
@@ -62,15 +70,16 @@
 def make_custom_builds_fn(
     *,
     zen_partial: Literal[False, None] = ...,
     populate_full_signature: Literal[False] = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> StdBuilds:
     ...
 
 
 # partial=False, pop-sig=bool
@@ -78,15 +87,16 @@
 def make_custom_builds_fn(
     *,
     zen_partial: Literal[False, None] = ...,
     populate_full_signature: bool,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> Union[FullBuilds, StdBuilds]:
     ...
 
 
 # partial=bool, pop-sig=False
@@ -94,15 +104,16 @@
 def make_custom_builds_fn(
     *,
     zen_partial: Union[bool, None],
     populate_full_signature: Literal[False] = ...,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> Union[PBuilds, StdBuilds]:
     ...
 
 
 # partial=bool, pop-sig=bool
@@ -110,29 +121,31 @@
 def make_custom_builds_fn(
     *,
     zen_partial: Union[bool, None],
     populate_full_signature: bool,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
     zen_meta: Optional[Mapping[str, Any]] = ...,
     hydra_recursive: Optional[bool] = ...,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = ...,
+    zen_dataclass: Optional[DataclassOptions] = ...,
     frozen: bool = ...,
     zen_convert: Optional[ZenConvert] = ...,
 ) -> Union[FullBuilds, PBuilds, StdBuilds]:
     ...
 
 
 def make_custom_builds_fn(
     *,
     zen_partial: Optional[bool] = None,
     populate_full_signature: bool = False,
     zen_wrappers: ZenWrappers[Callable[..., Any]] = tuple(),
     zen_meta: Optional[Mapping[str, Any]] = None,
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
+    zen_dataclass: Optional[DataclassOptions] = None,
     frozen: bool = False,
     zen_convert: Optional[ZenConvert] = None,
 ) -> Union[FullBuilds, PBuilds, StdBuilds]:
     """Returns the `builds` function, but with customized default values.
 
     E.g. ``make_custom_builds_fn(hydra_convert='all')`` will return a version
     of the `builds` function where the default value for ``hydra_convert``
@@ -158,21 +171,33 @@
 
         - `dataclass` : `bool` (default=True):
             If `True` any dataclass type/instance without a
             `_target_` field is automatically converted to a targeted config
             that will instantiate to that type/instance. Otherwise the dataclass
             type/instance will be passed through as-is.
 
+    zen_dataclass : Optional[DataclassOptions]
+        A dictionary can specify any option that is supported by
+        :py:func:`dataclasses.make_dataclass` other than `fields`.
+        The default value for `unsafe_hash` is `True`.
+
+        Additionally, the `module` field can be specified to enable pickle
+        compatibility. See `hydra_zen.typing.DataclassOptions` for details.
+
     hydra_recursive : Optional[bool], optional (default=True)
         Specifies a new the default value for ``builds(..., hydra_recursive=<..>)``
 
-    hydra_convert : Optional[Literal["none", "partial", "all"]], optional (default="none")
+    hydra_convert : Optional[Literal["none", "partial", "all", "object"]], optional (default="none")
         Specifies a new the default value for ``builds(..., hydra_convert=<..>)``
 
     frozen : bool, optional (default=False)
+        .. deprecated:: 0.9.0
+            `frozen` will be removed in hydra-zen 0.10.0. It is replaced by
+            `zen_dataclass={'frozen': <bool>}`.
+
         Specifies a new the default value for ``builds(..., frozen=<..>)``
 
     Returns
     -------
     custom_builds
         The function `builds`, but with customized default values.
 
@@ -226,31 +251,56 @@
 
     >>> instantiate(Conf, x="a")  # satisfies annotation: Literal["a", "b"]
     "a"
 
     >>> instantiate(Conf, x="c")  # violates annotation: Literal["a", "b"]
     <Validation error: "c" is not "a" or "b">
     """
-
     excluded_fields = frozenset({"dataclass_name", "hydra_defaults", "builds_bases"})
     LOCALS = locals()
 
     # Ensures that new defaults added to `builds` must be reflected
     # in the signature of `make_custom_builds_fn`.
     assert (set(__BUILDS_DEFAULTS) - excluded_fields) <= set(LOCALS)
 
     _new_defaults = {
         name: LOCALS[name] for name in __BUILDS_DEFAULTS if name not in excluded_fields
     }
 
+    _frozen = _new_defaults.pop("frozen")
+
     # let `builds` validate the new defaults!
     builds(builds, **_new_defaults)
 
+    _zen_dataclass: Optional[DataclassOptions] = _new_defaults.pop("zen_dataclass")
+    if _zen_dataclass is None:
+        _zen_dataclass = {}
+
+    if _frozen is True:
+        warnings.warn(
+            HydraZenDeprecationWarning(
+                "Specifying `builds(..., frozen=<...>)` is deprecated. Instead, "
+                "specify `builds(..., zen_dataclass={'frozen': <...>})"
+            ),
+            stacklevel=2,
+        )
+
+        _zen_dataclass["frozen"] = _frozen
+
+    _zen_dataclass = parse_dataclass_options(_zen_dataclass)
+
     @wraps(builds)
     def wrapped(*args: Any, **kwargs: Any):
         merged_kwargs: Dict[str, Any] = {}
+        _dataclass: Optional[DataclassOptions] = kwargs.pop("zen_dataclass", None)
+
+        if _dataclass is None:
+            _new_defaults["zen_dataclass"] = _zen_dataclass
+        else:
+            _new_defaults["zen_dataclass"] = {**_zen_dataclass, **_dataclass}
+
         merged_kwargs.update(_new_defaults)
         merged_kwargs.update(kwargs)
+
         return builds(*args, **merged_kwargs)
 
-    setattr(wrapped, "_zen_convert", zen_convert)
     return cast(Union[FullBuilds, PBuilds, StdBuilds], wrapped)
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_type_guards.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_type_guards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 # pyright: strict
+from dataclasses import MISSING
 from functools import partial
 from typing import TYPE_CHECKING, Any, Type, Union
 
 from typing_extensions import TypeGuard
 
 from hydra_zen._compatibility import HYDRA_SUPPORTS_PARTIAL
 from hydra_zen.funcs import get_obj, zen_processing
+from hydra_zen.structured_configs._utils import safe_name
 from hydra_zen.typing import Builds, Just, PartialBuilds
-from hydra_zen.typing._implementations import DataClass_
+from hydra_zen.typing._implementations import DataClass_, HasTarget
 
 from ._globals import (
     JUST_FIELD_NAME,
     PARTIAL_FIELD_NAME,
     TARGET_FIELD_NAME,
     ZEN_PARTIAL_FIELD_NAME,
     ZEN_PROCESSING_LOCATION,
@@ -31,29 +33,59 @@
 # The following functions perform these desired checks. Note that they do not
 # require that the provided object be a dataclass; this enables compatibility
 # with omegaconf containers.
 #
 # These are not part of the public API for now, but they may be in the future.
 
 
-def _get_target(x: Any):
-    return getattr(x, TARGET_FIELD_NAME)
+def safe_getattr(obj: Any, field: str, *default: Any) -> Any:
+    # We must access slotted class-attributes from a dataclass type
+    # via its `__dataclass_fields__`. Otherwise we will get a member
+    # descriptor
+
+    assert len(default) < 2
+    if (
+        hasattr(obj, "__slots__")
+        and isinstance(obj, type)
+        and is_dataclass(obj)
+        and field in obj.__slots__  # type: ignore
+    ):
+        try:
+            _field = obj.__dataclass_fields__[field]
+            if _field.default_factory is not MISSING or _field.default is MISSING:
+                raise AttributeError
+
+            return _field.default
+
+        except (KeyError, AttributeError):
+            if default:
+                return default[0]
+
+            raise AttributeError(
+                f"type object '{safe_name(obj)}' has no attribute '{field}'"
+            )
+
+    return getattr(obj, field, *default)
+
+
+def _get_target(x: HasTarget) -> Any:
+    return safe_getattr(x, TARGET_FIELD_NAME)
 
 
 def is_builds(x: Any) -> TypeGuard[Builds[Any]]:
     return hasattr(x, TARGET_FIELD_NAME)
 
 
 def is_just(x: Any) -> TypeGuard[Just[Any]]:
     if is_builds(x) and hasattr(x, JUST_FIELD_NAME):
         attr = _get_target(x)
         if attr == _get_target(Just) or attr is get_obj:
             return True
         else:
-            # ensures we conver this branch in tests
+            # ensures we convert this branch in tests
             return False
     return False
 
 
 if TYPE_CHECKING:  # pragma: no cover
 
     def is_dataclass(obj: Any) -> TypeGuard[Union[DataClass_, Type[DataClass_]]]:
@@ -65,15 +97,15 @@
 
 def is_old_partial_builds(x: Any) -> bool:  # pragma: no cover
     # We don't care about coverage here.
     # This will only be used in `get_target` and we'll be sure to cover that branch
     if is_builds(x) and hasattr(x, "_partial_target_"):
         attr = _get_target(x)
         if (attr == "hydra_zen.funcs.partial" or attr is partial) and is_just(
-            getattr(x, "_partial_target_")
+            safe_getattr(x, "_partial_target_")
         ):
             return True
         else:
             # ensures we cover this branch in tests
             return False
     return False
 
@@ -126,14 +158,15 @@
     _zen_exclude:
     - hidden_field
     a: 1
     hidden_field: null
     """
     if not is_builds(x) or not hasattr(x, ZEN_TARGET_FIELD_NAME):
         return False
+
     attr = _get_target(x)
     if attr != ZEN_PROCESSING_LOCATION and attr is not zen_processing:
         return False
     return True
 
 
 def is_partial_builds(x: Any) -> TypeGuard[PartialBuilds[Any]]:
@@ -186,14 +219,14 @@
     >>> instantiate(Conf)
     functools.partial(<class 'int'>, 0)
     """
     if is_builds(x):
         return (
             # check if partial'd config via Hydra
             HYDRA_SUPPORTS_PARTIAL
-            and getattr(x, PARTIAL_FIELD_NAME, False) is True
+            and safe_getattr(x, PARTIAL_FIELD_NAME, False) is True
         ) or (
             # check if partial'd config via `zen_processing`
             uses_zen_processing(x)
-            and (getattr(x, ZEN_PARTIAL_FIELD_NAME, False) is True)
+            and (safe_getattr(x, ZEN_PARTIAL_FIELD_NAME, False) is True)
         )
     return False
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_utils.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import inspect
 import sys
 import warnings
 from dataclasses import MISSING, field as _field, is_dataclass
 from enum import Enum
+from keyword import iskeyword
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
+    FrozenSet,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
@@ -35,26 +37,30 @@
     Unpack,
     _AnnotatedAlias,
 )
 
 from hydra_zen._compatibility import (
     HYDRA_SUPPORTED_PRIMITIVE_TYPES,
     HYDRA_SUPPORTS_NESTED_CONTAINER_TYPES,
+    HYDRA_SUPPORTS_OBJECT_CONVERT,
     HYDRA_SUPPORTS_PARTIAL,
     OMEGACONF_VERSION,
     PATCH_OMEGACONF_830,
     Version,
 )
 from hydra_zen.errors import HydraZenValidationError
+from hydra_zen.typing import DataclassOptions, ZenConvert
 from hydra_zen.typing._implementations import (
+    DEFAULT_DATACLASS_OPTIONS,
+    UNSUPPORTED_DATACLASS_OPTIONS,
     AllConvert,
     DataClass_,
     Field,
     InterpStr,
-    ZenConvert,
+    StrictDataclassOptions,
     convert_types,
 )
 
 try:
     from typing import get_args, get_origin
 except ImportError:  # pragma: no cover
     # remove at Python 3.7 end-of-life
@@ -277,15 +283,15 @@
         else:
             raise ModuleNotFoundError(f"{name} is not importable")
 
     if not is_classmethod(obj):
         return f"{module}.{name}"
     else:
 
-        # __qualname__ reflects name of class that originaly defines classmethod.
+        # __qualname__ reflects name of class that originally defines classmethod.
         # Does not point to child in case of inheritance.
         #
         # obj.__self__ -> parent object
         # obj.__name__ -> name of classmethod
         return f"{get_obj_path(obj.__self__)}.{obj.__name__}"
 
 
@@ -362,15 +368,15 @@
                 primitive_only=primitive_only,
                 wrap_optional=wrap_optional,
                 nested=nested,
             )
 
         # Python 3.7-3.8
         # type_: Annotated[x, y]; origin -> x
-        if isinstance(type_, _AnnotatedAlias):
+        if isinstance(type_, _AnnotatedAlias):  # pragma: no cover
             return sanitized_type(
                 origin,
                 primitive_only=primitive_only,
                 wrap_optional=wrap_optional,
                 nested=nested,
             )
 
@@ -407,15 +413,15 @@
                 ValueType = sanitized_type(
                     args[1], primitive_only=no_nested_container, nested=True
                 )
                 return Dict[KeyType, ValueType]  # type: ignore
             return Dict
 
         if (origin is tuple or origin is Tuple) and not nested:
-            # hydra silently supports tuples of homogenous types
+            # hydra silently supports tuples of homogeneous types
             # It has some weird behavior. It treats `Tuple[t1, t2, ...]` as `List[t1]`
             # It isn't clear that we want to perpetrate this on our end..
             # So we deal with inhomogeneous types as e.g. `Tuple[str, int]` -> `Tuple[Any, Any]`.
             #
             # Otherwise we preserve the annotation as accurately as possible
             if not args:
                 return Any if OMEGACONF_VERSION < (2, 2, 3) else Tuple
@@ -442,15 +448,16 @@
                 return Tuple[(_unique_type,) * len(args)]  # type: ignore
 
         return Any
 
     if HYDRA_SUPPORTS_PARTIAL and isinstance(type_, type) and issubclass(type_, Path):
         type_ = Path
 
-    if isinstance(type_, (ParamSpecArgs, ParamSpecKwargs)):
+    if isinstance(type_, (ParamSpecArgs, ParamSpecKwargs)):  # pragma: no cover
+        # Python 3.7 - 3.9
         # these aren't hashable -- can't check for membership in set
         return Any
 
     if (
         type_ is Any
         or type_ in _supported_types
         or is_dataclass(type_)
@@ -587,20 +594,134 @@
                 raise TypeError(
                     f"Setting {k}={v} specified a value of the wrong type. Expected type: {convert_types[k].__name__}"
                 )
             settings[k] = v
     return settings
 
 
+_DATACLASS_OPTION_KEYS: FrozenSet[str] = (
+    DataclassOptions.__required_keys__ | DataclassOptions.__optional_keys__
+)
+
+_STRICT_DATACLASS_OPTION_KEYS: FrozenSet[str] = (
+    StrictDataclassOptions.__required_keys__ | StrictDataclassOptions.__optional_keys__
+)
+_STRICT_DATACLASS_OPTION_KEYS.copy()
+
+
+def parse_dataclass_options(options: Mapping[str, Any]) -> DataclassOptions:
+    """
+    Ensures `options` adheres to `DataclassOptions` and merges hydra-zen defaults
+    for missing options.
+
+    All valid `@dataclass`/`make_dataclass` options are supported, even for features
+    introduced in later versions of Python. This function will remove valid options
+    that are not supported for by the current Python version.
+
+    Parameters
+    ----------
+    options : Mapping[str, Any]
+        User-specified options for `zen_dataclass` to be validated.
+
+    Returns
+    -------
+    DataclassOptions
+
+    Examples
+    --------
+    >>> parse_dataclass_options({})
+    {'unsafe_hash': True}
+
+    >>> parse_dataclass_options({"unsafe_hash": False, "cls_name": "Foo"})
+    {'unsafe_hash': False, 'cls_name': 'Foo'}
+
+    >>> parse_dataclass_options({"moo": 1})
+    ValueError: moo is not a valid dataclass option.
+
+    Options that are supported by `make_dataclass` for later versions of
+    Python are ignored/removed automatically by this function. E.g. the following
+    Python 3.10+ option has the following behavior in Python 3.9:
+
+    >>> parse_dataclass_options({"slots": False})
+    {'unsafe_hash': True}
+    """
+    if not isinstance(options, Mapping):
+        raise ValueError(
+            f"`zen_dataclass_options` is expected to be `None` or dict[str, bool]. Got "
+            f"{options} (type: {type(options)})."
+        )
+
+    merged = DEFAULT_DATACLASS_OPTIONS.copy()
+
+    for name, val in options.items():
+        if name in UNSUPPORTED_DATACLASS_OPTIONS:
+            continue
+        elif name not in _DATACLASS_OPTION_KEYS:
+            raise ValueError(f"{name} is not a valid dataclass option.")
+
+        if name == "module":
+            if not isinstance(val, str) or not all(
+                v.isidentifier() and not iskeyword(v) for v in val.split(".")
+            ):
+                raise ValueError(
+                    f"dataclass option `{name}` must be a valid module name, got {val}"
+                )
+        elif name == "cls_name":
+            if val is not None and (not isinstance(val, str) or not val.isidentifier()):
+                raise ValueError(
+                    f"dataclass option `{name}` must be a valid identifier, got {val}"
+                )
+        elif name == "bases":
+            if not isinstance(val, Iterable) or any(
+                not (is_dataclass(_b) and isinstance(_b, type)) for _b in val
+            ):
+                raise TypeError(
+                    f"dataclass option `{name}` must be a tuple of dataclass types"
+                )
+        elif name == "namespace":
+            if not isinstance(val, Mapping) or any(
+                not isinstance(v, str) or not v.isidentifier() for v in val
+            ):
+                raise ValueError(
+                    f"dataclass option `{name}` must be a mapping with string-valued keys "
+                    f"that are valid identifiers. Got {val}."
+                )
+        elif not isinstance(val, bool):
+            raise TypeError(
+                f"dataclass option `{name}` must be of type `bool`. Got {val} "
+                f"(type: {type(val)})"
+            )
+        merged[name] = val
+    return merged
+
+
+def parse_strict_dataclass_options(
+    options: Mapping[str, Any]
+) -> TypeGuard[StrictDataclassOptions]:
+    return (
+        options.keys() <= _STRICT_DATACLASS_OPTION_KEYS
+        and StrictDataclassOptions.__required_keys__ <= options.keys()
+    )
+
+
+_HYDRA_CONVERT_OPTIONS = (
+    {"none", "partial", "all", "object"}
+    if HYDRA_SUPPORTS_OBJECT_CONVERT
+    else {"none", "partial", "all"}
+)
+
+
 def validate_hydra_options(
     hydra_recursive: Optional[bool] = None,
-    hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
+    hydra_convert: Optional[Literal["none", "partial", "all", "object"]] = None,
 ) -> None:
     if hydra_recursive is not None and not isinstance(hydra_recursive, bool):
         raise TypeError(
             f"`hydra_recursive` must be a boolean type, got {hydra_recursive}"
         )
 
-    if hydra_convert is not None and hydra_convert not in {"none", "partial", "all"}:
+    if hydra_convert is not None and hydra_convert not in _HYDRA_CONVERT_OPTIONS:
         raise ValueError(
-            f"`hydra_convert` must be 'none', 'partial', or 'all', got: {hydra_convert}"
+            f"`hydra_convert` must be 'none', 'partial',"
+            f"{' object' if HYDRA_SUPPORTS_OBJECT_CONVERT else ''} or 'all', got: "
+            f"{hydra_convert}"
         )
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/structured_configs/_value_conversion.py` & `hydra_zen-0.9.1/src/hydra_zen/structured_configs/_value_conversion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import functools
 from collections import Counter, deque
-from dataclasses import dataclass, field
+from dataclasses import InitVar, dataclass, field
+from functools import partial
 from pathlib import Path, PosixPath, WindowsPath
-from typing import Any, Callable, Tuple, Type, TypeVar, cast
+from typing import Any, Tuple, Type, TypeVar, cast
 
 from hydra_zen._compatibility import ZEN_SUPPORTED_PRIMITIVES
 from hydra_zen.typing import Builds, Partial, PartialBuilds
 
-from ._implementations import ZEN_VALUE_CONVERSION, builds
+from ._implementations import ZEN_VALUE_CONVERSION, builds, sanitized_default_value
 from ._utils import get_obj_path
 
 _T = TypeVar("_T")
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class ConfigComplex:
     real: Any
     imag: Any
     _target_: str = field(default=get_obj_path(complex), init=False)
 
 
 def convert_complex(value: complex) -> Builds[Type[complex]]:
     return cast(Builds[Type[complex]], ConfigComplex(real=value.real, imag=value.imag))
 
 
 ZEN_VALUE_CONVERSION[complex] = convert_complex
 
 
-@dataclass
+@dataclass(unsafe_hash=True)
 class ConfigPath:
     _args_: Tuple[str]
     _target_: str = field(default=get_obj_path(Path), init=False)
 
 
 if Path in ZEN_SUPPORTED_PRIMITIVES:  # pragma: no cover
 
@@ -41,33 +42,73 @@
         return cast(Builds[Type[Path]], ConfigPath(_args_=(str(value),)))
 
     ZEN_VALUE_CONVERSION[Path] = convert_path
     ZEN_VALUE_CONVERSION[PosixPath] = convert_path
     ZEN_VALUE_CONVERSION[WindowsPath] = convert_path
 
 
-# registering value-conversions that depend on `builds`
-def _cast_via_tuple(dest_type: Type[_T]) -> Callable[[_T], Builds[Type[_T]]]:
-    def converter(value):
-        return builds(dest_type, tuple(value))()
-
-    return converter
-
-
 def _unpack_partial(value: Partial[_T]) -> PartialBuilds[Type[_T]]:
     target = cast(Type[_T], value.func)
     return builds(target, *value.args, **value.keywords, zen_partial=True)()
 
 
-ZEN_VALUE_CONVERSION[set] = _cast_via_tuple(set)
-ZEN_VALUE_CONVERSION[frozenset] = _cast_via_tuple(frozenset)
-ZEN_VALUE_CONVERSION[deque] = _cast_via_tuple(deque)
+@dataclass(unsafe_hash=True)
+class ConfigFromTuple:
+    _args_: Tuple[Any, ...]
+    _target_: str
+
+    def __post_init__(self):
+        self._args_ = (
+            sanitized_default_value(
+                tuple(self._args_),
+                convert_dataclass=True,
+                allow_zen_conversion=True,
+                structured_conf_permitted=True,
+            ),
+        )
+
+
+@dataclass(unsafe_hash=True)
+class ConfigFromDict:
+    _args_: Any
+    _target_: str
+
+    def __post_init__(self):
+        self._args_ = (
+            sanitized_default_value(
+                dict(self._args_),
+                convert_dataclass=True,
+                allow_zen_conversion=True,
+                structured_conf_permitted=True,
+            ),
+        )
+
+
+@dataclass(unsafe_hash=True)
+class ConfigRange:
+    start: InitVar[int]
+    stop: InitVar[int]
+    step: InitVar[int]
+    _target_: str = field(default=get_obj_path(range), init=False)
+    _args_: Tuple[int, ...] = field(default=(), init=False, repr=False)
+
+    def __post_init__(self, start, stop, step):
+        self._args_ = (start, stop, step)
+
+
+ZEN_VALUE_CONVERSION[set] = partial(ConfigFromTuple, _target_=get_obj_path(set))
+ZEN_VALUE_CONVERSION[frozenset] = partial(
+    ConfigFromTuple, _target_=get_obj_path(frozenset)
+)
+ZEN_VALUE_CONVERSION[deque] = partial(ConfigFromTuple, _target_=get_obj_path(deque))
 
 if bytes in ZEN_SUPPORTED_PRIMITIVES:  # pragma: no cover
-    ZEN_VALUE_CONVERSION[bytes] = _cast_via_tuple(bytes)
+    ZEN_VALUE_CONVERSION[bytes] = partial(ConfigFromTuple, _target_=get_obj_path(bytes))
 
-ZEN_VALUE_CONVERSION[bytearray] = _cast_via_tuple(bytearray)
-ZEN_VALUE_CONVERSION[range] = lambda value: builds(
-    range, value.start, value.stop, value.step
-)()
-ZEN_VALUE_CONVERSION[Counter] = lambda counter: builds(Counter, dict(counter))()
+ZEN_VALUE_CONVERSION[bytearray] = partial(
+    ConfigFromTuple, _target_=get_obj_path(bytearray)
+)
+ZEN_VALUE_CONVERSION[range] = lambda value: ConfigRange(
+    value.start, value.stop, value.step
+)
+ZEN_VALUE_CONVERSION[Counter] = partial(ConfigFromDict, _target_=get_obj_path(Counter))
 ZEN_VALUE_CONVERSION[functools.partial] = _unpack_partial
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/third_party/beartype.py` & `hydra_zen-0.9.1/src/hydra_zen/third_party/beartype.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import inspect
 from typing import Any, Callable, TypeVar, cast
 
 import beartype as bt
 
 from hydra_zen._utils.coerce import coerce_sequences
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/third_party/pydantic.py` & `hydra_zen-0.9.1/src/hydra_zen/third_party/pydantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 import inspect
 from typing import Any, Callable, TypeVar, cast
 
 import pydantic as _pyd
 
 _T = TypeVar("_T", bound=Callable[..., Any])
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/typing/__init__.py` & `hydra_zen-0.9.1/src/hydra_zen/typing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 
 from ._implementations import (
     Builds,
+    DataclassOptions,
     HydraPartialBuilds,
     Importable,
     Just,
     Partial,
     PartialBuilds,
     StoreEntry,
     SupportedPrimitive,
     ZenConvert,
     ZenPartialBuilds,
     ZenWrappers,
 )
 
 __all__ = [
     "Builds",
+    "DataclassOptions",
     "Importable",
     "Just",
     "Partial",
     "PartialBuilds",
     "SupportedPrimitive",
     "ZenWrappers",
     "ZenPartialBuilds",
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/typing/_builds_overloads.py` & `hydra_zen-0.9.1/src/hydra_zen/typing/_builds_overloads.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
+# Copyright (c) 2023 Massachusetts Institute of Technology
 # SPDX-License-Identifier: MIT
 
 # Stores overloads for `builds` with different default-values for signature
 # pyright: strict
 
 from typing import (
     Any,
@@ -18,14 +18,15 @@
 
 from typing_extensions import Literal, ParamSpec, Protocol
 
 from ._implementations import (
     Builds,
     BuildsWithSig,
     DataClass_,
+    DataclassOptions,
     DefaultsList,
     Importable,
     PartialBuilds,
     SupportedPrimitive,
     ZenConvert,
     ZenWrappers,
 )
@@ -50,14 +51,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[()] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
     ) -> Type[BuildsWithSig[Type[R], P]]:
         ...
 
     # partial=False, pop-sig=bool
     @overload
     def __call__(
@@ -70,14 +72,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Type[Builds[Importable]]:
         ...
 
     # partial=True, pop-sig=bool
     @overload
@@ -91,14 +94,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Type[PartialBuilds[Importable]]:
         ...
 
     # partial=bool, pop-sig=False
     @overload
@@ -112,14 +116,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[Type[Builds[Importable]], Type[PartialBuilds[Importable]],]:
         ...
 
     # partial=bool, pop-sig=bool
     @overload
@@ -133,14 +138,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -156,14 +162,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = None,
         hydra_recursive: Optional[bool] = None,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
         hydra_defaults: Optional[DefaultsList] = None,
         frozen: bool = False,
         builds_bases: Tuple[Type[DataClass_], ...] = (),
         dataclass_name: Optional[str] = None,
+        zen_dataclass: Optional[DataclassOptions] = None,
         zen_convert: Optional[ZenConvert] = None,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -185,14 +192,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[()] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
     ) -> Type[BuildsWithSig[Type[R], P]]:
         ...
 
     # partial=False, pop_sig=bool; has *args, **kwargs, and/or `builds_bases`
     @overload
     def __call__(
@@ -205,14 +213,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Type[Builds[Importable]]:
         ...
 
     # partial=True, pop-sig=bool
     @overload
@@ -226,14 +235,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Type[PartialBuilds[Importable]]:
         ...
 
     # partial=bool, pop-sig=False
     @overload
@@ -247,14 +257,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         frozen: bool = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         dataclass_name: Optional[str] = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[Type[Builds[Importable]], Type[PartialBuilds[Importable]]]:
         ...
 
     # partial=bool, pop-sig=bool
     @overload
@@ -268,14 +279,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         frozen: bool = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         dataclass_name: Optional[str] = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -291,14 +303,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = None,
         hydra_recursive: Optional[bool] = None,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
         hydra_defaults: Optional[DefaultsList] = None,
         frozen: bool = False,
         builds_bases: Tuple[Type[DataClass_], ...] = (),
         dataclass_name: Optional[str] = None,
+        zen_dataclass: Optional[DataclassOptions] = None,
         zen_convert: Optional[ZenConvert] = None,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -320,14 +333,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Type[PartialBuilds[Importable]]:
         ...
 
     # partial=False, pop-sig=True; no *args, **kwargs, nor builds_bases
     @overload
@@ -341,14 +355,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[()] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
     ) -> Type[BuildsWithSig[Type[R], P]]:
         ...
 
     # partial=bool, pop-sig=False
     @overload
     def __call__(
@@ -361,14 +376,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[Type[Builds[Importable]], Type[PartialBuilds[Importable]],]:
         ...
 
     # partial=bool, pop-sig=bool
     @overload
@@ -382,14 +398,15 @@
         zen_wrappers: ZenWrappers[Callable[..., Any]] = ...,
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -407,14 +424,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = ...,
         hydra_recursive: Optional[bool] = ...,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = ...,
         hydra_defaults: Optional[DefaultsList] = ...,
         dataclass_name: Optional[str] = ...,
         builds_bases: Tuple[Type[DataClass_], ...] = ...,
         frozen: bool = ...,
+        zen_dataclass: Optional[DataclassOptions] = ...,
         zen_convert: Optional[ZenConvert] = ...,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
@@ -430,14 +448,15 @@
         zen_meta: Optional[Mapping[str, SupportedPrimitive]] = None,
         hydra_recursive: Optional[bool] = None,
         hydra_convert: Optional[Literal["none", "partial", "all"]] = None,
         hydra_defaults: Optional[DefaultsList] = None,
         frozen: bool = False,
         builds_bases: Tuple[Type[DataClass_], ...] = (),
         dataclass_name: Optional[str] = None,
+        zen_dataclass: Optional[DataclassOptions] = None,
         zen_convert: Optional[ZenConvert] = None,
         **kwargs_for_target: SupportedPrimitive,
     ) -> Union[
         Type[Builds[Importable]],
         Type[PartialBuilds[Importable]],
         Type[BuildsWithSig[Type[R], P]],
     ]:
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen/wrapper/_implementations.py` & `hydra_zen-0.9.1/src/hydra_zen/wrapper/_implementations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Copyright (c) 2022 Massachusetts Institute of Technology
-# SPDX-License-Identifier: MIR
+# Copyright (c) 2023 Massachusetts Institute of Technology
+# SPDX-License-Identifier: MIT
 # pyright: strict
 
+import warnings
 from collections import defaultdict, deque
+from functools import wraps
 from inspect import Parameter, signature
 from typing import (
     Any,
     Callable,
     DefaultDict,
     Deque,
     Dict,
@@ -38,15 +40,17 @@
     Protocol,
     TypeAlias,
     TypedDict,
     TypeGuard,
 )
 
 from hydra_zen import instantiate, just, make_custom_builds_fn
+from hydra_zen._compatibility import HYDRA_VERSION, Version
 from hydra_zen.errors import HydraZenValidationError
+from hydra_zen.structured_configs._type_guards import safe_getattr
 from hydra_zen.structured_configs._utils import get_obj_path
 from hydra_zen.typing._implementations import (
     DataClass_,
     GroupName,
     Node,
     NodeName,
     StoreEntry,
@@ -156,15 +160,18 @@
             that will not be extracted from input configs by the zen-wrapped function.
 
             A single string of comma-separated names can be specified.
         """
         self.func: Callable[P, R] = __func
 
         try:
-            self.parameters: Mapping[str, Parameter] = signature(self.func).parameters
+            # Must cast to dict so that `self` is pickle-compatible.
+            self.parameters: Mapping[str, Parameter] = dict(
+                signature(self.func).parameters
+            )
         except (ValueError, TypeError):
             raise HydraZenValidationError(
                 "hydra_zen.zen can only wrap callables that possess inspectable signatures."
             )
 
         if not isinstance(unpack_kwargs, bool):  # type: ignore
             raise TypeError(f"`unpack_kwargs` must be type `bool` got {unpack_kwargs}")
@@ -297,14 +304,15 @@
                 missing_params.append(name)
 
         if missing_params:
             raise HydraZenValidationError(
                 f"`cfg` is missing the following fields: {', '.join(missing_params)}"
             )
 
+    # TODO: add "extract" option that enables returning dict of fields
     def __call__(self, __cfg: Union[ConfigLike, str]) -> R:
         """
         Extracts values from the input config based on the decorated function's
         signature, resolves & instantiates them, and calls the function with them.
 
         Parameters
         ----------
@@ -327,17 +335,17 @@
         if self.pre_call is not None:
             self.pre_call(cfg)
 
         args_ = list(getattr(cfg, "_args_", []))
 
         cfg_kwargs = {
             name: (
-                getattr(cfg, name, param.default)
+                safe_getattr(cfg, name, param.default)
                 if param.default is not param.empty
-                else getattr(cfg, name)
+                else safe_getattr(cfg, name)
             )
             for name, param in self.parameters.items()
             if param.kind not in SKIPPED_PARAM_KINDS and name not in self._exclude
         }
 
         extra_kwargs = {self.CFG_NAME: cfg} if self._has_zen_cfg else {}
         if self._unpack_kwargs:
@@ -366,45 +374,80 @@
     ) -> Callable[[Any], Any]:
         """
         Generates a Hydra-CLI for the wrapped function. Equivalent to `hydra.main(zen(func), [...])()`
 
         Parameters
         ----------
         config_path : Optional[str]
-            The config path, a directory relative to the declaring python file.
+            The config path, an absolute path to a directory or a directory relative to
+            the declaring python file. If `config_path` is not specified no directory is
+            added to the config search path.
 
-            If config_path is not specified no directory is added to the Config search path.
+            Specifying `config_path` via `Zen.hydra_main` is only supported for
+            Hydra 1.3.0+.
 
         config_name : Optional[str]
             The name of the config (usually the file name without the .yaml extension)
 
         version_base : Optional[str]
-            There are three classes of values that the version_base parameter supports, given new and existing users greater control of the default behaviors to use.
+            There are three classes of values that the version_base parameter supports,
+            given new and existing users greater control of the default behaviors to
+            use.
 
             - If the version_base parameter is not specified, Hydra 1.x will use defaults compatible with version 1.1. Also in this case, a warning is issued to indicate an explicit version_base is preferred.
             - If the version_base parameter is None, then the defaults are chosen for the current minor Hydra version. For example for Hydra 1.2, then would imply config_path=None and hydra.job.chdir=False.
             - If the version_base parameter is an explicit version string like "1.1", then the defaults appropriate to that version are used.
 
         Returns
         -------
         hydra_main : Callable[[Any], Any]
             Equivalent to `hydra.main(zen(func), [...])()`
         """
 
         kw = dict(config_name=config_name)
 
+        # For relative config paths, Hydra looks in the directory relative to the file
+        # in which the task function is defined. Unfortunately, it is only able to
+        # follow wrappers starting in Hydra 1.3.0. Thus `Zen.hydra_main` cannot
+        # handle string config_path entries until Hydra 1.3.0
+        if (config_path is _UNSPECIFIED_ and HYDRA_VERSION < Version(1, 2, 0)) or (
+            (
+                isinstance(config_path, str)
+                or (config_path is _UNSPECIFIED_ and version_base == "1.1")
+            )
+            and HYDRA_VERSION < Version(1, 3, 0)
+        ):  # pragma: no cover
+            warnings.warn(
+                "Specifying config_path via hydra_zen.zen(...).hydra_main "
+                "is only supported for Hydra 1.3.0+"
+            )
+        if Version(1, 3, 0) <= HYDRA_VERSION and isinstance(config_path, str):
+            # Here we create an on-the-fly wrapper so that Hydra can trace
+            # back through the wrapper to the original task function
+            # We could give `Zen` as `__wrapped__` attr, but this messes with
+            # things like `inspect.signature`.
+            #
+            # A downside of this is that `wrapper` is not pickle-able.
+            @wraps(self.func)
+            def wrapper(cfg: Any):
+                return self(cfg)
+
+            target = wrapper
+        else:
+            target = self
+
         if config_path is not _UNSPECIFIED_:
             kw["config_path"] = config_path
 
         if (
             SUPPORTS_VERSION_BASE and version_base is not _UNSPECIFIED_
         ):  # pragma: no cover
             kw["version_base"] = version_base
 
-        return hydra.main(**kw)(self)()
+        return hydra.main(**kw)(target)()
 
 
 @overload
 def zen(
     __func: Callable[P, R],
     *,
     unpack_kwargs: bool = ...,
@@ -511,14 +554,16 @@
                return func(**kwargs)
            return wrapped
 
     The presence of a parameter named "zen_cfg" in the wrapped function's signature
     will cause `zen` to pass the full, resolved config to that field. This specific
     parameter name can be overridden via `Zen.CFG_NAME`.
 
+    Specifying `config_path` via `Zen.hydra_main` is only supported for Hydra 1.3.0+.
+
     Examples
     --------
     **Basic Usage**
 
     >>> from hydra_zen import zen, make_config, builds
     >>> def f(x, y): return x + y
     >>> zen_f = zen(f)
@@ -543,22 +588,14 @@
     The wrapped function can be accessed directly
 
     >>> zen_f.func
     <function __main__.f(x, y)>
     >>> zen_f.func(-1, 1)
     0
 
-    `zen` can be used as a decorator
-
-    >>> @zen
-    ... def zen_g(x, y):
-    ...     return x + y
-    >>> zen_g({'x': 1, 'y': 2})
-    3
-
     `zen` is compatible with partial'd functions.
 
     >>> from functools import partial
     >>> pf = partial(lambda x, y: x + y, x=10)
     >>> zpf = zen(pf)
     >>> zpf(dict(y=1))
     11
@@ -635,29 +672,26 @@
     **Using `zen` instead of `@hydra.main`**
 
     The object returned by zen provides a convenience method – `Zen.hydra_main` –
     to generate a CLI for a zen-wrapped task function:
 
     .. code-block:: python
 
-        # example.py
-        from hydra.core.config_store import ConfigStore
-
-        from hydra_zen import builds, zen
-
-        def task(x: int, y: int):
-            print(x + y)
+       # example.py
+       from hydra_zen import zen, store
 
-        cs = ConfigStore.instance()
-        cs.store(name="my_app", node=builds(task, populate_full_signature=True))
+       @store(name="my_app")
+       def task(x: int, y: int):
+           print(x + y)
+
+       if __name__ == "__main__":
+           store.add_to_hydra_store()
+           zen(task).hydra_main(config_name="my_app", config_path=None, version_base="1.2")
 
 
-        if __name__ == "__main__":
-            zen(task).hydra_main(config_name="my_app", config_path=None)
-
     .. code-block:: console
 
        $ python example.py x=1 y=2
        3
 
 
     **Validating input configs**
@@ -758,15 +792,15 @@
     >>> print(to_yaml(default_to_config(func)))
     _target_: __main__.func
     x: ???
     'y': ???
     """
     if is_dataclass(target):
         if isinstance(target, type):
-            if get_obj_path(target).startswith("types."):
+            if not kw and get_obj_path(target).startswith("types."):
                 # handles dataclasses returned by make_config()
                 return target
             return fbuilds(target, **kw, builds_bases=(target,))
         if kw:
             raise ValueError(
                 "store(<dataclass-instance>, [...]) does not support specifying "
                 "keyword arguments"
@@ -819,15 +853,17 @@
     group=None,
     package=None,
     provider=None,
     to_config=default_to_config,
     __kw={},
 )
 
-_DEFAULT_KEYS: Final[FrozenSet[str]] = frozenset(_StoreCallSig.__required_keys__ - {"__kw"})  # type: ignore
+_DEFAULT_KEYS: Final[FrozenSet[str]] = frozenset(
+    _StoreCallSig.__required_keys__ - {"__kw"}
+)
 
 
 class _Deferred:
     __slots__ = ("to_config", "target", "kw")
 
     def __init__(
         self, to_config: Callable[[F], Node], target: F, kw: Dict[str, Any]
@@ -886,25 +922,26 @@
     entry must have an associated name. Optionally, a group, package, and/or provider
     may be specified for the entry as well.
 
     >>> config1 = {'name': 'Roger', 'age': 24}
     >>> config2 = {'name': 'Rita', 'age': 27}
     >>> _ = store(config1, name="roger", group="profiles")
     >>> _ = store(config2, name="rita", group="profiles")
+    >>> store
     zen_store
     {'profiles': ['roger', 'rita']}
 
     A store's entries are keyed by their `(group, name)` pairs (the default group is
     `None`).
 
     >>> store["profiles", "roger"]  # (group, name) -> config node
     {'name': 'Roger', age: 24}
 
     By default, the stored config(s) will be "enqueued" for addition to Hydra's config
-    store, and the method `.add_to_hydra_store()` must be called to add the enqueued
+    store. The method `.add_to_hydra_store()` must be called to add the enqueued
     configs to Hydra's central store.
 
     >>> store.has_enqueued()
     True
     >>> store.add_to_hydra_store()  # adds all enqueued entries to Hydra's global store
     >>> store.has_enqueued()
     False
@@ -973,24 +1010,25 @@
     a: 1
     b: 22
     >>> pyaml(store[None, "func2"])
     _target_: __main__.func
     b: ???
     a: -10
 
-    Note that, by default, the application of `to_config` via the store is deferred
-    until that entry is actually accessed. This defers the runtime cost of constructing
-    configs for the decorated function so that it need not be paid until necessary.
+    Note that, by default, the application of `to_config` via the store **is deferred
+    until that entry is actually accessed**. This offsets the runtime cost of
+    constructing configs for the decorated function so that it need not be paid until
+    the config is actually accessed by the store.
 
     .. _self-partial:
 
     **Customizable store defaults via 'self-partialing' patterns**
 
     The default values for a store's `__call__` parameters – `group`, `to_config`, etc.
-    – can easily be customized. Simpy call the store with those new values and
+    – can easily be customized. Simply call the store with those new values and
     without specifying an object to be stored. This will return a "mirrored" store
     instance – with the same internal state as the original store – with updated
     defaults.
 
     For example, let's create a store where we want to store multiple configs under a
     `'math'` group and under a `'functools'` group, respectively.
 
@@ -1466,20 +1504,39 @@
           'node': {'x': 3}}]
         """
         yield from (_resolve_node(v, copy=True) for v in self._internal_repo.values())
 
     def add_to_hydra_store(self, overwrite_ok: Optional[bool] = None) -> None:
         """Adds all of this store's enqueued entries to Hydra's global config store.
 
+        This method need not be called for a store initialized as
+        `ZenStore(deferred_hydra_store=False)`.
+
         Parameters
         ----------
         overwrite_ok : Optional[bool]
             If `False`, this method raises `ValueError` if an entry in Hydra's config
             store will be overwritten. Defaults to the value of `overwrite_ok`
-            specified when initializing this store."""
+            specified when initializing this store.
+
+        Examples
+        --------
+        >>> from hydra_zen import ZenStore
+        >>> store1 = ZenStore()
+        >>> store2 = ZenStore()
+
+        >>> store1({'a': 1}, name="x")
+        >>> store1.add_to_hydra_store()
+        >>> store2({'a': 2}, name="x")
+        >>> store2.add_to_hydra_store()
+        ValueError: (name=x group=None): Hydra config store entry already exists. Specify `overwrite_ok=True` to enable replacing config store entries
+
+        >>> store2.add_to_hydra_store(overwrite_ok=True)  # successfully overwrites entry
+
+        """
 
         while self._queue:
             entry = _resolve_node(self._queue.popleft(), copy=False)
             if (
                 overwrite_ok is False
                 or (overwrite_ok is None and not self._overwrite_ok)
             ) and self._exists_in_hydra_store(name=entry["name"], group=entry["group"]):
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/PKG-INFO` & `hydra_zen-0.9.1/src/hydra_zen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-zen
-Version: 0.9.0rc5
+Version: 0.9.1
 Summary: Configurable, reproducible, and scalable workflows in Python, via Hydra
 Author-email: Ryan Soklaski <ryan.soklaski@ll.mit.edu>, Justin Goodwin <jgoodwin@ll.mit.edu>
 Maintainer-email: Ryan Soklaski <ryan.soklaski@ll.mit.edu>
 License: MIT
 Project-URL: Homepage, https://mit-ll-responsible-ai.github.io/hydra-zen/
 Project-URL: Bug Reports, https://github.com/mit-ll-responsible-ai/hydra-zen/issues
 Project-URL: Source, https://github.com/mit-ll-responsible-ai/hydra-zen
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: pydantic
 Provides-Extra: beartype
@@ -31,15 +32,15 @@
 
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/hydra-zen">
     <img src="https://img.shields.io/pypi/v/hydra-zen.svg" alt="PyPI" />
   </a>
   <a>
-    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.10-blue.svg" alt="Python version support" />
+    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.11-blue.svg" alt="Python version support" />
   </a>
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://github.com/mit-ll-responsible-ai/hydra-zen/workflows/Tests/badge.svg" alt="GitHub Actions" />
   <a href="https://github.com/mit-ll-responsible-ai/hydra-zen/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://img.shields.io/badge/coverage-100%25-green.svg" alt="Code Coverage" />
   <a href="https://github.com/microsoft/pyright/blob/92b4028cd5fd483efcf3f1cdb8597b2d4edd8866/docs/typed-libraries.md#verifying-type-completeness">
     <img src="https://img.shields.io/badge/type%20completeness-100%25-green.svg" alt="Type-Completeness Score" />
@@ -109,15 +110,15 @@
 }
 ```
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.
 
-© 2022 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+© 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
     
     Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
     SPDX-License-Identifier: MIT
     
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: hydra-zen Version: 0.9.0rc5 Summary: Configurable,
+Metadata-Version: 2.1 Name: hydra-zen Version: 0.9.1 Summary: Configurable,
 reproducible, and scalable workflows in Python, via Hydra Author-email: Ryan
 Soklaski
 soklaski@ll.mit.edu>, Justin Goodwin
 ll.mit.edu> Maintainer-email: Ryan Soklaski
 soklaski@ll.mit.edu> License: MIT Project-URL: Homepage, https://mit-ll-
 responsible-ai.github.io/hydra-zen/ Project-URL: Bug Reports, https://
 github.com/mit-ll-responsible-ai/hydra-zen/issues Project-URL: Source, https://
 github.com/mit-ll-responsible-ai/hydra-zen Keywords: machine
 learning,research,configuration,scalable,reproducible,yaml,Hydra,dataclass
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering Classifier:
-Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: test Provides-Extra: pydantic
-Provides-Extra: beartype License-File: LICENSE.txt # hydra-zen ![image](brand/
-Hydra-Zen_logo_full_filled_bkgrnd_small.png)
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering Classifier: Programming Language :: Python :: 3
+:: Only Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: pydantic Provides-Extra: beartype License-
+File: LICENSE.txt # hydra-zen ![image](brand/Hydra-
+Zen_logo_full_filled_bkgrnd_small.png)
                        [PyPI] [Python version support]
                                [GitHub_Actions]
                                [Code_Coverage]
          [Type-Completeness_Score]_[Tested_with_Hypothesis]_[Cite_Us]
 A_library_that_facilitates_configurable,_reproducible,_and_scalable_workflows,
                                  using_Hydra.
                Check_out_our_documentation_for_more_information.
@@ -51,15 +52,15 @@
 the Discussion Share ideas, ask questions, and chat with us over at [hydra-
 zen's discussion board](https://github.com/mit-ll-responsible-ai/hydra-zen/
 discussions). ## Citation Using `hydra-zen` for your research? Please cite the
 following publication: ``` @article{soklaski2022tools, title={Tools and
 Practices for Responsible AI Engineering}, author={Soklaski, Ryan and Goodwin,
 Justin and Brown, Olivia and Yee, Michael and Matterer, Jason}, journal={arXiv
 preprint arXiv:2201.05647}, year={2022} } ``` ## Disclaimer DISTRIBUTION
-STATEMENT A. Approved for public release: distribution unlimited. Â© 2022
+STATEMENT A. Approved for public release: distribution unlimited. Â© 2023
 MASSACHUSETTS INSTITUTE OF TECHNOLOGY Subject to FAR 52.227-11 â Patent
 Rights â Ownership by the Contractor (May 2014) SPDX-License-Identifier: MIT
 This material is based upon work supported by the Under Secretary of Defense
 for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any
 opinions, findings, conclusions or recommendations expressed in this material
 are those of the author(s) and do not necessarily reflect the views of the
 Under Secretary of Defense for Research and Engineering. A portion of this
```

### Comparing `hydra_zen-0.9.0rc5/src/hydra_zen.egg-info/SOURCES.txt` & `hydra_zen-0.9.1/src/hydra_zen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 brand/HydraZen_logo_border.png
 brand/HydraZen_logo_border.svg
 brand/HydraZen_logo_transparent.png
 brand/HydraZen_logo_transparent.svg
 brand/README.md
 brand/hydra_zen_favicon_32x32.ico
 brand/hydra_zen_favicon_64x64.ico
+deps/requirements-pyright.txt
 docs/Makefile
 docs/README.md
 docs/make.bat
 docs/requirements.txt
 docs/source/api_reference.rst
 docs/source/changes.rst
 docs/source/conf.py
@@ -59,14 +60,15 @@
 docs/source/generated/hydra_zen.load_from_yaml.rst
 docs/source/generated/hydra_zen.make_config.rst
 docs/source/generated/hydra_zen.make_custom_builds_fn.rst
 docs/source/generated/hydra_zen.save_as_yaml.rst
 docs/source/generated/hydra_zen.third_party.beartype.validates_with_beartype.rst
 docs/source/generated/hydra_zen.third_party.pydantic.validates_with_pydantic.rst
 docs/source/generated/hydra_zen.to_yaml.rst
+docs/source/generated/hydra_zen.typing.DataclassOptions.rst
 docs/source/generated/hydra_zen.typing.ZenConvert.rst
 docs/source/generated/hydra_zen.uses_zen_processing.rst
 docs/source/generated/hydra_zen.wrapper.Zen.rst
 docs/source/generated/hydra_zen.wrapper.default_to_config.rst
 docs/source/generated/hydra_zen.zen.rst
 docs/source/how_to/beartype.rst
 docs/source/how_to/partial_config.rst
```

