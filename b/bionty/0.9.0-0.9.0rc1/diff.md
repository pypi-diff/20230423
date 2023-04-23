# Comparing `tmp/bionty-0.9.0.tar.gz` & `tmp/bionty-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bionty-0.9.0.tar", last modified: Mon Mar 20 08:30:08 2023, max compression
+gzip compressed data, was "bionty-0.9.0rc1.tar", last modified: Mon Mar 20 04:17:59 2023, max compression
```

## Comparing `bionty-0.9.0.tar` & `bionty-0.9.0rc1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     2961 2023-03-14 04:26:15.628168 bionty-0.9.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      565 2023-03-09 16:33:42.761504 bionty-0.9.0/.github/workflows/check_ontologies_reachable.yml
--rw-r--r--   0        0        0      133 2022-06-10 04:02:03.586438 bionty-0.9.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-06-10 04:02:03.586557 bionty-0.9.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1656 2022-12-08 13:47:44.595593 bionty-0.9.0/.gitignore
--rw-r--r--   0        0        0     2032 2023-03-20 08:14:10.065284 bionty-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-05-24 03:41:13.749291 bionty-0.9.0/LICENSE
--rw-r--r--   0        0        0      475 2023-03-09 04:37:19.892337 bionty-0.9.0/README.md
--rw-r--r--   0        0        0     1709 2023-03-20 08:16:21.626965 bionty-0.9.0/bionty/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 03:04:01.466966 bionty-0.9.0/bionty/_compat/__init__.py
--rw-r--r--   0        0        0     1229 2023-03-20 03:04:01.467112 bionty-0.9.0/bionty/_compat/bionty_0_8_1.py
--rw-r--r--   0        0        0      537 2023-03-20 03:04:01.467226 bionty-0.9.0/bionty/_compat/update_yaml_format.py
--rw-r--r--   0        0        0     2370 2023-03-20 03:04:01.467703 bionty-0.9.0/bionty/_display_versions.py
--rw-r--r--   0        0        0    14118 2023-03-20 03:04:01.467894 bionty-0.9.0/bionty/_entity.py
--rw-r--r--   0        0        0      498 2023-02-20 04:29:37.647082 bionty-0.9.0/bionty/_lookup.py
--rw-r--r--   0        0        0     1021 2023-03-14 04:26:15.629396 bionty-0.9.0/bionty/_md5.py
--rw-r--r--   0        0        0     1192 2023-03-02 03:05:01.759857 bionty-0.9.0/bionty/_normalize.py
--rw-r--r--   0        0        0     1829 2023-01-10 08:57:12.651924 bionty-0.9.0/bionty/_ontology.py
--rw-r--r--   0        0        0     2035 2023-03-02 03:05:01.760487 bionty-0.9.0/bionty/_settings.py
--rw-r--r--   0        0        0     1668 2023-03-20 07:20:37.651077 bionty-0.9.0/bionty/_sync_versions.py
--rw-r--r--   0        0        0      406 2023-03-02 03:05:01.761968 bionty-0.9.0/bionty/dev/__init__.py
--rw-r--r--   0        0        0     4813 2023-03-14 04:26:15.630746 bionty-0.9.0/bionty/dev/_fix_index.py
--rw-r--r--   0        0        0     4562 2023-03-20 08:14:10.065837 bionty-0.9.0/bionty/dev/_handle_versions.py
--rw-r--r--   0        0        0     1788 2023-03-20 03:04:01.469593 bionty-0.9.0/bionty/dev/_io.py
--rw-r--r--   0        0        0      518 2022-12-01 08:16:29.966943 bionty-0.9.0/bionty/dev/_ontology.py
--rw-r--r--   0        0        0        0 2023-03-07 09:45:48.623022 bionty-0.9.0/bionty/entities/__init__.py
--rw-r--r--   0        0        0      715 2023-03-07 09:45:48.623165 bionty-0.9.0/bionty/entities/_cellline.py
--rw-r--r--   0        0        0     1468 2023-03-14 05:49:23.374924 bionty-0.9.0/bionty/entities/_cellmarker.py
--rw-r--r--   0        0        0      869 2023-03-07 09:45:48.623356 bionty-0.9.0/bionty/entities/_celltype.py
--rw-r--r--   0        0        0      871 2023-03-08 13:54:18.303730 bionty-0.9.0/bionty/entities/_disease.py
--rw-r--r--   0        0        0     3282 2023-03-14 05:49:23.375321 bionty-0.9.0/bionty/entities/_gene.py
--rw-r--r--   0        0        0      698 2023-03-20 03:04:01.469740 bionty-0.9.0/bionty/entities/_pathway.py
--rw-r--r--   0        0        0      710 2023-03-07 09:45:48.623628 bionty-0.9.0/bionty/entities/_phenotype.py
--rw-r--r--   0        0        0     2186 2023-03-14 05:49:23.375661 bionty-0.9.0/bionty/entities/_protein.py
--rw-r--r--   0        0        0     4261 2023-03-09 06:29:48.135984 bionty-0.9.0/bionty/entities/_readout.py
--rw-r--r--   0        0        0     1077 2023-03-07 09:45:48.623896 bionty-0.9.0/bionty/entities/_shared_docstrings.py
--rw-r--r--   0        0        0     1524 2023-03-14 05:49:23.387965 bionty-0.9.0/bionty/entities/_species.py
--rw-r--r--   0        0        0      682 2023-03-08 13:54:18.304039 bionty-0.9.0/bionty/entities/_tissue.py
--rw-r--r--   0        0        0     3802 2023-03-20 05:48:42.793246 bionty-0.9.0/bionty/versions/versions.yaml
--rw-r--r--   0        0        0       48 2022-06-13 03:49:31.099594 bionty-0.9.0/docs/api.md
--rw-r--r--   0        0        0    22228 2023-03-20 08:16:32.702543 bionty-0.9.0/docs/changelog.md
--rw-r--r--   0        0        0      443 2023-03-08 13:54:18.304698 bionty-0.9.0/docs/faq/faq.md
--rw-r--r--   0        0        0       42 2023-03-02 03:05:01.763048 bionty-0.9.0/docs/faq/index.md
--rw-r--r--   0        0        0     1635 2023-03-14 10:15:14.338245 bionty-0.9.0/docs/guide/config.md
--rw-r--r--   0        0        0     9769 2023-03-20 07:42:24.790645 bionty-0.9.0/docs/guide/curate.ipynb
--rw-r--r--   0        0        0     4794 2023-03-14 04:26:15.633240 bionty-0.9.0/docs/guide/extend.md
--rw-r--r--   0        0        0     2032 2023-03-11 10:10:31.170729 bionty-0.9.0/docs/guide/index.md
--rw-r--r--   0        0        0     7281 2023-03-20 07:42:24.793719 bionty-0.9.0/docs/guide/lookup.ipynb
--rw-r--r--   0        0        0     8229 2023-03-20 07:42:24.811377 bionty-0.9.0/docs/guide/ontology.ipynb
--rw-r--r--   0        0        0    62594 2023-03-11 10:10:31.172325 bionty-0.9.0/docs/img/gene_lookup.png
--rw-r--r--   0        0        0    61944 2023-03-11 10:10:31.173143 bionty-0.9.0/docs/img/lookup_pd1.png
--rw-r--r--   0        0        0     2956 2023-03-20 03:04:01.472303 bionty-0.9.0/docs/index.md
--rw-r--r--   0        0        0      127 2022-09-28 12:15:29.983077 bionty-0.9.0/lamin-project.yaml
--rw-r--r--   0        0        0      597 2023-03-09 16:33:42.762922 bionty-0.9.0/noxfile.py
--rw-r--r--   0        0        0     1032 2023-03-20 07:48:49.103830 bionty-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2067 2023-03-14 04:26:15.635383 bionty-0.9.0/scripts/check_ontologies_reachable.py
--rw-r--r--   0        0        0     1136 2023-03-08 13:54:18.306236 bionty-0.9.0/tests/entities/test_cellline.py
--rw-r--r--   0        0        0     1019 2023-03-08 13:54:18.306304 bionty-0.9.0/tests/entities/test_cellmarker.py
--rw-r--r--   0        0        0     2135 2023-03-08 13:54:18.306378 bionty-0.9.0/tests/entities/test_celltype.py
--rw-r--r--   0        0        0     2180 2023-03-08 13:54:18.306445 bionty-0.9.0/tests/entities/test_disease.py
--rw-r--r--   0        0        0      712 2023-03-08 13:54:18.306508 bionty-0.9.0/tests/entities/test_gene.py
--rw-r--r--   0        0        0      545 2023-03-20 03:04:01.472424 bionty-0.9.0/tests/entities/test_pathway.py
--rw-r--r--   0        0        0     1116 2023-03-08 13:54:18.306607 bionty-0.9.0/tests/entities/test_phenotype.py
--rw-r--r--   0        0        0     1087 2023-03-08 13:54:18.306667 bionty-0.9.0/tests/entities/test_protein.py
--rw-r--r--   0        0        0     1043 2023-03-08 13:54:18.306765 bionty-0.9.0/tests/entities/test_readout.py
--rw-r--r--   0        0        0     1117 2023-03-08 13:54:18.306822 bionty-0.9.0/tests/entities/test_species.py
--rw-r--r--   0        0        0     1139 2023-03-08 13:54:18.306921 bionty-0.9.0/tests/entities/test_tissue.py
--rw-r--r--   0        0        0      831 2022-08-28 18:47:20.621380 bionty-0.9.0/tests/test_curate.py
--rw-r--r--   0        0        0      167 2023-03-02 03:05:01.765791 bionty-0.9.0/tests/test_current_db_version.py
--rw-r--r--   0        0        0      649 2023-03-02 03:05:01.765888 bionty-0.9.0/tests/test_entity.py
--rw-r--r--   0        0        0     1194 2022-08-27 13:16:44.258336 bionty-0.9.0/tests/test_fix_index.py
--rw-r--r--   0        0        0      170 2023-02-20 04:29:37.649130 bionty-0.9.0/tests/test_lookup.py
--rw-r--r--   0        0        0      765 2023-03-14 04:26:15.635704 bionty-0.9.0/tests/test_md5.py
--rw-r--r--   0        0        0      503 2023-02-06 09:05:53.384967 bionty-0.9.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      263 2023-03-02 03:05:01.765946 bionty-0.9.0/tests/test_ontology.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 bionty-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2961 2023-03-14 04:26:15.628168 bionty-0.9.0rc1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      565 2023-03-09 16:33:42.761504 bionty-0.9.0rc1/.github/workflows/check_ontologies_reachable.yml
+-rw-r--r--   0        0        0      133 2022-06-10 04:02:03.586438 bionty-0.9.0rc1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-06-10 04:02:03.586557 bionty-0.9.0rc1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1656 2022-12-08 13:47:44.595593 bionty-0.9.0rc1/.gitignore
+-rw-r--r--   0        0        0     2025 2023-03-07 09:45:48.622428 bionty-0.9.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-05-24 03:41:13.749291 bionty-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0      475 2023-03-09 04:37:19.892337 bionty-0.9.0rc1/README.md
+-rw-r--r--   0        0        0     1712 2023-03-20 04:16:13.262896 bionty-0.9.0rc1/bionty/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-20 03:04:01.466966 bionty-0.9.0rc1/bionty/_compat/__init__.py
+-rw-r--r--   0        0        0     1229 2023-03-20 03:04:01.467112 bionty-0.9.0rc1/bionty/_compat/bionty_0_8_1.py
+-rw-r--r--   0        0        0      537 2023-03-20 03:04:01.467226 bionty-0.9.0rc1/bionty/_compat/update_yaml_format.py
+-rw-r--r--   0        0        0     2370 2023-03-20 03:04:01.467703 bionty-0.9.0rc1/bionty/_display_versions.py
+-rw-r--r--   0        0        0    14118 2023-03-20 03:04:01.467894 bionty-0.9.0rc1/bionty/_entity.py
+-rw-r--r--   0        0        0      498 2023-02-20 04:29:37.647082 bionty-0.9.0rc1/bionty/_lookup.py
+-rw-r--r--   0        0        0     1021 2023-03-14 04:26:15.629396 bionty-0.9.0rc1/bionty/_md5.py
+-rw-r--r--   0        0        0     1192 2023-03-02 03:05:01.759857 bionty-0.9.0rc1/bionty/_normalize.py
+-rw-r--r--   0        0        0     1829 2023-01-10 08:57:12.651924 bionty-0.9.0rc1/bionty/_ontology.py
+-rw-r--r--   0        0        0     2035 2023-03-02 03:05:01.760487 bionty-0.9.0rc1/bionty/_settings.py
+-rw-r--r--   0        0        0     1668 2023-03-20 03:04:01.468578 bionty-0.9.0rc1/bionty/_sync_versions.py
+-rw-r--r--   0        0        0      406 2023-03-02 03:05:01.761968 bionty-0.9.0rc1/bionty/dev/__init__.py
+-rw-r--r--   0        0        0     4813 2023-03-14 04:26:15.630746 bionty-0.9.0rc1/bionty/dev/_fix_index.py
+-rw-r--r--   0        0        0     3810 2023-03-20 03:04:01.468812 bionty-0.9.0rc1/bionty/dev/_handle_versions.py
+-rw-r--r--   0        0        0     1788 2023-03-20 03:04:01.469593 bionty-0.9.0rc1/bionty/dev/_io.py
+-rw-r--r--   0        0        0      518 2022-12-01 08:16:29.966943 bionty-0.9.0rc1/bionty/dev/_ontology.py
+-rw-r--r--   0        0        0        0 2023-03-07 09:45:48.623022 bionty-0.9.0rc1/bionty/entities/__init__.py
+-rw-r--r--   0        0        0      715 2023-03-07 09:45:48.623165 bionty-0.9.0rc1/bionty/entities/_cellline.py
+-rw-r--r--   0        0        0     1468 2023-03-14 05:49:23.374924 bionty-0.9.0rc1/bionty/entities/_cellmarker.py
+-rw-r--r--   0        0        0      869 2023-03-07 09:45:48.623356 bionty-0.9.0rc1/bionty/entities/_celltype.py
+-rw-r--r--   0        0        0      871 2023-03-08 13:54:18.303730 bionty-0.9.0rc1/bionty/entities/_disease.py
+-rw-r--r--   0        0        0     3282 2023-03-14 05:49:23.375321 bionty-0.9.0rc1/bionty/entities/_gene.py
+-rw-r--r--   0        0        0      698 2023-03-20 03:04:01.469740 bionty-0.9.0rc1/bionty/entities/_pathway.py
+-rw-r--r--   0        0        0      710 2023-03-07 09:45:48.623628 bionty-0.9.0rc1/bionty/entities/_phenotype.py
+-rw-r--r--   0        0        0     2186 2023-03-14 05:49:23.375661 bionty-0.9.0rc1/bionty/entities/_protein.py
+-rw-r--r--   0        0        0     4261 2023-03-09 06:29:48.135984 bionty-0.9.0rc1/bionty/entities/_readout.py
+-rw-r--r--   0        0        0     1077 2023-03-07 09:45:48.623896 bionty-0.9.0rc1/bionty/entities/_shared_docstrings.py
+-rw-r--r--   0        0        0     1524 2023-03-14 05:49:23.387965 bionty-0.9.0rc1/bionty/entities/_species.py
+-rw-r--r--   0        0        0      682 2023-03-08 13:54:18.304039 bionty-0.9.0rc1/bionty/entities/_tissue.py
+-rw-r--r--   0        0        0     3802 2023-03-20 03:04:01.470315 bionty-0.9.0rc1/bionty/versions/versions.yaml
+-rw-r--r--   0        0        0       48 2022-06-13 03:49:31.099594 bionty-0.9.0rc1/docs/api.md
+-rw-r--r--   0        0        0    22071 2023-03-20 04:17:10.961187 bionty-0.9.0rc1/docs/changelog.md
+-rw-r--r--   0        0        0      443 2023-03-08 13:54:18.304698 bionty-0.9.0rc1/docs/faq/faq.md
+-rw-r--r--   0        0        0       42 2023-03-02 03:05:01.763048 bionty-0.9.0rc1/docs/faq/index.md
+-rw-r--r--   0        0        0     1635 2023-03-14 10:15:14.338245 bionty-0.9.0rc1/docs/guide/config.md
+-rw-r--r--   0        0        0     9769 2023-03-20 03:04:01.471316 bionty-0.9.0rc1/docs/guide/curate.ipynb
+-rw-r--r--   0        0        0     4794 2023-03-14 04:26:15.633240 bionty-0.9.0rc1/docs/guide/extend.md
+-rw-r--r--   0        0        0     2032 2023-03-11 10:10:31.170729 bionty-0.9.0rc1/docs/guide/index.md
+-rw-r--r--   0        0        0     7281 2023-03-20 03:04:01.471483 bionty-0.9.0rc1/docs/guide/lookup.ipynb
+-rw-r--r--   0        0        0     8229 2023-03-20 03:04:01.471920 bionty-0.9.0rc1/docs/guide/ontology.ipynb
+-rw-r--r--   0        0        0    62594 2023-03-11 10:10:31.172325 bionty-0.9.0rc1/docs/img/gene_lookup.png
+-rw-r--r--   0        0        0    61944 2023-03-11 10:10:31.173143 bionty-0.9.0rc1/docs/img/lookup_pd1.png
+-rw-r--r--   0        0        0     2956 2023-03-20 03:04:01.472303 bionty-0.9.0rc1/docs/index.md
+-rw-r--r--   0        0        0      127 2022-09-28 12:15:29.983077 bionty-0.9.0rc1/lamin-project.yaml
+-rw-r--r--   0        0        0      597 2023-03-09 16:33:42.762922 bionty-0.9.0rc1/noxfile.py
+-rw-r--r--   0        0        0     1032 2023-03-02 03:05:01.765683 bionty-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2067 2023-03-14 04:26:15.635383 bionty-0.9.0rc1/scripts/check_ontologies_reachable.py
+-rw-r--r--   0        0        0     1136 2023-03-08 13:54:18.306236 bionty-0.9.0rc1/tests/entities/test_cellline.py
+-rw-r--r--   0        0        0     1019 2023-03-08 13:54:18.306304 bionty-0.9.0rc1/tests/entities/test_cellmarker.py
+-rw-r--r--   0        0        0     2135 2023-03-08 13:54:18.306378 bionty-0.9.0rc1/tests/entities/test_celltype.py
+-rw-r--r--   0        0        0     2180 2023-03-08 13:54:18.306445 bionty-0.9.0rc1/tests/entities/test_disease.py
+-rw-r--r--   0        0        0      712 2023-03-08 13:54:18.306508 bionty-0.9.0rc1/tests/entities/test_gene.py
+-rw-r--r--   0        0        0      545 2023-03-20 03:04:01.472424 bionty-0.9.0rc1/tests/entities/test_pathway.py
+-rw-r--r--   0        0        0     1116 2023-03-08 13:54:18.306607 bionty-0.9.0rc1/tests/entities/test_phenotype.py
+-rw-r--r--   0        0        0     1087 2023-03-08 13:54:18.306667 bionty-0.9.0rc1/tests/entities/test_protein.py
+-rw-r--r--   0        0        0     1043 2023-03-08 13:54:18.306765 bionty-0.9.0rc1/tests/entities/test_readout.py
+-rw-r--r--   0        0        0     1117 2023-03-08 13:54:18.306822 bionty-0.9.0rc1/tests/entities/test_species.py
+-rw-r--r--   0        0        0     1139 2023-03-08 13:54:18.306921 bionty-0.9.0rc1/tests/entities/test_tissue.py
+-rw-r--r--   0        0        0      831 2022-08-28 18:47:20.621380 bionty-0.9.0rc1/tests/test_curate.py
+-rw-r--r--   0        0        0      167 2023-03-02 03:05:01.765791 bionty-0.9.0rc1/tests/test_current_db_version.py
+-rw-r--r--   0        0        0      649 2023-03-02 03:05:01.765888 bionty-0.9.0rc1/tests/test_entity.py
+-rw-r--r--   0        0        0     1194 2022-08-27 13:16:44.258336 bionty-0.9.0rc1/tests/test_fix_index.py
+-rw-r--r--   0        0        0      170 2023-02-20 04:29:37.649130 bionty-0.9.0rc1/tests/test_lookup.py
+-rw-r--r--   0        0        0      765 2023-03-14 04:26:15.635704 bionty-0.9.0rc1/tests/test_md5.py
+-rw-r--r--   0        0        0      503 2023-02-06 09:05:53.384967 bionty-0.9.0rc1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      263 2023-03-02 03:05:01.765946 bionty-0.9.0rc1/tests/test_ontology.py
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 bionty-0.9.0rc1/PKG-INFO
```

### Comparing `bionty-0.9.0/.github/workflows/build.yml` & `bionty-0.9.0rc1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/.github/workflows/check_ontologies_reachable.yml` & `bionty-0.9.0rc1/.github/workflows/check_ontologies_reachable.yml`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/.github/workflows/latest-changes.yml` & `bionty-0.9.0rc1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/.gitignore` & `bionty-0.9.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/.pre-commit-config.yaml` & `bionty-0.9.0rc1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - id: flake8
         additional_dependencies:
           - flake8-black>=0.1.1
           - flake8-typing-imports==1.10.0
         language_version: python3
         args:
           - --max-line-length=88
-          - --ignore=E203,BLK100
+          - --ignore=E203
           - --min-python-version=3.8.0
         exclude: |
           (?x)(
               __init__.py
           )
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.6.2
```

### Comparing `bionty-0.9.0/LICENSE` & `bionty-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/__init__.py` & `bionty-0.9.0rc1/bionty/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 .. autosummary::
    :toctree: .
 
    dev
 
 """
 
-__version__ = "0.9.0"  # denote release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.9.0rc1"  # denote release candidate for 0.1.0 with 0.1rc1
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
 
 from . import _sync_versions
```

### Comparing `bionty-0.9.0/bionty/_compat/bionty_0_8_1.py` & `bionty-0.9.0rc1/bionty/_compat/bionty_0_8_1.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_compat/update_yaml_format.py` & `bionty-0.9.0rc1/bionty/_compat/update_yaml_format.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_display_versions.py` & `bionty-0.9.0rc1/bionty/_display_versions.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_entity.py` & `bionty-0.9.0rc1/bionty/_entity.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_md5.py` & `bionty-0.9.0rc1/bionty/_md5.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_normalize.py` & `bionty-0.9.0rc1/bionty/_normalize.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_ontology.py` & `bionty-0.9.0rc1/bionty/_ontology.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_settings.py` & `bionty-0.9.0rc1/bionty/_settings.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/_sync_versions.py` & `bionty-0.9.0rc1/bionty/_sync_versions.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/dev/_fix_index.py` & `bionty-0.9.0rc1/bionty/dev/_fix_index.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/dev/_handle_versions.py` & `bionty-0.9.0rc1/bionty/dev/_handle_versions.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bionty.dev._io import load_yaml, write_yaml
 
 ROOT = Path(__file__).parent.parent / "versions"
 VERSIONS_PATH = ROOT / "versions.yaml"
 _CURRENT_PATH = ROOT / "._current.yaml"
 _LNDB_PATH = ROOT / "._lndb.yaml"
 
-LOCAL_PATH = settings.versionsdir / "local.yaml"
+_LOCAL_PATH = settings.versionsdir / "local.yaml"
 
 
 def latest_db_version(db: str) -> str:
     """Lookup the latest version of a database.
 
     Args:
         db: The database to look up the version for.
@@ -52,15 +52,15 @@
 
     Args:
         overwrite: Whether to overwrite the _current.yaml even if it exists already.
         source: The yaml source to use to create the _current.yaml . Defaults to local.
     """
     if not _CURRENT_PATH.exists() or overwrite:
         versions = (
-            load_yaml(VERSIONS_PATH) if source == "versions" else load_yaml(LOCAL_PATH)
+            load_yaml(VERSIONS_PATH) if source == "versions" else load_yaml(_LOCAL_PATH)
         )
 
         def _write_current_yaml(versions):
             _current = {}
             for name, db_versions in versions.items():
                 if name == "version":
                     continue
@@ -72,68 +72,51 @@
             return _current
 
         _current = _write_current_yaml(versions)
         write_yaml(_current, _CURRENT_PATH)
 
 
 def create_local(overwrite: bool = True) -> None:
-    """If local.yaml doesn't exist, copy from versions.yaml and create it.
+    """If _local.yaml doesn't exist, copy from versions.yaml and create it.
 
     Args:
-        overwrite: Whether to overwrite the current local.yaml .
+        overwrite: Whether to overwrite the current _local.yaml .
     """
-    if not LOCAL_PATH.exists() or overwrite:
+    if not _LOCAL_PATH.exists() or overwrite:
         versions = load_yaml(VERSIONS_PATH)
-        # convert all non string keys to strings
-        local_versions = {}
-        for entity, dbs in versions.items():
-            local_versions[entity] = versions[entity]
-            if entity == "version":
-                continue
-            for db_name, v in dbs.items():
-                # list is needed here to avoid dict key change error
-                for version in list(v["versions"]):
-                    if isinstance(version, str):
-                        continue
-                    local_versions[entity][db_name]["versions"][
-                        str(version)
-                    ] = local_versions[entity][db_name]["versions"].pop(version)
 
-        write_yaml(local_versions, LOCAL_PATH)
+        write_yaml(versions, _LOCAL_PATH)
 
 
 def update_local() -> None:
     """Update _local to add additional entries from the public versions.yaml table.
 
     Args:
-        to_update_yaml: Dictionary of the current local.yaml .
+        to_update_yaml: Dictionary of the current _local.yaml .
     """
-    to_update_yaml = load_yaml(LOCAL_PATH)
+    to_update_yaml = load_yaml(_LOCAL_PATH)
 
     versions = load_yaml(VERSIONS_PATH)
 
     for entity, dbs in versions.items():
         if entity == "version":
             continue
         if entity not in to_update_yaml:
             to_update_yaml[entity] = versions[entity]
         else:
             for db_name, v in dbs.items():
                 if db_name not in to_update_yaml[entity]:
                     to_update_yaml[entity][db_name] = dbs[db_name]
                 else:
                     for version in v["versions"]:
-                        if (
-                            str(version)
-                            not in to_update_yaml[entity][db_name]["versions"]
-                        ):
+                        if version not in to_update_yaml[entity][db_name]["versions"]:
                             to_update_yaml[entity][db_name]["versions"][version] = v[
                                 "versions"
                             ][version]
 
-    write_yaml(to_update_yaml, LOCAL_PATH)
+    write_yaml(to_update_yaml, _LOCAL_PATH)
 
 
 def create_lndb() -> None:
     """If no ._lndb file, write ._current to ._lndb for lndb."""
     if not _LNDB_PATH.exists():
         shutil.copy2(_CURRENT_PATH, _LNDB_PATH)
```

### Comparing `bionty-0.9.0/bionty/dev/_io.py` & `bionty-0.9.0rc1/bionty/dev/_io.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/dev/_ontology.py` & `bionty-0.9.0rc1/bionty/dev/_ontology.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_cellline.py` & `bionty-0.9.0rc1/bionty/entities/_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_cellmarker.py` & `bionty-0.9.0rc1/bionty/entities/_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_celltype.py` & `bionty-0.9.0rc1/bionty/entities/_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_disease.py` & `bionty-0.9.0rc1/bionty/entities/_disease.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_gene.py` & `bionty-0.9.0rc1/bionty/entities/_gene.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_pathway.py` & `bionty-0.9.0rc1/bionty/entities/_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_phenotype.py` & `bionty-0.9.0rc1/bionty/entities/_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_protein.py` & `bionty-0.9.0rc1/bionty/entities/_protein.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_readout.py` & `bionty-0.9.0rc1/bionty/entities/_readout.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_shared_docstrings.py` & `bionty-0.9.0rc1/bionty/entities/_shared_docstrings.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_species.py` & `bionty-0.9.0rc1/bionty/entities/_species.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/entities/_tissue.py` & `bionty-0.9.0rc1/bionty/entities/_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/bionty/versions/versions.yaml` & `bionty-0.9.0rc1/bionty/versions/versions.yaml`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/changelog.md` & `bionty-0.9.0rc1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | User | Date | Patch
 --- | --- | --- | --- | ---
-🚑 Ensure version names are strings | [269](https://github.com/laminlabs/bionty/pull/269) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-20 | 0.9.0
 ✨ Add pathway ontology | [267](https://github.com/laminlabs/bionty/pull/267) | [Zethson](https://github.com/Zethson) | 2023-03-17 | 0.9.0rc1
 ✨ Add compatibility functions | [264](https://github.com/laminlabs/bionty/pull/264) | [Zethson](https://github.com/Zethson) | 2023-03-17 |
 ✨ Add latest version inference if only db is passed | [256](https://github.com/laminlabs/bionty/pull/256) | [Zethson](https://github.com/Zethson) | 2023-03-14 |
 🐛 Fix default ids | [257](https://github.com/laminlabs/bionty/pull/257) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-14 |
 Add md5 sums | [249](https://github.com/laminlabs/bionty/pull/249) | [Zethson](https://github.com/Zethson) | 2023-03-13 |
 🎨 Fixed case sensitivity, lookup output as namedtuple | [255](https://github.com/laminlabs/bionty/pull/255) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-11 |
 💥 Lookup returns the full record | [254](https://github.com/laminlabs/bionty/pull/254) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-11 |
```

### Comparing `bionty-0.9.0/docs/guide/config.md` & `bionty-0.9.0rc1/docs/guide/config.md`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/guide/curate.ipynb` & `bionty-0.9.0rc1/docs/guide/curate.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/guide/extend.md` & `bionty-0.9.0rc1/docs/guide/extend.md`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/guide/index.md` & `bionty-0.9.0rc1/docs/guide/index.md`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/guide/lookup.ipynb` & `bionty-0.9.0rc1/docs/guide/lookup.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/guide/ontology.ipynb` & `bionty-0.9.0rc1/docs/guide/ontology.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/img/gene_lookup.png` & `bionty-0.9.0rc1/docs/img/gene_lookup.png`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/img/lookup_pd1.png` & `bionty-0.9.0rc1/docs/img/lookup_pd1.png`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/docs/index.md` & `bionty-0.9.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/noxfile.py` & `bionty-0.9.0rc1/noxfile.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/pyproject.toml` & `bionty-0.9.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/scripts/check_ontologies_reachable.py` & `bionty-0.9.0rc1/scripts/check_ontologies_reachable.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_cellline.py` & `bionty-0.9.0rc1/tests/entities/test_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_cellmarker.py` & `bionty-0.9.0rc1/tests/entities/test_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_celltype.py` & `bionty-0.9.0rc1/tests/entities/test_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_disease.py` & `bionty-0.9.0rc1/tests/entities/test_disease.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_gene.py` & `bionty-0.9.0rc1/tests/entities/test_gene.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_pathway.py` & `bionty-0.9.0rc1/tests/entities/test_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_phenotype.py` & `bionty-0.9.0rc1/tests/entities/test_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_protein.py` & `bionty-0.9.0rc1/tests/entities/test_protein.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_readout.py` & `bionty-0.9.0rc1/tests/entities/test_readout.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_species.py` & `bionty-0.9.0rc1/tests/entities/test_species.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/entities/test_tissue.py` & `bionty-0.9.0rc1/tests/entities/test_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/test_curate.py` & `bionty-0.9.0rc1/tests/test_curate.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/test_entity.py` & `bionty-0.9.0rc1/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/test_fix_index.py` & `bionty-0.9.0rc1/tests/test_fix_index.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/tests/test_md5.py` & `bionty-0.9.0rc1/tests/test_md5.py`

 * *Files identical despite different names*

### Comparing `bionty-0.9.0/PKG-INFO` & `bionty-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionty
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Bionty: Data model generator for biology.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

