# Comparing `tmp/colrev-0.8.2.tar.gz` & `tmp/colrev-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colrev-0.8.2.tar", max compression
+gzip compressed data, was "colrev-0.8.3.tar", max compression
```

## Comparing `colrev-0.8.2.tar` & `colrev-0.8.3.tar`

### file list

```diff
@@ -1,420 +1,338 @@
--rw-r--r--   0        0        0     8176 2023-04-05 07:20:58.614422 colrev-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     3322 2023-04-05 07:20:58.614422 colrev-0.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1070 2023-04-05 07:20:58.614422 colrev-0.8.2/LICENSE
--rw-r--r--   0        0        0     4498 2023-04-05 07:20:58.614422 colrev-0.8.2/README.md
--rw-r--r--   0        0        0      314 2023-04-05 07:20:58.614422 colrev-0.8.2/colrev/__init__.py
--rw-r--r--   0        0        0      128 2023-04-05 07:20:58.614422 colrev-0.8.2/colrev/__version__.py
--rw-r--r--   0        0        0    30842 2023-04-05 07:20:58.614422 colrev-0.8.2/colrev/advisor.py
--rw-r--r--   0        0        0    31724 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/checker.py
--rw-r--r--   0        0        0    44602 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/dataset.py
--rw-r--r--   0        0        0      105 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/__init__.py
--rw-r--r--   0        0        0    13523 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/environment_manager.py
--rw-r--r--   0        0        0     2281 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/grobid_service.py
--rw-r--r--   0        0        0     3619 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/language_service.py
--rw-r--r--   0        0        0    51292 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/local_index.py
--rw-r--r--   0        0        0    40166 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/package_manager.py
--rw-r--r--   0        0        0     2070 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/pdf_hash_service.py
--rw-r--r--   0        0        0     2308 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/resources.py
--rw-r--r--   0        0        0     3971 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/screenshot_service.py
--rw-r--r--   0        0        0    35182 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/tei_parser.py
--rw-r--r--   0        0        0     4665 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/utils.py
--rw-r--r--   0        0        0     2564 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/env/zotero_translation_service.py
--rw-r--r--   0        0        0    16807 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/exceptions.py
--rw-r--r--   0        0        0      151 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/exit_codes.py
--rw-r--r--   0        0        0       86 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/hooks/__init__.py
--rwxr-xr-x   0        0        0      352 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/hooks/check.py
--rwxr-xr-x   0        0        0      391 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/hooks/format.py
--rwxr-xr-x   0        0        0      468 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/hooks/report.py
--rwxr-xr-x   0        0        0      360 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/hooks/share.py
--rw-r--r--   0        0        0     3129 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/logger.py
--rw-r--r--   0        0        0     7802 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/operation.py
--rw-r--r--   0        0        0       92 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/__init__.py
--rw-r--r--   0        0        0      119 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/__init__.py
--rw-r--r--   0        0        0      135 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/__init__.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/bibliography_export.md
--rw-r--r--   0        0        0     9249 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/bibliography_export.py
--rw-r--r--   0        0        0     1084 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/colrev_curation.md
--rw-r--r--   0        0        0    14317 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/colrev_curation.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/github_pages.md
--rw-r--r--   0        0        0     9666 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/github_pages.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/obsidian.md
--rw-r--r--   0        0        0     9287 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/obsidian.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/paper_md.md
--rw-r--r--   0        0        0    31776 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/paper_md.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/prisma.md
--rw-r--r--   0        0        0     9374 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/prisma.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/structured.md
--rw-r--r--   0        0        0    11144 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/data/structured.py
--rw-r--r--   0        0        0      126 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/__init__.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/active_learning_dedup_io.md
--rw-r--r--   0        0        0    39873 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/active_learning_dedup_io.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/curation_dedupe.md
--rw-r--r--   0        0        0    25065 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/curation_dedupe.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/curation_missing_dedupe.md
--rw-r--r--   0        0        0    14175 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/curation_missing_dedupe.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/simple_dedupe.md
--rw-r--r--   0        0        0    14284 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/simple_dedupe.py
--rw-r--r--   0        0        0     1999 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/dedupe/utils.py
--rw-r--r--   0        0        0      135 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/load_conversion/__init__.py
--rw-r--r--   0        0        0      189 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/load_conversion/bib_pybtex_loader.md
--rw-r--r--   0        0        0     5404 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/load_conversion/bib_pybtex_loader.py
--rw-r--r--   0        0        0      189 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/load_conversion/bibutils_loader.md
--rw-r--r--   0        0        0     4481 2023-04-05 07:20:58.618422 colrev-0.8.2/colrev/ops/built_in/load_conversion/bibutils_loader.py
--rw-r--r--   0        0        0      189 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/markdown_loader.md
--rw-r--r--   0        0        0     2970 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/markdown_loader.py
--rw-r--r--   0        0        0      189 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/table_loader.md
--rw-r--r--   0        0        0     8838 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/table_loader.py
--rw-r--r--   0        0        0      189 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/zotero_loader.md
--rw-r--r--   0        0        0     3477 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/load_conversion/zotero_loader.py
--rw-r--r--   0        0        0      127 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/__init__.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/local_index_pdf_get.md
--rw-r--r--   0        0        0     2583 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/local_index_pdf_get.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/unpaywall.md
--rw-r--r--   0        0        0     4836 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/unpaywall.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/website_screenshot.md
--rw-r--r--   0        0        0     1886 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get/website_screenshot.py
--rw-r--r--   0        0        0      131 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get_man/__init__.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.md
--rw-r--r--   0        0        0    11024 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.py
--rw-r--r--   0        0        0      128 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/__init__.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/check_ocr.md
--rw-r--r--   0        0        0     5121 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/check_ocr.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/completeness_validation.md
--rw-r--r--   0        0        0     7043 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/completeness_validation.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/cover_page.md
--rw-r--r--   0        0        0     7699 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/cover_page.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/last_page.md
--rw-r--r--   0        0        0     5341 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/last_page.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/metadata_validation.md
--rw-r--r--   0        0        0     6694 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/metadata_validation.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/tei_prep.md
--rw-r--r--   0        0        0     2285 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep/tei_prep.py
--rw-r--r--   0        0        0      132 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep_man/__init__.py
--rw-r--r--   0        0        0      167 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.md
--rw-r--r--   0        0        0    10279 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.py
--rw-r--r--   0        0        0      124 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/__init__.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/bibtex_crossref_resolution.md
--rw-r--r--   0        0        0     2838 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/bibtex_crossref_resolution.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/citeas_prep.md
--rw-r--r--   0        0        0     4780 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/citeas_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/crossref_metadata_prep.md
--rw-r--r--   0        0        0     2662 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/crossref_metadata_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/curation_prep.md
--rw-r--r--   0        0        0     2826 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/curation_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/dblp_metadata_prep.md
--rw-r--r--   0        0        0     2116 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/dblp_metadata_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/doi_from_urls_prep.md
--rw-r--r--   0        0        0     4196 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/doi_from_urls_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/doi_metadata_prep.md
--rw-r--r--   0        0        0     2140 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/doi_metadata_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/europe_pmc_prep.md
--rw-r--r--   0        0        0     1880 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/europe_pmc_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_collections.md
--rw-r--r--   0        0        0     1612 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_collections.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_complementary_materials.md
--rw-r--r--   0        0        0     2464 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_complementary_materials.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_languages.md
--rw-r--r--   0        0        0     5530 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_languages.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_non_latin_alphabets.md
--rw-r--r--   0        0        0     2562 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/exclude_non_latin_alphabets.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/general_polish.md
--rw-r--r--   0        0        0     2180 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/general_polish.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/global_id_consistency.md
--rw-r--r--   0        0        0     6013 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/global_id_consistency.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/local_index_prep.md
--rw-r--r--   0        0        0     2608 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/local_index_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/open_library_prep.md
--rw-r--r--   0        0        0     2237 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/open_library_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/pubmed_metadata_prep.md
--rw-r--r--   0        0        0     2497 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/pubmed_metadata_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/remove_broken_ids.md
--rw-r--r--   0        0        0     2504 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/remove_broken_ids.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/remove_error500_urls.md
--rw-r--r--   0        0        0     2507 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/remove_error500_urls.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/semantic_scholar_prep.md
--rw-r--r--   0        0        0     7170 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/semantic_scholar_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/source_specific_prep.md
--rw-r--r--   0        0        0     3119 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/source_specific_prep.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/update_masterdata_status.md
--rw-r--r--   0        0        0     1510 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/update_masterdata_status.py
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/year_vol_iss_prep.md
--rw-r--r--   0        0        0     8513 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep/year_vol_iss_prep.py
--rw-r--r--   0        0        0      128 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep_man/__init__.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.md
--rw-r--r--   0        0        0     1983 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.py
--rw-r--r--   0        0        0      161 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep_man/prep_man_export.md
--rw-r--r--   0        0        0     9001 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prep_man/prep_man_export.py
--rw-r--r--   0        0        0      129 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/__init__.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/asreview.md
--rw-r--r--   0        0        0     9888 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/asreview.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/conditional_prescreen.md
--rw-r--r--   0        0        0     2128 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/conditional_prescreen.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_cli.md
--rw-r--r--   0        0        0     5142 2023-04-05 07:20:58.622423 colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_cli.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_table.md
--rw-r--r--   0        0        0     9636 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_table.py
--rw-r--r--   0        0        0      165 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/prescreen/scope_prescreen.md
--rw-r--r--   0        0        0     8803 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/prescreen/scope_prescreen.py
--rw-r--r--   0        0        0      132 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/__init__.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/conceptual_review.md
--rw-r--r--   0        0        0     1296 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/conceptual_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/critical_review.md
--rw-r--r--   0        0        0     1349 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/critical_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/curated_masterdata.md
--rw-r--r--   0        0        0     4705 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/curated_masterdata.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/descriptive_review.md
--rw-r--r--   0        0        0     1363 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/descriptive_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/literature_review.md
--rw-r--r--   0        0        0     1312 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/literature_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/meta_analysis.md
--rw-r--r--   0        0        0     1845 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/meta_analysis.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/narrative_review.md
--rw-r--r--   0        0        0     1291 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/narrative_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/qualitative_systematic_review.md
--rw-r--r--   0        0        0     1924 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/qualitative_systematic_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/scientometric.md
--rw-r--r--   0        0        0     1378 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/scientometric.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/scoping_review.md
--rw-r--r--   0        0        0     1483 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/scoping_review.py
--rw-r--r--   0        0        0      511 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/theoretical_review.md
--rw-r--r--   0        0        0     1442 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/review_types/theoretical_review.py
--rw-r--r--   0        0        0      126 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/__init__.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/screen_cli.md
--rw-r--r--   0        0        0     9272 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/screen_cli.py
--rw-r--r--   0        0        0      159 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/screen_table.md
--rw-r--r--   0        0        0     8641 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/screen_table.py
--rw-r--r--   0        0        0     2703 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/screen/utils.py
--rw-r--r--   0        0        0      133 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/__init__.py
--rw-r--r--   0        0        0      425 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/abi_inform_proquest.md
--rw-r--r--   0        0        0     4484 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/abi_inform_proquest.py
--rw-r--r--   0        0        0      377 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/acm_digital_library.md
--rw-r--r--   0        0        0     4017 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/acm_digital_library.py
--rw-r--r--   0        0        0      376 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/aisel.md
--rw-r--r--   0        0        0    21127 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/aisel.py
--rw-r--r--   0        0        0      333 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/colrev_project.md
--rw-r--r--   0        0        0     7702 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/colrev_project.py
--rw-r--r--   0        0        0      372 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/crossref.md
--rw-r--r--   0        0        0    34871 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/crossref.py
--rw-r--r--   0        0        0      360 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/dblp.md
--rw-r--r--   0        0        0    30401 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/dblp.py
--rw-r--r--   0        0        0     6286 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/doi_org.py
--rw-r--r--   0        0        0      377 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/ebsco_host.md
--rw-r--r--   0        0        0     3164 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/ebsco_host.py
--rw-r--r--   0        0        0      363 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/eric.md
--rw-r--r--   0        0        0     3642 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/eric.py
--rw-r--r--   0        0        0      371 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/europe_pmc.md
--rw-r--r--   0        0        0    17820 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/europe_pmc.py
--rw-r--r--   0        0        0      378 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/google_scholar.md
--rw-r--r--   0        0        0     5030 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/google_scholar.py
--rw-r--r--   0        0        0      377 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/ieee.md
--rw-r--r--   0        0        0     3929 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/ieee.py
--rw-r--r--   0        0        0      366 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/jstor.md
--rw-r--r--   0        0        0     3741 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/jstor.py
--rw-r--r--   0        0        0      333 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/local_index.md
--rw-r--r--   0        0        0    36485 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/local_index.py
--rw-r--r--   0        0        0      378 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/open_citations_forward_search.md
--rw-r--r--   0        0        0     9902 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/open_citations_forward_search.py
--rw-r--r--   0        0        0      374 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/open_library.md
--rw-r--r--   0        0        0    10046 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/open_library.py
--rw-r--r--   0        0        0      388 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/pdf_backward_search.md
--rw-r--r--   0        0        0    11442 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/pdf_backward_search.py
--rw-r--r--   0        0        0      388 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/pdfs_dir.md
--rw-r--r--   0        0        0    29429 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/pdfs_dir.py
--rw-r--r--   0        0        0      390 2023-04-05 07:20:58.626423 colrev-0.8.2/colrev/ops/built_in/search_sources/psycinfo.md
--rw-r--r--   0        0        0     3684 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/psycinfo.py
--rw-r--r--   0        0        0      377 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/pubmed.md
--rw-r--r--   0        0        0    27882 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/pubmed.py
--rw-r--r--   0        0        0      366 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/scopus.md
--rw-r--r--   0        0        0     5355 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/scopus.py
--rw-r--r--   0        0        0      377 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/springer_link.md
--rw-r--r--   0        0        0     5947 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/springer_link.py
--rw-r--r--   0        0        0      433 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/systematic_review_datasets.md
--rw-r--r--   0        0        0     4822 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/systematic_review_datasets.py
--rw-r--r--   0        0        0      385 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/taylor_and_francis.md
--rw-r--r--   0        0        0     3231 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/taylor_and_francis.py
--rw-r--r--   0        0        0      364 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/trid.md
--rw-r--r--   0        0        0     3975 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/trid.py
--rw-r--r--   0        0        0      333 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/unknown_source.md
--rw-r--r--   0        0        0    13639 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/unknown_source.py
--rw-r--r--   0        0        0     6682 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/utils.py
--rw-r--r--   0        0        0      333 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/video_dir.md
--rw-r--r--   0        0        0     6426 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/video_dir.py
--rw-r--r--   0        0        0      383 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/web_of_science.md
--rw-r--r--   0        0        0     4720 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/web_of_science.py
--rw-r--r--   0        0        0     5592 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/website.py
--rw-r--r--   0        0        0      376 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/wiley.md
--rw-r--r--   0        0        0     3776 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/built_in/search_sources/wiley.py
--rw-r--r--   0        0        0     1472 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/clone.py
--rw-r--r--   0        0        0     9104 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/commit.py
--rw-r--r--   0        0        0     7310 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/correct.py
--rw-r--r--   0        0        0    14206 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/data.py
--rw-r--r--   0        0        0    39086 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/dedupe.py
--rw-r--r--   0        0        0     4937 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/distribute.py
--rw-r--r--   0        0        0    16525 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/init.py
--rw-r--r--   0        0        0    42744 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/load.py
--rw-r--r--   0        0        0     9324 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/merge.py
--rw-r--r--   0        0        0    26016 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/pdf_get.py
--rw-r--r--   0        0        0     7879 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/pdf_get_man.py
--rw-r--r--   0        0        0    18096 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/pdf_prep.py
--rw-r--r--   0        0        0    13404 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/pdf_prep_man.py
--rw-r--r--   0        0        0    39684 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/prep.py
--rw-r--r--   0        0        0    11171 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/prep_man.py
--rw-r--r--   0        0        0    12576 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/prescreen.py
--rw-r--r--   0        0        0     1728 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/pull.py
--rw-r--r--   0        0        0     5748 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/push.py
--rw-r--r--   0        0        0     2329 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/remove.py
--rw-r--r--   0        0        0    17173 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/repare.py
--rw-r--r--   0        0        0     1126 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/review_types.py
--rw-r--r--   0        0        0    15726 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/screen.py
--rw-r--r--   0        0        0    22433 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/search.py
--rw-r--r--   0        0        0     1650 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/search_sources.py
--rwxr-xr-x   0        0        0    22158 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/status.py
--rw-r--r--   0        0        0     8944 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/sync.py
--rw-r--r--   0        0        0     4470 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/trace.py
--rw-r--r--   0        0        0    10863 2023-04-05 07:20:58.630423 colrev-0.8.2/colrev/ops/upgrade.py
--rw-r--r--   0        0        0    21848 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/ops/validate.py
--rw-r--r--   0        0        0        0 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/py.typed
--rw-r--r--   0        0        0      104 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/readme.md
--rw-r--r--   0        0        0   114141 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/record.py
--rw-r--r--   0        0        0    25155 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/review_manager.py
--rw-r--r--   0        0        0    11405 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/service.py
--rw-r--r--   0        0        0    19647 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/settings.py
--rw-r--r--   0        0        0     1882 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_data_script.py
--rw-r--r--   0        0        0     1157 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_pdf_get_script.py
--rw-r--r--   0        0        0     1418 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_pdf_prep_script.py
--rw-r--r--   0        0        0     1566 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_prep_script.py
--rw-r--r--   0        0        0     1882 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_prescreen_script.py
--rw-r--r--   0        0        0     2398 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_screen_script.py
--rw-r--r--   0        0        0     3301 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/custom_scripts/custom_search_source_script.py
--rw-r--r--   0        0        0    15707 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/example/30_example_records.bib
--rw-r--r--   0        0        0      155 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/github_pages/_config.yml
--rw-r--r--   0        0        0       73 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/github_pages/about.md
--rw-r--r--   0        0        0     4953 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/github_pages/index.html
--rw-r--r--   0        0        0    18650 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/LICENSE-CC-BY-4.0.txt
--rw-r--r--   0        0        0     1752 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/colrev_update.yml
--rw-r--r--   0        0        0     1537 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/colrev_update_curation.yml
--rw-r--r--   0        0        0       54 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/gitattributes
--rw-r--r--   0        0        0       85 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/markdownlint.yaml
--rw-r--r--   0        0        0     1068 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/pre-commit-config.yaml
--rw-r--r--   0        0        0      480 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/pre-commit.yml
--rw-r--r--   0        0        0      282 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/readme.md
--rw-r--r--   0        0        0     5280 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/init/settings.json
--rw-r--r--   0        0        0      930 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/commit_report_details.txt
--rw-r--r--   0        0        0      271 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/commit_report_header.txt
--rw-r--r--   0        0        0      352 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/complementary_material_keywords.txt
--rw-r--r--   0        0        0      318 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/complementary_material_strings.txt
--rw-r--r--   0        0        0      494 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/masterdata_curations.csv
--rw-r--r--   0        0        0      462 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/pdf_get_man_mail.txt
--rw-r--r--   0        0        0    76341 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/predatory_journals_beall.csv
--rw-r--r--   0        0        0     2729 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/prep_man_curation.ipynb
--rw-r--r--   0        0        0     3830 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/ops/status.txt
--rw-r--r--   0        0        0    60690 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/package_endpoints.json
--rw-r--r--   0        0        0    12325 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/package_status.json
--rw-r--r--   0        0        0       94 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/packages.json
--rw-r--r--   0        0        0    25233 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/paper_md/APA-7.docx
--rw-r--r--   0        0        0      381 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/paper_md/non_sample_references.bib
--rw-r--r--   0        0        0      673 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/paper_md/paper.md
--rw-r--r--   0        0        0     4935 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/prisma/PRISMA.csv
--rw-r--r--   0        0        0     5108 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/prisma/PRISMA_original.csv
--rw-r--r--   0        0        0      872 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/prisma/prisma-refs.bib
--rw-r--r--   0        0        0      262 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/prisma/prisma_text.md
--rw-r--r--   0        0        0     1506 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/review_type/curated_masterdata/curations_github_colrev_update.yml
--rw-r--r--   0        0        0      460 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/review_type/curated_masterdata/readme.md
--rw-r--r--   0        0        0      586 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/template/review_type/meta_analysis/paper.md
--rw-r--r--   0        0        0      104 2023-04-05 07:20:58.634423 colrev-0.8.2/colrev/ui_cli/__init__.py
--rw-r--r--   0        0        0     5555 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/add_packages.py
--rw-r--r--   0        0        0    75563 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/cli.py
--rw-r--r--   0        0        0      146 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/cli_colors.py
--rw-r--r--   0        0        0     9090 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/cli_status_printer.py
--rw-r--r--   0        0        0     7530 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/cli_validation.py
--rw-r--r--   0        0        0     2891 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_cli/show_printer.py
--rw-r--r--   0        0        0      337 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/.gitignore
--rw-r--r--   0        0        0     2160 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/README.md
--rw-r--r--   0        0        0      100 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/__init__.py
--rw-r--r--   0        0        0      518 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/favicon.ico
--rw-r--r--   0        0        0      638 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/index.html
--rw-r--r--   0        0        0     5347 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/logo192.png
--rw-r--r--   0        0        0     9664 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/logo512.png
--rw-r--r--   0        0        0      492 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/manifest.json
--rw-r--r--   0        0        0       67 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/robots.txt
--rw-r--r--   0        0        0   198854 2023-04-05 07:20:58.638423 colrev-0.8.2/colrev/ui_web/build/static/css/main.2b978a68.css
--rw-r--r--   0        0        0   482091 2023-04-05 07:20:58.642423 colrev-0.8.2/colrev/ui_web/build/static/css/main.2b978a68.css.map
--rw-r--r--   0        0        0     4604 2023-04-05 07:20:58.642423 colrev-0.8.2/colrev/ui_web/build/static/js/787.87f1ca01.chunk.js
--rw-r--r--   0        0        0    10282 2023-04-05 07:20:58.642423 colrev-0.8.2/colrev/ui_web/build/static/js/787.87f1ca01.chunk.js.map
--rw-r--r--   0        0        0   328609 2023-04-05 07:20:58.642423 colrev-0.8.2/colrev/ui_web/build/static/js/main.b6a12663.js
--rw-r--r--   0        0        0     1572 2023-04-05 07:20:58.642423 colrev-0.8.2/colrev/ui_web/build/static/js/main.b6a12663.js.LICENSE.txt
--rw-r--r--   0        0        0  1257869 2023-04-05 07:20:58.650424 colrev-0.8.2/colrev/ui_web/build/static/js/main.b6a12663.js.map
--rw-r--r--   0        0        0  1044369 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/package-lock.json
--rw-r--r--   0        0        0     1118 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/package.json
--rw-r--r--   0        0        0     3870 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/favicon.ico
--rw-r--r--   0        0        0     1766 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/index.html
--rw-r--r--   0        0        0     5347 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/logo192.png
--rw-r--r--   0        0        0     9664 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/logo512.png
--rw-r--r--   0        0        0      492 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/manifest.json
--rw-r--r--   0        0        0       67 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/public/robots.txt
--rw-r--r--   0        0        0     4975 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/settings_editor.py
--rw-r--r--   0        0        0       54 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/App.css
--rw-r--r--   0        0        0      273 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/App.test.tsx
--rw-r--r--   0        0        0      430 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/App.tsx
--rw-r--r--   0        0        0      212 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/common/Expander.tsx
--rw-r--r--   0        0        0     1523 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/common/ExpanderItem.tsx
--rw-r--r--   0        0        0     2434 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/common/ModalWindow.tsx
--rw-r--r--   0        0        0      577 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/common/icons/DeleteIcon.tsx
--rw-r--r--   0        0        0      726 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/common/icons/EditIcon.tsx
--rw-r--r--   0        0        0      805 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/data/DataEditor.tsx
--rw-r--r--   0        0        0     1911 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/dedupe/DedupeEditor.tsx
--rw-r--r--   0        0        0     1690 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/fields/FieldsEditor.tsx
--rw-r--r--   0        0        0     4091 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/packages/PackageEditWizard.tsx
--rw-r--r--   0        0        0     8162 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/packages/PackageParametersEditor.tsx
--rw-r--r--   0        0        0      485 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/packages/PackageTitle.tsx
--rw-r--r--   0        0        0     3316 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/packages/PackagesEditor.tsx
--rw-r--r--   0        0        0    12053 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/pages/SettingsEditor.tsx
--rw-r--r--   0        0        0       92 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/pages/Test.tsx
--rw-r--r--   0        0        0     4188 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/pdf/PdfGetEditor.tsx
--rw-r--r--   0        0        0     2167 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/pdf/PdfPrepEditor.tsx
--rw-r--r--   0        0        0     4532 2023-04-05 07:20:58.654424 colrev-0.8.2/colrev/ui_web/src/components/prep/PrepEditor.tsx
--rw-r--r--   0        0        0     1373 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/prescreen/PrescreenEditor.tsx
--rw-r--r--   0        0        0     5347 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/project/AuthorsEditor.tsx
--rw-r--r--   0        0        0     4891 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/project/ProjectEditor.tsx
--rw-r--r--   0        0        0     5991 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/screen/ScreenEditor.tsx
--rw-r--r--   0        0        0     1175 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/search/SearchEditor.tsx
--rw-r--r--   0        0        0      561 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/components/sources/SourcesEditor.tsx
--rw-r--r--   0        0        0       49 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/config.json
--rw-r--r--   0        0        0      366 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/index.css
--rw-r--r--   0        0        0      695 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/index.tsx
--rw-r--r--   0        0        0     2633 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/logo.svg
--rw-r--r--   0        0        0      323 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/author.ts
--rw-r--r--   0        0        0      104 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/data.ts
--rw-r--r--   0        0        0      147 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/dedupe.ts
--rw-r--r--   0        0        0      456 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/package.ts
--rw-r--r--   0        0        0      143 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/packageDefinition.ts
--rw-r--r--   0        0        0      411 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/packageParameterDefinition.ts
--rw-r--r--   0        0        0      186 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/packageParameterType.ts
--rw-r--r--   0        0        0      285 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/pdfGet.ts
--rw-r--r--   0        0        0      197 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/pdfPrep.ts
--rw-r--r--   0        0        0      228 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/prep.ts
--rw-r--r--   0        0        0      174 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/prepRound.ts
--rw-r--r--   0        0        0      145 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/prescreen.ts
--rw-r--r--   0        0        0      373 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/project.ts
--rw-r--r--   0        0        0      242 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/screen.ts
--rw-r--r--   0        0        0      186 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/screenCriteria.ts
--rw-r--r--   0        0        0       81 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/search.ts
--rw-r--r--   0        0        0      769 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/models/settings.ts
--rw-r--r--   0        0        0       41 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/reportWebVitals.ts
--rw-r--r--   0        0        0      644 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/dataSectionDataSerice.ts
--rw-r--r--   0        0        0     8278 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/dataService.ts
--rw-r--r--   0        0        0      789 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/dedupeDataService.ts
--rw-r--r--   0        0        0      408 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/httpService.ts
--rw-r--r--   0        0        0     2162 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/packageDataService.ts
--rw-r--r--   0        0        0     2221 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/pdfDataService.ts
--rw-r--r--   0        0        0     1529 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/prepDataService.ts
--rw-r--r--   0        0        0      820 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/prescreenDataService.ts
--rw-r--r--   0        0        0     1113 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/projectDataService.ts
--rw-r--r--   0        0        0     1673 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/screenDataService.ts
--rw-r--r--   0        0        0      483 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/services/searchDataService.ts
--rw-r--r--   0        0        0      241 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/src/setupTests.ts
--rw-r--r--   0        0        0      561 2023-04-05 07:20:58.658424 colrev-0.8.2/colrev/ui_web/tsconfig.json
--rw-r--r--   0        0        0     2769 2023-04-05 07:20:58.682425 colrev-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     7506 1970-01-01 00:00:00.000000 colrev-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     8240 2023-04-23 07:21:47.573349 colrev-0.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3322 2023-04-23 07:21:47.573349 colrev-0.8.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1070 2023-04-23 07:21:47.573349 colrev-0.8.3/LICENSE
+-rw-r--r--   0        0        0     4729 2023-04-23 07:21:47.573349 colrev-0.8.3/README.md
+-rw-r--r--   0        0        0      314 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/__init__.py
+-rw-r--r--   0        0        0      128 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/__version__.py
+-rw-r--r--   0        0        0    31610 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/advisor.py
+-rw-r--r--   0        0        0    31965 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/checker.py
+-rw-r--r--   0        0        0    44778 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/dataset.py
+-rw-r--r--   0        0        0      105 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/__init__.py
+-rw-r--r--   0        0        0    13575 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/environment_manager.py
+-rw-r--r--   0        0        0     2355 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/grobid_service.py
+-rw-r--r--   0        0        0     3695 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/language_service.py
+-rw-r--r--   0        0        0    52628 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/local_index.py
+-rw-r--r--   0        0        0    39359 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/package_manager.py
+-rw-r--r--   0        0        0     2308 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/resources.py
+-rw-r--r--   0        0        0     3971 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/screenshot_service.py
+-rw-r--r--   0        0        0    35435 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/tei_parser.py
+-rw-r--r--   0        0        0     4696 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/utils.py
+-rw-r--r--   0        0        0     2564 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/env/zotero_translation_service.py
+-rw-r--r--   0        0        0    16896 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/exceptions.py
+-rw-r--r--   0        0        0      151 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/exit_codes.py
+-rw-r--r--   0        0        0       86 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/hooks/__init__.py
+-rwxr-xr-x   0        0        0      352 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/hooks/check.py
+-rwxr-xr-x   0        0        0      391 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/hooks/format.py
+-rwxr-xr-x   0        0        0      468 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/hooks/report.py
+-rwxr-xr-x   0        0        0      360 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/hooks/share.py
+-rw-r--r--   0        0        0     1903 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/linter/colrev_lint.py
+-rw-r--r--   0        0        0      310 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/linter/readme.md
+-rw-r--r--   0        0        0     3129 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/logger.py
+-rw-r--r--   0        0        0     7802 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/operation.py
+-rw-r--r--   0        0        0       92 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/ops/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/ops/built_in/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/ops/built_in/data/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/ops/built_in/data/bibliography_export.md
+-rw-r--r--   0        0        0     9291 2023-04-23 07:21:47.573349 colrev-0.8.3/colrev/ops/built_in/data/bibliography_export.py
+-rw-r--r--   0        0        0     1084 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/colrev_curation.md
+-rw-r--r--   0        0        0    14501 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/colrev_curation.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/github_pages.md
+-rw-r--r--   0        0        0    13511 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/github_pages.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/obsidian.md
+-rw-r--r--   0        0        0     9253 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/obsidian.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/paper_md.md
+-rw-r--r--   0        0        0    31713 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/paper_md.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/prisma.md
+-rw-r--r--   0        0        0     9301 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/prisma.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/structured.md
+-rw-r--r--   0        0        0    11323 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/data/structured.py
+-rw-r--r--   0        0        0      126 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/active_learning_dedup_io.md
+-rw-r--r--   0        0        0    42848 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/active_learning_dedup_io.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/curation_dedupe.md
+-rw-r--r--   0        0        0    25576 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/curation_dedupe.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/curation_missing_dedupe.md
+-rw-r--r--   0        0        0    14416 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/curation_missing_dedupe.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/simple_dedupe.md
+-rw-r--r--   0        0        0    14320 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/simple_dedupe.py
+-rw-r--r--   0        0        0     1999 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/dedupe/utils.py
+-rw-r--r--   0        0        0      135 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/bib_pybtex_loader.md
+-rw-r--r--   0        0        0     5404 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/bib_pybtex_loader.py
+-rw-r--r--   0        0        0      189 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/bibutils_loader.md
+-rw-r--r--   0        0        0     4481 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/bibutils_loader.py
+-rw-r--r--   0        0        0      189 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/markdown_loader.md
+-rw-r--r--   0        0        0     2970 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/markdown_loader.py
+-rw-r--r--   0        0        0      189 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/table_loader.md
+-rw-r--r--   0        0        0     8928 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/table_loader.py
+-rw-r--r--   0        0        0      189 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/zotero_loader.md
+-rw-r--r--   0        0        0     3477 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/load_conversion/zotero_loader.py
+-rw-r--r--   0        0        0      127 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/local_index_pdf_get.md
+-rw-r--r--   0        0        0     2583 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/local_index_pdf_get.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/unpaywall.md
+-rw-r--r--   0        0        0     4836 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/unpaywall.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/website_screenshot.md
+-rw-r--r--   0        0        0     1885 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get/website_screenshot.py
+-rw-r--r--   0        0        0      131 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get_man/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.md
+-rw-r--r--   0        0        0    11024 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.py
+-rw-r--r--   0        0        0      128 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/check_ocr.md
+-rw-r--r--   0        0        0     5323 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/check_ocr.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/completeness_validation.md
+-rw-r--r--   0        0        0     7043 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/completeness_validation.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/cover_page.md
+-rw-r--r--   0        0        0     8028 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/cover_page.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/last_page.md
+-rw-r--r--   0        0        0     5067 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/last_page.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/metadata_validation.md
+-rw-r--r--   0        0        0     6614 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/metadata_validation.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/tei_prep.md
+-rw-r--r--   0        0        0     2285 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep/tei_prep.py
+-rw-r--r--   0        0        0      132 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep_man/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.md
+-rw-r--r--   0        0        0    10197 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.py
+-rw-r--r--   0        0        0      124 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/bibtex_crossref_resolution.md
+-rw-r--r--   0        0        0     2838 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/bibtex_crossref_resolution.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/citeas_prep.md
+-rw-r--r--   0        0        0     4701 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/citeas_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/crossref_metadata_prep.md
+-rw-r--r--   0        0        0     2583 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/crossref_metadata_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/curation_prep.md
+-rw-r--r--   0        0        0     2748 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/curation_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/dblp_metadata_prep.md
+-rw-r--r--   0        0        0     2037 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/dblp_metadata_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/doi_from_urls_prep.md
+-rw-r--r--   0        0        0     4117 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/doi_from_urls_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/doi_metadata_prep.md
+-rw-r--r--   0        0        0     2061 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/doi_metadata_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/europe_pmc_prep.md
+-rw-r--r--   0        0        0     1801 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/europe_pmc_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_collections.md
+-rw-r--r--   0        0        0     1612 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_collections.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_complementary_materials.md
+-rw-r--r--   0        0        0     2385 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_complementary_materials.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_languages.md
+-rw-r--r--   0        0        0     5919 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_languages.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_non_latin_alphabets.md
+-rw-r--r--   0        0        0     2483 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/exclude_non_latin_alphabets.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/general_polish.md
+-rw-r--r--   0        0        0     2180 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/general_polish.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/global_id_consistency.md
+-rw-r--r--   0        0        0     5936 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/global_id_consistency.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/local_index_prep.md
+-rw-r--r--   0        0        0     2529 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/local_index_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/open_library_prep.md
+-rw-r--r--   0        0        0     2158 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/open_library_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/pubmed_metadata_prep.md
+-rw-r--r--   0        0        0     2418 2023-04-23 07:21:47.577349 colrev-0.8.3/colrev/ops/built_in/prep/pubmed_metadata_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/remove_broken_ids.md
+-rw-r--r--   0        0        0     2504 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/remove_broken_ids.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/remove_error500_urls.md
+-rw-r--r--   0        0        0     2408 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/remove_error500_urls.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/semantic_scholar_prep.md
+-rw-r--r--   0        0        0     7091 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/semantic_scholar_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/source_specific_prep.md
+-rw-r--r--   0        0        0     3073 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/source_specific_prep.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/update_masterdata_status.md
+-rw-r--r--   0        0        0     1510 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/update_masterdata_status.py
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/year_vol_iss_prep.md
+-rw-r--r--   0        0        0     7850 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep/year_vol_iss_prep.py
+-rw-r--r--   0        0        0      128 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep_man/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.md
+-rw-r--r--   0        0        0     1983 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.py
+-rw-r--r--   0        0        0      161 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep_man/prep_man_export.md
+-rw-r--r--   0        0        0     9070 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prep_man/prep_man_export.py
+-rw-r--r--   0        0        0      129 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/asreview.md
+-rw-r--r--   0        0        0     9888 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/asreview.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/conditional_prescreen.md
+-rw-r--r--   0        0        0     2128 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/conditional_prescreen.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_cli.md
+-rw-r--r--   0        0        0     5142 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_cli.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_table.md
+-rw-r--r--   0        0        0     9738 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_table.py
+-rw-r--r--   0        0        0      165 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/scope_prescreen.md
+-rw-r--r--   0        0        0     9071 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/prescreen/scope_prescreen.py
+-rw-r--r--   0        0        0      132 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/__init__.py
+-rw-r--r--   0        0        0      509 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/conceptual_review.md
+-rw-r--r--   0        0        0     1296 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/conceptual_review.py
+-rw-r--r--   0        0        0      507 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/critical_review.md
+-rw-r--r--   0        0        0     1349 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/critical_review.py
+-rw-r--r--   0        0        0     1141 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/curated_masterdata.md
+-rw-r--r--   0        0        0     4705 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/curated_masterdata.py
+-rw-r--r--   0        0        0      510 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/descriptive_review.md
+-rw-r--r--   0        0        0     1363 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/descriptive_review.py
+-rw-r--r--   0        0        0      509 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/literature_review.md
+-rw-r--r--   0        0        0     1312 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/literature_review.py
+-rw-r--r--   0        0        0      704 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/meta_analysis.md
+-rw-r--r--   0        0        0     1845 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/meta_analysis.py
+-rw-r--r--   0        0        0      508 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/narrative_review.md
+-rw-r--r--   0        0        0     1291 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/narrative_review.py
+-rw-r--r--   0        0        0      521 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/qualitative_systematic_review.md
+-rw-r--r--   0        0        0     1924 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/qualitative_systematic_review.py
+-rw-r--r--   0        0        0      633 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/scientometric.md
+-rw-r--r--   0        0        0     1378 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/scientometric.py
+-rw-r--r--   0        0        0      506 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/scoping_review.md
+-rw-r--r--   0        0        0     1483 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/scoping_review.py
+-rw-r--r--   0        0        0      510 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/theoretical_review.md
+-rw-r--r--   0        0        0     1442 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/review_types/theoretical_review.py
+-rw-r--r--   0        0        0      126 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/screen_cli.md
+-rw-r--r--   0        0        0     9915 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/screen_cli.py
+-rw-r--r--   0        0        0      159 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/screen_table.md
+-rw-r--r--   0        0        0     8939 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/screen_table.py
+-rw-r--r--   0        0        0     2703 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/screen/utils.py
+-rw-r--r--   0        0        0      133 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/__init__.py
+-rw-r--r--   0        0        0      425 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/abi_inform_proquest.md
+-rw-r--r--   0        0        0     4484 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/abi_inform_proquest.py
+-rw-r--r--   0        0        0      377 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/acm_digital_library.md
+-rw-r--r--   0        0        0     4017 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/acm_digital_library.py
+-rw-r--r--   0        0        0      376 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/aisel.md
+-rw-r--r--   0        0        0    19905 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/aisel.py
+-rw-r--r--   0        0        0      333 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/colrev_project.md
+-rw-r--r--   0        0        0     7702 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/colrev_project.py
+-rw-r--r--   0        0        0      372 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/crossref.md
+-rw-r--r--   0        0        0    35337 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/crossref.py
+-rw-r--r--   0        0        0      360 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/dblp.md
+-rw-r--r--   0        0        0    30401 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/dblp.py
+-rw-r--r--   0        0        0     6286 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/doi_org.py
+-rw-r--r--   0        0        0      377 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/ebsco_host.md
+-rw-r--r--   0        0        0     3164 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/ebsco_host.py
+-rw-r--r--   0        0        0      363 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/eric.md
+-rw-r--r--   0        0        0     3642 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/eric.py
+-rw-r--r--   0        0        0      371 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/europe_pmc.md
+-rw-r--r--   0        0        0    17728 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/europe_pmc.py
+-rw-r--r--   0        0        0      378 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/google_scholar.md
+-rw-r--r--   0        0        0     5030 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/google_scholar.py
+-rw-r--r--   0        0        0      377 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/ieee.md
+-rw-r--r--   0        0        0     3929 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/ieee.py
+-rw-r--r--   0        0        0      366 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/jstor.md
+-rw-r--r--   0        0        0     3741 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/jstor.py
+-rw-r--r--   0        0        0      333 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/local_index.md
+-rw-r--r--   0        0        0    36650 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/local_index.py
+-rw-r--r--   0        0        0      378 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/open_citations_forward_search.md
+-rw-r--r--   0        0        0     9915 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/open_citations_forward_search.py
+-rw-r--r--   0        0        0      374 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/open_library.md
+-rw-r--r--   0        0        0    11328 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/open_library.py
+-rw-r--r--   0        0        0      388 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/pdf_backward_search.md
+-rw-r--r--   0        0        0    11442 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/pdf_backward_search.py
+-rw-r--r--   0        0        0      388 2023-04-23 07:21:47.581349 colrev-0.8.3/colrev/ops/built_in/search_sources/pdfs_dir.md
+-rw-r--r--   0        0        0    29908 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/pdfs_dir.py
+-rw-r--r--   0        0        0      390 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/psycinfo.md
+-rw-r--r--   0        0        0     3684 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/psycinfo.py
+-rw-r--r--   0        0        0      570 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/pubmed.md
+-rw-r--r--   0        0        0    27264 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/pubmed.py
+-rw-r--r--   0        0        0      366 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/scopus.md
+-rw-r--r--   0        0        0     5355 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/scopus.py
+-rw-r--r--   0        0        0      377 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/springer_link.md
+-rw-r--r--   0        0        0     6247 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/springer_link.py
+-rw-r--r--   0        0        0      433 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/systematic_review_datasets.md
+-rw-r--r--   0        0        0     4822 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/systematic_review_datasets.py
+-rw-r--r--   0        0        0      385 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/taylor_and_francis.md
+-rw-r--r--   0        0        0     3231 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/taylor_and_francis.py
+-rw-r--r--   0        0        0      364 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/trid.md
+-rw-r--r--   0        0        0     3975 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/trid.py
+-rw-r--r--   0        0        0      333 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/unknown_source.md
+-rw-r--r--   0        0        0    14293 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/unknown_source.py
+-rw-r--r--   0        0        0     5396 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/utils.py
+-rw-r--r--   0        0        0      333 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/video_dir.md
+-rw-r--r--   0        0        0     6426 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/video_dir.py
+-rw-r--r--   0        0        0      383 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/web_of_science.md
+-rw-r--r--   0        0        0     4720 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/web_of_science.py
+-rw-r--r--   0        0        0     5592 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/website.py
+-rw-r--r--   0        0        0      376 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/wiley.md
+-rw-r--r--   0        0        0     3776 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/built_in/search_sources/wiley.py
+-rw-r--r--   0        0        0     1472 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/clone.py
+-rw-r--r--   0        0        0     9208 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/commit.py
+-rw-r--r--   0        0        0     7310 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/correct.py
+-rw-r--r--   0        0        0    15016 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/data.py
+-rw-r--r--   0        0        0    39649 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/dedupe.py
+-rw-r--r--   0        0        0     4937 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/distribute.py
+-rw-r--r--   0        0        0    16525 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/init.py
+-rw-r--r--   0        0        0    42205 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/load.py
+-rw-r--r--   0        0        0     9491 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/merge.py
+-rw-r--r--   0        0        0    26382 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/pdf_get.py
+-rw-r--r--   0        0        0     7993 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/pdf_get_man.py
+-rw-r--r--   0        0        0    17923 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/pdf_prep.py
+-rw-r--r--   0        0        0    13434 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/pdf_prep_man.py
+-rw-r--r--   0        0        0    41454 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/prep.py
+-rw-r--r--   0        0        0    11172 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/prep_man.py
+-rw-r--r--   0        0        0    12700 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/prescreen.py
+-rw-r--r--   0        0        0     1728 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/pull.py
+-rw-r--r--   0        0        0     5748 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/push.py
+-rw-r--r--   0        0        0     2329 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/remove.py
+-rw-r--r--   0        0        0    16311 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/repare.py
+-rw-r--r--   0        0        0     1126 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/review_types.py
+-rw-r--r--   0        0        0    16066 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/screen.py
+-rw-r--r--   0        0        0    23419 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/search.py
+-rw-r--r--   0        0        0     1650 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/search_sources.py
+-rwxr-xr-x   0        0        0    22158 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/status.py
+-rw-r--r--   0        0        0     8944 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/sync.py
+-rw-r--r--   0        0        0     4470 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/trace.py
+-rw-r--r--   0        0        0    12184 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/upgrade.py
+-rw-r--r--   0        0        0    21848 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/ops/validate.py
+-rw-r--r--   0        0        0        0 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/py.typed
+-rw-r--r--   0        0        0      112 2023-04-23 07:21:47.585349 colrev-0.8.3/colrev/qm/__init__.py
+-rw-r--r--   0        0        0     8373 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/qm/colrev_id.py
+-rw-r--r--   0        0        0     1519 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/qm/colrev_pdf_id.py
+-rw-r--r--   0        0        0      104 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/readme.md
+-rw-r--r--   0        0        0   105965 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/record.py
+-rw-r--r--   0        0        0    25378 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/review_manager.py
+-rw-r--r--   0        0        0    11405 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/service.py
+-rw-r--r--   0        0        0    19627 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/settings.py
+-rw-r--r--   0        0        0     1882 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_data_script.py
+-rw-r--r--   0        0        0     1157 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_pdf_get_script.py
+-rw-r--r--   0        0        0     1427 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_pdf_prep_script.py
+-rw-r--r--   0        0        0     1414 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_prep_script.py
+-rw-r--r--   0        0        0     1891 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_prescreen_script.py
+-rw-r--r--   0        0        0     2407 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_screen_script.py
+-rw-r--r--   0        0        0     3301 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/custom_scripts/custom_search_source_script.py
+-rw-r--r--   0        0        0    15707 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/example/30_example_records.bib
+-rw-r--r--   0        0        0      143 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/github_pages/README.md
+-rw-r--r--   0        0        0      155 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/github_pages/_config.yml
+-rw-r--r--   0        0        0       73 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/github_pages/about.md
+-rw-r--r--   0        0        0     4953 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/github_pages/index.html
+-rw-r--r--   0        0        0      185 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/github_pages/pre-commit-config.yaml
+-rw-r--r--   0        0        0    18650 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/LICENSE-CC-BY-4.0.txt
+-rw-r--r--   0        0        0     1752 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/colrev_update.yml
+-rw-r--r--   0        0        0     1537 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/colrev_update_curation.yml
+-rw-r--r--   0        0        0       54 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/gitattributes
+-rw-r--r--   0        0        0       85 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/markdownlint.yaml
+-rw-r--r--   0        0        0      936 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/pre-commit-config.yaml
+-rw-r--r--   0        0        0      480 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/pre-commit.yml
+-rw-r--r--   0        0        0      282 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/readme.md
+-rw-r--r--   0        0        0     5280 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/init/settings.json
+-rw-r--r--   0        0        0      930 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/commit_report_details.txt
+-rw-r--r--   0        0        0      271 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/commit_report_header.txt
+-rw-r--r--   0        0        0      352 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/complementary_material_keywords.txt
+-rw-r--r--   0        0        0      318 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/complementary_material_strings.txt
+-rw-r--r--   0        0        0      494 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/masterdata_curations.csv
+-rw-r--r--   0        0        0      462 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/pdf_get_man_mail.txt
+-rw-r--r--   0        0        0    76341 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/predatory_journals_beall.csv
+-rw-r--r--   0        0        0     2729 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/prep_man_curation.ipynb
+-rw-r--r--   0        0        0     3830 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/ops/status.txt
+-rw-r--r--   0        0        0    50756 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/package_endpoints.json
+-rw-r--r--   0        0        0    13058 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/package_status.json
+-rw-r--r--   0        0        0       94 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/packages.json
+-rw-r--r--   0        0        0    25233 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/paper_md/APA-7.docx
+-rw-r--r--   0        0        0      381 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/paper_md/non_sample_references.bib
+-rw-r--r--   0        0        0      673 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/paper_md/paper.md
+-rw-r--r--   0        0        0     4935 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/prisma/PRISMA.csv
+-rw-r--r--   0        0        0     5108 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/prisma/PRISMA_original.csv
+-rw-r--r--   0        0        0      872 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/prisma/prisma-refs.bib
+-rw-r--r--   0        0        0      262 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/prisma/prisma_text.md
+-rw-r--r--   0        0        0     1506 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/review_type/curated_masterdata/curations_github_colrev_update.yml
+-rw-r--r--   0        0        0      460 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/review_type/curated_masterdata/readme.md
+-rw-r--r--   0        0        0      586 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/template/review_type/meta_analysis/paper.md
+-rw-r--r--   0        0        0      104 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/__init__.py
+-rw-r--r--   0        0        0     5572 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/add_packages.py
+-rw-r--r--   0        0        0    75528 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/cli.py
+-rw-r--r--   0        0        0      146 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/cli_colors.py
+-rw-r--r--   0        0        0     9090 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/cli_status_printer.py
+-rw-r--r--   0        0        0     7419 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/cli_validation.py
+-rw-r--r--   0        0        0     2891 2023-04-23 07:21:47.589349 colrev-0.8.3/colrev/ui_cli/show_printer.py
+-rw-r--r--   0        0        0     2869 2023-04-23 07:21:47.613349 colrev-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     7940 1970-01-01 00:00:00.000000 colrev-0.8.3/PKG-INFO
```

### Comparing `colrev-0.8.2/CHANGELOG.md` & `colrev-0.8.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0).
 
-## [Unreleased]
+## Unreleased
 
 ### Added
 
 ### Changed
 
 ### Removed
 
 ### Fixed
 
+## 0.8.3 - 2023-04-22
 
-## [0.8.2] - 2023-04-05
+### Changed
+
+- CoLRev pdf IDs are now based on the mupdf library
+
+## 0.8.2 - 2023-04-05
 
 ### Fixed
 
 - Fix InvalidGitRepositoryError (raised upon status in empty directories)
 
-## [0.8.1] - 2023-04-04
+## 0.8.1 - 2023-04-04
 
 ### Changed
 
 - Update the Github action workflows in CoLRev repositories
 - Add auto-upgrade flag to settings
 
-## [0.8.0] - 2023-03-26
+## 0.8.0 - 2023-03-26
 
 ### Added
 
 - Unit tests: increased test coverage to 70%, added Github actions matrix tests across OS and Python versions
 - Completed OpenSSF Best Practices checks ([1](https://bestpractices.coreinfrastructure.org/de/projects/7148))
 - Added forward and backward searches based on [OpenCitations](https://opencitations.net/)
 - Moved documentation to [readthedocs](https://colrev.readthedocs.io/en/latest/) and revised documentation
@@ -57,21 +62,21 @@
 - Simplified upgrade operation and activated upgrades per default
 - Extracted and refactored language-service
 
 ### Fixed
 
 - Several bugfixes
 
-### [0.7.1] - 2023-03-25
+### 0.7.1 - 2023-03-25
 
 ### Changed
 
 - Changed package prefix from ``colrev_built_in`` to ``colrev``
 
-### [0.7.0] - 2023-01-16
+### 0.7.0 - 2023-01-16
 
 ### Added
 
 - Add retrieve and pdfs as high-level operations
 - Metadata preparation can add records to separate origin feeds
 - Initial package manager functionality (registering packages and displaying them in the docs)
 - Search: update of records and propagation of changes
@@ -106,15 +111,15 @@
 
 ### Fixed
 
 - **kwargs calls in ReviewManager
 - Indexing of non-curated records
 - Address special cases in dedupe (active learning)
 
-### [0.6.0] - 2022-10-12
+### 0.6.0 - 2022-10-12
 
 ### Added
 
 - Web-based editor for project settings
 - Comprehensive architecture refactoring
 - Conformance with pylint, mypy, flake8
 - Introduced packages
@@ -131,15 +136,15 @@
 - Switch to Jinja templates (instead of concatenating multiple strings)
 
 ### Fixed
 
 - Concurrent request session handling
 - StatusStats calculations
 
-### [0.5.0] - 2022-06-28
+### 0.5.0 - 2022-06-28
 
 ### Added
 
 - Push/pull (including corrections), sync, validate, service operations
 - Data provenance model (colrev_data_provenance, colrev_masterdata_provenance)
 - Extensible endpoints (search, prep, prescreen, pdf-get, pdf-prep, screen, data)
 - Prescreen scope
@@ -152,15 +157,15 @@
 - LocalIndex: Elasticsearch to Opensearch
 - Dedupe: testing and parameter optimization (option to prevent same-source merges)
 - Settings.json and validation
 - Updated documentation
 - Testing and refactoring (e.g., for Windows, prefer keyword arguments in functions, python package type information)
 
 
-### [0.4.0] - 2022-04-06
+### 0.4.0 - 2022-04-06
 
 ### Added
 
 - Extract functionality: ReviewDataset, Process
 - Developed LocalIndex, EnvironmentManager, OpenSearch
 - Curation model, including Resource installation and a "correction path"
 - Search operation (reintegrating paper_feed and local_paper_index)
@@ -175,15 +180,15 @@
 - Structured data extraction based on csv
 
 ### Fixed
 
 - Loggers
 - Performance issues in prep and status
 
-### [0.3.0] - 2022-02-05
+### 0.3.0 - 2022-02-05
 
 ### Added
 
 - Introduced ReviewManager and integrated hooks/checks
 - Fetch metadata from Open Library
 - Required fields for misc
 - Information on needs_manual_preparation (man_prep_hints)
@@ -205,15 +210,15 @@
 
 ### Fixed
 
 - Initializing repositories
 - Backward search adds two entries to search_details
 - Logging (reinitialize after batches/commits)
 
-### [0.2.0] - 2021-09-12
+### 0.2.0 - 2021-09-12
 
 ### Added
 
 - Status model (rev_status, md_status, pdf_status)
 - Implemented cli interface
 - Import formats (bib, ris, endn, pdf, text list of references)
 - Docker services for import, ocr, building the paper etc.
@@ -240,13 +245,13 @@
 
 - Bugs in `analysis/combine_individual_search_results.py` and in `analysis/acquire_pdfs.py`
 - Catch exceptions and check bad responses in `analysis/acquire_pdfs.py`
 - Bug in git modification check for `references.bib` in `analysis/utils.py`
 - Exception in `anaylsis/screen_2.py` (IndexError)
 - Global constant conflict with `analysis/entry_hash_function.py` (nameparser.config/CONSTANTS)
 
-### [0.1.0] - 2021-05-08
+### 0.1.0 - 2021-05-08
 
 ### Added
 
 - First version of the pipeline, including `status`, `reformat_bibliography`, `trace_entry`, `trace_hash_id`, `combine_individual_search_results`, `cleanse_records`, `screen_sheet`, `screen_1`, `acquire_pdfs`, `screen_2`, `data_sheet` and `data_pages`
 - Environment setup including `Dockerfile` and `Makefiles`
```

### Comparing `colrev-0.8.2/CONTRIBUTING.md` & `colrev-0.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/LICENSE` & `colrev-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/README.md` & `colrev-0.8.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/colrev)
 [![License](https://img.shields.io/github/license/CoLRev-Ecosystem/colrev.svg)](https://github.com/CoLRev-Environment/colrev/releases/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Documentation Status](https://readthedocs.org/projects/colrev/badge/?version=latest)](https://colrev.readthedocs.io/en/latest/?badge=latest)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Ecosystem/colrev/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/CoLRev-Ecosystem/colrev/main.svg)](https://results.pre-commit.ci/latest/github/CoLRev-Ecosystem/colrev/main)
 ![Coverage](https://raw.githubusercontent.com/CoLRev-Ecosystem/colrev/main/tests/coverage.svg)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bd4e44c6cda646e4b9e494c4c4d9487b)](https://app.codacy.com/gh/CoLRev-Environment/colrev/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 ![GitHub last commit](https://img.shields.io/github/last-commit/CoLRev-Ecosystem/colrev)
 [![Downloads](https://static.pepy.tech/badge/colrev/month)](https://pepy.tech/project/colrev)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7148/badge)](https://bestpractices.coreinfrastructure.org/projects/7148)
 [![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/CoLRev-Environment/colrev/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/CoLRev-Environment/colrev/)
 <!-- ![PyPI](https://img.shields.io/pypi/v/colrev) -->
 <!-- [![](https://img.shields.io/badge/-documentation-green)](https://colrev.readthedocs.io/) -->
 
 </div>
 
 ## Summary
 
-CoLRev is an open-source environment for collaborative literature reviews. It takes care of the data, integrates with differerent synthesis tools, and facilitates Git-based collaboration.
+CoLRev is an open-source environment for collaborative literature reviews. It integrates with differerent synthesis tools, takes care of the data, and facilitates Git-based collaboration.
 
 To accomplish these goals, CoLRev advances the design of review technology at the intersection of methods, design, cognition, and community building.
 The following features stand out:
 
 - An open and extensible environment based on shared data and process standards
 - Builds on git and its transparent collaboration model for the entire literature review process
 - Offers a self-explanatory, fault-tolerant, and configurable user workflow
-- Operates a model for data quality, record identification, content curation, and reuse
+- Operates a model for data quality, content curation, and reuse
 - Enables typological and methodological pluralism throughout the process
 
-See the [statements of development status](https://colrev.readthedocs.io/en/latest/foundations/roadmap.html) and [documentation](https://colrev.readthedocs.io/en/latest/) for more details. A brief overview presented at ESMARConf2023 is available on [YouTube](https://www.youtube.com/watch?v=yfGGraQC6vs).
+See the [statements of development status](https://colrev.readthedocs.io/en/latest/foundations/dev_status.html) and [documentation](https://colrev.readthedocs.io/en/latest/) for more details. A brief overview presented at ESMARConf2023 is available on [YouTube](https://www.youtube.com/watch?v=yfGGraQC6vs).
 
 ## Contributing, changes, and releases
 
 Contributions, code and features are always welcome
 
-- See [contributing guidelines](CONTRIBUTING.md), [help page](docs/build/user_resources/help.html), and [github repository](https://github.com/CoLRev-Environment/colrev).
+- See [contributing guidelines](CONTRIBUTING.md), [help page](https://colrev.readthedocs.io/en/latest/manual/help.html), and [github repository](https://github.com/CoLRev-Environment/colrev).
 - Bug reports or feedback? Please use the [issue tracker](https://github.com/CoLRev-Environment/colrev/issues) and let us know.
 - To get your work included, fork the repository, implement your changes, and create a [pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 For further information, see [tests](tests/readme.md), [changes](CHANGELOG.md), and [releases](https://github.com/CoLRev-Environment/colrev/releases).
 
 ## License
```

### Comparing `colrev-0.8.2/colrev/advisor.py` & `colrev-0.8.3/colrev/advisor.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     ) -> None:
         # Notify when changes in bib files are not staged
         # (this may raise unexpected errors)
 
         non_staged = [
             item.a_path
             for item in git_repo.index.diff(None)
-            if ".bib" == item.a_path[-4:]
+            if item.a_path[-4:] == ".bib"
         ]
         if len(non_staged) > 0:
             item = {
                 "title": f"Non-staged changes: {','.join(non_staged)}",
                 "level": "WARNING",
             }
             collaboration_instructions["items"].append(item)
@@ -276,24 +276,24 @@
         if self.review_manager.dataset.records_changed():
             # Detect and validate transitions
             transitioned_records = status_stats.get_transitioned_records(
                 current_origin_states_dict=current_origin_states_dict
             )
 
             for transitioned_record in transitioned_records:
-                if "no_source_state" == transitioned_record["dest"]:
+                if transitioned_record["dest"] == "no_source_state":
                     print(f"Error (no source_state): {transitioned_record}")
                     review_instructions.append(
                         {
                             "msg": "Resolve committed colrev_status "
                             + f"of {transitioned_record}",
                             "priority": "yes",
                         }
                     )
-                if "invalid_transition" == transitioned_record["operations_type"]:
+                if transitioned_record["operations_type"] == "invalid_transition":
                     msg = (
                         f"Resolve invalid transition ({transitioned_record['ID']}): "
                         + f"{transitioned_record['source']} to "
                         + f"{transitioned_record['dest']}"
                     )
                     if msg not in [ri["msg"] for ri in review_instructions]:
                         review_instructions.append(
@@ -323,74 +323,78 @@
                     + "(save and revert the other) and commit before continuing!\n"
                     + f"  Records: {rec_str}",
                     # "cmd": f"colrev {in_progress_processes}",
                     "priority": "yes",
                 }
                 review_instructions.append(instruction)
 
-    def __append_next_operation_instructions(
-        self,
-        *,
-        review_instructions: list,
-        status_stats: colrev.ops.status.StatusStats,
-        current_origin_states_dict: dict,
-    ) -> None:
-        # pylint: disable=too-many-branches
+    def __append_initial_operations(
+        self, *, review_instructions: list, status_stats: colrev.ops.status.StatusStats
+    ) -> bool:
+        if not Path(self.review_manager.search_dir).iterdir():
+            instruction = {
+                "msg": "Add search results to data/search",
+                "priority": "yes",
+            }
+            review_instructions.append(instruction)
+            return True
 
         if status_stats.overall.md_retrieved == 0:
-            if not Path(self.review_manager.search_dir).iterdir():
-                instruction = {
-                    "msg": "Add search results to data/search",
-                    "priority": "yes",
-                }
-                review_instructions.append(instruction)
-            else:
-                instruction = {
-                    "msg": self._next_step_description["retrieve"],
-                    "cmd": "colrev retrieve",
-                    "priority": "yes",
-                }
-                review_instructions.append(instruction)
+            instruction = {
+                "msg": self._next_step_description["retrieve"],
+                "cmd": "colrev retrieve",
+                "priority": "yes",
+            }
+            review_instructions.append(instruction)
+            return True
 
         if status_stats.currently.md_retrieved > 0:
             instruction = {
                 "msg": self._next_step_description["retrieve"],
                 "cmd": "colrev retrieve",
                 "priority": "yes",
             }
             review_instructions.append(instruction)
 
             if not self.review_manager.verbose_mode:
-                return
+                return True
+        return False
 
-        active_processing_functions = status_stats.get_active_operations(
+    def __append_active_operations(
+        self,
+        *,
+        status_stats: colrev.ops.status.StatusStats,
+        current_origin_states_dict: dict,
+        review_instructions: list,
+    ) -> None:
+        active_operations = status_stats.get_active_operations(
             current_origin_states_dict=current_origin_states_dict
         )
 
-        priority_processing_functions = status_stats.get_priority_operations(
+        priority_processing_operations = status_stats.get_priority_operations(
             current_origin_states_dict=current_origin_states_dict
         )
 
-        for active_processing_function in active_processing_functions:
-            if active_processing_function in ["load", "prep", "dedupe"]:
+        for active_operation in active_operations:
+            if active_operation in ["load", "prep", "dedupe"]:
                 instruction = {
                     "msg": self._next_step_description["retrieve"],
                     "cmd": "colrev retrieve",
                 }
-            if active_processing_function in ["pdf_get", "pdf_prep"]:
+            if active_operation in ["pdf_get", "pdf_prep"]:
                 instruction = {
                     "msg": self._next_step_description["pdfs"],
                     "cmd": "colrev pdfs",
                 }
             else:
                 instruction = {
-                    "msg": self._next_step_description[active_processing_function],
-                    "cmd": f"colrev {active_processing_function.replace('_', '-')}",
+                    "msg": self._next_step_description[active_operation],
+                    "cmd": f"colrev {active_operation.replace('_', '-')}",
                 }
-            if active_processing_function in priority_processing_functions:
+            if active_operation in priority_processing_operations:
                 # keylist = [list(x.keys()) for x in review_instructions]
                 # keys = [item for sublist in keylist for item in sublist]
                 # if "priority" not in keys:
                 instruction["priority"] = "yes"
             else:
                 if (
                     self.review_manager.settings.project.delay_automated_processing
@@ -398,14 +402,15 @@
                 ):
                     continue
             if instruction["cmd"] not in [
                 ri["cmd"] for ri in review_instructions if "cmd" in ri
             ]:
                 review_instructions.append(instruction)
 
+    def __append_data_operation_advice(self, *, review_instructions: list) -> None:
         if (
             len(review_instructions) == 1
             or self.review_manager.verbose_mode
             or self.review_manager.settings.is_curated_masterdata_repo()
         ):
             if (
                 "colrev data" in [ri["cmd"] for ri in review_instructions]
@@ -432,14 +437,34 @@
                     )
                     endpoint = endpoint_dict[data_package_endpoint["endpoint"]]
 
                     advice = endpoint.get_advice(self.review_manager)  # type: ignore
                     if advice:
                         review_instructions.append(advice)
 
+    def __append_next_operation_instructions(
+        self,
+        *,
+        review_instructions: list,
+        status_stats: colrev.ops.status.StatusStats,
+        current_origin_states_dict: dict,
+    ) -> None:
+        if self.__append_initial_operations(
+            review_instructions=review_instructions, status_stats=status_stats
+        ):
+            return
+
+        self.__append_active_operations(
+            status_stats=status_stats,
+            current_origin_states_dict=current_origin_states_dict,
+            review_instructions=review_instructions,
+        )
+
+        self.__append_data_operation_advice(review_instructions=review_instructions)
+
     def __get_missing_files(
         self, *, status_stats: colrev.ops.status.StatusStats
     ) -> list:
         # excluding pdf_not_available
         file_required_status = [
             colrev.record.RecordState.pdf_imported,
             colrev.record.RecordState.pdf_needs_manual_preparation,
@@ -626,18 +651,18 @@
         """Get instructions related to downloading outlets (resources)"""
 
         # pylint: disable=too-many-locals
 
         with open(self.review_manager.dataset.records_file, encoding="utf8") as file:
             outlets = []
             for line in file.readlines():
-                if "journal" == line.lstrip()[:7]:
+                if line.lstrip()[:7] == "journal":
                     journal = line[line.find("{") + 1 : line.rfind("}")]
                     outlets.append(journal)
-                if "booktitle" == line.lstrip()[:9]:
+                if line.lstrip()[:9] == "booktitle":
                     booktitle = line[line.find("{") + 1 : line.rfind("}")]
                     outlets.append(booktitle)
 
         outlet_counter: typing.List[typing.Tuple[str, int]] = [
             (j, x) for j, x in Counter(outlets).most_common(10) if x > 5
         ]
         selected = []
```

### Comparing `colrev-0.8.2/colrev/checker.py` & `colrev-0.8.3/colrev/checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         if not all((self.review_manager.path / x).is_file() for x in required_paths):
             return False
         return True
 
     def __get_installed_hooks(self) -> list:
         installed_hooks = []
         with open(".pre-commit-config.yaml", encoding="utf8") as pre_commit_y:
-            pre_commit_config = yaml.load(pre_commit_y, Loader=yaml.FullLoader)
+            pre_commit_config = yaml.load(pre_commit_y, Loader=yaml.SafeLoader)
         for repository in pre_commit_config["repos"]:
             installed_hooks.extend([hook["id"] for hook in repository["hooks"]])
         return installed_hooks
 
     def __require_colrev_hooks_installed(self) -> bool:
         required_hooks = [
             "colrev-hooks-check",
@@ -307,15 +307,15 @@
                     field_errors.append(
                         "Screening criteria field not matching "
                         f"pattern: {screen_crit} ({record_id}; criteria: {criteria})"
                     )
 
                 elif str(colrev.record.RecordState.rev_excluded) == status:
                     if ["NA"] == criteria:
-                        if "NA" == screen_crit:
+                        if screen_crit == "NA":
                             continue
                         field_errors.append(f"screen_crit field not NA: {screen_crit}")
 
                     if "=out" not in screen_crit:
                         self.review_manager.logger.error("criteria: %s", criteria)
                         field_errors.append(
                             "Excluded record with no screening_criterion violated: "
@@ -343,82 +343,99 @@
                             f"screen: {record_id}, {status}"
                         )
         if field_errors:
             raise colrev_exceptions.FieldValueError(
                 "\n    " + "\n    ".join(field_errors)
             )
 
+    def __check_change_in_propagated_id_in_file(
+        self,
+        *,
+        notifications: list,
+        root: str,
+        filename: str,
+        prior_id: str,
+        new_id: str,
+    ) -> None:
+        if prior_id == str(Path(filename).name):
+            msg = (
+                f"Old ID ({prior_id}, changed to {new_id} in the "
+                + f"RECORDS_FILE) found in filepath: {filename}"
+            )
+            if msg not in notifications:
+                notifications.append(msg)
+
+        # self.review_manager.logger.debug("Checking %s", name)
+        if filename.endswith(".bib"):
+            retrieved_ids = self.__retrieve_ids_from_bib(
+                file_path=Path(os.path.join(root, filename))
+            )
+            if prior_id in retrieved_ids:
+                msg = (
+                    f"Old ID ({prior_id}, changed to {new_id} in "
+                    + f"the RECORDS_FILE) found in file: {filename}"
+                )
+                if msg not in notifications:
+                    notifications.append(msg)
+        else:
+            with open(os.path.join(root, filename), encoding="utf8") as file:
+                line = file.readline()
+                while line:
+                    if filename.endswith(".bib") and "@" in line[:5]:
+                        line = file.readline()
+                    if prior_id in line:
+                        msg = (
+                            f"Old ID ({prior_id}, to {new_id} in "
+                            + f"the RECORDS_FILE) found in file: {filename}"
+                        )
+                        if msg not in notifications:
+                            notifications.append(msg)
+                    line = file.readline()
+
     def check_change_in_propagated_id(
         self, *, prior_id: str, new_id: str = "TBD", project_context: Path
     ) -> list:
         """Check whether propagated IDs were changed
 
         A propagated ID is a record ID that is stored outside the records.bib.
         Propagated IDs should not be changed in the records.bib
         because this would break the link between the propagated ID and its metadata.
         """
-        # pylint: disable=too-many-branches
 
         ignore_patterns = [
             ".git",
             ".report.log",
             ".pre-commit-config.yaml",
             "data/search",
         ]
 
         text_formats = [".txt", ".csv", ".md", ".bib", ".yaml"]
-        notifications = []
+        notifications: typing.List[str] = []
         for root, dirs, files in os.walk(project_context, topdown=False):
-            for name in files:
-                if any((x in name) or (x in root) for x in ignore_patterns):
-                    continue
-                if prior_id == str(Path(name).name):
-                    msg = (
-                        f"Old ID ({prior_id}, changed to {new_id} in the "
-                        + f"RECORDS_FILE) found in filepath: {name}"
-                    )
-                    if msg not in notifications:
-                        notifications.append(msg)
-
-                if not any(name.endswith(x) for x in text_formats):
+            for filename in files:
+                if any(
+                    (x in filename) or (x in root) for x in ignore_patterns
+                ) or not any(filename.endswith(x) for x in text_formats):
                     # self.review_manager.logger.debug("Skipping %s", name)
                     continue
-                # self.review_manager.logger.debug("Checking %s", name)
-                if name.endswith(".bib"):
-                    retrieved_ids = self.__retrieve_ids_from_bib(
-                        file_path=Path(os.path.join(root, name))
-                    )
-                    if prior_id in retrieved_ids:
-                        msg = (
-                            f"Old ID ({prior_id}, changed to {new_id} in "
-                            + f"the RECORDS_FILE) found in file: {name}"
-                        )
-                        if msg not in notifications:
-                            notifications.append(msg)
-                else:
-                    with open(os.path.join(root, name), encoding="utf8") as file:
-                        line = file.readline()
-                        while line:
-                            if name.endswith(".bib") and "@" in line[:5]:
-                                line = file.readline()
-                            if prior_id in line:
-                                msg = (
-                                    f"Old ID ({prior_id}, to {new_id} in "
-                                    + f"the RECORDS_FILE) found in file: {name}"
-                                )
-                                if msg not in notifications:
-                                    notifications.append(msg)
-                            line = file.readline()
-            for name in dirs:
-                if any((x in name) or (x in root) for x in ignore_patterns):
+                self.__check_change_in_propagated_id_in_file(
+                    notifications=notifications,
+                    root=root,
+                    filename=filename,
+                    prior_id=prior_id,
+                    new_id=new_id,
+                )
+
+            for dir_name in dirs:
+                if any((x in dir_name) or (x in root) for x in ignore_patterns):
                     continue
-                if prior_id in name:
+                if prior_id in dir_name:
                     notifications.append(
                         f"Old ID ({prior_id}, changed to {new_id} in the "
-                        f"RECORDS_FILE) found in filepath: {name}"
+                        f"RECORDS_FILE) found in filepath: {dir_name}"
                     )
         return notifications
 
     def __check_change_in_propagated_ids(
         self, *, prior: dict, status_data: dict
     ) -> None:
         """Check for changes in propagated IDs"""
```

### Comparing `colrev-0.8.2/colrev/dataset.py` & `colrev-0.8.3/colrev/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         "data/pdfs",
         ".report.log",
         "__pycache__",
         "output",
         "data/pdf_get_man/missing_pdf_files.csv",
         "data/.tei/",
         "data/prep_man/records_prep_man.bib",
+        "data/prep/",
+        "data/dedupe/",
     ]
     DEPRECATED_GIT_IGNORE_ITEMS = [
         "missing_pdf_files.csv",
         "manual_cleansing_statistics.csv",
         ".references_learned_settings",
         "pdfs",
         ".tei",
@@ -227,31 +229,31 @@
         return list(records_dict.values())
 
     @classmethod
     def __load_field_dict(cls, *, value: str, field: str) -> dict:
         # pylint: disable=too-many-branches
 
         return_dict = {}
-        if "colrev_masterdata_provenance" == field:
-            if "CURATED" == value[:7]:
+        if field == "colrev_masterdata_provenance":
+            if value[:7] == "CURATED":
                 if value.count(";") == 0:
                     value += ";;"  # Note : temporary fix (old format)
                 if value.count(";") == 1:
                     value += ";"  # Note : temporary fix (old format)
 
                 if ":" in value:
                     source = value[value.find(":") + 1 : value[:-1].rfind(";")]
                 else:
                     source = ""
                 return_dict["CURATED"] = {
                     "source": source,
                     "note": "",
                 }
 
-            elif "" != value:
+            elif value != "":
                 # Pybtex automatically replaces \n in fields.
                 # For consistency, we also do that for header_only mode:
                 if "\n" in value:
                     value = value.replace("\n", " ")
                 items = [x.lstrip() + ";" for x in (value + " ").split("; ") if x != ""]
 
                 for item in items:
@@ -263,19 +265,19 @@
                         return_dict[key] = {
                             "source": source,
                             "note": note,
                         }
                     else:
                         print(f"problem with masterdata_provenance_item {item}")
 
-        elif "colrev_data_provenance" == field:
-            if "" != value:
+        elif field == "colrev_data_provenance":
+            if value != "":
                 # Note : pybtex replaces \n upon load
                 for item in (value + " ").split("; "):
-                    if "" == item:
+                    if item == "":
                         continue
                     item += ";"  # removed by split
                     key_source = item[: item[:-1].rfind(";")]
                     note = item[item[:-1].rfind(";") + 1 : -1]
                     if ":" in key_source:
                         key, source = key_source.split(":", 1)
                         return_dict[key] = {
@@ -362,23 +364,23 @@
                     key, value = current_key_value_pair_str.split(" = ", 1)
                 else:
                     key = "ID"
                     value = current_key_value_pair_str.split("{")[1]
 
                 key = key.lstrip().rstrip()
                 value = value.lstrip().rstrip().lstrip("{").rstrip("},")
-                if "colrev_origin" == key:
+                if key == "colrev_origin":
                     value_list = value.replace("\n", "").split(";")
                     value_list = [x.lstrip(" ").rstrip(" ") for x in value_list if x]
                     return key, value_list
-                if "colrev_status" == key:
+                if key == "colrev_status":
                     return key, colrev.record.RecordState[value]
-                if "colrev_masterdata_provenance" == key:
+                if key == "colrev_masterdata_provenance":
                     return key, self.__load_field_dict(value=value, field=key)
-                if "file" == key:
+                if key == "file":
                     return key, Path(value)
             except IndexError as exc:
                 raise colrev_exceptions.BrokenFilesError(
                     msg="parsing records.bib"
                 ) from exc
 
             return key, value
@@ -413,33 +415,33 @@
 
             if current_header_item_count > number_required_header_items or "}" == line:
                 record_header_items.append(record_header_item)
                 record_header_item = default.copy()
                 current_header_item_count = 0
                 continue
 
-            if "@" in line[:2] and "NA" != record_header_item["ID"]:
+            if "@" in line[:2] and record_header_item["ID"] != "NA":
                 record_header_items.append(record_header_item)
                 record_header_item = default.copy()
                 current_header_item_count = 0
 
             current_key_value_pair_str += line
             if "}," in line or "@" in line[:2]:
                 key, value = parse_k_v(current_key_value_pair_str)
-                if "colrev_masterdata_provenance" == key:
-                    if "NA" == value:
+                if key == "colrev_masterdata_provenance":
+                    if value == "NA":
                         value = {}
-                if "NA" == value:
+                if value == "NA":
                     current_key_value_pair_str = ""
                     continue
                 current_key_value_pair_str = ""
                 if key in record_header_item:
                     current_header_item_count += 1
                     record_header_item[key] = value
-        if "NA" != record_header_item["colrev_origin"]:
+        if record_header_item["colrev_origin"] != "NA":
             record_header_items.append(record_header_item)
         return [
             {k: v for k, v in record_header_item.items() if "NA" != v}
             for record_header_item in record_header_items
         ]
 
     def load_records_dict(
@@ -552,15 +554,15 @@
             ]
 
             record = colrev.record.Record(data=record_dict)
             record_dict = record.get_data(stringify=True)
 
             for ordered_field in field_order:
                 if ordered_field in record_dict:
-                    if "" == record_dict[ordered_field]:
+                    if record_dict[ordered_field] == "":
                         continue
                     bibtex_str += format_field(
                         ordered_field, record_dict[ordered_field]
                     )
 
             for key, value in record_dict.items():
                 if key in field_order + ["ID", "ENTRYTYPE"]:
@@ -700,15 +702,15 @@
 
     # ID creation, update and lookup ---------------------------------------
 
     def reprocess_id(self, *, paper_ids: str) -> None:
         """Remove an ID (set of IDs) from the bib_db (for reprocessing)"""
 
         saved_args = locals()
-        if "all" == paper_ids:
+        if paper_ids == "all":
             # self.review_manager.logger.info("Removing/reprocessing all records")
             os.remove(self.records_file)
             self.__git_repo.index.remove(
                 [str(self.RECORDS_FILE_RELATIVE)],
                 working_tree=True,
             )
         else:
@@ -736,15 +738,15 @@
             if "curated_metadata" in str(self.review_manager.path):
                 raise colrev_exceptions.RecordNotInIndexException()
 
         except (
             colrev_exceptions.RecordNotInIndexException,
             colrev_exceptions.NotEnoughDataToIdentifyException,
         ):
-            if "" != record_dict.get("author", record_dict.get("editor", "")):
+            if record_dict.get("author", record_dict.get("editor", "")) != "":
                 authors_string = record_dict.get(
                     "author", record_dict.get("editor", "Anonymous")
                 )
                 authors = colrev.record.PrepRecord.format_author_field(
                     input_string=authors_string
                 ).split(" and ")
             else:
@@ -879,22 +881,24 @@
                 and not self.review_manager.force_mode
             ):
                 continue
             old_id = record_id
 
             temp_stat = record_dict["colrev_status"]
             if selected_ids:
-                record_dict["colrev_status"] = colrev.record.RecordState.md_prepared
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(target_state=colrev.record.RecordState.md_prepared)
             new_id = self.__generate_id(
                 local_index=local_index,
                 record_dict=record_dict,
                 existing_ids=[x for x in id_list if x != record_id],
             )
             if selected_ids:
-                record_dict["colrev_status"] = temp_stat
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(target_state=temp_stat)
 
             id_list.append(new_id)
             if old_id != new_id:
                 # We need to insert the a new element into records
                 # to make sure that the IDs are actually saved
                 record_dict.update(ID=new_id)
                 records[new_id] = record_dict
@@ -974,24 +978,24 @@
         self, *, relative_path: Optional[Path] = None, change_type: str = "all"
     ) -> bool:
         """Check whether the relative path (or the git repository) has changes"""
 
         if relative_path:
             main_recs_changed = False
             try:
-                if "all" == change_type:
+                if change_type == "all":
                     main_recs_changed = str(relative_path) in [
                         item.a_path for item in self.__git_repo.index.diff(None)
                     ] + [item.a_path for item in self.__git_repo.head.commit.diff()]
-                elif "staged" == change_type:
+                elif change_type == "staged":
                     main_recs_changed = str(relative_path) in [
                         item.a_path for item in self.__git_repo.head.commit.diff()
                     ]
 
-                elif "unstaged" == change_type:
+                elif change_type == "unstaged":
                     main_recs_changed = str(relative_path) in [
                         item.a_path for item in self.__git_repo.index.diff(None)
                     ]
             except ValueError:
                 pass
             return main_recs_changed
 
@@ -1167,14 +1171,14 @@
             origin = self.__git_repo.remotes.origin
             origin.pull()
 
     def get_remote_url(self) -> str:  # pragma: no cover
         """Get the remote url"""
         remote_url = "NA"
         for remote in self.__git_repo.remotes:
-            if "origin" == remote.name:
+            if remote.name == "origin":
                 remote_url = remote.url
         return remote_url
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/env/environment_manager.py` & `colrev-0.8.3/colrev/env/environment_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Optional
 
 import docker
 import git
 import pandas as pd
 import yaml
 from docker.errors import DockerException
+from git.exc import InvalidGitRepositoryError
 from yaml import safe_load
 
 import colrev.env.local_index
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
@@ -283,28 +284,30 @@
                     if remote.url:
                         repo["remote"] = True
                 repo[
                     "behind_remote"
                 ] = check_operation.review_manager.dataset.behind_remote()
 
                 repos.append(repo)
-            except colrev_exceptions.CoLRevException:
+            except (
+                colrev_exceptions.CoLRevException,
+                InvalidGitRepositoryError,
+            ):
                 broken_links.append(repo)
         return {"repos": repos, "broken_links": broken_links}
 
     def get_curated_outlets(self) -> list:
         """Get the curated outlets"""
         curated_outlets: typing.List[str] = []
         for repo_source_path in [
             x["repo_source_path"]
             for x in self.load_environment_registry()
             if "colrev/curated_metadata/" in x["repo_source_path"]
         ]:
             try:
-                # TODO : should come from the curation_data endpoint!
                 with open(f"{repo_source_path}/readme.md", encoding="utf-8") as file:
                     first_line = file.readline()
                 curated_outlets.append(first_line.lstrip("# ").replace("\n", ""))
 
                 with open(
                     f"{repo_source_path}/data/records.bib", encoding="utf-8"
                 ) as file:
@@ -313,22 +316,22 @@
                         # Note : the second part ("journal:"/"booktitle:")
                         # ensures that data provenance fields are skipped
                         if (
                             "journal" == line.lstrip()[:7]
                             and "journal:" != line.lstrip()[:8]
                         ):
                             journal = line[line.find("{") + 1 : line.rfind("}")]
-                            if "UNKNOWN" != journal:
+                            if journal != "UNKNOWN":
                                 outlets.append(journal)
                         if (
-                            "booktitle" == line.lstrip()[:9]
-                            and "booktitle:" != line.lstrip()[:10]
+                            line.lstrip()[:9] == "booktitle"
+                            and line.lstrip()[:10] != "booktitle:"
                         ):
                             booktitle = line[line.find("{") + 1 : line.rfind("}")]
-                            if "UNKNOWN" != booktitle:
+                            if booktitle != "UNKNOWN":
                                 outlets.append(booktitle)
 
                     if len(set(outlets)) > 1:
                         raise colrev_exceptions.CuratedOutletNotUnique(
                             "Error: Duplicate outlets in curated_metadata of "
                             f"{repo_source_path} : {','.join(list(set(outlets)))}"
                         )
```

### Comparing `colrev-0.8.2/colrev/env/grobid_service.py` & `colrev-0.8.3/colrev/env/grobid_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,23 +56,28 @@
                 return
         except requests.exceptions.ConnectionError:
             pass
 
         logging.info("Running docker container created from %s", self.grobid_image)
 
         logging.info("Starting grobid service...")
-        start_cmd = (
-            f'docker run -t --rm -m "4g" -p 8070:8070 -p 8071:8071 {self.grobid_image}'
-        )
-        subprocess.Popen(
-            [start_cmd],
-            shell=True,
-            stdin=None,
-            stdout=open(os.devnull, "wb"),
-            stderr=None,
-            close_fds=True,
-        )
+        start_cmd = [
+            "docker",
+            "run",
+            "-t",
+            "--rm",
+            "-m",
+            "4g",
+            "-p",
+            "8070:8070",
+            "-p",
+            "8071:8071",
+            self.grobid_image,
+        ]
+        with open(os.devnull, "w", encoding="utf-8") as devnull:
+            subprocess.Popen(start_cmd, shell=False, stdout=devnull)
+
         self.check_grobid_availability()
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/env/language_service.py` & `colrev-0.8.3/colrev/env/language_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
             predictions_unified.append((lang.iso_code_639_3.name.lower(), conf))
 
         return predictions_unified
 
     def validate_iso_639_3_language_codes(self, *, lang_code_list: list) -> None:
         """Validates whether a list of language codes complies with the ISO 639-3 standard"""
 
+        assert isinstance(lang_code_list, list)
+
         invalid_language_codes = [x for x in lang_code_list if 3 != len(x)]
         if invalid_language_codes:
             raise colrev_exceptions.InvalidLanguageCodeException(
                 invalid_language_codes=invalid_language_codes
             )
 
     def unify_to_iso_639_3_language_codes(
@@ -80,21 +82,24 @@
 
         if record.data["language"].lower() in ["en"]:
             record.data["language"] = "eng"
 
         elif record.data["language"].lower() in ["fr"]:
             record.data["language"] = "fra"
 
+        elif record.data["language"].lower() in ["ar"]:
+            record.data["language"] = "ara"
+
+        elif record.data["language"].lower() in ["de"]:
+            record.data["language"] = "deu"
+
         if 3 != len(record.data["language"]):
             if record.data["language"].lower() in self.__lang_code_mapping:
-                print(record.data["language"])
-                print(self.__lang_code_mapping[record.data["language"].lower()])
                 record.data["language"] = self.__lang_code_mapping[
                     record.data["language"].lower()
                 ]
-                print(record.data["language"])
 
         self.validate_iso_639_3_language_codes(lang_code_list=[record.data["language"]])
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/env/local_index.py` & `colrev-0.8.3/colrev/env/local_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import colrev.env.resources
 import colrev.env.tei_parser
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
 
+
 # import binascii
 
 # pylint: disable=too-many-lines
 
 
 class LocalIndex:
     """The LocalIndex implements indexing and retrieval of records across projects"""
@@ -56,14 +57,39 @@
     # to ensure that the indexing-ids do not exceed limits
     # such as the opensearch limit of 512 bytes.
     # This enables efficient retrieval based on id=hash(colrev_id)
     # but also search-based retrieval using only colrev_ids
 
     RECORD_INDEX = "record_index"
     TOC_INDEX = "toc_index"
+    UPDATE_LAYERD_FIELDS_QUERY = """
+            UPDATE record_index SET
+            layered_fields=?
+            WHERE id=?"""
+
+    SELECT_LAYERD_FIELDS_QUERY = "SELECT layered_fields FROM record_index WHERE id=?"
+
+    SELECT_ALL_QUERIES = {
+        TOC_INDEX: "SELECT * FROM toc_index WHERE",
+        RECORD_INDEX: "SELECT * FROM record_index WHERE",
+    }
+
+    SELECT_KEY_QUERIES = {
+        (RECORD_INDEX, "id"): "SELECT * FROM record_index WHERE id=?",
+        (TOC_INDEX, "toc_key"): "SELECT * FROM toc_index WHERE toc_key=?",
+        (RECORD_INDEX, "colrev_id"): "SELECT * FROM record_index WHERE colrev_id=?",
+        (RECORD_INDEX, "doi"): "SELECT * FROM record_index where doi=?",
+        (RECORD_INDEX, "dblp_key"): "SELECT * FROM record_index WHERE dblp_key=?",
+        (
+            RECORD_INDEX,
+            "colrev_pdf_id",
+        ): "SELECT * FROM record_index WHERE colrev_pdf_id=?",
+        (RECORD_INDEX, "url"): "SELECT * FROM record_index WHERE url=?",
+    }
+
     # AUTHOR_INDEX = "author_index"
     # AUTHOR_RECORD_INDEX = "author_record_index"
     # CITATIONS_INDEX = "citations_index"
 
     RECORDS_INDEX_KEYS = [
         "id",
         "colrev_id",
@@ -96,15 +122,15 @@
 
         self.thread_lock = Lock()
 
     def __get_sqlite_cursor(self, *, init: bool = False) -> sqlite3.Cursor:
         if init:
             Path(self.SQLITE_PATH).unlink(missing_ok=True)
 
-        self.sqlite_connection = sqlite3.connect(self.SQLITE_PATH)
+        self.sqlite_connection = sqlite3.connect(self.SQLITE_PATH, timeout=90)
         self.sqlite_connection.row_factory = self.__dict_factory
         return self.sqlite_connection.cursor()
         # raise colrev_exceptions.ServiceNotAvailableException(dep="local_index")
 
     def __dict_factory(self, cursor: sqlite3.Cursor, row: dict) -> dict:
         ret_dict = {}
         for idx, col in enumerate(cursor.description):
@@ -187,17 +213,15 @@
         self, *, cur: sqlite3.Cursor, item: dict, curated_fields: list
     ) -> None:
         """Adds layered fields to amend existing records"""
 
         record_dict = self.__get_record_from_row(row=item)
 
         layered_fields = []
-        cur.execute(
-            f"SELECT layered_fields FROM {self.RECORD_INDEX} WHERE id='{item['id']}'"
-        )
+        cur.execute(self.SELECT_LAYERD_FIELDS_QUERY, (item["id"],))
         for row in cur.fetchall():
             if row["layered_fields"]:
                 layered_fields = json.loads(row["layered_fields"])
 
             break
         for curated_field in curated_fields:
             if curated_field not in record_dict:
@@ -208,26 +232,25 @@
                     "key": curated_field,
                     "value": record_dict[curated_field],
                     "source": source,
                 }
             )
 
         cur.execute(
-            f"UPDATE {self.RECORD_INDEX} SET "
-            f"layered_fields='{json.dumps(layered_fields)}'"
-            f" WHERE id='{item['id']}'"
+            self.UPDATE_LAYERD_FIELDS_QUERY,
+            (json.dumps(layered_fields), item["id"]),
         )
 
     def get_fields_to_remove(self, *, record_dict: dict) -> list:
         """Compares the record to available toc items and
         returns fields to remove (if any)"""
         # pylint: disable=too-many-return-statements
 
         fields_to_remove: typing.List[str] = []
-        if "journal" not in record_dict and "article" != record_dict["ENTRYTYPE"]:
+        if "journal" not in record_dict and record_dict["ENTRYTYPE"] != "article":
             return fields_to_remove
 
         internal_record_dict = deepcopy(record_dict)
 
         if all(x in internal_record_dict.keys() for x in ["volume", "number"]):
             try:
                 toc_key_full = colrev.record.Record(
@@ -238,32 +261,32 @@
                     return fields_to_remove
             except colrev_exceptions.NotTOCIdentifiableException:
                 return fields_to_remove
             wo_nr = deepcopy(internal_record_dict)
             del wo_nr["number"]
             toc_key_wo_nr = colrev.record.Record(data=wo_nr).get_toc_key()
 
-            if "NA" != toc_key_wo_nr:
+            if toc_key_wo_nr != "NA":
                 if self.__toc_exists(toc_item=toc_key_wo_nr):
                     fields_to_remove.append("number")
                     return fields_to_remove
 
             wo_vol = deepcopy(internal_record_dict)
             del wo_vol["volume"]
             toc_key_wo_vol = colrev.record.Record(data=wo_vol).get_toc_key()
-            if "NA" != toc_key_wo_vol:
+            if toc_key_wo_vol != "NA":
                 if self.__toc_exists(toc_item=toc_key_wo_vol):
                     fields_to_remove.append("volume")
                     return fields_to_remove
 
             wo_vol_nr = deepcopy(internal_record_dict)
             del wo_vol_nr["volume"]
             del wo_vol_nr["number"]
             toc_key_wo_vol_nr = colrev.record.Record(data=wo_vol_nr).get_toc_key()
-            if "NA" != toc_key_wo_vol_nr:
+            if toc_key_wo_vol_nr != "NA":
                 if self.__toc_exists(toc_item=toc_key_wo_vol_nr):
                     fields_to_remove.append("number")
                     fields_to_remove.append("volume")
                     return fields_to_remove
 
         return fields_to_remove
 
@@ -298,15 +321,15 @@
             return
         cur = self.sqlite_connection.cursor()
         for item in list_to_add:
             while True:
                 for records_index_required_key in self.RECORDS_INDEX_KEYS:
                     if records_index_required_key not in item:
                         item[records_index_required_key] = ""
-                if "" == item["id"]:
+                if item["id"] == "":
                     print("NO ID IN RECORD")
                     break
                 try:
                     cur.execute(
                         f"INSERT INTO {self.RECORD_INDEX} "
                         f"VALUES(:{', :'.join(self.RECORDS_INDEX_KEYS)})",
                         item,
@@ -404,16 +427,14 @@
             target_path = Path(temp_path) / Path(gh_url.split("/")[-1])
             if not target_path.is_dir():
                 git.Repo.clone_from(
                     gh_url,  # .replace("https://github.com/", "git@github.com:") + ".git",
                     str(target_path),
                     depth=1,
                 )
-                # TODO : save info on curations that were not available
-                # (to be displayed in gh-action/pull-request)
 
             content = ""
             with open(target_path / Path("data/records.bib"), encoding="utf-8") as file:
                 content = file.read()
 
             parser = bibtex.Parser()
             bib_data = parser.parse_string(content)
@@ -487,27 +508,28 @@
                 del record_dict["file"]
 
         if not include_colrev_ids and "colrev_id" in record_dict:
             if "colrev_id" in record_dict:
                 del record_dict["colrev_id"]
 
         if include_file:
-            if "NA" != fulltext_backup:
+            if fulltext_backup != "NA":
                 record_dict["fulltext"] = fulltext_backup
         else:
             if "file" in record_dict:
                 del record_dict["file"]
             if "file" in record_dict.get("colrev_data_provenance", {}):
                 del record_dict["colrev_data_provenance"]["file"]
             if "colrev_pdf_id" in record_dict:
                 del record_dict["colrev_pdf_id"]
             if "colrev_pdf_id" in record_dict.get("colrev_data_provenance", {}):
                 del record_dict["colrev_data_provenance"]["colrev_pdf_id"]
 
-        record_dict["colrev_status"] = colrev.record.RecordState.md_prepared
+        record = colrev.record.Record(data=record_dict)
+        record.set_status(target_state=colrev.record.RecordState.md_prepared)
 
         if "CURATED" in record_dict.get("colrev_masterdata_provenance", {}):
             identifier_string = (
                 record_dict["colrev_masterdata_provenance"]["CURATED"]["source"]
                 + "#"
                 + record_dict["ID"]
             )
@@ -559,26 +581,18 @@
                 return True
 
         except colrev_exceptions.CuratedOutletNotUnique as exc:
             print(exc)
             return True
         return False
 
-    def _prepare_record_for_indexing(self, *, record_dict: dict) -> dict:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+    def __apply_status_requirements(self, *, record_dict: dict) -> None:
         if "colrev_status" not in record_dict:
             raise colrev_exceptions.RecordNotIndexableException()
 
-        # Do not cover deprecated fields
-        for deprecated_field in ["pdf_hash"]:
-            if deprecated_field in record_dict:
-                print(f"Removing deprecated field: {deprecated_field}")
-                del record_dict[deprecated_field]
-
         # It is important to exclude md_prepared if the LocalIndex
         # is used to dissociate duplicates
         if (
             record_dict["colrev_status"]
             in colrev.record.RecordState.get_non_processed_states()
         ):
             raise colrev_exceptions.RecordNotIndexableException()
@@ -586,88 +600,80 @@
         # Some prescreen_excluded records are not prepared
         if (
             record_dict["colrev_status"]
             == colrev.record.RecordState.rev_prescreen_excluded
         ):
             raise colrev_exceptions.RecordNotIndexableException()
 
+    def __remove_fields(self, record_dict: dict) -> None:
+        # Do not cover deprecated fields
+        for deprecated_field in ["pdf_hash"]:
+            if deprecated_field in record_dict:
+                print(f"Removing deprecated field: {deprecated_field}")
+                del record_dict[deprecated_field]
+
         if "screening_criteria" in record_dict:
             del record_dict["screening_criteria"]
         # Note: if the colrev_pdf_id has not been checked,
         # we cannot use it for retrieval or preparation.
         post_pdf_prepared_states = colrev.record.RecordState.get_post_x_states(
             state=colrev.record.RecordState.pdf_prepared
         )
         if record_dict["colrev_status"] not in post_pdf_prepared_states:
             if "colrev_pdf_id" in record_dict:
                 del record_dict["colrev_pdf_id"]
 
-        # Note : this is the first run, no need to split/list
-        if "colrev/curated_metadata" in record_dict["metadata_source_repository_paths"]:
-            # Note : local_curated_metadata is important to identify non-duplicates
-            # between curated_metadata_repositories
-            record_dict["local_curated_metadata"] = "yes"
-
-        if "colrev_origin" in record_dict:
-            del record_dict["colrev_origin"]
-
         # Note : numbers of citations change regularly.
         # They should be retrieved from sources like crossref/doi.org
         if "cited_by" in record_dict:
             del record_dict["cited_by"]
-
-        # Note : file paths should be absolute when added to the LocalIndex
-        if "file" in record_dict:
-            pdf_path = Path(record_dict["file"])
-            if pdf_path.is_file():
-                record_dict["file"] = str(pdf_path)
-            else:
-                del record_dict["file"]
-
         if record_dict.get("year", "NA").isdigit():
             record_dict["year"] = int(record_dict["year"])
         else:
             raise colrev_exceptions.RecordNotIndexableException()
 
         if "language" in record_dict:
             if len(record_dict["language"]) != 3:
                 print(f'Language not in ISO 639-3 format: {record_dict["language"]}')
                 del record_dict["language"]
 
+    def __adjust_provenance_for_indexint(self, *, record_dict: dict) -> None:
         # Provenance should point to the original repository path.
         # If the provenance/source was example.bib (and the record is amended during indexing)
         # we wouldn't know where the example.bib belongs to.
         record = colrev.record.Record(data=record_dict)
         for key in list(record.data.keys()):
-            if key not in colrev.record.Record.identifying_field_keys:
-                if key not in colrev.record.Record.provenance_keys + [
+            if (
+                key
+                not in colrev.record.Record.identifying_field_keys
+                + colrev.record.Record.provenance_keys
+                + [
                     "ID",
                     "ENTRYTYPE",
                     "local_curated_metadata",
                     "metadata_source_repository_paths",
-                ]:
-                    if key not in record.data.get("colrev_data_provenance", {}):
-                        record.add_data_provenance(
-                            key=key,
-                            source=record_dict["metadata_source_repository_paths"],
-                        )
-                    else:
-                        if (
-                            "CURATED"
-                            not in record.data["colrev_data_provenance"][key]["source"]
-                        ):
-                            record.add_data_provenance(
-                                key=key,
-                                source=record_dict["metadata_source_repository_paths"],
-                            )
-            else:
-                if not record.masterdata_is_curated():
-                    record.add_masterdata_provenance(
-                        key=key, source=record_dict["metadata_source_repository_paths"]
+                ]
+            ):
+                if key not in record.data.get("colrev_data_provenance", {}):
+                    record.add_data_provenance(
+                        key=key,
+                        source=record_dict["metadata_source_repository_paths"],
+                    )
+                elif (
+                    "CURATED"
+                    not in record.data["colrev_data_provenance"][key]["source"]
+                ):
+                    record.add_data_provenance(
+                        key=key,
+                        source=record_dict["metadata_source_repository_paths"],
                     )
+            elif not record.masterdata_is_curated():
+                record.add_masterdata_provenance(
+                    key=key, source=record_dict["metadata_source_repository_paths"]
+                )
 
         # Make sure that we don't add provenance information without corresponding fields
         if "colrev_data_provenance" in record.data:
             provenance_keys = list(record.data.get("colrev_data_provenance", {}).keys())
             for provenance_key in provenance_keys:
                 if provenance_key not in record.data:
                     del record.data["colrev_data_provenance"][provenance_key]
@@ -676,15 +682,42 @@
                 provenance_keys = list(
                     record.data.get("colrev_masterdata_provenance", {}).keys()
                 )
                 for provenance_key in provenance_keys:
                     if provenance_key not in record.data:
                         del record.data["colrev_masterdata_provenance"][provenance_key]
 
-        return record.get_data()
+        record_dict = record.get_data()
+
+    def __prep_fields_for_indexing(self, *, record_dict: dict) -> None:
+        # Note : this is the first run, no need to split/list
+        if "colrev/curated_metadata" in record_dict["metadata_source_repository_paths"]:
+            # Note : local_curated_metadata is important to identify non-duplicates
+            # between curated_metadata_repositories
+            record_dict["local_curated_metadata"] = "yes"
+
+        # Note : file paths should be absolute when added to the LocalIndex
+        if "file" in record_dict:
+            pdf_path = Path(record_dict["file"])
+            if pdf_path.is_file():
+                record_dict["file"] = str(pdf_path)
+            else:
+                del record_dict["file"]
+
+        if "colrev_origin" in record_dict:
+            del record_dict["colrev_origin"]
+
+        self.__adjust_provenance_for_indexint(record_dict=record_dict)
+
+    def _prepare_record_for_indexing(self, *, record_dict: dict) -> dict:
+        self.__apply_status_requirements(record_dict=record_dict)
+        self.__remove_fields(record_dict=record_dict)
+        self.__prep_fields_for_indexing(record_dict=record_dict)
+
+        return record_dict
 
     def __get_index_record(self, *, record_dict: dict) -> dict:
         try:
             record_dict = self._prepare_record_for_indexing(record_dict=record_dict)
             cid_to_index = colrev.record.Record(data=record_dict).create_colrev_id()
             record_dict["colrev_id"] = cid_to_index
             record_dict["citation_key"] = record_dict["ID"]
@@ -821,15 +854,15 @@
                 path_str=str(repo_source_path)
             )
 
             check_operation = colrev.operation.CheckOperation(
                 review_manager=review_manager
             )
 
-            if "main" != review_manager.dataset.get_repo().active_branch.name:
+            if review_manager.dataset.get_repo().active_branch.name != "main":
                 print(
                     f"{colors.ORANGE}Warning: {repo_source_path} not on main branch{colors.END}"
                 )
 
             if not check_operation.review_manager.dataset.records_file.is_file():
                 return
             records = check_operation.review_manager.dataset.load_records_dict()
@@ -955,80 +988,83 @@
         ) as exc:
             raise colrev_exceptions.TOCNotAvailableException() from exc
 
     def __toc_exists(self, *, toc_item: str) -> bool:
         try:
             self.thread_lock.acquire(timeout=60)
             cur = self.__get_sqlite_cursor()
-            selected_row = None
-            cur.execute(f"SELECT * FROM {self.TOC_INDEX} WHERE toc_key='{toc_item}'")
-            for row in cur.fetchall():
-                selected_row = row
-                break
+            cur.execute(
+                self.SELECT_KEY_QUERIES[(self.TOC_INDEX, "toc_key")], (toc_item,)
+            )
+            selected_row = cur.fetchone()
             self.thread_lock.release()
             if not selected_row:
                 return False
             return True
         except sqlite3.OperationalError:
             self.thread_lock.release()
         except AttributeError:  # ie. no sqlite database available
             return False
-
         return False
 
-    def retrieve_from_toc(
-        self,
-        *,
-        record_dict: dict,
-        similarity_threshold: float,
-        include_file: bool = False,
-        search_across_tocs: bool = False,
-    ) -> dict:
-        """Retrieve a record from the toc (table-of-contents)"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
+    def __get_toc_items_for_toc_retrieval(
+        self, *, toc_key: str, search_across_tocs: bool
+    ) -> list:
+        toc_items = []
 
-        # 1. get TOC
-        toc_items, toc_key = [], "NA"
-        try:
-            toc_key = colrev.record.Record(data=record_dict).get_toc_key()
-        except colrev_exceptions.NotTOCIdentifiableException as exc:
-            if not search_across_tocs:
-                raise colrev_exceptions.RecordNotInIndexException() from exc
         if self.__toc_exists(toc_item=toc_key):
             res = self.__get_item_from_index(
                 index_name=self.TOC_INDEX, key="toc_key", value=toc_key
             )
             toc_items = res.get("colrev_ids", "").split(";")  # type: ignore
         else:
             if not search_across_tocs:
                 raise colrev_exceptions.RecordNotInIndexException()
 
         if not toc_items and search_across_tocs:
             try:
                 partial_toc_key = toc_key.replace("|-", "")
                 retrieved_tocs = self.__get_items_from_index(
                     index_name=self.TOC_INDEX,
-                    query=f"toc_key LIKE '{partial_toc_key}%'",
+                    query=("toc_key LIKE ?", [f"{partial_toc_key}%"]),
                 )
                 toc_items = [x["colrev_ids"].split(";") for x in retrieved_tocs]
                 toc_items = [item for sublist in toc_items for item in sublist]
 
             except (
                 colrev_exceptions.NotTOCIdentifiableException,
                 KeyError,
             ) as exc:
                 raise colrev_exceptions.RecordNotInIndexException() from exc
 
         if not toc_items:
             raise colrev_exceptions.RecordNotInIndexException()
+        return toc_items
+
+    def retrieve_from_toc(
+        self,
+        *,
+        record_dict: dict,
+        similarity_threshold: float,
+        include_file: bool = False,
+        search_across_tocs: bool = False,
+    ) -> dict:
+        """Retrieve a record from the toc (table-of-contents)"""
 
-        # 2. get most similar record_dict
         try:
+            try:
+                toc_key = colrev.record.Record(data=record_dict).get_toc_key()
+            except colrev_exceptions.NotTOCIdentifiableException as exc:
+                if not search_across_tocs:
+                    raise colrev_exceptions.RecordNotInIndexException() from exc
+
+            toc_items = self.__get_toc_items_for_toc_retrieval(
+                toc_key=toc_key, search_across_tocs=search_across_tocs
+            )
+
             if search_across_tocs:
                 record_colrev_id = colrev.record.Record(
                     data=record_dict
                 ).create_colrev_id(assume_complete=True)
 
             else:
                 record_colrev_id = colrev.record.Record(
@@ -1075,19 +1111,22 @@
             colrev_exceptions.NotEnoughDataToIdentifyException,
             KeyError,
         ):
             pass
 
         raise colrev_exceptions.RecordNotInIndexException()
 
-    def __get_items_from_index(self, *, index_name: str, query: str) -> list:
+    def __get_items_from_index(
+        self, *, index_name: str, query: typing.Tuple[str, list[str]]
+    ) -> list:
         try:
             self.thread_lock.acquire(timeout=60)
             cur = self.__get_sqlite_cursor()
-            cur.execute(f"SELECT * FROM {index_name} WHERE {query}")
+            select_all_query = f"{self.SELECT_ALL_QUERIES[index_name]} {query[0]}"
+            cur.execute(select_all_query, query[1])
             results = cur.fetchall()
             self.thread_lock.release()
             return results
 
         except sqlite3.OperationalError as exc:
             self.thread_lock.release()
             raise colrev_exceptions.RecordNotInIndexException() from exc
@@ -1100,31 +1139,29 @@
             cur = self.__get_sqlite_cursor()
 
             # in the following, collisions should be handled.
             # paper_hash = hashlib.sha256(cid_to_retrieve.encode("utf-8")).hexdigest()
             # Collision
             # paper_hash = self.__increment_hash(paper_hash=paper_hash)
 
-            selected_row = None
-            cur.execute(f"SELECT * FROM {index_name} WHERE {key}='{value}'")
-            for row in cur.fetchall():
-                selected_row = row
-                break
+            cur.execute(self.SELECT_KEY_QUERIES[(index_name, key)], (value,))
+
+            selected_row = cur.fetchone()
             self.thread_lock.release()
 
             if not selected_row:
                 raise colrev_exceptions.RecordNotInIndexException()
 
             retrieved_record = {}
             if self.RECORD_INDEX == index_name:
                 retrieved_record = self.__get_record_from_row(row=selected_row)
             else:
                 retrieved_record = selected_row
 
-            if "colrev_id" == key:
+            if key == "colrev_id":
                 if (
                     value
                     != colrev.record.Record(data=retrieved_record).create_colrev_id()
                 ):
                     raise colrev_exceptions.RecordNotInIndexException()
             else:
                 if key not in retrieved_record:
```

### Comparing `colrev-0.8.2/colrev/env/package_manager.py` & `colrev-0.8.3/colrev/env/package_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,15 +799,15 @@
         endpoint_class = package_details["import_name"]  # type: ignore
         to_remove = []
         for package_identifier, package_class in packages_dict.items():
             params = {
                 package_details["operation_name"]: operation,
                 "settings": package_class["settings"],
             }
-            if "search_source" == package_type:
+            if package_type == "search_source":
                 del params["check_operation"]
 
             if "endpoint" not in package_class:
                 raise colrev_exceptions.MissingDependencyError(
                     f"{package_identifier} is not available"
                 )
 
@@ -818,15 +818,15 @@
                     )
                     if only_ci_supported:
                         if not packages_dict[package_identifier].ci_supported:
                             to_remove.append(package_identifier)
                             continue
                     verifyObject(endpoint_class, packages_dict[package_identifier])
                 except colrev_exceptions.ServiceNotAvailableException as sna_exc:
-                    if "docker" == sna_exc.dep:
+                    if sna_exc.dep == "docker":
                         print(
                             f"{colors.ORANGE}Docker not available. Deactivate "
                             f"{package_identifier}{colors.END}"
                         )
                         to_remove.append(package_identifier)
                     else:
                         raise sna_exc
@@ -881,22 +881,19 @@
                             "status": "RED",
                         }
                     )
                     endpoint_item["status"] = "RED"
 
                 endpoint_item["status"] = (
                     endpoint_item["status"]
-                    .replace("GREEN", "🟢")
-                    .replace("ORANGE", "🟡")
-                    .replace("RED", "🔴")
-                )
-                endpoint_item["status_linked"] = (
-                    f"`{endpoint_item['status']} "
-                    + "<https://colrev.readthedocs.io/en/latest/foundations/roadmap.html>`_"
+                    .replace("STABLE", "|STABLE|")
+                    .replace("MATURING", "|MATURING|")
+                    .replace("EXPERIMENTAL", "|EXPERIMENTAL|")
                 )
+                endpoint_item["status_linked"] = endpoint_item["status"]
 
                 # Generate the contents displayed in the docs (see "datatemplate:json")
                 # load short_description dynamically...
                 short_description = endpoint.__doc__
                 if "\n" in endpoint.__doc__:
                     short_description = endpoint.__doc__.split("\n")[0]
                 endpoint_item["short_description"] = short_description
@@ -911,32 +908,17 @@
                 code_link = code_link[: code_link.rfind("/")]
                 code_link += ".md"
                 if hasattr(endpoint, "link"):
                     link = endpoint.link
                 else:
                     link = code_link
                 # Note: link format for the sphinx docs
-                endpoint_item["link"] = f"`Link <{link}>`_"
-                if (
-                    PackageEndpointType.search_source
-                    == PackageEndpointType[endpoint_type]
-                ):
-                    # Note : heuristic_status is mandatory (interface definition)
-                    endpoint_item["heuristic"] = (
-                        str(endpoint.heuristic_status)
-                        .replace("oni", "ONI")
-                        .replace("supported", "Supported")
-                        .replace("na", "NA")
-                    )
-
-                    if endpoint.api_search_supported:
-                        endpoint_item["api_search"] = "Supported"
-                    else:
-                        endpoint_item["api_search"] = "NA"
-                    endpoint_item["link"] = f"`{endpoint.short_name} <{link}>`_"
+                endpoint_item["short_description"] = (
+                    endpoint_item["short_description"] + f" (`instructions <{link}>`_)"
+                )
 
             endpoint_list += package_endpoints["endpoints"][endpoint_type]
 
     def __load_packages_json(self) -> list:
         filedata = colrev.env.utils.get_package_file_content(
             file_path=Path("template/packages.json")
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `colrev-0.8.2/colrev/env/resources.py` & `colrev-0.8.3/colrev/env/resources.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/env/screenshot_service.py` & `colrev-0.8.3/colrev/env/screenshot_service.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/env/tei_parser.py` & `colrev-0.8.3/colrev/env/tei_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 #! /usr/bin/env python
 """Service parsing metadata from PDFs/TEIs (created by GROBID)."""
 from __future__ import annotations
 
 import re
 from pathlib import Path
 from typing import Optional
+from xml import etree
 from xml.etree.ElementTree import Element
 
+import defusedxml
 import requests
-from lxml import etree
+from defusedxml.ElementTree import fromstring
 
 import colrev.env.grobid_service
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.record
 
 # xpath alternative:
 # tree.xpath("//tei:sourceDesc/tei:biblStruct/tei:monogr/tei:idno",
 # namespaces={"tei": "http://www.tei-c.org/ns/1.0"})
 # abstract_node =tree.xpath("//tei:profileDesc/tei:abstract",
 # namespaces={"tei": "http://www.tei-c.org/ns/1.0"})
 # etree.tostring(abstract_node[0]).decode("utf-8")
 
 
+# defuse std xml lib
+defusedxml.defuse_stdlib()
+
+
 class TEIParser:
     """Environment service for TEI parsing"""
 
     ns = {
         "tei": "{http://www.tei-c.org/ns/1.0}",
         "w3": "{http://www.w3.org/XML/1998/namespace}",
     }
@@ -77,27 +83,25 @@
         """Read a TEI from file"""
         with open(self.tei_path, "rb") as data:
             xslt_content = data.read()
 
         if b"[BAD_INPUT_DATA]" in xslt_content[:100]:
             raise colrev_exceptions.TEIException()
 
-        return etree.XML(xslt_content)
+        return etree.ElementTree.XML(xslt_content)
 
     def __create_tei(self) -> None:
         """Create the TEI (based on GROBID)"""
         grobid_service = colrev.env.grobid_service.GrobidService(
             environment_manager=self.environment_manager
         )
         grobid_service.start()
         # Note: we have more control and transparency over the consolidation
         # if we do it in the colrev process
-        options = {}
-        options["consolidateHeader"] = "0"
-        options["consolidateCitations"] = "0"
+        options = {"consolidateHeader": "0", "consolidateCitations": "0"}
 
         # Note: Grobid offers direct export of Bibtex:
         # r = requests.post(
         #     GROBID_SERVICE.GROBID_URL() + "/api/processHeaderDocument",
         #     headers={"Accept": "application/x-bibtex"},
         # But parsing the metadata from the tei gives us more control of the details
 
@@ -119,36 +123,36 @@
 
             if ret.status_code != 200:
                 raise colrev_exceptions.TEIException()
 
             if b"[TIMEOUT]" in ret.content:
                 raise colrev_exceptions.TEITimeoutException()
 
-            self.root = etree.fromstring(ret.content)
+            self.root = fromstring(ret.content)
 
             if self.tei_path is not None:
                 self.tei_path.parent.mkdir(exist_ok=True, parents=True)
                 with open(self.tei_path, "wb") as file:
                     file.write(ret.content)
 
                 # Note : reopen/write to prevent format changes in the enhancement
                 with open(self.tei_path, "rb") as file:
                     xml_fstring = file.read()
-                self.root = etree.fromstring(xml_fstring)
+                self.root = fromstring(xml_fstring)
 
-                tree = etree.ElementTree(self.root)
-                tree.write(str(self.tei_path), pretty_print=True, encoding="utf-8")
+                tree = etree.ElementTree.ElementTree(self.root)
+                tree.write(str(self.tei_path), encoding="utf-8")
         except requests.exceptions.ConnectionError as exc:
             print(exc)
             print(str(self.pdf_path))
 
     def get_tei_str(self) -> str:
         """Get the TEI string"""
-
-        return etree.tostring(self.root).decode("utf-8")
+        etree.ElementTree.register_namespace("tei", "http://www.tei-c.org/ns/1.0")
+        return etree.ElementTree.tostring(self.root).decode("utf-8")
 
     def get_grobid_version(self) -> str:
         """Get the GROBID version used for TEI creation"""
         grobid_version = "NA"
         encoding_description = self.root.find(".//" + self.ns["tei"] + "encodingDesc")
         if encoding_description is not None:
             app_info_node = encoding_description.find(
@@ -193,15 +197,15 @@
                 journal_node = file_description.find(".//" + self.ns["tei"] + "monogr")
                 if journal_node is not None:
                     jtitle_node = journal_node.find(".//" + self.ns["tei"] + "title")
                     if jtitle_node is not None:
                         journal_name = (
                             jtitle_node.text if jtitle_node.text is not None else "NA"
                         )
-                        if "NA" != journal_name:
+                        if journal_name != "NA":
                             words = journal_name.split()
                             if sum(word.isupper() for word in words) / len(words) > 0.8:
                                 words = [word.capitalize() for word in words]
                                 journal_name = " ".join(words)
         return journal_name
 
     def __get_paper_journal_volume(self) -> str:
@@ -401,15 +405,15 @@
 
         abstract_text = "NA"
         profile_description = self.root.find(".//" + self.ns["tei"] + "profileDesc")
         if profile_description is not None:
             abstract_node = profile_description.find(
                 ".//" + self.ns["tei"] + "abstract"
             )
-            html_str = etree.tostring(abstract_node).decode("utf-8")
+            html_str = etree.ElementTree.tostring(abstract_node).decode("utf-8")
             abstract_text = cleanhtml(html_str)
         abstract_text = abstract_text.lstrip().rstrip()
         return abstract_text
 
     def get_metadata(self) -> dict:
         """Get the metadata of the PDF (title, author, ...) as a dict"""
 
@@ -422,15 +426,15 @@
             "volume": self.__get_paper_journal_volume(),
             "number": self.__get_paper_journal_issue(),
             "pages": self.__get_paper_journal_pages(),
             "doi": self.__get_paper_doi(),
         }
 
         for key, value in record.items():
-            if "file" != key:
+            if key != "file":
                 record[key] = value.replace("}", "").replace("{", "").rstrip("\\")
             else:
                 print(f"problem in filename: {key}")
 
         return record
 
     def get_paper_keywords(self) -> list:
@@ -518,15 +522,15 @@
             .replace("~", "")
             .replace("®", "")
             .replace("|", "")
         )
 
         if author_string is None:
             author_string = "NA"
-        if "" == author_string.replace(" ", "").replace(",", "").replace(";", ""):
+        if author_string.replace(" ", "").replace(",", "").replace(";", "") == "":
             author_string = "NA"
         return author_string
 
     def __get_reference_title_string(self, *, reference: Element) -> str:
         title_string = ""
         if reference.find(self.ns["tei"] + "analytic") is not None:
             analytic_node = reference.find(self.ns["tei"] + "analytic")
@@ -664,18 +668,18 @@
     def __get_entrytype(self, *, reference: Element) -> str:
         entrytype = "misc"
         if reference.find(self.ns["tei"] + "monogr") is not None:
             monogr_node = reference.find(self.ns["tei"] + "monogr")
             if monogr_node is not None:
                 title_node = monogr_node.find(self.ns["tei"] + "title")
                 if title_node is not None:
-                    if "j" == title_node.get("level", "NA"):
-                        entrytype = "article"
-                    else:
+                    if title_node.get("level", "NA") != "j":
                         entrytype = "book"
+                    else:
+                        entrytype = "article"
         return entrytype
 
     def __get_tei_id_count(self, *, tei_id: str) -> int:
         count = 0
 
         for reference in self.root.iter(self.ns["tei"] + "ref"):
             if "target" in reference.keys():
@@ -701,15 +705,15 @@
                     if min_intext_citations > 0:
                         if (
                             self.__get_tei_id_count(tei_id=tei_id)
                             < min_intext_citations
                         ):
                             continue
 
-                    if "article" == entrytype:
+                    if entrytype == "article":
                         ref_rec = {
                             "ID": tei_id,
                             "ENTRYTYPE": entrytype,
                             "tei_id": tei_id,
                             "reference_bibliography_id": self.__get_reference_bibliography_id(
                                 reference=reference
                             ),
@@ -731,15 +735,15 @@
                             "number": self.__get_reference_number_string(
                                 reference=reference
                             ),
                             "pages": self.__get_reference_page_string(
                                 reference=reference
                             ),
                         }
-                    elif "book" == entrytype:
+                    elif entrytype == "book":
                         ref_rec = {
                             "ID": tei_id,
                             "ENTRYTYPE": entrytype,
                             "tei_id": tei_id,
                             "reference_bibliography_id": self.__get_reference_bibliography_id(
                                 reference=reference
                             ),
@@ -749,51 +753,53 @@
                             "title": self.__get_reference_title_string(
                                 reference=reference
                             ),
                             "year": self.__get_reference_year_string(
                                 reference=reference
                             ),
                         }
-                    elif "misc" == entrytype:
+                    elif entrytype == "misc":
                         ref_rec = {
                             "ID": tei_id,
                             "ENTRYTYPE": entrytype,
                             "tei_id": tei_id,
                             "reference_bibliography_id": self.__get_reference_bibliography_id(
                                 reference=reference
                             ),
                             "author": self.__get_reference_author_string(
                                 reference=reference
                             ),
                             "title": self.__get_reference_title_string(
                                 reference=reference
                             ),
                         }
-                except etree.XMLSyntaxError:
+                except etree.ElementTree.ParseError:
                     continue
 
                 ref_rec = {k: v for k, v in ref_rec.items() if v is not None}
                 # print(ref_rec)
                 tei_bib_db.append(ref_rec)
 
         return tei_bib_db
 
     def get_citations_per_section(self) -> dict:
         """Get a dict of section-names and list-of-citations"""
         section_citations = {}
-        sections = self.root.iter(self.ns["tei"] + "head")
+        parent_map = {c: p for p in self.root.iter() for c in p}
+        sections = self.root.iter(f'{self.ns["tei"]}head')
         for section in sections:
             section_name = section.text
             if section_name is None:
                 continue
-            citation_nodes = section.getparent().iter(self.ns["tei"] + "ref")
+            parent = parent_map[section]
+            citation_nodes = parent.findall(f'.//{self.ns["tei"]}ref')
             citations = [
                 x.get("target", "NA").replace("#", "")
                 for x in citation_nodes
-                if "bibr" == x.get("type", "NA")
+                if x.get("type", "NA") == "bibr"
             ]
             citations = list(filter(lambda a: a != "NA", citations))
             if len(citations) > 0:
                 section_citations[section_name.lower()] = citations
         return section_citations
 
     def mark_references(self, *, records: dict):  # type: ignore
@@ -819,29 +825,29 @@
                 if rec_sim > max_sim:
                     max_sim_record = local_record_dict
                     max_sim = rec_sim
             if len(max_sim_record) == 0:
                 continue
 
             # Record found: mark in tei
-            bibliography = self.root.find(".//" + self.ns["tei"] + "listBibl")
+            bibliography = self.root.find(f".//{self.ns['tei']}listBibl")
             # mark reference in bibliography
             for ref in bibliography:
-                if ref.get(self.ns["w3"] + "id") == record_dict["tei_id"]:
+                if ref.get(f'{self.ns["w3"]}id') == record_dict["tei_id"]:
                     ref.set("ID", max_sim_record["ID"])
             # mark reference in in-text citations
-            for reference in self.root.iter(self.ns["tei"] + "ref"):
+            for reference in self.root.iter(f'{self.ns["tei"]}ref'):
                 if "target" in reference.keys():
                     if reference.get("target") == f"#{record_dict['tei_id']}":
                         reference.set("ID", max_sim_record["ID"])
 
             # if settings file available: dedupe_io match agains records
 
         if self.tei_path:
-            tree = etree.ElementTree(self.root)
-            tree.write(str(self.tei_path), pretty_print=True, encoding="utf-8")
+            tree = etree.ElementTree.ElementTree(self.root)
+            tree.write(str(self.tei_path))
 
         return self.root
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/env/utils.py` & `colrev-0.8.3/colrev/env/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     with open(filename, "w", encoding="utf8") as file:
         content = content.replace(old_string, new_string)
         file.write(content)
 
 
 def get_template(*, template_path: str) -> Template:
     """Load a jinja template"""
-    environment = Environment(loader=FunctionLoader(__load_jinja_template))
+    environment = Environment(
+        loader=FunctionLoader(__load_jinja_template), autoescape=True
+    )
     template = environment.get_template(template_path)
     return template
 
 
 def __load_jinja_template(template_path: str) -> str:
     filedata_b = pkgutil.get_data("colrev", template_path)
     if filedata_b:
```

### Comparing `colrev-0.8.2/colrev/env/zotero_translation_service.py` & `colrev-0.8.3/colrev/env/zotero_translation_service.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/exceptions.py` & `colrev-0.8.3/colrev/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,18 @@
 # Prep
 
 
 class RecordNotFoundInPrepSourceException(CoLRevException):
     """The record was not found in the prep search source."""
 
 
+class PreparationBreak(CoLRevException):
+    """Event interrupting the preparation."""
+
+
 # Dedupe
 
 
 class DedupeError(CoLRevException):
     """An exception in the dedupe operation"""
 
     def __init__(self, message: str) -> None:
```

### Comparing `colrev-0.8.2/colrev/logger.py` & `colrev-0.8.3/colrev/logger.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/operation.py` & `colrev-0.8.3/colrev/operation.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/bibliography_export.py` & `colrev-0.8.3/colrev/ops/built_in/data/bibliography_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 
 @zope.interface.implementer(colrev.env.package_manager.DataPackageEndpointInterface)
 @dataclass
 class BibliographyExport(JsonSchemaMixin):
     """Export the sample references in Endpoint format"""
 
+    settings: BibliographyExportSettings
+
     ZOTERO_FORMATS = [
         BibFormats.endnote,
         BibFormats.mendeley,
         BibFormats.rdf_bibliontology,
     ]
     PYBTEX_FORMATS = [BibFormats.citavi, BibFormats.jabref, BibFormats.zotero]
 
@@ -157,15 +159,15 @@
         ret = requests.post(
             "http://127.0.0.1:1969/import",
             headers=headers,
             files={"file": str.encode(content)},
             timeout=30,
         )
         headers = {"Content-type": "application/json"}
-        if "No suitable translators found" == ret.content.decode("utf-8"):
+        if ret.content.decode("utf-8") == "No suitable translators found":
             raise colrev_exceptions.ImportException(
                 "Zotero translators: No suitable translators found"
             )
 
         try:
             json_content = json.loads(ret.content)
             export = requests.post(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/colrev_curation.md` & `colrev-0.8.3/colrev/ops/built_in/data/colrev_curation.md`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/colrev_curation.py` & `colrev-0.8.3/colrev/ops/built_in/data/colrev_curation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
 import colrev.record
 
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.data
 
 
 @zope.interface.implementer(colrev.env.package_manager.DataPackageEndpointInterface)
 @dataclass
 class ColrevCuration(JsonSchemaMixin):
     """CoLRev Curation"""
 
+    settings: ColrevCurationSettings
     ci_supported: bool = True
 
     @dataclass
     class ColrevCurationSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Colrev Curation settings"""
@@ -184,15 +186,14 @@
 
     def __update_table_in_readme(
         self,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         markdown_output: str,
     ) -> None:
-        # pylint: disable=duplicate-code
         table_summary_tag = "<!-- TABLE_SUMMARY -->"
         readme_path = review_manager.readme
         with open(readme_path, "r+b") as file:
             appended = False
             seekpos = file.tell()
             line = file.readline()
             while line:
@@ -345,26 +346,32 @@
 
         identical_colrev_ids: typing.Dict[str, list] = {}
         non_identifiable_records = []
         for record_dict in records.values():
             try:
                 if record_dict[
                     "colrev_status"
-                ] in colrev.record.RecordState.get_post_x_states(
+                ] not in colrev.record.RecordState.get_post_x_states(
                     state=colrev.record.RecordState.md_prepared
                 ):
-                    cid = colrev.record.Record(data=record_dict).create_colrev_id(
-                        assume_complete=True
-                    )
-                    if cid in identical_colrev_ids:
-                        identical_colrev_ids[cid] = identical_colrev_ids[cid] + [
-                            record_dict["ID"]
-                        ]
-                    else:
-                        identical_colrev_ids[cid] = [record_dict["ID"]]
+                    continue
+                if (
+                    record_dict["colrev_status"]
+                    == colrev.record.RecordState.rev_prescreen_excluded
+                ):
+                    continue
+                cid = colrev.record.Record(data=record_dict).create_colrev_id(
+                    assume_complete=True
+                )
+                if cid in identical_colrev_ids:
+                    identical_colrev_ids[cid] = identical_colrev_ids[cid] + [
+                        record_dict["ID"]
+                    ]
+                else:
+                    identical_colrev_ids[cid] = [record_dict["ID"]]
             except colrev_exceptions.NotEnoughDataToIdentifyException:
                 non_identifiable_records.append(record_dict["ID"])
 
         identical_colrev_ids = {
             k: v for k, v in identical_colrev_ids.items() if len(v) > 1
         }
         if identical_colrev_ids:
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/github_pages.py` & `colrev-0.8.3/colrev/ops/built_in/data/github_pages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 #! /usr/bin/env python
 """Creation of a github-page for the review as part of the data operations"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 
+import git
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.env.utils
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
 
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.data
-        import git
 
 
 @zope.interface.implementer(colrev.env.package_manager.DataPackageEndpointInterface)
 @dataclass
 class GithubPages(JsonSchemaMixin):
     """Export the literature review into a Github Page"""
 
+    settings: GHPagesSettings
+
     ci_supported: bool = False
 
     @dataclass
     class GHPagesSettings(colrev.env.package_manager.DefaultSettings, JsonSchemaMixin):
         """Settings for GithubPages"""
 
         endpoint: str
@@ -72,90 +75,120 @@
 
         return github_pages_endpoint_details
 
     def __setup_github_pages_branch(
         self, *, data_operation: colrev.ops.data.Data, git_repo: git.Repo
     ) -> None:
         # if branch does not exist: create and add index.html
-        data_operation.review_manager.logger.info("Setup github pages")
-        git_repo.create_head(self.GH_PAGES_BRANCH_NAME)
-        git_repo.git.checkout(self.GH_PAGES_BRANCH_NAME)
-        title = "Manuscript template"
-        readme_file = data_operation.review_manager.readme
-        if readme_file.is_file():
-            with open(readme_file, encoding="utf-8") as file:
-                title = file.readline()
-                title = title.replace("# ", "").replace("\n", "")
-                title = '"' + title + '"'
+        data_operation.review_manager.logger.info("Setup gh-pages branch")
+        git_repo.git.checkout("--orphan", self.GH_PAGES_BRANCH_NAME)
         git_repo.git.rm("-rf", Path("."))
 
-        gitignore_file = Path(".gitignore")
-        git_repo.git.checkout("HEAD", "--", gitignore_file)
-        with gitignore_file.open("a", encoding="utf-8") as file:
-            file.write("status.yaml\n")
-        data_operation.review_manager.dataset.add_changes(path=gitignore_file)
+        colrev.env.utils.retrieve_package_file(
+            template_file=Path("template/github_pages/README.md"),
+            target=Path("README.md"),
+        )
+        project_title = data_operation.review_manager.settings.project.title
+        colrev.env.utils.inplace_change(
+            filename=Path("README.md"),
+            old_string="{{project_title}}",
+            new_string=project_title.rstrip(" ").capitalize(),
+        )
+        data_operation.review_manager.dataset.add_changes(path=Path("README.md"))
 
         colrev.env.utils.retrieve_package_file(
             template_file=Path("template/github_pages/index.html"),
             target=Path("index.html"),
         )
         data_operation.review_manager.dataset.add_changes(path=Path("index.html"))
+
         colrev.env.utils.retrieve_package_file(
             template_file=Path("template/github_pages/_config.yml"),
             target=Path("_config.yml"),
         )
         colrev.env.utils.inplace_change(
             filename=Path("_config.yml"),
             old_string="{{project_title}}",
-            new_string=title,
+            new_string=project_title,
         )
         data_operation.review_manager.dataset.add_changes(path=Path("_config.yml"))
+
         colrev.env.utils.retrieve_package_file(
             template_file=Path("template/github_pages/about.md"),
             target=Path("about.md"),
         )
         data_operation.review_manager.dataset.add_changes(path=Path("about.md"))
 
+        data_operation.review_manager.create_commit(
+            msg="Setup gh-pages branch", skip_status_yaml=True
+        )
+
     def __update_data(
-        self, *, data_operation: colrev.ops.data.Data, silent_mode: bool
+        self,
+        *,
+        data_operation: colrev.ops.data.Data,
+        git_repo: git.Repo,
+        silent_mode: bool,
     ) -> None:
         if not silent_mode:
             data_operation.review_manager.logger.info("Update data on github pages")
+
         records = data_operation.review_manager.dataset.load_records_dict()
 
-        # pylint: disable=duplicate-code
         included_records = {
             r["ID"]: r
             for r in records.values()
             if r["colrev_status"]
             in [
                 colrev.record.RecordState.rev_synthesized,
                 colrev.record.RecordState.rev_included,
             ]
         }
+
+        git_repo.git.checkout(self.GH_PAGES_BRANCH_NAME)
+        if not Path("pre-commit-config.yaml").is_file():
+            colrev.env.utils.retrieve_package_file(
+                template_file=Path("template/github_pages/pre-commit-config.yaml"),
+                target=Path(".pre-commit-config.yaml"),
+            )
+            data_operation.review_manager.dataset.add_changes(
+                path=Path(".pre-commit-config.yaml")
+            )
+
         data_file = Path("data.bib")
         data_operation.review_manager.dataset.save_records_dict_to_file(
             records=included_records, save_path=data_file
         )
         data_operation.review_manager.dataset.add_changes(path=data_file)
 
-        data_operation.review_manager.create_commit(msg="Update sample")
+        data_operation.review_manager.create_commit(
+            msg="Update sample", skip_status_yaml=True
+        )
 
     def __push_branch(
         self,
         *,
         data_operation: colrev.ops.data.Data,
         git_repo: git.Repo,
         silent_mode: bool,
     ) -> None:
         if not silent_mode:
             data_operation.review_manager.logger.info("Push to github pages")
         if "origin" in git_repo.remotes:
             if "origin/gh-pages" in [r.name for r in git_repo.remotes.origin.refs]:
-                git_repo.git.push("origin", self.GH_PAGES_BRANCH_NAME, "--no-verify")
+                try:
+                    git_repo.remotes.origin.push(
+                        refspec=f"{self.GH_PAGES_BRANCH_NAME}:{self.GH_PAGES_BRANCH_NAME}"
+                    )
+                except git.exc.GitCommandError:  # pylint: disable=no-member
+                    data_operation.review_manager.logger.error(
+                        "Could not push branch gh-pages. Please resolve manually, i.e., run "
+                        f"{colors.ORANGE}git switch gh-pages && "
+                        f"git pull --rebase && git push{colors.END}"
+                    )
             else:
                 git_repo.git.push(
                     "--set-upstream",
                     "origin",
                     self.GH_PAGES_BRANCH_NAME,
                     "--no-verify",
                 )
@@ -176,32 +209,36 @@
     def __check_gh_pages_setup(self, *, git_repo: git.Repo) -> None:
         username, project = (
             git_repo.remotes.origin.url.replace("https://github.com/", "")
             .replace(".git", "")
             .split("/")
         )
         gh_page_link = f"https://{username}.github.io/{project}/"
-        if gh_page_link not in (self.review_manager.path / Path("readme.md")).read_text(
-            encoding="utf-8"
-        ):
-            print(
-                f"{colors.ORANGE}The Github page is not yet linked in the readme.md file.\n"
-                "To make it easier to access the page, add the following to the readme.md file:\n"
-                f"\n    [Github page]({gh_page_link}){colors.END}\n"
-            )
+        if Path("readme.md").is_file():
+            if gh_page_link in (self.review_manager.path / Path("readme.md")).read_text(
+                encoding="utf-8"
+            ):
+                return
+        print(
+            f"{colors.ORANGE}The Github page is not yet linked in the readme.md file.\n"
+            "To make it easier to access the page, add the following to the readme.md file:\n"
+            f"\n    [Github page]({gh_page_link}){colors.END}\n"
+        )
 
     def update_data(
         self,
         data_operation: colrev.ops.data.Data,
         records: dict,  # pylint: disable=unused-argument
         synthesized_record_status_matrix: dict,  # pylint: disable=unused-argument
         silent_mode: bool,
     ) -> None:
         """Update the data/github pages"""
 
+        # pylint: disable=too-many-branches
+
         if data_operation.review_manager.in_ci_environment():
             data_operation.review_manager.logger.error(
                 "Running in CI environment. Skipping github-pages generation."
             )
             return
 
         if data_operation.review_manager.dataset.has_changes():
@@ -209,26 +246,92 @@
                 "Cannot update github pages because there are uncommited changes."
             )
             return
 
         git_repo = data_operation.review_manager.dataset.get_repo()
         active_branch = git_repo.active_branch
 
-        if self.GH_PAGES_BRANCH_NAME not in [h.name for h in git_repo.heads]:
-            self.__setup_github_pages_branch(
-                data_operation=data_operation, git_repo=git_repo
-            )
+        # check if there is an "origin" remote
 
-        self.__check_gh_pages_setup(git_repo=git_repo)
-        git_repo.git.checkout(self.GH_PAGES_BRANCH_NAME)
+        if "origin" in git_repo.remotes:
+            # check if remote.origin has a gh-pages branch
+            git_repo.remotes.origin.fetch()
+            if f"origin/{self.GH_PAGES_BRANCH_NAME}" in [
+                r.name for r in git_repo.remotes.origin.refs
+            ]:
+                try:
+                    if "origin/gh-pages" not in [
+                        r.name for r in git_repo.remotes.origin.refs
+                    ]:
+                        git_repo.git.push(
+                            "--set-upstream",
+                            "origin",
+                            self.GH_PAGES_BRANCH_NAME,
+                            "--no-verify",
+                        )
+                    else:
+                        git_repo.remotes.origin.pull(ff_only=True)
+
+                    # update
+                    git_repo.git.checkout(active_branch)
+                    self.__update_data(
+                        data_operation=data_operation,
+                        git_repo=git_repo,
+                        silent_mode=silent_mode,
+                    )
+
+                    # Push gh-pages branch to remote origin
+                    if self.settings.auto_push:
+                        self.__push_branch(
+                            data_operation=data_operation,
+                            git_repo=git_repo,
+                            silent_mode=silent_mode,
+                        )
+                except git.exc.GitCommandError as exc:  # pylint: disable=no-member
+                    print("Error in gh-pages:")
+                    print(exc)
+                    return
+            else:
+                # create branch
+                if self.GH_PAGES_BRANCH_NAME not in [h.name for h in git_repo.heads]:
+                    self.__setup_github_pages_branch(
+                        data_operation=data_operation, git_repo=git_repo
+                    )
+
+                # update
+                git_repo.git.checkout(active_branch)
+                self.__update_data(
+                    data_operation=data_operation,
+                    git_repo=git_repo,
+                    silent_mode=silent_mode,
+                )
 
-        self.__update_data(data_operation=data_operation, silent_mode=silent_mode)
+                # Push gh-pages branch to remote origin
+                if self.settings.auto_push:
+                    self.__push_branch(
+                        data_operation=data_operation,
+                        git_repo=git_repo,
+                        silent_mode=silent_mode,
+                    )
+            git_repo.git.checkout(active_branch)
+            self.__check_gh_pages_setup(git_repo=git_repo)
+        else:
+            data_operation.review_manager.logger.warning(
+                "Cannot push github pages because there is no remote origin. "
+                "gh-pages branch will only be created locally."
+            )
+            # create branch
+            if self.GH_PAGES_BRANCH_NAME not in [h.name for h in git_repo.heads]:
+                self.__setup_github_pages_branch(
+                    data_operation=data_operation, git_repo=git_repo
+                )
 
-        if self.settings.auto_push:
-            self.__push_branch(
+            # update
+            git_repo.git.checkout(active_branch)
+            self.__update_data(
                 data_operation=data_operation,
                 git_repo=git_repo,
                 silent_mode=silent_mode,
             )
 
         git_repo.git.checkout(active_branch)
 
@@ -249,15 +352,15 @@
         review_manager: colrev.review_manager.ReviewManager,
     ) -> dict:
         """Get advice on the next steps (for display in the colrev status)"""
 
         data_endpoint = "Data operation [github pages data endpoint]: "
 
         advice = {"msg": f"{data_endpoint}", "detailed_msg": "TODO"}
-        if "NA" == review_manager.dataset.get_remote_url():
+        if review_manager.dataset.get_remote_url() == "NA":
             advice["msg"] += (
                 "\n    - To make the repository available on Github pages, "
                 + "push it to a Github repository\nhttps://github.com/new"
             )
         else:
             advice[
                 "msg"
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/obsidian.py` & `colrev-0.8.3/colrev/ops/built_in/data/obsidian.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.data
 
-# pylint: disable=duplicate-code
-
 
 @zope.interface.implementer(colrev.env.package_manager.DataPackageEndpointInterface)
 @dataclass
 class Obsidian(JsonSchemaMixin):
     """Export the sample into an Obsidian database"""
 
     ci_supported: bool = False
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/paper_md.py` & `colrev-0.8.3/colrev/ops/built_in/data/paper_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import colrev.env.package_manager
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
 
-# pylint: disable=duplicate-code
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.data
 
 
@@ -200,15 +200,15 @@
         git_repo = self.data_operation.review_manager.dataset.get_repo()
         try:
             commits_list = list(git_repo.iter_commits())
             commits_authors = []
 
             for commit in commits_list:
                 committer = git_repo.git.show("-s", "--format=%cn", commit.hexsha)
-                if "GitHub" == committer:
+                if committer == "GitHub":
                     continue
                 commits_authors.append(committer)
                 # author = git_repo.git.show("-s", "--format=%an", commit.hexsha)
                 # mail = git_repo.git.show("-s", "--format=%ae", commit.hexsha)
             author = ", ".join(dict(Counter(commits_authors)))
         except ValueError:
             author, _ = self.data_operation.review_manager.get_committer()
@@ -281,24 +281,24 @@
                             f"Added to {paper_path.name}".ljust(24)
                             + f"{nr_records_added}".rjust(15, " ")
                             + " records"
                         )
 
                     # skip empty lines between to connect lists
                     line = reader.readline()
-                    if "\n" != line:
+                    if line != "\n":
                         writer.write(line)
 
                     appended = True
 
                 elif appended and not completed:
-                    if "- @" == line[:3]:
+                    if line[:3] == "- @":
                         writer.write(line)
                     else:
-                        if "\n" != line:
+                        if line != "\n":
                             writer.write("\n")
                         writer.write(line)
                         completed = True
                 else:
                     writer.write(line)
                 line = reader.readline()
 
@@ -616,15 +616,14 @@
                 )
             except AttributeError:
                 pass
 
     def __call_docker_build_process(
         self, *, data_operation: colrev.ops.data.Data, script: str
     ) -> None:
-        # pylint: disable=duplicate-code
         try:
             uid = os.stat(data_operation.review_manager.dataset.records_file).st_uid
             gid = os.stat(data_operation.review_manager.dataset.records_file).st_gid
             user = f"{uid}:{gid}"
 
             client = docker.from_env()
             msg = f"Running docker container created from image {self.pandoc_image}"
@@ -795,17 +794,17 @@
     ) -> dict:
         """Get advice on the next steps (for display in the colrev status)"""
 
         data_endpoint = "Data operation [paper_md endpoint]: "
 
         advice = {
             "msg": f"{data_endpoint}"
-            + "\n    1. Edit the paper (data/paper.md)"
+            + "\n    1. Edit the paper (data/data/paper.md)"
             + "\n    2. To build the paper (output/paper.docx), run: colrev data"
-            + "\n    3. To create a version, run: git add data/paper.md && "
+            + "\n    3. To create a version, run: git add data/data/paper.md && "
             + "git commit -m 'update paper'",
             "detailed_msg": "... with a link to the docs etc.",
         }
         return advice
 
 
 class PaperMarkdownRecordSourceTagError(Exception):
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/prisma.py` & `colrev-0.8.3/colrev/ops/built_in/data/prisma.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from docker.errors import DockerException
 
 import colrev.env.package_manager
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
 import colrev.record
 
-# pylint: disable=duplicate-code
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.data
 
 
@@ -178,15 +178,14 @@
                 data_operation=data_operation, script=script
             )
             csv_relative_path.unlink()
 
     def __call_docker_build_process(
         self, *, data_operation: colrev.ops.data.Data, script: str
     ) -> None:
-        # pylint: disable=duplicate-code
         try:
             uid = os.stat(data_operation.review_manager.settings_path).st_uid
             gid = os.stat(data_operation.review_manager.settings_path).st_gid
             user = f"{uid}:{gid}"
 
             client = docker.from_env()
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/data/structured.py` & `colrev-0.8.3/colrev/ops/built_in/data/structured.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 @zope.interface.implementer(colrev.env.package_manager.DataPackageEndpointInterface)
 @dataclass
 class StructuredData(JsonSchemaMixin):
     """Summarize the literature in a structured data extraction (a table)"""
 
+    settings: StructuredDataSettings
     ci_supported: bool = False
 
     @dataclass
     class StructuredDataSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Settings for StructuredData"""
@@ -151,15 +152,21 @@
         print(self.__FULL_DATA_FIELD_EXPLANATION)
         while "y" == input("Add a data field [y,n]?"):
             short_name = input("Provide a short name: ")
             explanation = input("Provide a short explanation: ")
             data_type = input("Provide the data type (str, int, double):")
 
             self.settings.fields.append(
-                {"name": short_name, "explanation": explanation, "data_type": data_type}
+                Field(
+                    **{
+                        "name": short_name,
+                        "explanation": explanation,
+                        "data_type": data_type,
+                    }
+                )
             )
 
             print()
 
         # Note : the following should be easier...
         for i, candidate in enumerate(
             self.review_manager.settings.data.data_package_endpoints
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/dedupe/active_learning_dedup_io.py` & `colrev-0.8.3/colrev/ops/built_in/dedupe/active_learning_dedup_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 
 @zope.interface.implementer(colrev.env.package_manager.DedupePackageEndpointInterface)
 @dataclass
 class ActiveLearningDedupeTraining(JsonSchemaMixin):
     """Active learning: training phase (minimum sample size of 50 required)"""
 
+    # pylint: disable=too-many-instance-attributes
+
+    __n_match: int
+    __n_distinct: int
+    __manual: bool
+
     settings_class = colrev.env.package_manager.DefaultSettings
     TRAINING_FILE_RELATIVE = Path(".records_dedupe_training.json")
     SETTINGS_FILE_RELATIVE = Path(".records_learned_settings")
 
     deduper: dedupe_io.Deduper
 
     ci_supported: bool = False
@@ -64,20 +70,23 @@
         self.training_file = (
             dedupe_operation.review_manager.path / self.TRAINING_FILE_RELATIVE
         )
         self.settings_file = (
             dedupe_operation.review_manager.path / self.SETTINGS_FILE_RELATIVE
         )
 
+        self.local_index = dedupe_operation.review_manager.get_local_index()
+        self.review_manager = dedupe_operation.review_manager
+
         if hasattr(dedupe_operation.review_manager, "dataset"):
             dedupe_operation.review_manager.dataset.update_gitignore(
                 add=[self.SETTINGS_FILE_RELATIVE]
             )
 
-    def __setup_active_learning_dedupe(
+    def setup_active_learning_dedupe(
         self,
         *,
         dedupe_operation: colrev.ops.dedupe.Dedupe,
         retrain: bool,
         in_memory: bool,
     ) -> None:
         """Prepare data for active learning setup"""
@@ -240,20 +249,21 @@
 
     def __get_nr_duplicates(self, *, result_list: list) -> int:
         return len([i for i in result_list if "duplicate" == i["decision"]])
 
     def __get_nr_non_duplicates(self, *, result_list: list) -> int:
         return len([i for i in result_list if "no_duplicate" == i["decision"]])
 
-    def __apply_active_learning(
+    def apply_active_learning(
         self,
         *,
         dedupe_operation: colrev.ops.dedupe.Dedupe,
         results: list,
     ) -> None:
+        """Apply the active learning results"""
         if (
             self.__get_nr_duplicates(result_list=results) > 10
             and self.__get_nr_non_duplicates(result_list=results) > 10
         ):
             dedupe_operation.apply_merges(results=results, complete_dedupe=False)
 
             dedupe_operation.review_manager.logger.info("Training deduper.")
@@ -299,201 +309,285 @@
                     )
                     return
 
         if (
             self.__get_nr_duplicates(result_list=results) == 0
             and self.__get_nr_non_duplicates(result_list=results) > 100
         ):
-            if "y" == input("Set remaining records to md_processed (no duplicates)?"):
+            if input("Set remaining records to md_processed (no duplicates)?") == "y":
                 dedupe_operation.apply_merges(results=results, complete_dedupe=True)
                 dedupe_operation.review_manager.create_commit(
                     msg="Set remaining records to non-duplicated",
                     manual_author=True,
                 )
 
-    def __adapted_console_label(
+    def __get_record_pair_for_labeling(
         self,
         *,
-        dedupe_operation: colrev.ops.dedupe.Dedupe,
-        manual: bool,
-        max_associations_to_check: int = 1000,
-    ) -> None:
-        """
-        Train a matcher instance (Dedupe, RecordLink, or Gazetteer) from the cli.
-        Example
-
-        .. code:: python
+        use_previous: bool,
+        examples_buffer: list,
+        uncertain_pairs: list[TrainingExample],
+    ) -> TrainingExample:
+        if use_previous:
+            record_pair, _ = examples_buffer.pop(0)
+        else:
+            # try:
+            if not uncertain_pairs:
+                uncertain_pairs = self.deduper.uncertain_pairs()
+
+            record_pair = uncertain_pairs.pop()
+            # except IndexError:
+            #     break
+        return record_pair
+
+    def __identical_colrev_ids(self, *, record_pair: TrainingExample) -> bool:
+        # if any of the colrev_ids NA,
+        # we don't know whether we have a duplicate.
+        return (
+            record_pair[0]["colrev_id"] == record_pair[1]["colrev_id"]
+            and "NA" != record_pair[0]["colrev_id"]
+            and "NA" != record_pair[1]["colrev_id"]
+        )
 
-        > deduper = dedupe.Dedupe(variables)
-        > deduper.prepare_training(data)
-        > dedupe.console_label(deduper)
-        """
+    def __active_label_duplicate(
+        self,
+        *,
+        manual_dedupe_decision_list: typing.List[dict],
+        record_pair: TrainingExample,
+        examples_buffer: list[
+            tuple[TrainingExample, typing.Literal["match", "distinct", "uncertain"]]
+        ],
+    ) -> None:
+        manual_dedupe_decision_list.append(
+            {
+                "ID1": record_pair[0]["ID"],
+                "ID2": record_pair[1]["ID"],
+                "decision": "duplicate",
+            }
+        )
+        examples_buffer.insert(0, (record_pair, "match"))
+        msg = (
+            f"Marked as duplicate: {record_pair[0]['ID']} - "
+            + f"{record_pair[1]['ID']}"
+        )
+        self.review_manager.report_logger.info(msg)
 
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-        # pylint: disable=too-many-locals
+    def __active_label_no_duplicate(
+        self,
+        *,
+        manual_dedupe_decision_list: typing.List[dict],
+        record_pair: TrainingExample,
+        examples_buffer: list,
+    ) -> None:
+        if not self.__manual:
+            # Ensure that non-dupes do not exceed 3x dupes
+            # (for balanced training data)
+            if self.__n_distinct > self.__n_match * 3:
+                examples_buffer.insert(0, (record_pair, "uncertain"))
+                # continue
 
-        dedupe_operation.review_manager.logger.info(
-            "Note: duplicate associations available in the LocalIndex "
-            "are applied automatically."
+        manual_dedupe_decision_list.append(
+            {
+                "ID1": record_pair[0]["ID"],
+                "ID2": record_pair[1]["ID"],
+                "decision": "no_duplicate",
+            }
         )
-        dedupe_operation.review_manager.logger.info("Press Enter to start.")
-        input()
+        examples_buffer.insert(0, (record_pair, "distinct"))
+        msg = (
+            f"Marked as non-duplicate: {record_pair[0]['ID']}"
+            + f" - {record_pair[1]['ID']}"
+        )
+        self.review_manager.report_logger.info(msg)
 
-        local_index = dedupe_operation.review_manager.get_local_index()
-        finished, use_previous = False, False
+    def __active_label_uncertain(
+        self, *, examples_buffer: list, record_pair: TrainingExample
+    ) -> None:
+        examples_buffer.insert(0, (record_pair, "uncertain"))
 
-        keys = unique(
-            field.field for field in self.deduper.data_model.primary_variables
+    def __active_label_check_finished(
+        self, *, manual_dedupe_decision_list: list
+    ) -> bool:
+        nr_duplicates = self.__get_nr_duplicates(
+            result_list=manual_dedupe_decision_list
+        )
+        nr_non_duplicates = self.__get_nr_non_duplicates(
+            result_list=manual_dedupe_decision_list
         )
+        if not nr_duplicates > 30 or not nr_non_duplicates > 30:
+            if "y" != input(
+                "The machine-learning requires "
+                "30 duplicates and 30 non-duplicates. "
+                "Quit anyway [y,n]?"
+            ):
+                return False
+        os.system("cls" if os.name == "nt" else "clear")
+        print("Finished labeling")
+        return True
+
+    def __check_finised_labeling(
+        self, *, examples_buffer: list, max_associations_to_check: int
+    ) -> bool:
+        self.__n_match = len(self.deduper.training_pairs["match"]) + sum(
+            label == "match" for _, label in examples_buffer
+        )
+        self.__n_distinct = len(self.deduper.training_pairs["distinct"]) + sum(
+            label == "distinct" for _, label in examples_buffer
+        )
+        if (self.__n_match + self.__n_distinct) > max_associations_to_check:
+            return True
+        return False
+
+    def __mark_active_labeling_pairs(self, *, examples_buffer: list) -> None:
+        if len(examples_buffer) > 1:  # Max number of previous operations
+            record_pair, label = examples_buffer.pop()
+            if label in {"distinct", "match"}:
+                examples: TrainingData = {"distinct": [], "match": []}
+                examples[label].append(record_pair)
+                self.deduper.mark_pairs(examples)
 
-        buffer_len = 1  # Max number of previous operations
+    def __adapted_console_label_active_label(
+        self,
+        *,
+        manual_dedupe_decision_list: list,
+        max_associations_to_check: int,
+        keys: list,
+        uncertain_pairs: list,
+    ) -> list[tuple[TrainingExample, typing.Literal["match", "distinct", "uncertain"]]]:
         examples_buffer: list[
             tuple[TrainingExample, typing.Literal["match", "distinct", "uncertain"]]
         ] = []
-        uncertain_pairs: list[TrainingExample] = []
-
-        manual_dedupe_decision_list = []
+        finished, use_previous = False, False
 
         while not finished:
+            record_pair = self.__get_record_pair_for_labeling(
+                use_previous=use_previous,
+                examples_buffer=examples_buffer,
+                uncertain_pairs=uncertain_pairs,
+            )
             if use_previous:
-                record_pair, _ = examples_buffer.pop(0)
                 use_previous = False
-            else:
-                try:
-                    if not uncertain_pairs:
-                        uncertain_pairs = self.deduper.uncertain_pairs()
-
-                    record_pair = uncertain_pairs.pop()
-                except IndexError:
-                    break
 
-            n_match = len(self.deduper.training_pairs["match"]) + sum(
-                label == "match" for _, label in examples_buffer
+            finished = self.__check_finised_labeling(
+                examples_buffer=examples_buffer,
+                max_associations_to_check=max_associations_to_check,
             )
-            n_distinct = len(self.deduper.training_pairs["distinct"]) + sum(
-                label == "distinct" for _, label in examples_buffer
-            )
-            if (n_match + n_distinct) > max_associations_to_check:
-                finished = True
 
             user_input = "u"
-            if (
-                record_pair[0]["colrev_id"] == record_pair[1]["colrev_id"]
-                # if any of the colrev_ids NA,
-                # we don't know whether we have a duplicate.
-                and "NA" != record_pair[0]["colrev_id"]
-                and "NA" != record_pair[1]["colrev_id"]
-            ):
+            if self.__identical_colrev_ids(record_pair=record_pair):
                 user_input = "y"
             else:
                 # Check local_index for duplicate information
-                curations_dupe_info = local_index.is_duplicate(
+                curations_dupe_info = self.local_index.is_duplicate(
                     record1_colrev_id=record_pair[0]["colrev_id"].split(";"),
                     record2_colrev_id=record_pair[1]["colrev_id"].split(";"),
                 )
 
                 user_input = (
                     colrev.ops.built_in.dedupe.utils.console_duplicate_instance_label(
                         record_pair,
                         keys,
-                        manual,
+                        self.__manual,
                         curations_dupe_info,
-                        n_match,
-                        n_distinct,
+                        self.__n_match,
+                        self.__n_distinct,
                         examples_buffer,
                     )
                 )
 
             if user_input == "y":
-                manual_dedupe_decision_list.append(
-                    {
-                        "ID1": record_pair[0]["ID"],
-                        "ID2": record_pair[1]["ID"],
-                        "decision": "duplicate",
-                    }
-                )
-                examples_buffer.insert(0, (record_pair, "match"))
-                msg = (
-                    f"Marked as duplicate: {record_pair[0]['ID']} - "
-                    + f"{record_pair[1]['ID']}"
+                self.__active_label_duplicate(
+                    manual_dedupe_decision_list=manual_dedupe_decision_list,
+                    record_pair=record_pair,
+                    examples_buffer=examples_buffer,
                 )
-                dedupe_operation.review_manager.report_logger.info(msg)
 
             elif user_input == "n":
-                if not manual:
-                    # Ensure that non-dupes do not exceed 3x dupes
-                    # (for balanced training data)
-                    if n_distinct > n_match * 3:
-                        examples_buffer.insert(0, (record_pair, "uncertain"))
-                        continue
-
-                manual_dedupe_decision_list.append(
-                    {
-                        "ID1": record_pair[0]["ID"],
-                        "ID2": record_pair[1]["ID"],
-                        "decision": "no_duplicate",
-                    }
+                self.__active_label_no_duplicate(
+                    manual_dedupe_decision_list=manual_dedupe_decision_list,
+                    record_pair=record_pair,
+                    examples_buffer=examples_buffer,
                 )
-                examples_buffer.insert(0, (record_pair, "distinct"))
-                msg = (
-                    f"Marked as non-duplicate: {record_pair[0]['ID']}"
-                    + f" - {record_pair[1]['ID']}"
-                )
-                dedupe_operation.review_manager.report_logger.info(msg)
 
             elif user_input == "u":
-                examples_buffer.insert(0, (record_pair, "uncertain"))
+                self.__active_label_uncertain(
+                    examples_buffer=examples_buffer, record_pair=record_pair
+                )
 
             elif user_input == "f":
-                nr_duplicates = self.__get_nr_duplicates(
-                    result_list=manual_dedupe_decision_list
+                finished = self.__active_label_check_finished(
+                    manual_dedupe_decision_list=manual_dedupe_decision_list
                 )
-                nr_non_duplicates = self.__get_nr_non_duplicates(
-                    result_list=manual_dedupe_decision_list
-                )
-
-                if not nr_duplicates > 30 or not nr_non_duplicates > 30:
-                    if "y" != input(
-                        "The machine-learning requires "
-                        "30 duplicates and 30 non-duplicates. "
-                        "Quit anyway [y,n]?"
-                    ):
-                        continue
-                os.system("cls" if os.name == "nt" else "clear")
-                print("Finished labeling")
-                finished = True
+                if not finished:
+                    continue
 
             elif user_input == "p":
                 use_previous = True
                 uncertain_pairs.append(record_pair)
 
-            if len(examples_buffer) > buffer_len:
-                record_pair, label = examples_buffer.pop()
-                if label in {"distinct", "match"}:
-                    examples: TrainingData = {"distinct": [], "match": []}
-                    examples[label].append(record_pair)
-                    self.deduper.mark_pairs(examples)
+            self.__mark_active_labeling_pairs(examples_buffer=examples_buffer)
+
+        return examples_buffer
+
+    def __adapted_console_label(
+        self,
+        *,
+        dedupe_operation: colrev.ops.dedupe.Dedupe,
+        manual: bool,
+        max_associations_to_check: int = 1000,
+    ) -> None:
+        """
+        Train a matcher instance (Dedupe, RecordLink, or Gazetteer) from the cli.
+        Example
+
+        .. code:: python
+
+        > deduper = dedupe.Dedupe(variables)
+        > deduper.prepare_training(data)
+        > dedupe.console_label(deduper)
+        """
+
+        dedupe_operation.review_manager.logger.info(
+            "Note: duplicate associations available in the LocalIndex "
+            "are applied automatically."
+        )
+        dedupe_operation.review_manager.logger.info("Press Enter to start.")
+        input()
+        self.__manual = manual
+
+        keys = unique(
+            field.field for field in self.deduper.data_model.primary_variables
+        )
+
+        uncertain_pairs: list[TrainingExample] = []
+        manual_dedupe_decision_list: typing.List[dict] = []
+
+        examples_buffer = self.__adapted_console_label_active_label(
+            manual_dedupe_decision_list=manual_dedupe_decision_list,
+            max_associations_to_check=max_associations_to_check,
+            keys=keys,
+            uncertain_pairs=uncertain_pairs,
+        )
 
         for record_pair, label in examples_buffer:
             if label in ["distinct", "match"]:
-                examples = {"distinct": [], "match": []}
+                examples: typing.Dict[str, list] = {"distinct": [], "match": []}
                 examples[label].append(record_pair)
                 self.deduper.mark_pairs(examples)
 
         # Note : for debugging:
         # import csv
         # keys = manual_dedupe_decision_list[0].keys()
         # with open("manual_dedupe_decision_list.csv", "w", newline="") as output_file:
         #     dict_writer = csv.DictWriter(output_file, keys)
         #     dict_writer.writeheader()
         #     dict_writer.writerows(manual_dedupe_decision_list)
 
         # Apply and commit
-        self.__apply_active_learning(
+        self.apply_active_learning(
             dedupe_operation=dedupe_operation,
             results=manual_dedupe_decision_list,
         )
 
     def run_dedupe(self, dedupe_operation: colrev.ops.dedupe.Dedupe) -> None:
         """Run the console labeling to train the active learning model"""
 
@@ -501,27 +595,28 @@
         records_headers = dedupe_operation.review_manager.dataset.load_records_dict(
             header_only=True
         )
         sample_size = len(list(records_headers.values()))
         ram = psutil.virtual_memory().total
         in_memory = sample_size * 5000000 < ram
 
-        self.__setup_active_learning_dedupe(
+        self.setup_active_learning_dedupe(
             dedupe_operation=dedupe_operation, retrain=False, in_memory=in_memory
         )
 
         dedupe_io.console_label = self.__adapted_console_label
         dedupe_io.console_label(dedupe_operation=dedupe_operation, manual=True)
 
 
 @zope.interface.implementer(colrev.env.package_manager.DedupePackageEndpointInterface)
 @dataclass
 class ActiveLearningDedupeAutomated(JsonSchemaMixin):
     """Applies trained (active learning) model"""
 
+    settings: ActiveLearningSettings
     ci_supported: bool = False
 
     @dataclass
     class ActiveLearningSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Settings for ActiveLearning"""
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/dedupe/curation_dedupe.py` & `colrev-0.8.3/colrev/ops/built_in/dedupe/curation_dedupe.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 @zope.interface.implementer(colrev.env.package_manager.DedupePackageEndpointInterface)
 @dataclass
 class CurationDedupe(JsonSchemaMixin):
     """Deduplication endpoint for curations with full journals/proceedings
     retrieved from different sources (identifying duplicates in groups of
     volumes/issues or years)"""
 
+    settings: CurationDedupeSettings
     ci_supported: bool = True
 
     @dataclass
     class CurationDedupeSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Settings for CurationDedupe"""
@@ -55,14 +56,22 @@
         self,
         *,
         dedupe_operation: colrev.ops.dedupe.Dedupe,  # pylint: disable=unused-argument
         settings: dict,
     ):
         self.settings = self.settings_class.load_settings(data=settings)
 
+        pdf_prep_operation = dedupe_operation.review_manager.get_pdf_prep_operation()
+        self.pdf_metadata_validation = (
+            colrev.ops.built_in.pdf_prep.metadata_validation.PDFMetadataValidation(
+                pdf_prep_operation=pdf_prep_operation,
+                settings={"endpoint": "dedupe_pdf_md_validation"},
+            )
+        )
+
     def __get_similarity(self, *, df_a: pd.Series, df_b: pd.Series) -> float:
         author_similarity = fuzz.ratio(df_a["author"], df_b["author"]) / 100
 
         title_similarity = (
             fuzz.ratio(df_a["title"].lower(), df_b["title"].lower()) / 100
         )
 
@@ -122,23 +131,23 @@
 
         return similarity_array, tuples_to_process
 
     def __get_toc_items(self, *, records_list: list) -> list:
         toc_items = []
         for record in records_list:
             toc_item = {}
-            if "article" == record["ENTRYTYPE"]:
+            if record["ENTRYTYPE"] == "article":
                 if "journal" in record:
                     toc_item["journal"] = record["journal"]
                 if "volume" in record:
                     toc_item["volume"] = record["volume"]
                 if "number" in record:
                     toc_item["number"] = record["number"]
 
-            if "inproceedings" == record["ENTRYTYPE"]:
+            if record["ENTRYTYPE"] == "inproceedings":
                 if "booktitle" in record:
                     toc_item["booktitle"] = record["booktitle"]
                     toc_item["year"] = record["year"]
             if len(toc_item) > 0:
                 toc_items.append(toc_item)
 
         temp = {tuple(sorted(sub.items())) for sub in toc_items}
@@ -165,15 +174,15 @@
             ]
             if len(sources_missing_in_dedupe) > 0:
                 dedupe_operation.review_manager.logger.warning(
                     f"{colors.ORANGE}Sources missing in "
                     "dedupe.scripts.colrev.curation_full_outlet_dedupe: "
                     f"{','.join(sources_missing_in_dedupe)}{colors.END}"
                 )
-                if "y" == input("Add sources [y,n]?"):
+                if input("Add sources [y,n]?") == "y":
                     for source_missing_in_dedupe in sources_missing_in_dedupe:
                         dedupe_package_endpoints = (
                             dedupe_operation.review_manager.settings.dedupe.dedupe_package_endpoints
                         )
                         penultimate_position = len(dedupe_package_endpoints) - 1
                         dedupe_script_to_add = {
                             "endpoint": "colrev.curation_full_outlet_dedupe",
@@ -251,17 +260,20 @@
                     )
                 if recs_unique:
                     for source_record_dict in source_records:
                         if all(
                             source_record_dict.get(k, "NA") == v
                             for k, v in toc_item.items()
                         ):
-                            source_record_dict[
-                                "colrev_status"
-                            ] = colrev.record.RecordState.md_processed
+                            source_record = colrev.record.Record(
+                                data=source_record_dict
+                            )
+                            source_record.set_status(
+                                target_state=colrev.record.RecordState.md_processed
+                            )
             else:
                 print(toc_item)
                 print("Pre-imported records found for this toc_item (skipping)")
                 # print(processed_same_toc_same_source_records)
 
         for record in records.values():
             record.pop("container_title")
@@ -371,166 +383,193 @@
                                 }
                             )
                             print("TODO : validate whether it merges correctly:")
                             input(decision_list)
 
         return decision_list
 
+    def __validate_potential_merge(
+        self, *, rec1: dict, rec2: dict, dedupe_operation: colrev.ops.dedupe.Dedupe
+    ) -> dict:
+        if "file" in rec2:
+            updated_record = rec1.copy()
+            updated_record["file"] = rec2["file"]
+        elif "file" in rec1:
+            updated_record = rec2.copy()
+            updated_record["file"] = rec1["file"]
+        else:  # None of the records is curated
+            raise FileNotFoundError
+
+        record = colrev.record.Record(data=updated_record)
+        validation_info = self.pdf_metadata_validation.validates_based_on_metadata(
+            review_manager=dedupe_operation.review_manager,
+            record=record,
+        )
+        return validation_info
+
+    def __process_pdf_tuple(
+        self,
+        *,
+        tuple_to_process: tuple,
+        records: dict,
+        decision_list: list,
+        curated_record_ids: list,
+        pdf_record_ids: list,
+        dedupe_operation: colrev.ops.dedupe.Dedupe,
+    ) -> None:
+        rec1 = records[tuple_to_process[0]]
+        rec2 = records[tuple_to_process[1]]
+
+        # Note : Focus on merges between
+        # curated_records and pdf_same_toc_records
+        # Note : this should also ensure that pdf groups are not merged
+        # until a corresponding curated record group is available.
+        if (rec1["ID"] in curated_record_ids and rec2["ID"] in curated_record_ids) or (
+            rec1["ID"] in pdf_record_ids and rec2["ID"] in pdf_record_ids
+        ):
+            return
+
+        try:
+            validation_info = self.__validate_potential_merge(
+                rec1=rec1, rec2=rec2, dedupe_operation=dedupe_operation
+            )
+        except FileNotFoundError:
+            return
+
+        overlapping_colrev_ids = colrev.record.Record(
+            data=rec1
+        ).has_overlapping_colrev_id(record=colrev.record.Record(data=rec2))
+        if validation_info["validates"] or overlapping_colrev_ids:
+            # Note : make sure that we merge into the CURATED record
+            if "file" in rec1:
+                if tuple_to_process[0] in [x["ID1"] for x in decision_list]:
+                    return
+                if rec1["colrev_status"] < rec2["colrev_status"]:
+                    decision_list.append(
+                        {
+                            "ID1": tuple_to_process[1],
+                            "ID2": tuple_to_process[0],
+                            "decision": "duplicate",
+                        }
+                    )
+                else:
+                    decision_list.append(
+                        {
+                            "ID1": tuple_to_process[0],
+                            "ID2": tuple_to_process[1],
+                            "decision": "duplicate",
+                        }
+                    )
+            else:
+                if tuple_to_process[1] in [x["ID1"] for x in decision_list]:
+                    return
+                if rec1["colrev_status"] < rec2["colrev_status"]:
+                    decision_list.append(
+                        {
+                            "ID1": tuple_to_process[1],
+                            "ID2": tuple_to_process[0],
+                            "decision": "duplicate",
+                        }
+                    )
+                else:
+                    decision_list.append(
+                        {
+                            "ID1": tuple_to_process[0],
+                            "ID2": tuple_to_process[1],
+                            "decision": "duplicate",
+                        }
+                    )
+
+    def __dedupe_pdf_toc_item(
+        self,
+        *,
+        decision_list: list[dict],
+        toc_item: dict,
+        records: dict,
+        source_records: list,
+        dedupe_operation: colrev.ops.dedupe.Dedupe,
+    ) -> None:
+        processed_same_toc_records = [
+            r
+            for r in records.values()
+            if all(r.get(k, "NA") == v for k, v in toc_item.items())
+            and r["colrev_status"]
+            not in [
+                colrev.record.RecordState.md_imported,
+                colrev.record.RecordState.md_needs_manual_preparation,
+                colrev.record.RecordState.md_prepared,
+                colrev.record.RecordState.rev_prescreen_excluded,
+            ]
+            and not any(
+                self.settings.selected_source.replace("data/search/", "") in co
+                for co in r["colrev_origin"]
+            )
+        ]
+        pdf_same_toc_records = [
+            r
+            for r in source_records
+            if all(r.get(k, "NA") == v for k, v in toc_item.items())
+        ]
+
+        references = pd.DataFrame.from_records(
+            processed_same_toc_records + pdf_same_toc_records
+        )
+
+        nr_entries = references.shape[0]
+        if nr_entries == 0:
+            return
+        similarity_array = np.zeros([nr_entries, nr_entries])
+
+        # Note : min_similarity only means that the PDF will be considered
+        # for validates_based_on_metadata(...), which is the acutal test!
+        similarity_array, tuples_to_process = self.__calculate_similarities(
+            similarity_array=similarity_array,
+            references=references,
+            min_similarity=0.7,
+        )
+
+        curated_record_ids = [r["ID"] for r in processed_same_toc_records]
+        pdf_record_ids = [r["ID"] for r in pdf_same_toc_records]
+        for tuple_to_process in tuples_to_process:
+            self.__process_pdf_tuple(
+                tuple_to_process=tuple_to_process,
+                records=records,
+                decision_list=decision_list,
+                curated_record_ids=curated_record_ids,
+                pdf_record_ids=pdf_record_ids,
+                dedupe_operation=dedupe_operation,
+            )
+
     def __dedupe_pdf_source(
         self, *, dedupe_operation: colrev.ops.dedupe.Dedupe, records: dict
     ) -> list[dict]:
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-nested-blocks
-
         dedupe_operation.review_manager.logger.info("Processing as a pdf source")
 
         source_records = [
             r
             for r in records.values()
             if r["colrev_status"] == colrev.record.RecordState.md_prepared
             and any(
                 self.settings.selected_source.replace("data/search/", "") in co
                 for co in r["colrev_origin"]
             )
         ]
 
-        toc_items = self.__get_toc_items(records_list=source_records)
-
         decision_list: list[dict] = []
         # decision_list =[{'ID1': ID1, 'ID2': ID2, 'decision': 'duplicate'}]
 
-        pdf_prep_operation = dedupe_operation.review_manager.get_pdf_prep_operation()
-        pdf_metadata_validation = (
-            colrev.ops.built_in.pdf_prep.metadata_validation.PDFMetadataValidation(
-                pdf_prep_operation=pdf_prep_operation,
-                settings={"endpoint": "dedupe_pdf_md_validation"},
+        for toc_item in tqdm(self.__get_toc_items(records_list=source_records)):
+            self.__dedupe_pdf_toc_item(
+                decision_list=decision_list,
+                toc_item=toc_item,
+                records=records,
+                source_records=source_records,
+                dedupe_operation=dedupe_operation,
             )
-        )
-
-        for toc_item in tqdm(toc_items):
-            processed_same_toc_records = [
-                r
-                for r in records.values()
-                if all(r.get(k, "NA") == v for k, v in toc_item.items())
-                and r["colrev_status"]
-                not in [
-                    colrev.record.RecordState.md_imported,
-                    colrev.record.RecordState.md_needs_manual_preparation,
-                    colrev.record.RecordState.md_prepared,
-                    colrev.record.RecordState.rev_prescreen_excluded,
-                ]
-                and not any(
-                    self.settings.selected_source.replace("data/search/", "") in co
-                    for co in r["colrev_origin"]
-                )
-            ]
-            pdf_same_toc_records = [
-                r
-                for r in source_records
-                if all(r.get(k, "NA") == v for k, v in toc_item.items())
-            ]
-
-            references = pd.DataFrame.from_records(
-                processed_same_toc_records + pdf_same_toc_records
-            )
-
-            nr_entries = references.shape[0]
-            if nr_entries == 0:
-                continue
-            similarity_array = np.zeros([nr_entries, nr_entries])
-
-            # Note : min_similarity only means that the PDF will be considered
-            # for validates_based_on_metadata(...), which is the acutal test!
-            min_similarity = 0.7
-            similarity_array, tuples_to_process = self.__calculate_similarities(
-                similarity_array=similarity_array,
-                references=references,
-                min_similarity=min_similarity,
-            )
-
-            curated_record_ids = [r["ID"] for r in processed_same_toc_records]
-            pdf_record_ids = [r["ID"] for r in pdf_same_toc_records]
-            for tuple_to_process in tuples_to_process:
-                rec1 = records[tuple_to_process[0]]
-                rec2 = records[tuple_to_process[1]]
-
-                # Note : Focus on merges between
-                # curated_records and pdf_same_toc_records
-                # Note : this should also ensure that pdf groups are not merged
-                # until a corresponding curated record group is available.
-                if (
-                    rec1["ID"] in curated_record_ids
-                    and rec2["ID"] in curated_record_ids
-                ):
-                    continue
-                if rec1["ID"] in pdf_record_ids and rec2["ID"] in pdf_record_ids:
-                    continue
-
-                if "file" in rec2:
-                    updated_record = rec1.copy()
-                    updated_record["file"] = rec2["file"]
-                elif "file" in rec1:
-                    updated_record = rec2.copy()
-                    updated_record["file"] = rec1["file"]
-                else:  # None of the records is curated
-                    continue
-
-                record = colrev.record.Record(data=updated_record)
-                try:
-                    validation_info = (
-                        pdf_metadata_validation.validates_based_on_metadata(
-                            review_manager=dedupe_operation.review_manager,
-                            record=record,
-                        )
-                    )
-                except FileNotFoundError:
-                    continue
 
-                overlapping_colrev_ids = colrev.record.Record(
-                    data=rec1
-                ).has_overlapping_colrev_id(record=colrev.record.Record(data=rec2))
-                if validation_info["validates"] or overlapping_colrev_ids:
-                    # Note : make sure that we merge into the CURATED record
-                    if "file" in rec1:
-                        if tuple_to_process[0] not in [x["ID1"] for x in decision_list]:
-                            if rec1["colrev_status"] < rec2["colrev_status"]:
-                                decision_list.append(
-                                    {
-                                        "ID1": tuple_to_process[1],
-                                        "ID2": tuple_to_process[0],
-                                        "decision": "duplicate",
-                                    }
-                                )
-                            else:
-                                decision_list.append(
-                                    {
-                                        "ID1": tuple_to_process[0],
-                                        "ID2": tuple_to_process[1],
-                                        "decision": "duplicate",
-                                    }
-                                )
-                    else:
-                        if tuple_to_process[1] not in [x["ID1"] for x in decision_list]:
-                            if rec1["colrev_status"] < rec2["colrev_status"]:
-                                decision_list.append(
-                                    {
-                                        "ID1": tuple_to_process[1],
-                                        "ID2": tuple_to_process[0],
-                                        "decision": "duplicate",
-                                    }
-                                )
-                            else:
-                                decision_list.append(
-                                    {
-                                        "ID1": tuple_to_process[0],
-                                        "ID2": tuple_to_process[1],
-                                        "decision": "duplicate",
-                                    }
-                                )
         return decision_list
 
     def __pdf_source_selected(
         self, *, dedupe_operation: colrev.ops.dedupe.Dedupe
     ) -> bool:
         pdf_source = False
         relevant_source = [
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/dedupe/curation_missing_dedupe.py` & `colrev-0.8.3/colrev/ops/built_in/dedupe/curation_missing_dedupe.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,23 @@
 
     settings_class = colrev.env.package_manager.DefaultSettings
     ci_supported: bool = False
 
     def __init__(
         self,
         *,
-        dedupe_operation: colrev.ops.dedupe.Dedupe,  # pylint: disable=unused-argument
+        dedupe_operation: colrev.ops.dedupe.Dedupe,
         settings: dict,
     ):
         self.settings = self.settings_class.load_settings(data=settings)
+        self.review_manager = dedupe_operation.review_manager
+
+        self.__post_md_prepared_states = colrev.record.RecordState.get_post_x_states(
+            state=colrev.record.RecordState.md_processed
+        )
 
     def __create_dedupe_source_stats(
         self, *, dedupe_operation: colrev.ops.dedupe.Dedupe
     ) -> None:
         # Note : reload to generate correct statistics
 
         Path("dedupe").mkdir(exist_ok=True)
@@ -107,147 +112,153 @@
                 if "number" in keys:
                     records_df.number = pd.to_numeric(
                         records_df.number, errors="coerce"
                     )
                 records_df.sort_values(by=keys, inplace=True)
                 records_df.to_excel(f"dedupe/{source_origin}.xlsx", index=False)
 
-    def __process_missing_duplicates(
-        self, *, dedupe_operation: colrev.ops.dedupe.Dedupe
-    ) -> dict:
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+    def __get_same_toc_recs(
+        self, *, record: colrev.record.Record, records: dict
+    ) -> list:
+        if self.review_manager.force_mode:
+            if record.data["colrev_status"] in self.__post_md_prepared_states:
+                return []
+        else:
+            # only dedupe md_prepared records
+            if record.data["colrev_status"] not in [
+                colrev.record.RecordState.md_prepared
+            ]:
+                return []
+        if record.data.get("title", "") == "":
+            return []
+
+        try:
+            toc_key = record.get_toc_key()
+        except colrev_exceptions.NotTOCIdentifiableException:
+            return []
 
-        records = dedupe_operation.review_manager.dataset.load_records_dict()
+        same_toc_recs = []
+        for record_candidate in records.values():
+            try:
+                candidate_toc_key = colrev.record.Record(
+                    data=record_candidate
+                ).get_toc_key()
+            except colrev_exceptions.NotTOCIdentifiableException:
+                continue
+            if toc_key != candidate_toc_key:
+                continue
+            if record_candidate["ID"] == record.data["ID"]:
+                continue
+            if record_candidate["colrev_status"] in [
+                colrev.record.RecordState.md_prepared,
+                colrev.record.RecordState.md_needs_manual_preparation,
+                colrev.record.RecordState.md_imported,
+            ]:
+                continue
+            same_toc_recs.append(record_candidate)
+        return same_toc_recs
 
-        post_md_prepared_states = colrev.record.RecordState.get_post_x_states(
-            state=colrev.record.RecordState.md_processed
+    def __print_same_toc_recs(
+        self, *, same_toc_recs: list, record: colrev.record.Record
+    ) -> None:
+        for same_toc_rec in same_toc_recs:
+            same_toc_rec["similarity"] = colrev.record.PrepRecord.get_record_similarity(
+                record_a=colrev.record.Record(data=same_toc_rec), record_b=record
+            )
+
+        same_toc_recs = sorted(
+            same_toc_recs, key=lambda d: d["similarity"], reverse=True
         )
-        if dedupe_operation.review_manager.force_mode:
-            dedupe_operation.review_manager.logger.info(
+        if len(same_toc_recs) > 20:
+            same_toc_recs = same_toc_recs[0:20]
+
+        i = 0
+        for i, same_toc_rec in enumerate(same_toc_recs):
+            author_title_string = (
+                f"{same_toc_rec.get('author', 'NO_AUTHOR')} : "
+                + f"{same_toc_rec.get('title', 'NO_TITLE')}"
+            )
+
+            if same_toc_rec["similarity"] > 0.8:
+                print(f"{i + 1} - {colors.ORANGE}{author_title_string}{colors.END}")
+
+            else:
+                print(f"{i + 1} - {author_title_string}")
+
+    def __get_nr_recs_to_merge(self, *, records: dict) -> int:
+        if self.review_manager.force_mode:
+            self.review_manager.logger.info(
                 "Scope: md_prepared, md_needs_manual_preparation, md_imported"
             )
             nr_recs_to_merge = len(
                 [
                     x
                     for x in records.values()
-                    if x["colrev_status"] not in post_md_prepared_states
+                    if x["colrev_status"] not in self.__post_md_prepared_states
                 ]
             )
         else:
-            dedupe_operation.review_manager.logger.info("Scope: md_prepared")
+            self.review_manager.logger.info("Scope: md_prepared")
             nr_recs_to_merge = len(
                 [
                     x
                     for x in records.values()
                     if x["colrev_status"] in [colrev.record.RecordState.md_prepared]
                 ]
             )
+        return nr_recs_to_merge
+
+    def __process_missing_duplicates(
+        self, *, dedupe_operation: colrev.ops.dedupe.Dedupe
+    ) -> dict:
+        records = dedupe_operation.review_manager.dataset.load_records_dict()
+
+        nr_recs_to_merge = self.__get_nr_recs_to_merge(records=records)
 
         nr_recs_checked = 0
         results: typing.Dict[str, list] = {
             "decision_list": [],
             "add_records_to_md_processed_list": [],
             "records_to_prepare": [],
         }
 
         for record_dict in records.values():
-            if dedupe_operation.review_manager.force_mode:
-                if record_dict["colrev_status"] in post_md_prepared_states:
-                    continue
-            else:
-                # only dedupe md_prepared records
-                if record_dict["colrev_status"] not in [
-                    colrev.record.RecordState.md_prepared
-                ]:
-                    continue
-            if "" == record_dict.get("title", ""):
-                continue
-
             record = colrev.record.Record(data=record_dict)
 
-            try:
-                toc_key = record.get_toc_key()
-            except colrev_exceptions.NotTOCIdentifiableException:
-                continue
-
-            same_toc_recs = []
-            for record_candidate in records.values():
-                try:
-                    candidate_toc_key = colrev.record.Record(
-                        data=record_candidate
-                    ).get_toc_key()
-                except colrev_exceptions.NotTOCIdentifiableException:
-                    continue
-                if toc_key != candidate_toc_key:
-                    continue
-                if record_candidate["ID"] == record.data["ID"]:
-                    continue
-                if record_candidate["colrev_status"] in [
-                    colrev.record.RecordState.md_prepared,
-                    colrev.record.RecordState.md_needs_manual_preparation,
-                    colrev.record.RecordState.md_imported,
-                ]:
-                    continue
-                same_toc_recs.append(record_candidate)
+            same_toc_recs = self.__get_same_toc_recs(record=record, records=records)
 
             if len(same_toc_recs) == 0:
                 print("no same toc records")
                 continue
 
             print("\n\n\n")
             print(colors.ORANGE)
             record.print_citation_format()
             print(colors.END)
 
-            for same_toc_rec in same_toc_recs:
-                same_toc_rec[
-                    "similarity"
-                ] = colrev.record.PrepRecord.get_record_similarity(
-                    record_a=colrev.record.Record(data=same_toc_rec), record_b=record
-                )
-
-            same_toc_recs = sorted(
-                same_toc_recs, key=lambda d: d["similarity"], reverse=True
-            )
-            if len(same_toc_recs) > 20:
-                same_toc_recs = same_toc_recs[0:20]
-
-            i = 0
-            for i, same_toc_rec in enumerate(same_toc_recs):
-                author_title_string = (
-                    f"{same_toc_rec.get('author', 'NO_AUTHOR')} : "
-                    + f"{same_toc_rec.get('title', 'NO_TITLE')}"
-                )
-
-                if same_toc_rec["similarity"] > 0.8:
-                    print(f"{i + 1} - {colors.ORANGE}{author_title_string}{colors.END}")
-
-                else:
-                    print(f"{i + 1} - {author_title_string}")
-
+            self.__print_same_toc_recs(same_toc_recs=same_toc_recs, record=record)
+            i = len(same_toc_recs)
             valid_selection = False
             quit_pressed = False
             while not valid_selection:
                 ret = input(
                     f"({nr_recs_checked}/{nr_recs_to_merge}) "
                     f"Merge with record [{1}...{i+1} / s / a / p / q]?   "
                 )
-                if "s" == ret:
+                if ret == "s":
                     valid_selection = True
-                elif "q" == ret:
+                elif ret == "q":
                     quit_pressed = True
                     valid_selection = True
-                elif "a" == ret:
+                elif ret == "a":
                     results["add_records_to_md_processed_list"].append(
                         record.data["ID"]
                     )
                     valid_selection = True
-                elif "p" == ret:
+                elif ret == "p":
                     results["records_to_prepare"].append(record.data["ID"])
                     valid_selection = True
                 elif ret.isdigit():
                     if int(ret) - 1 <= i:
                         rec2 = same_toc_recs[int(ret) - 1]
                         if record.data["colrev_status"] < rec2["colrev_status"]:
                             results["decision_list"].append(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/dedupe/simple_dedupe.py` & `colrev-0.8.3/colrev/ops/built_in/dedupe/simple_dedupe.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 @zope.interface.implementer(colrev.env.package_manager.DedupePackageEndpointInterface)
 @dataclass
 class SimpleDedupe(JsonSchemaMixin):
     """Simple duplicate identification (for small sample sizes)"""
 
+    settings: SimpleDedupeSettings
+
     ci_supported: bool = True
 
     @dataclass
     class SimpleDedupeSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Settings for SimpleDedupe"""
@@ -289,18 +291,18 @@
             user_input = (
                 colrev.ops.built_in.dedupe.utils.console_duplicate_instance_label(
                     record_pair, keys, True, "TODO", n_match, n_distinct, []
                 )
             )
 
             # set potential_duplicates
-            if "y" == user_input:
+            if user_input == "y":
                 potential_duplicate["decision"] = "duplicate"
                 n_match += 1
-            if "n" == user_input:
+            if user_input == "n":
                 potential_duplicate["decision"] = "no_duplicate"
                 n_distinct += 1
 
         return potential_duplicates
 
     def run_dedupe(self, dedupe_operation: colrev.ops.dedupe.Dedupe) -> None:
         """Pairwise identification of duplicates based on static similarity measure
@@ -341,15 +343,15 @@
             dedupe_batch_results.append(merge_item)
 
         # dedupe_batch[-1]['queue'].to_csv('last_records.csv')
 
         dedupe_operation.apply_merges(
             results=dedupe_batch_results, complete_dedupe=True
         )
-        if [x for x in dedupe_batch_results if "duplicate" == x["decision"]]:
+        if [x for x in dedupe_batch_results if x["decision"] == "duplicate"]:
             dedupe_operation.review_manager.logger.info(
                 "Completed application of merges"
             )
 
         dedupe_operation.review_manager.create_commit(
             msg="Merge duplicate records",
         )
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/dedupe/utils.py` & `colrev-0.8.3/colrev/ops/built_in/dedupe/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     """Convenience function for console duplicate labeling"""
 
     if manual:
         os.system("cls" if os.name == "nt" else "clear")
         colrev.record.Record.print_diff_pair(record_pair=record_pair, keys=keys)
 
     user_input = "unsure"
-    if "yes" == curations_dupe_info:
+    if curations_dupe_info == "yes":
         user_input = "y"
         if manual:
             print(f"{n_match} positive, {n_distinct} negative")
             print("#")
             print("# curations_dupe_info: yes/duplicate")
             print("#")
             time.sleep(0.6)
-    elif "no" == curations_dupe_info:
+    elif curations_dupe_info == "no":
         user_input = "n"
         if manual:
             print(f"{n_match} positive, {n_distinct} negative")
             print("#")
             print("# curations_dupe_info: no duplicate")
             print("#")
             time.sleep(0.6)
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/load_conversion/bib_pybtex_loader.py` & `colrev-0.8.3/colrev/ops/built_in/load_conversion/bib_pybtex_loader.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/load_conversion/bibutils_loader.py` & `colrev-0.8.3/colrev/ops/built_in/load_conversion/bibutils_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def load(
         self, load_operation: colrev.ops.load.Load, source: colrev.settings.SearchSource
     ) -> dict:
         """Load records from the source"""
 
         def bibutils_convert(script: str, data: str) -> str:
-            if "xml2bib" == script:
+            if script == "xml2bib":
                 script = script + " -b -w -sk "
             else:
                 script = script + " -i unicode "
 
             try:
                 client = docker.APIClient()
                 container = client.create_container(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/load_conversion/markdown_loader.py` & `colrev-0.8.3/colrev/ops/built_in/load_conversion/markdown_loader.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/load_conversion/table_loader.py` & `colrev-0.8.3/colrev/ops/built_in/load_conversion/table_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,110 +23,128 @@
 # pylint: disable=duplicate-code
 
 
 class TableLoadUtility:
     """Utility for tables loading"""
 
     @classmethod
-    def preprocess_records(cls, *, records: list) -> dict:
-        """Preprocess records imported from a table"""
+    def __rename_fields(cls, *, record_dict: dict) -> dict:
+        if "issue" in record_dict and "number" not in record_dict:
+            record_dict["number"] = record_dict["issue"]
+            if record_dict["number"] == "no issue":
+                del record_dict["number"]
+            del record_dict["issue"]
+
+        if "authors" in record_dict and "author" not in record_dict:
+            record_dict["author"] = record_dict["authors"]
+            del record_dict["authors"]
+
+        if "publication_year" in record_dict and "year" not in record_dict:
+            record_dict["year"] = record_dict["publication_year"]
+            del record_dict["publication_year"]
+
+        # Note: this is a simple heuristic:
+        if (
+            "journal/book" in record_dict
+            and "journal" not in record_dict
+            and "doi" in record_dict
+        ):
+            record_dict["journal"] = record_dict["journal/book"]
+            del record_dict["journal/book"]
+
+        return record_dict
+
+    @classmethod
+    def __set_entrytype(cls, *, record_dict: dict) -> dict:
+        record_dict["ENTRYTYPE"] = "misc"
+        if "type" in record_dict:
+            record_dict["ENTRYTYPE"] = record_dict["type"]
+            del record_dict["type"]
+            if record_dict["ENTRYTYPE"] == "inproceedings":
+                if "journal" in record_dict and "booktitle" not in record_dict:
+                    record_dict["booktitle"] = record_dict["journal"]
+                    del record_dict["journal"]
+            if record_dict["ENTRYTYPE"] == "article":
+                if "booktitle" in record_dict and "journal" not in record_dict:
+                    record_dict["journal"] = record_dict["booktitle"]
+                    del record_dict["booktitle"]
+
+        if "ENTRYTYPE" not in record_dict:
+            if record_dict.get("journal", "") != "":
+                record_dict["ENTRYTYPE"] = "article"
+            if record_dict.get("booktitle", "") != "":
+                record_dict["ENTRYTYPE"] = "inproceedings"
+        return record_dict
+
+    @classmethod
+    def __parse_record_dict(cls, *, record_dict: dict) -> dict:
+        record_dict = cls.__set_entrytype(record_dict=record_dict)
+
+        for key, value in record_dict.items():
+            record_dict[key] = str(value)
+
+        record_dict = cls.__rename_fields(record_dict=record_dict)
 
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+        return record_dict
 
+    @classmethod
+    def __get_records_dict(cls, *, records: list) -> dict:
         next_id = 1
         for record_dict in records:
-            if "type" in record_dict:
-                record_dict["ENTRYTYPE"] = record_dict["type"]
-                del record_dict["type"]
-                if "inproceedings" == record_dict["ENTRYTYPE"]:
-                    if "journal" in record_dict and "booktitle" not in record_dict:
-                        record_dict["booktitle"] = record_dict["journal"]
-                        del record_dict["journal"]
-                if "article" == record_dict["ENTRYTYPE"]:
-                    if "booktitle" in record_dict and "journal" not in record_dict:
-                        record_dict["journal"] = record_dict["booktitle"]
-                        del record_dict["booktitle"]
-
-            if "ENTRYTYPE" not in record_dict:
-                if "" != record_dict.get("journal", ""):
-                    record_dict["ENTRYTYPE"] = "article"
-                if "" != record_dict.get("booktitle", ""):
-                    record_dict["ENTRYTYPE"] = "inproceedings"
-                else:
-                    record_dict["ENTRYTYPE"] = "misc"
-
             if "ID" not in record_dict:
                 if "citation_key" in record_dict:
                     record_dict["ID"] = record_dict["citation_key"]
                 else:
                     record_dict["ID"] = next_id
                     next_id += 1
-
-            if "issue" in record_dict and "number" not in record_dict:
-                record_dict["number"] = record_dict["issue"]
-                if "no issue" == record_dict["number"]:
-                    del record_dict["number"]
-                del record_dict["issue"]
-
-            for key, value in record_dict.items():
-                record_dict[key] = str(value)
-
-            if "authors" in record_dict and "author" not in record_dict:
-                record_dict["author"] = record_dict["authors"]
-                del record_dict["authors"]
-            if "publication_year" in record_dict and "year" not in record_dict:
-                record_dict["year"] = record_dict["publication_year"]
-                del record_dict["publication_year"]
-            # Note: this is a simple heuristic:
-            if (
-                "journal/book" in record_dict
-                and "journal" not in record_dict
-                and "doi" in record_dict
-            ):
-                record_dict["journal"] = record_dict["journal/book"]
-                del record_dict["journal/book"]
-
-            if "no Times-Cited" == record_dict.get("cited_by", ""):
-                del record_dict["cited_by"]
+            record_dict = cls.__parse_record_dict(record_dict=record_dict)
 
         if all("ID" in r for r in records):
             records_dict = {r["ID"]: r for r in records}
         else:
             records_dict = {}
             for i, record in enumerate(records):
                 records_dict[str(i)] = record
 
+        return records_dict
+
+    @classmethod
+    def __drop_fields(cls, *, records_dict: dict) -> dict:
         for r_dict in records_dict.values():
-            if "no year" == r_dict.get("year", "NA"):
-                del r_dict["year"]
-            if "no journal" == r_dict.get("journal", "NA"):
-                del r_dict["journal"]
-            if "no volume" == r_dict.get("volume", "NA"):
-                del r_dict["volume"]
-            if "no pages" == r_dict.get("pages", "NA"):
-                del r_dict["pages"]
-            if "no issue" == r_dict.get("issue", "NA"):
-                del r_dict["issue"]
-            if "no number" == r_dict.get("number", "NA"):
-                del r_dict["number"]
-            if "no doi" == r_dict.get("doi", "NA"):
-                del r_dict["doi"]
-            if "no type" == r_dict.get("type", "NA"):
-                del r_dict["type"]
-            if "author_count" in r_dict:
-                del r_dict["author_count"]
-            if "no Number-of-Cited-References" == r_dict.get(
-                "number_of_cited_references", "NA"
+            for key in list(r_dict.keys()):
+                if r_dict[key] == f"no {key}":
+                    del r_dict[key]
+            if (
+                r_dict.get("number_of_cited_references", "NA")
+                == "no Number-of-Cited-References"
             ):
                 del r_dict["number_of_cited_references"]
             if "no file" in r_dict.get("file_name", "NA"):
                 del r_dict["file_name"]
-            if "times_cited" == r_dict.get("times_cited", "NA"):
-                del r_dict["times_cited"]
+
+            if r_dict.get("cited_by", "NA") in [
+                "no Times-Cited",
+            ]:
+                del r_dict["cited_by"]
+
+            if "author_count" in r_dict:
+                del r_dict["author_count"]
+            if "entrytype" in r_dict:
+                del r_dict["entrytype"]
+            if "citation_key" in r_dict:
+                del r_dict["citation_key"]
+
+        return records_dict
+
+    @classmethod
+    def preprocess_records(cls, *, records: list) -> dict:
+        """Preprocess records imported from a table"""
+
+        records_dict = cls.__get_records_dict(records=records)
+        records_dict = cls.__drop_fields(records_dict=records_dict)
 
         return records_dict
 
 
 @zope.interface.implementer(
     colrev.env.package_manager.LoadConversionPackageEndpointInterface
 )
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/load_conversion/zotero_loader.py` & `colrev-0.8.3/colrev/ops/built_in/load_conversion/zotero_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         files = {"file": open(source.filename, "rb")}
         headers = {"Content-type": "text/plain"}
         ret = requests.post(
             "http://127.0.0.1:1969/import", headers=headers, files=files, timeout=30
         )
 
         headers = {"Content-type": "application/json"}
-        if "No suitable translators found" == ret.content.decode("utf-8"):
+        if ret.content.decode("utf-8") == "No suitable translators found":
             raise colrev_exceptions.ImportException(
                 "Zotero translators: No suitable import translators found"
             )
 
         try:
             zotero_format = json.loads(ret.content)
             ret = requests.post(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_get/local_index_pdf_get.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_get/local_index_pdf_get.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_get/unpaywall.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_get/unpaywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             return record
 
         pdf_filepath = pdf_get_operation.get_target_filepath(record=record)
 
         url = self.__unpaywall(
             review_manager=pdf_get_operation.review_manager, doi=record.data["doi"]
         )
-        if "NA" == url:
+        if url == "NA":
             return record
         if "Invalid/unknown DOI" in url:
             return record
 
         try:
             res = requests.get(
                 url,
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_get/website_screenshot.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_get/website_screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # pylint: disable=too-few-public-methods
 
 
 @zope.interface.implementer(colrev.env.package_manager.PDFGetPackageEndpointInterface)
 @dataclass
 class WebsiteScreenshot(JsonSchemaMixin):
-    """Get PDFs from webisite screenshot (for "online" ENTRYTYPES)"""
+    """Get PDFs from website screenshot (for "online" ENTRYTYPES)"""
 
     settings_class = colrev.env.package_manager.DefaultSettings
     ci_supported: bool = False
 
     def __init__(
         self,
         *,
@@ -38,15 +38,15 @@
         self.settings = self.settings_class.load_settings(data=settings)
 
     def get_pdf(
         self, pdf_get_operation: colrev.ops.pdf_get.PDFGet, record: colrev.record.Record
     ) -> colrev.record.Record:
         """Get a PDF of the website (screenshot)"""
 
-        if "online" != record.data["ENTRYTYPE"]:
+        if record.data["ENTRYTYPE"] != "online":
             return record
 
         screenshot_service = pdf_get_operation.review_manager.get_screenshot_service()
         screenshot_service.start_screenshot_service()
 
         pdf_filepath = pdf_get_operation.review_manager.PDF_DIR_RELATIVE / Path(
             f"{record.data['ID']}.pdf"
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_get_man/pdf_get_man_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
             retrieval_script,
         ) in retrieval_scripts.items():
             # pdf_get_man_operation.review_manager.logger.debug(
             #     f'{script_name}({record.data["ID"]}) called'
             # )
             record = retrieval_script(pdf_get_man_operation, record)
 
-            if "y" == input("Retrieved (y/n)?"):
+            if input("Retrieved (y/n)?") == "y":
                 if self.__get_from_downloads_folder:
                     self.__retrieve_record_from_downloads_folder(
                         pdf_get_man_operation=pdf_get_man_operation, record=record
                     )
                 filepath = self.__get_filepath(
                     pdf_get_man_operation=pdf_get_man_operation, record=record
                 )
@@ -248,15 +248,15 @@
                     pdf_get_man_operation.pdf_get_man_record(
                         record=record,
                         filepath=filepath,
                     )
                     break
 
         if not filepath.is_file():
-            if "n" == input("Is the PDF available (y/n)?"):
+            if input("Is the PDF available (y/n)?") == "n":
                 pdf_get_man_operation.pdf_get_man_record(
                     record=record,
                     filepath=None,
                 )
 
         pdf_get_man_operation.review_manager.update_status_yaml()
 
@@ -266,18 +266,18 @@
         """Get the PDF manually based on a cli"""
 
         pdf_get_man_operation.review_manager.logger.info("Retrieve PDFs manually")
         pdf_get_operation = pdf_get_man_operation.review_manager.get_pdf_get_operation()
         pdf_dir = pdf_get_man_operation.review_manager.pdf_dir
 
         records = pdf_get_man_operation.review_manager.dataset.load_records_dict()
-        if "y" == input("Check existing unlinked PDFs (y/n)?"):
+        if input("Check existing unlinked PDFs (y/n)?") == "y":
             records = pdf_get_operation.check_existing_unlinked_pdfs(records=records)
 
-        if "y" == input("Get PDF from Downloads folder (y/n)?"):
+        if input("Get PDF from Downloads folder (y/n)?") == "y":
             self.__get_from_downloads_folder = True
 
         for record_dict in records.values():
             record = colrev.record.Record(data=record_dict)
             pdf_get_operation.link_pdf(record=record).get_data()
 
         pdf_get_man_operation.export_retrieval_table(records=records)
@@ -297,15 +297,15 @@
             print(f"\n\n{stat}")
 
             self.__pdf_get_man_record_cli(
                 pdf_get_man_operation=pdf_get_man_operation, record=record
             )
 
         if pdf_get_man_operation.review_manager.dataset.has_changes():
-            if "y" == input("Create commit (y/n)?"):
+            if input("Create commit (y/n)?") == "y":
                 pdf_get_man_operation.review_manager.create_commit(
                     msg="Retrieve PDFs manually",
                     manual_author=True,
                 )
         else:
             pdf_get_man_operation.review_manager.logger.info(
                 "Retrieve PDFs manually and copy the files to "
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/check_ocr.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/check_ocr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/env python
 """OCR as a PDF preparation operation"""
 from __future__ import annotations
 
+import os
 import subprocess
 from dataclasses import dataclass
 from pathlib import Path
 
 import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
@@ -50,15 +51,15 @@
 
     def __text_is_english(self, *, text: str) -> bool:
         # Format: ENGLISH
         confidence_values = self.language_service.compute_language_confidence_values(
             text=text
         )
         lang, conf = confidence_values.pop(0)
-        if "eng" == lang:
+        if lang == "eng":
             if conf > 0.1:
                 return True
 
         return False
 
     def __apply_ocr(
         self,
@@ -70,39 +71,52 @@
         pdf_path = review_manager.path / Path(record_dict["file"])
         ocred_filename = Path(str(pdf_path).replace(".pdf", "_ocr.pdf"))
 
         orig_path = (
             pdf_path.parents[0] if pdf_path.is_file() else review_manager.pdf_dir
         )
 
-        options = f"--jobs {4}"
+        # options = ""
         # if rotate:
         #     options = options + '--rotate-pages '
         # if deskew:
         #     options = options + '--deskew '
         docker_home_path = Path("/home/docker")
-        command = (
-            'docker run --rm --user "$(id -u):$(id -g)" -v "'
-            + str(orig_path)
-            + f':/home/docker" {self.ocrmypdf_image} --force-ocr '
-            + options
-            + ' -l eng "'
-            + str(docker_home_path / pdf_path.name)
-            + '"  "'
-            + str(docker_home_path / ocred_filename.name)
-            + '"'
-        )
-        subprocess.check_output([command], stderr=subprocess.STDOUT, shell=True)
+
+        command = [
+            "docker",
+            "run",
+            "--rm",
+            "--user",
+            # "$(id -u):$(id -g)",
+            f"{os.geteuid()}:{os.getegid()}",
+            "-v",
+            f"{orig_path}:/home/docker",
+            self.ocrmypdf_image,
+            "--force-ocr",
+            # options,
+            "--jobs",
+            "4",
+            "-l",
+            "eng",
+            str(docker_home_path / pdf_path.name),
+            str(docker_home_path / ocred_filename.name),
+        ]
+
+        with subprocess.Popen(
+            command, stdout=subprocess.PIPE, shell=False
+        ) as ocr_process:
+            ocr_process.wait()
 
         record = colrev.record.Record(data=record_dict)
         record.add_data_provenance_note(key="file", note="pdf_processed with OCRMYPDF")
         record.data["file"] = str(ocred_filename.relative_to(review_manager.path))
         record.set_text_from_pdf(project_path=review_manager.path)
 
-    @timeout_decorator.timeout(120, use_signals=False)
+    @timeout_decorator.timeout(300, use_signals=False)
     def prep_pdf(
         self,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,
         record: colrev.record.Record,
         pad: int,
     ) -> dict:
         """Prepare the PDF by checking/applying OCR"""
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/completeness_validation.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/completeness_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 f"{__roman_to_int(s=start_page)}--{__roman_to_int(s=end_page)}"
             )
         roman_page_matched = re.match(self.roman_page_pattern, pages_metadata)
         if roman_page_matched:
             page = roman_page_matched.group()
             pages_metadata = f"{__roman_to_int(s=page)}"
 
-        if "NA" == pages_metadata or not re.match(r"^\d+--\d+|\d+$", pages_metadata):
+        if pages_metadata == "NA" or not re.match(r"^\d+--\d+|\d+$", pages_metadata):
             msg = (
                 f'{record.data["ID"]}'.ljust(pad - 1, " ")
                 + "Could not validate completeness: no pages in metadata"
             )
             record.add_data_provenance_note(key="file", note="no_pages_in_metadata")
             record.data.update(
                 colrev_status=colrev.record.RecordState.pdf_needs_manual_preparation
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/cover_page.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/cover_page.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 from PyPDF2 import PdfFileReader
 
 import colrev.env.package_manager
 import colrev.env.utils
+import colrev.qm.colrev_pdf_id
 import colrev.record
 
 # pylint: disable=duplicate-code
 
 
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
@@ -39,18 +40,140 @@
     def __init__(
         self,
         *,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
+        self.review_manager = pdf_prep_operation.review_manager
 
-        if not pdf_prep_operation.review_manager.in_ci_environment():
-            # Note : to pull image if not available
-            pdf_prep_operation.review_manager.get_pdf_hash_service()
+    def __check_scholarworks_first_page(self, *, page0: str, coverpages: list) -> None:
+        if "followthisandadditionalworksat:https://scholarworks" in page0:
+            coverpages.append(0)
+
+    def __check_researchgate_first_page(self, *, page0: str, coverpages: list) -> None:
+        if (
+            "discussions,stats,andauthorprofilesforthispublicationat:"
+            + "https://www.researchgate.net/publication"
+            in page0
+            or "discussions,stats,andauthorproﬁlesforthispublicationat:"
+            + "https://www.researchgate.net/publication"
+            in page0
+        ):
+            coverpages.append(0)
+
+    def __check_jstor_first_page(self, *, page0: str, coverpages: list) -> None:
+        if (
+            "pleasecontactsupport@jstor.org.youruseofthejstorarchiveindicatesy"
+            + "ouracceptanceoftheterms&conditionsofuse"
+            in page0
+            or "formoreinformationregardingjstor,pleasecontactsupport@jstor.org"
+            in page0
+        ):
+            coverpages.append(0)
+
+    def __check_emerald_first_page(self, *, page0: str, coverpages: list) -> None:
+        if (
+            "emeraldisbothcounter4andtransfercompliant.theorganizationisapartnero"
+            "fthecommitteeonpublicationethics(cope)andalsoworkswithporticoandthe"
+            "lockssinitiativefordigitalarchivepreservation.*relatedcontentand"
+            "downloadinformationcorrectattimeofdownload" in page0
+        ):
+            coverpages.append(0)
+
+    def __check_informs_first_page(
+        self, *, page0: str, page1: str, coverpages: list
+    ) -> None:
+        if (
+            "thisarticlewasdownloadedby" in page0
+            and "fulltermsandconditionsofuse:" in page0
+        ):
+            coverpages.append(0)
+        if (
+            "thisarticlemaybeusedonlyforthepurposesofresearch" in page0
+            and "abstract" not in page0
+            and "keywords" not in page0
+            and "abstract" in page1
+            and "keywords" in page1
+        ):
+            coverpages.append(0)
+
+    def __check_ais_first_page(self, *, page0: str, coverpages: list) -> None:
+        if (
+            "associationforinformationsystemsaiselectroniclibrary(aisel)" in page0
+            and "abstract" not in page0
+            and "keywords" not in page0
+        ):
+            coverpages.append(0)
+
+    def __check_tandf_first_page(
+        self, *, page0: str, page1: str, coverpages: list
+    ) -> None:
+        if ("pleasescrolldownforarticle" in page0) or ("viewrelatedarticles" in page0):
+            if "abstract" not in page0 and "keywords" not in page0:
+                coverpages.append(0)
+                if (
+                    "terms-and-conditions" in page1
+                    and "abstract" not in page1
+                    and "keywords" not in page1
+                ):
+                    coverpages.append(1)
+
+    def __get_coverpages(self, *, pdf: str) -> typing.List[int]:
+        coverpages: typing.List[int] = []
+
+        try:
+            pdf_reader = PdfFileReader(str(pdf), strict=False)
+        except ValueError:
+            return coverpages
+
+        if len(pdf_reader.pages) == 1:
+            return coverpages
+
+        first_page_average_hash_16 = colrev.qm.colrev_pdf_id.get_pdf_hash(
+            pdf_path=Path(pdf),
+            page_nr=1,
+            hash_size=16,
+        )
+
+        # Note : to generate hashes from a directory containing single-page PDFs:
+        # colrev pdf-prep --get_hashes path
+        first_page_hashes = [
+            "ffff83ff81ff81ffc3ff803f81ff80ffc03fffffffffffffffff96ff9fffffff",
+            "ffffffffc0ffc781c007c007cfffc7ffffffffffffffc03fc007c003c827ffff",
+            "84ff847ffeff83ff800783ff801f800180038fffffffffffbfff8007bffff83f",
+            "83ff03ff03ff83ffffff807f807f9fff87ffffffffffffffffff809fbfffffff",
+            "ffffffffc0ffc781c03fc01fffffffffffffffffffffc03fc01fc003ffffffff",
+            "ffffffffc0ffc781c007c007cfffc7ffffffffffffffc03fc007c003ce27ffff",
+            "ffffe7ffe3ffc3fffeff802780ff8001c01fffffffffffffffff80079ffffe3f",
+            "ffffffffc0ffc781c00fc00fc0ffc7ffffffffffffffc03fc007c003cf27ffff",
+            "ffffffffc0ffc781c007c003cfffcfffffffffffffffc03fc003c003cc27ffff",
+            "ffffe7ffe3ffc3ffffff80e780ff80018001ffffffffffffffff93ff83ff9fff",
+        ]
+
+        if str(first_page_average_hash_16) in first_page_hashes:
+            coverpages.append(0)
+
+        res = pdf_reader.getPage(0).extract_text()
+        page0 = res.replace(" ", "").replace("\n", "").lower()
+
+        res = pdf_reader.getPage(1).extract_text()
+        page1 = res.replace(" ", "").replace("\n", "").lower()
+
+        # input(page0)
+
+        self.__check_scholarworks_first_page(page0=page0, coverpages=coverpages)
+        self.__check_researchgate_first_page(page0=page0, coverpages=coverpages)
+        self.__check_jstor_first_page(page0=page0, coverpages=coverpages)
+        self.__check_emerald_first_page(page0=page0, coverpages=coverpages)
+        self.__check_informs_first_page(page0=page0, page1=page1, coverpages=coverpages)
+        self.__check_ais_first_page(page0=page0, coverpages=coverpages)
+        self.__check_tandf_first_page(page0=page0, page1=page1, coverpages=coverpages)
+
+        return list(set(coverpages))
 
     @timeout_decorator.timeout(60, use_signals=False)
     def prep_pdf(
         self,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,
         record: colrev.record.Record,
         pad: int,  # pylint: disable=unused-argument
@@ -60,134 +183,15 @@
         if not record.data["file"].endswith(".pdf"):
             return record.data
 
         local_index = pdf_prep_operation.review_manager.get_local_index()
         cp_path = local_index.local_environment_path / Path(".coverpages")
         cp_path.mkdir(exist_ok=True)
 
-        def __get_coverpages(*, pdf: str) -> typing.List[int]:
-            # pylint: disable=too-many-branches
-
-            coverpages: typing.List[int] = []
-
-            try:
-                pdf_reader = PdfFileReader(str(pdf), strict=False)
-            except ValueError:
-                return coverpages
-
-            if len(pdf_reader.pages) == 1:
-                return coverpages
-
-            pdf_hash_service = pdf_prep_operation.review_manager.get_pdf_hash_service()
-
-            first_page_average_hash_16 = pdf_hash_service.get_pdf_hash(
-                pdf_path=Path(pdf),
-                page_nr=1,
-                hash_size=16,
-            )
-
-            # Note : to generate hashes from a directory containing single-page PDFs:
-            # colrev pdf-prep --get_hashes path
-            first_page_hashes = [
-                "ffff83ff81ff81ffc3ff803f81ff80ffc03fffffffffffffffff96ff9fffffff",
-                "ffffffffc0ffc781c007c007cfffc7ffffffffffffffc03fc007c003c827ffff",
-                "84ff847ffeff83ff800783ff801f800180038fffffffffffbfff8007bffff83f",
-                "83ff03ff03ff83ffffff807f807f9fff87ffffffffffffffffff809fbfffffff",
-                "ffffffffc0ffc781c03fc01fffffffffffffffffffffc03fc01fc003ffffffff",
-                "ffffffffc0ffc781c007c007cfffc7ffffffffffffffc03fc007c003ce27ffff",
-                "ffffe7ffe3ffc3fffeff802780ff8001c01fffffffffffffffff80079ffffe3f",
-                "ffffffffc0ffc781c00fc00fc0ffc7ffffffffffffffc03fc007c003cf27ffff",
-                "ffffffffc0ffc781c007c003cfffcfffffffffffffffc03fc003c003cc27ffff",
-                "ffffe7ffe3ffc3ffffff80e780ff80018001ffffffffffffffff93ff83ff9fff",
-            ]
-
-            if str(first_page_average_hash_16) in first_page_hashes:
-                coverpages.append(0)
-
-            res = pdf_reader.getPage(0).extract_text()
-            page0 = res.replace(" ", "").replace("\n", "").lower()
-
-            res = pdf_reader.getPage(1).extract_text()
-            page1 = res.replace(" ", "").replace("\n", "").lower()
-
-            # input(page0)
-
-            # scholarworks.lib.csusb first page
-            if "followthisandadditionalworksat:https://scholarworks" in page0:
-                coverpages.append(0)
-
-            # Researchgate First Page
-            if (
-                "discussions,stats,andauthorprofilesforthispublicationat:"
-                + "https://www.researchgate.net/publication"
-                in page0
-                or "discussions,stats,andauthorproﬁlesforthispublicationat:"
-                + "https://www.researchgate.net/publication"
-                in page0
-            ):
-                coverpages.append(0)
-
-            # JSTOR  First Page
-            if (
-                "pleasecontactsupport@jstor.org.youruseofthejstorarchiveindicatesy"
-                + "ouracceptanceoftheterms&conditionsofuse"
-                in page0
-                or "formoreinformationregardingjstor,pleasecontactsupport@jstor.org"
-                in page0
-            ):
-                coverpages.append(0)
-
-            # Emerald first page
-            if (
-                "emeraldisbothcounter4andtransfercompliant.theorganizationisapartnero"
-                "fthecommitteeonpublicationethics(cope)andalsoworkswithporticoandthe"
-                "lockssinitiativefordigitalarchivepreservation.*relatedcontentand"
-                "downloadinformationcorrectattimeofdownload" in page0
-            ):
-                coverpages.append(0)
-
-            # INFORMS First Page
-            if (
-                "thisarticlewasdownloadedby" in page0
-                and "fulltermsandconditionsofuse:" in page0
-            ):
-                coverpages.append(0)
-            if (
-                "thisarticlemaybeusedonlyforthepurposesofresearch" in page0
-                and "abstract" not in page0
-                and "keywords" not in page0
-                and "abstract" in page1
-                and "keywords" in page1
-            ):
-                coverpages.append(0)
-
-            # AIS First Page
-            if (
-                "associationforinformationsystemsaiselectroniclibrary(aisel)" in page0
-                and "abstract" not in page0
-                and "keywords" not in page0
-            ):
-                coverpages.append(0)
-
-            # Remove Taylor and Francis First Page
-            if ("pleasescrolldownforarticle" in page0) or (
-                "viewrelatedarticles" in page0
-            ):
-                if "abstract" not in page0 and "keywords" not in page0:
-                    coverpages.append(0)
-                    if (
-                        "terms-and-conditions" in page1
-                        and "abstract" not in page1
-                        and "keywords" not in page1
-                    ):
-                        coverpages.append(1)
-
-            return list(set(coverpages))
-
-        coverpages = __get_coverpages(pdf=record.data["file"])
+        coverpages = self.__get_coverpages(pdf=record.data["file"])
         if not coverpages:
             return record.data
         if coverpages:
             original = pdf_prep_operation.review_manager.path / Path(
                 record.data["file"]
             )
             file_copy = pdf_prep_operation.review_manager.path / Path(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/last_page.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/last_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,14 @@
         self,
         *,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
-        if not pdf_prep_operation.review_manager.in_ci_environment():
-            # Note : to pull image if not available
-            pdf_prep_operation.review_manager.get_pdf_hash_service()
-
     @timeout_decorator.timeout(60, use_signals=False)
     def prep_pdf(
         self,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,
         record: colrev.record.Record,
         pad: int,  # pylint: disable=unused-argument
     ) -> dict:
@@ -68,17 +64,15 @@
             try:
                 pdf_reader = PdfFileReader(str(pdf), strict=False)
             except ValueError:
                 return last_pages
 
             last_page_nr = len(pdf_reader.pages) - 1
 
-            pdf_hash_service = pdf_prep_operation.review_manager.get_pdf_hash_service()
-
-            last_page_average_hash_16 = pdf_hash_service.get_pdf_hash(
+            last_page_average_hash_16 = colrev.qm.colrev_pdf_id.get_pdf_hash(
                 pdf_path=Path(pdf),
                 page_nr=last_page_nr + 1,
                 hash_size=16,
             )
 
             if last_page_nr == 1:
                 return last_pages
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/metadata_validation.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/metadata_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,15 @@
 
         try:
             retrieved_record = local_index.retrieve(record_dict=record.data)
 
             pdf_path = pdf_prep_operation.review_manager.path / Path(
                 record.data["file"]
             )
-            current_cpid = record.get_colrev_pdf_id(
-                review_manager=pdf_prep_operation.review_manager, pdf_path=pdf_path
-            )
+            current_cpid = record.get_colrev_pdf_id(pdf_path=pdf_path)
 
             if "colrev_pdf_id" in retrieved_record:
                 if retrieved_record["colrev_pdf_id"] == str(current_cpid):
                     # pdf_prep_operation.review_manager.logger.debug(
                     #     "validated pdf metadata based on local_index "
                     #     f"({record.data['ID']})"
                     # )
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep/tei_prep.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep/tei_prep.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.py` & `colrev-0.8.3/colrev/ops/built_in/pdf_prep_man/pdf_prep_man_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,48 +53,48 @@
         print(
             "Update metadata fields: "
             "(a)uthor, (c)ontainer title, (t)itle, (v)olume, (n)umber, (p)ages  or (s)ave"
         )
         while user_selection not in valid_selections:
             user_selection = input("Selection: ")
 
-            if "s" == user_selection:
+            if user_selection == "s":
                 break
-            if "a" == user_selection:
+            if user_selection == "a":
                 author = input("Authors:")
                 record.update_field(
                     key="author", value=author, source="manual_correction"
                 )
-            elif "c" == user_selection:
+            elif user_selection == "c":
                 if "journal" in record.data:
                     journal = input("Journal:")
                     record.update_field(
                         key="journal", value=journal, source="manual_correction"
                     )
                 if "booktitle" in record.data:
                     booktitle = input("Booktitle:")
                     record.update_field(
                         key="booktitle", value=booktitle, source="manual_correction"
                     )
-            elif "t" == user_selection:
+            elif user_selection == "t":
                 title = input("Title:")
                 record.update_field(
                     key="title", value=title, source="manual_correction"
                 )
-            elif "v" == user_selection:
+            elif user_selection == "v":
                 volume = input("Volume:")
                 record.update_field(
                     key="volume", value=volume, source="manual_correction"
                 )
-            elif "n" == user_selection:
+            elif user_selection == "n":
                 number = input("Number:")
                 record.update_field(
                     key="number", value=number, source="manual_correction"
                 )
-            elif "p" == user_selection:
+            elif user_selection == "p":
                 pages = input("Pages:")
                 record.update_field(
                     key="pages", value=pages, source="manual_correction"
                 )
             user_selection = ""
 
         return record
@@ -143,17 +143,15 @@
 
             filepath = pdf_prep_man.review_manager.path / Path(record_dict["file"])
             if not filepath.is_file():
                 filepath = (
                     pdf_prep_man.review_manager.pdf_dir / f"{record_dict['ID']}.pdf"
                 )
             record.data.update(
-                colrev_pdf_id=record.get_colrev_pdf_id(
-                    review_manager=pdf_prep_man.review_manager, pdf_path=filepath
-                )
+                colrev_pdf_id=record.get_colrev_pdf_id(pdf_path=filepath)
             )
             if filepath.is_file():
                 current_platform = platform.system()
                 if current_platform == "Linux":
                     subprocess.call(["xdg-open", filepath])
                 else:
                     os.startfile(filepath)  # type: ignore
@@ -174,31 +172,31 @@
                 while user_selection not in valid_selections:
                     user_selection = input("Selection: ")
                     if user_selection.startswith("s"):
                         if user_selection[1:].isdigit():
                             nonlocal to_skip
                             to_skip = int(user_selection[1:])
                         return records
-                    if "q" == user_selection:
+                    if user_selection == "q":
                         raise QuitPressedException()
 
-                    if "m" == user_selection:
+                    if user_selection == "m":
                         self.__update_metadata(record=record)
                         print(intro_paragraph)
-                    elif "c" == user_selection:
+                    elif user_selection == "c":
                         try:
                             pdf_prep_man_operation.extract_coverpage(filepath=filepath)
                         except colrev_exceptions.InvalidPDFException:
                             pass
-                    elif "l" == user_selection:
+                    elif user_selection == "l":
                         try:
                             pdf_prep_man_operation.extract_lastpage(filepath=filepath)
                         except colrev_exceptions.InvalidPDFException:
                             pass
-                    elif "r" == user_selection:
+                    elif user_selection == "r":
                         range_str = ""
                         while not re.match(r"(\d)+-(\d)+", range_str):
                             range_str = input('Page range to remove (e.g., "0-10"):')
 
                         pages_to_exclude = list(
                             range(
                                 int(range_str[: range_str.find("-")]),
@@ -208,17 +206,17 @@
                         try:
                             pdf_prep_man_operation.extract_pages(
                                 filepath=filepath, pages_to_remove=pages_to_exclude
                             )
                         except colrev_exceptions.InvalidPDFException:
                             pass
 
-                    elif "y" == user_selection:
+                    elif user_selection == "y":
                         pdf_prep_man_operation.set_pdf_man_prepared(record=record)
-                    elif "n" == user_selection:
+                    elif user_selection == "n":
                         record.remove_field(key="file")
                         record.set_status(
                             target_state=colrev.record.RecordState.pdf_needs_manual_retrieval
                         )
                         if filepath.is_file():
                             filepath.unlink()
                     else:
@@ -247,15 +245,15 @@
             except QuitPressedException:
                 break
 
         pdf_prep_man_operation.review_manager.dataset.save_records_dict(records=records)
         pdf_prep_man_operation.review_manager.dataset.add_record_changes()
 
         if pdf_prep_man_operation.pdfs_prepared_manually():
-            if "y" == input("Create commit (y/n)?"):
+            if input("Create commit (y/n)?") == "y":
                 pdf_prep_man_operation.review_manager.create_commit(
                     msg="Prepare PDFs manually",
                     manual_author=True,
                 )
         else:
             pdf_prep_man_operation.review_manager.logger.info(
                 "Prepare PDFs manually. Afterwards, use colrev pdf-get-man"
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/bibtex_crossref_resolution.py` & `colrev-0.8.3/colrev/ops/built_in/prep/bibtex_crossref_resolution.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
 
+# pylint: disable=duplicate-code
+# pylint: disable=too-few-public-methods
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.prep
         import colrev.env.local_index
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=duplicate-code
-
 
 @zope.interface.implementer(colrev.env.package_manager.PrepPackageEndpointInterface)
 @dataclass
 class BibTexCrossrefResolutionPrep(JsonSchemaMixin):
     """Prepares records by resolving BibTex crossref links (e.g., to proceedings)"""
 
     settings_class = colrev.env.package_manager.DefaultSettings
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/citeas_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/citeas_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """Consolidation of metadata based on CiteAs API as a prep operation"""
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 
 import requests
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.search_sources
 import colrev.record
@@ -79,15 +78,14 @@
         if "DOI" in data["metadata"]:
             retrieved_record.update(doi=data["metadata"]["DOI"])
 
         record = colrev.record.PrepRecord(data=retrieved_record)
         record.add_provenance_all(source=url)
         return record
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record based on citeas"""
 
         if record.data.get("ENTRYTYPE", "NA") not in ["misc", "software"]:
             return record
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/crossref_metadata_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/crossref_metadata_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on Crossref API as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.crossref as crossref_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -58,15 +57,14 @@
 
     def check_availability(
         self, *, source_operation: colrev.operation.Operation
     ) -> None:
         """Check status (availability) of the Crossref API"""
         self.crossref_source.check_availability(source_operation=source_operation)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare a record based on Crossref metadata"""
 
         if any(
             crossref_prefix in o
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/curation_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/curation_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Preparation of curations"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
 
@@ -39,15 +38,14 @@
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
         self.prep_operation = prep_operation
 
-    @timeout_decorator.timeout(20, use_signals=False)
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare records in a CoLRev curation"""
 
@@ -56,17 +54,17 @@
         if (
             record.data["colrev_status"]
             == colrev.record.RecordState.rev_prescreen_excluded
         ):
             return record
 
         if record.data.get("year", "UNKNOWN") == "UNKNOWN":
-            record.data[
-                "colrev_status"
-            ] = colrev.record.RecordState.md_needs_manual_preparation
+            record.set_status(
+                target_state=colrev.record.RecordState.md_needs_manual_preparation
+            )
             colrev.record.Record(data=record.data).add_masterdata_provenance(
                 key="year",
                 source="colrev_curation.masterdata_restrictions",
                 note="missing",
             )
             return record
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/dblp_metadata_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/dblp_metadata_prep.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on DBLP API as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.dblp as dblp_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -50,15 +49,14 @@
 
     def check_availability(
         self, *, source_operation: colrev.operation.Operation
     ) -> None:
         """Check status (availability) of the Crossref API"""
         self.dblp_source.check_availability(source_operation=source_operation)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare a record by retrieving its metadata from DBLP"""
 
         self.dblp_source.get_masterdata(prep_operation=prep_operation, record=record)
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/doi_from_urls_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/doi_from_urls_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import collections
 import re
 from dataclasses import dataclass
 from sqlite3 import OperationalError
 
 import requests
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.built_in.search_sources.doi_org as doi_connector
 import colrev.ops.search_sources
@@ -56,15 +55,14 @@
             self.session = prep_operation.review_manager.get_cached_session()
         except OperationalError as exc:
             raise colrev_exceptions.ServiceNotAvailableException(
                 dep="sqlite-requests-cache"
             ) from exc
         _, self.email = prep_operation.review_manager.get_committer()
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record by retrieving its DOI from the website (url) if available"""
 
         if ("url" not in record.data and "fulltext" not in record.data) or (
             "doi" in record.data
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/doi_metadata_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/doi_metadata_prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on DOI metadata as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.doi_org as doi_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -42,15 +41,14 @@
         self,
         *,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record by retrieving its metadata from doi.org"""
 
         if "doi" not in record.data:
             return record
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/europe_pmc_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/europe_pmc_prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on Europe PMC API as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.europe_pmc as europe_pmc_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -38,15 +37,14 @@
         self,
         *,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare a record based on Europe PMC metadata"""
 
         # pylint: disable=invalid-name
         EuropePMCSearchSource = europe_pmc_connector.EuropePMCSearchSource(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/exclude_collections.py` & `colrev-0.8.3/colrev/ops/built_in/prep/exclude_collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare records by excluding collections (proceedings)"""
 
-        if "proceedings" == record.data["ENTRYTYPE"].lower():
+        if record.data["ENTRYTYPE"].lower() == "proceedings":
             record.prescreen_exclude(reason="collection/proceedings")
 
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/exclude_complementary_materials.py` & `colrev-0.8.3/colrev/ops/built_in/prep/exclude_complementary_materials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Exclude complementary materials as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from alphabet_detector import AlphabetDetector
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
@@ -49,15 +48,14 @@
         )
 
         # for exact matches:
         self.complementary_materials_strings = (
             colrev.env.utils.load_complementary_material_strings()
         )
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare the records by excluding complementary materials"""
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/exclude_languages.py` & `colrev-0.8.3/colrev/ops/built_in/prep/exclude_languages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python
 """Exclude records based on language as a prep operation"""
 from __future__ import annotations
 
+import re
+import statistics
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.language_service
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
@@ -56,15 +57,25 @@
                     scope_prescreen.get("LanguageScope", ["eng"])
                 )
         self.language_service.validate_iso_639_3_language_codes(
             lang_code_list=languages_to_include
         )
         self.languages_to_include = list(set(languages_to_include))
 
-    @timeout_decorator.timeout(60, use_signals=False)
+    def __title_has_multiple_languages(self, *, title: str) -> bool:
+        if "[" not in title:
+            return False
+        split_titles = [
+            re.sub(r"\d", "", x.rstrip().rstrip("]")) for x in title.split("[")
+        ]
+        min_len = statistics.mean(len(x) for x in split_titles) - 20
+        if all(len(x) > min_len for x in split_titles):
+            return True
+        return False
+
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare the record by excluding records whose metadata is not in English"""
 
@@ -84,15 +95,15 @@
         # To avoid misclassifications for short titles
         if len(record.data.get("title", "")) < 30:
             # If language not in record, add language
             # (always - needed in dedupe.)
             record.data["language"] = "eng"
             return record
 
-        if record.data.get("title", "").count("[") == 0:
+        if not self.__title_has_multiple_languages(title=record.data.get("title", "")):
             language = self.language_service.compute_language(text=record.data["title"])
             record.update_field(
                 key="language",
                 value=language,
                 source="LanguageDetector",
                 note="",
                 append_edit=False,
@@ -120,15 +131,15 @@
                 else:
                     record.update_field(
                         key=f"title_{lang_split_title}",
                         value=split_title.rstrip("]"),
                         source="LanguageDetector_split",
                     )
 
-        if "" == record.data.get("language", ""):
+        if record.data.get("language", "") == "":
             record.update_field(
                 key="title",
                 value=record.data.get("title", ""),
                 source="LanguageDetector",
                 note="language-not-found",
             )
             record.set_status(
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/exclude_non_latin_alphabets.py` & `colrev-0.8.3/colrev/ops/built_in/prep/exclude_non_latin_alphabets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Exclude records with non-latin alphabets as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from alphabet_detector import AlphabetDetector
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
@@ -40,15 +39,14 @@
         self,
         *,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare the records by excluding records whose metadata is not in Latin alphabet"""
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/general_polish.py` & `colrev-0.8.3/colrev/ops/built_in/prep/general_polish.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/global_id_consistency.py` & `colrev-0.8.3/colrev/ops/built_in/prep/global_id_consistency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Checks of consistency between global IDs a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 from thefuzz import fuzz
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.crossref as crossref_connector
 import colrev.ops.built_in.search_sources.website as website_connector
@@ -74,31 +73,31 @@
 
         for key, value in crossref_md.data.items():
             if key not in self.__fields_to_check:
                 continue
             if not isinstance(value, str):
                 continue
             if key in record.data:
-                if "UNKNOWN" == record.data[key]:
+                if record.data[key] == "UNKNOWN":
                     continue
                 if key in ["author", "title", "journal"]:
                     if len(crossref_md.data[key]) < 5 or len(record.data[key]) < 5:
                         continue
                 if (
                     fuzz.partial_ratio(
                         record.data[key].lower(), crossref_md.data[key].lower()
                     )
                     < 70
                 ):
                     if record.masterdata_is_curated():
                         record.remove_field(key="doi")
                     else:
-                        record.data[
-                            "colrev_status"
-                        ] = colrev.record.RecordState.md_needs_manual_preparation
+                        record.set_status(
+                            target_state=colrev.record.RecordState.md_needs_manual_preparation
+                        )
                         record.add_masterdata_provenance_note(
                             key=key, note="disagreement with doi metadata"
                         )
 
     def __validate_against_url_metadata(self, *, record: colrev.record.Record) -> None:
         if "url" not in record.data:
             return
@@ -127,25 +126,24 @@
                             record.data[key].lower(), url_record.data[key].lower()
                         )
                         < 70
                     ):
                         if record.masterdata_is_curated():
                             record.remove_field(key="url")
                         else:
-                            record.data[
-                                "colrev_status"
-                            ] = colrev.record.RecordState.md_needs_manual_preparation
+                            record.set_status(
+                                target_state=colrev.record.RecordState.md_needs_manual_preparation
+                            )
                             record.add_masterdata_provenance_note(
                                 key=key,
                                 note=f"disagreement with website metadata ({value})",
                             )
         except AttributeError:
             pass
 
-    @timeout_decorator.timeout(40, use_signals=False)
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,
         record: colrev.record.PrepRecord,
     ) -> colrev.record.Record:
         """Prepare records by removing IDs (DOIs/URLs) that do not match with the metadata
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/local_index_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/local_index_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Conslidation of metadata based on LocalIndex as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.local_index as local_index_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -42,15 +41,14 @@
     def __init__(self, *, prep_operation: colrev.ops.prep.Prep, settings: dict) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
         self.local_index_source = local_index_connector.LocalIndexSearchSource(
             source_operation=prep_operation
         )
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record metadata based on local-index"""
 
         # don't move to  jour_iss_number_year prep
         # because toc-retrieval relies on adequate toc items!
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/open_library_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/open_library_prep.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on OpenLibrary API as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.open_library as open_library_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -49,15 +48,14 @@
         self, *, source_operation: colrev.operation.Operation
     ) -> None:
         """Check status (availability) of the Crossref API"""
         self.open_library_connector.check_availability(
             source_operation=source_operation
         )
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record metadata based on OpenLibrary"""
 
         if record.data.get("ENTRYTYPE", "NA") != "book":
             return record
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/pubmed_metadata_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/pubmed_metadata_prep.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #! /usr/bin/env python
 """Consolidation of metadata based on the Pubmed API as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.built_in.search_sources.pubmed as pubmed_connector
 import colrev.ops.search_sources
 import colrev.record
@@ -56,15 +55,14 @@
 
     def check_availability(
         self, *, source_operation: colrev.operation.Operation
     ) -> None:
         """Check status (availability) of the Pubmed API"""
         self.pubmed_source.check_availability(source_operation=source_operation)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare a record based on Pubmed metadata"""
 
         if any(
             pubmed_prefix in o
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/remove_broken_ids.py` & `colrev-0.8.3/colrev/ops/built_in/prep/remove_broken_ids.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/remove_error500_urls.py` & `colrev-0.8.3/colrev/ops/built_in/prep/remove_error500_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #! /usr/bin/env python
 """Removal of broken URLs (error 500) a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 import requests
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
 
@@ -38,29 +37,28 @@
         self,
         *,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record by removing URLs with 500 errors"""
 
         session = prep_operation.review_manager.get_cached_session()
 
         try:
             if "url" in record.data:
                 ret = session.request(
                     "GET",
                     record.data["url"],
                     headers=prep_operation.requests_headers,
-                    timeout=prep_operation.timeout,
+                    timeout=60,
                 )
                 if ret.status_code >= 500:
                     record.remove_field(key="url")
         except requests.exceptions.RequestException:
             pass
         try:
             if "fulltext" in record.data:
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/semantic_scholar_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/semantic_scholar_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """Consolidation of metadata based on SemanticScholar API as a prep operation"""
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 
 import requests
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.search_sources
 import colrev.record
@@ -62,15 +61,15 @@
             authors_string = colrev.record.PrepRecord.format_author_field(
                 input_string=authors_string
             )
             retrieved_record.update(author=authors_string)
         if "abstract" in item:
             retrieved_record.update(abstract=item["abstract"])
         if "doi" in item:
-            if "none" != str(item["doi"]).lower():
+            if str(item["doi"]).lower() != "none":
                 retrieved_record.update(doi=str(item["doi"]).upper())
         if "title" in item:
             retrieved_record.update(title=item["title"])
         if "year" in item:
             retrieved_record.update(year=item["year"])
         # Note: semantic scholar does not provide data on the type of venue.
         # we therefore use the original ENTRYTYPE
@@ -128,15 +127,14 @@
         item = json.loads(ret_ent.text)
 
         record = self.__get_record_from_item(item=item, record_in=record_in)
         record.add_provenance_all(source=record_retrieval_url)
 
         return record
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare a record based on metadata from SemanticScholar"""
 
         same_record_type_required = (
             prep_operation.review_manager.settings.is_curated_masterdata_repo()
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/source_specific_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/source_specific_prep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 """Source-specific preparation as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
 
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.ops.search_sources
 import colrev.record
 
+# pylint: disable=duplicate-code
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.prep
 
 # pylint: disable=too-few-public-methods
@@ -41,15 +41,14 @@
     ) -> None:
         self.settings = self.settings_class.load_settings(data=settings)
 
         self.search_sources = colrev.ops.search_sources.SearchSources(
             review_manager=prep_operation.review_manager
         )
 
-    @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
     ) -> colrev.record.Record:
         """Prepare the record by applying source-specific fixes"""
 
         # Note : we take the first origin (ie., the source-specific prep should
         # be one of the first in the prep-list)
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/update_masterdata_status.py` & `colrev-0.8.3/colrev/ops/built_in/prep/update_masterdata_status.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep/year_vol_iss_prep.py` & `colrev-0.8.3/colrev/ops/built_in/prep/year_vol_iss_prep.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #! /usr/bin/env python
 """Completion of metadata based on year-volume-issue dependency as a prep operation"""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 import requests
-import timeout_decorator
 import zope.interface
 from dataclasses_jsonschema import JsonSchemaMixin
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.built_in.search_sources.crossref as crossref_connector
 import colrev.ops.search_sources
@@ -84,97 +83,74 @@
                         ] = record["year"]
                     else:
                         # do not use inconsistent data (has/has no number)
                         del vol_nr_dict[record["journal"]][record["volume"]]
 
         self.vol_nr_dict = vol_nr_dict
 
-    @timeout_decorator.timeout(60, use_signals=False)
-    def prepare(
-        self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
-    ) -> colrev.record.Record:
-        """Prepare a record based on year-volume-issue dependency"""
-
-        # pylint: disable=too-many-nested-blocks
-        # pylint: disable=too-many-return-statements
-        # pylint: disable=too-many-branches
-
-        if record.data.get("year", "NA").isdigit() or record.masterdata_is_curated():
-            return record
-
+    def __get_year_from_toc(self, *, record: colrev.record.Record) -> None:
         # TBD: maybe extract the following three lines as a separate script...
         try:
             year = self.local_index.get_year_from_toc(record_dict=record.get_data())
             record.update_field(
                 key="year",
                 value=year,
                 source="LocalIndexPrep",
                 note="",
                 keep_source_if_equal=True,
             )
-            return record
         except colrev_exceptions.TOCNotAvailableException:
             pass
 
-        if "journal" in record.data:
-            if record.data["journal"] in self.vol_nr_dict:
-                if "volume" in record.data:
-                    if (
+    def __get_year_from_vol_nr_dict(self, *, record: colrev.record.Record) -> None:
+        if "journal" not in record.data or "volume" not in record.data:
+            return
+
+        if record.data["journal"] not in self.vol_nr_dict:
+            return
+
+        if record.data["volume"] not in self.vol_nr_dict[record.data["journal"]]:
+            return
+
+        if "number" in record.data:
+            if (
+                record.data["number"]
+                in self.vol_nr_dict[record.data["journal"]][record.data["volume"]]
+            ):
+                record.update_field(
+                    key="year",
+                    value=self.vol_nr_dict[record.data["journal"]][
                         record.data["volume"]
-                        in self.vol_nr_dict[record.data["journal"]]
-                    ):
-                        if "number" in record.data:
-                            if (
-                                record.data["number"]
-                                in self.vol_nr_dict[record.data["journal"]][
-                                    record.data["volume"]
-                                ]
-                            ):
-                                record.update_field(
-                                    key="year",
-                                    value=self.vol_nr_dict[record.data["journal"]][
-                                        record.data["volume"]
-                                    ][record.data["number"]],
-                                    source="year_vol_iss_prep",
-                                    note="",
-                                )
-                                record.update_masterdata_provenance()
-                                return record
-                        else:
-                            if isinstance(
-                                self.vol_nr_dict[record.data["journal"]][
-                                    record.data["volume"]
-                                ],
-                                (str, int),
-                            ):
-                                record.update_field(
-                                    key="year",
-                                    value=self.vol_nr_dict[record.data["journal"]][
-                                        record.data["volume"]
-                                    ],
-                                    source="year_vol_iss_prep",
-                                    note="",
-                                )
-                                record.update_masterdata_provenance()
-                                return record
-
-        # The year depends on journal x volume x issue
-        if (
-            "journal" in record.data
-            and "volume" in record.data
-            and "number" in record.data
-        ) and "UNKNOWN" == record.data.get("year", "UNKNOWN"):
-            pass
+                    ][record.data["number"]],
+                    source="year_vol_iss_prep",
+                    note="",
+                )
+                record.update_masterdata_provenance()
         else:
-            return record
+            if isinstance(
+                self.vol_nr_dict[record.data["journal"]][record.data["volume"]],
+                (str, int),
+            ):
+                record.update_field(
+                    key="year",
+                    value=self.vol_nr_dict[record.data["journal"]][
+                        record.data["volume"]
+                    ],
+                    source="year_vol_iss_prep",
+                    note="",
+                )
+                record.update_masterdata_provenance()
 
-        crossref_source = crossref_connector.CrossrefSearchSource(
-            source_operation=prep_operation
-        )
+    def __get_year_from_crossref(
+        self, *, record: colrev.record.Record, prep_operation: colrev.ops.prep.Prep
+    ) -> None:
         try:
+            crossref_source = crossref_connector.CrossrefSearchSource(
+                source_operation=prep_operation
+            )
             retrieved_records = crossref_source.crossref_query(
                 review_manager=prep_operation.review_manager,
                 record_input=record,
                 jour_vol_iss_list=True,
                 timeout=prep_operation.timeout,
             )
             retries = 0
@@ -185,36 +161,56 @@
                 retrieved_records = crossref_source.crossref_query(
                     review_manager=prep_operation.review_manager,
                     record_input=record,
                     jour_vol_iss_list=True,
                     timeout=prep_operation.timeout,
                 )
             if 0 == len(retrieved_records):
-                return record
+                return
 
             retrieved_records = [
                 retrieved_record
                 for retrieved_record in retrieved_records
                 if retrieved_record.data.get("volume", "NA")
                 == record.data.get("volume", "NA")
                 and retrieved_record.data.get("journal", "NA")
                 == record.data.get("journal", "NA")
                 and retrieved_record.data.get("number", "NA")
                 == record.data.get("number", "NA")
             ]
 
             years = [r.data["year"] for r in retrieved_records]
             if len(years) == 0:
-                return record
+                return
             most_common = max(years, key=years.count)
             if years.count(most_common) > 3:
                 record.update_field(
                     key="year", value=most_common, source="CROSSREF(average)", note=""
                 )
         except requests.exceptions.RequestException:
             pass
 
+    def prepare(
+        self, prep_operation: colrev.ops.prep.Prep, record: colrev.record.PrepRecord
+    ) -> colrev.record.Record:
+        """Prepare a record based on year-volume-issue dependency"""
+
+        if record.data.get("year", "NA").isdigit() or record.masterdata_is_curated():
+            return record
+
+        self.__get_year_from_toc(record=record)
+
+        if "year" in record.data:
+            return record
+
+        self.__get_year_from_vol_nr_dict(record=record)
+
+        if "year" in record.data:
+            return record
+
+        self.__get_year_from_crossref(record=record, prep_operation=prep_operation)
+
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.py` & `colrev-0.8.3/colrev/ops/built_in/prep_man/curation_jupyter_prep_man.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/prep_man/prep_man_export.py` & `colrev-0.8.3/colrev/ops/built_in/prep_man/prep_man_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 from PyPDF2 import PdfFileReader
 from PyPDF2 import PdfFileWriter
 
 import colrev.env.package_manager
 import colrev.env.utils
 import colrev.record
 
+# pylint: disable=duplicate-code
+# pylint: disable=too-few-public-methods
+
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.prep_man
 
-# pylint: disable=too-few-public-methods
-
 
 @zope.interface.implementer(colrev.env.package_manager.PrepManPackageEndpointInterface)
 @dataclass
 class ExportManPrep(JsonSchemaMixin):
     """Manual preparation based on exported and imported metadata (and PDFs if any)"""
 
+    settings: ExportManPrepSettings
     ci_supported: bool = False
 
     RELATIVE_PREP_MAN_PATH = Path("records_prep_man.bib")
 
     @dataclass
     class ExportManPrepSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
@@ -79,18 +81,18 @@
         prep_man_path_pdfs.mkdir(exist_ok=True, parents=True)
 
         for record in records.values():
             if "file" in record:
                 target_path = self.review_manager.prep_dir / Path(record["file"])
                 target_path.parents[0].mkdir(exist_ok=True, parents=True)
 
-                if "symlink" == self.settings.pdf_handling_mode:
+                if self.settings.pdf_handling_mode == "symlink":
                     target_path.symlink_to(Path(record["file"]).resolve())
 
-                if "copy_first_page" == self.settings.pdf_handling_mode:
+                if self.settings.pdf_handling_mode == "copy_first_page":
                     pdf_reader = PdfFileReader(str(record["file"]), strict=False)
                     if len(pdf_reader.pages) >= 1:
                         writer = PdfFileWriter()
                         writer.addPage(pdf_reader.getPage(0))
                         with open(target_path, "wb") as outfile:
                             writer.write(outfile)
 
@@ -213,15 +215,15 @@
             self.__export_prep_man(
                 prep_man_operation=prep_man_operation, records=records
             )
         else:
             selected_path = self.prep_man_bib_path.relative_to(
                 prep_man_operation.review_manager.path
             )
-            if "y" == input(f"Import changes from {selected_path} [y,n]?"):
+            if input(f"Import changes from {selected_path} [y,n]?") == "y":
                 self.__import_prep_man(prep_man_operation=prep_man_operation)
 
         return records
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prescreen/asreview.py` & `colrev-0.8.3/colrev/ops/built_in/prescreen/asreview.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,20 +177,20 @@
             # f"\n{prescreen.review_manager.p_printer.pformat(json_data['settings'])}"
             # )
 
         if asreview_project_file.suffix == ".csv":  # "Export results" in asreview
             to_import = pd.read_csv(asreview_project_file)
             for _, row in to_import.iterrows():
                 prescreen_record = colrev.record.Record(data=records[row["ID"]])
-                if "1" == str(row["included"]):
+                if str(row["included"]) == "1":
                     prescreen_operation.prescreen(
                         record=prescreen_record,
                         prescreen_inclusion=True,
                     )
-                elif "0" == str(row["included"]):
+                elif str(row["included"]) == "0":
                     prescreen_operation.prescreen(
                         record=prescreen_record,
                         prescreen_inclusion=False,
                     )
                 else:
                     print(f'not prescreened: {row["ID"]}')
 
@@ -244,19 +244,19 @@
 
             try:
                 asreview = LABEntryPoint()
                 asreview.execute(argv={})
             except KeyboardInterrupt:
                 print("\n\n\nCompleted prescreen. ")
 
-        if "y" == input("Import prescreen from asreview [y,n]?"):
+        if input("Import prescreen from asreview [y,n]?") == "y":
             self.__import_from_asreview(prescreen_operation, records)
 
             if prescreen_operation.review_manager.dataset.has_changes():
-                if "y" == input("create commit [y,n]?"):
+                if input("create commit [y,n]?") == "y":
                     prescreen_operation.review_manager.create_commit(
                         msg="Pre-screen (asreview)",
                         manual_author=True,
                     )
 
         return records
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prescreen/conditional_prescreen.py` & `colrev-0.8.3/colrev/ops/built_in/prescreen/conditional_prescreen.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_cli.py` & `colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         *,
         prescreen_operation: colrev.ops.prescreen.Prescreen,
         prescreen_data: dict,
         split: list,
         stat_len: int,
         padding: int,
     ) -> bool:
-        if "" == prescreen_operation.review_manager.settings.prescreen.explanation:
+        if prescreen_operation.review_manager.settings.prescreen.explanation == "":
             print(
                 f"\n{colors.ORANGE}Provide a short explanation of the prescreen{colors.END} "
                 "(why should particular papers be included?):"
             )
             print(
                 'Example objective: "Include papers that focus on digital technology."'
             )
@@ -87,26 +87,26 @@
             record.print_prescreen_record()
 
             while ret not in ["y", "n", "s", "q"]:
                 ret = input(
                     "\nInclude this record "
                     "[enter y,n,s,q for yes, no, skip/decide later, quit-and-save]? "
                 )
-                if "q" == ret:
+                if ret == "q":
                     quit_pressed = True
-                elif "s" == ret:
+                elif ret == "s":
                     continue
                 else:
                     inclusion_decision_str = ret.replace("y", "yes").replace("n", "no")
 
             if quit_pressed:
                 prescreen_operation.review_manager.logger.info("Stop prescreen")
                 break
 
-            if "s" == ret:
+            if ret == "s":
                 continue
 
             inclusion_decision = "yes" == inclusion_decision_str
             prescreen_operation.prescreen(
                 record=record,
                 prescreen_inclusion=inclusion_decision,
                 PAD=padding,
@@ -143,15 +143,15 @@
 
         # Note : currently, it is easier to create a commit in all cases.
         # Upon continuing the prescreen, the scope-based prescreen commits the changes,
         # which is misleading.
         # Users can still squash commits.
         # Note: originall: completed = self.__fun_cli_prescreen(...
         # if not completed:
-        #     if "y" != input("Create commit (y/n)?"):
+        #     if input("Create commit (y/n)?") != "y":
         #         return records
 
         prescreen_operation.review_manager.create_commit(
             msg="Pre-screening (manual)", manual_author=True
         )
         return records
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prescreen/prescreen_table.py` & `colrev-0.8.3/colrev/ops/built_in/prescreen/prescreen_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,20 +106,20 @@
                 "pages": record.get("pages", ""),
                 "doi": record.get("doi", ""),
                 "abstract": record.get("abstract", ""),
                 "presceen_inclusion": inclusion_1,
             }
             tbl.append(row)
 
-        if "csv" == export_table_format.lower():
+        if export_table_format.lower() == "csv":
             screen_df = pd.DataFrame(tbl)
             screen_df.to_csv("prescreen.csv", index=False, quoting=csv.QUOTE_ALL)
             prescreen_operation.review_manager.logger.info("Created prescreen.csv")
 
-        if "xlsx" == export_table_format.lower():
+        if export_table_format.lower() == "xlsx":
             screen_df = pd.DataFrame(tbl)
             screen_df.to_excel("prescreen.xlsx", index=False, sheet_name="screen")
             prescreen_operation.review_manager.logger.info("Created prescreen.xlsx")
 
         prescreen_operation.review_manager.logger.info(
             f"To prescreen records, {colors.ORANGE}enter [in|out] "
             f"in the presceen_inclusion column.{colors.END}"
@@ -160,47 +160,49 @@
 
         prescreen_included = 0
         prescreen_excluded = 0
         nr_todo = 0
         prescreen_operation.review_manager.logger.info("Update prescreen results")
         for prescreened_record in prescreened_records:
             if prescreened_record.get("ID", "") in records:
-                record = records[prescreened_record.get("ID", "")]
-                if record[
+                record = colrev.record.Record(
+                    data=records[prescreened_record.get("ID", "")]
+                )
+                if record.data[
                     "colrev_status"
                 ] in colrev.record.RecordState.get_post_x_states(
                     state=colrev.record.RecordState.rev_prescreen_included
                 ):
                     if (
-                        "in" == prescreened_record.get("presceen_inclusion", "")
+                        "in" == prescreened_record.data.get("presceen_inclusion", "")
                         and colrev.record.RecordState.rev_prescreen_excluded
-                        != record["colrev_status"]
+                        != record.data["colrev_status"]
                     ):
                         continue
 
-                if "out" == prescreened_record.get("presceen_inclusion", ""):
+                if prescreened_record.get("presceen_inclusion", "") == "out":
                     if (
-                        record["colrev_status"]
+                        record.data["colrev_status"]
                         != colrev.record.RecordState.rev_prescreen_excluded
                     ):
                         prescreen_excluded += 1
-                    record[
-                        "colrev_status"
-                    ] = colrev.record.RecordState.rev_prescreen_excluded
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_prescreen_excluded
+                    )
 
-                elif "in" == prescreened_record.get("presceen_inclusion", ""):
+                elif prescreened_record.get("presceen_inclusion", "") == "in":
                     if (
-                        record["colrev_status"]
+                        record.data["colrev_status"]
                         != colrev.record.RecordState.rev_prescreen_included
                     ):
                         prescreen_included += 1
-                    record[
-                        "colrev_status"
-                    ] = colrev.record.RecordState.rev_prescreen_included
-                elif "TODO" == prescreened_record.get("presceen_inclusion", ""):
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_prescreen_included
+                    )
+                elif prescreened_record.get("presceen_inclusion", "") == "TODO":
                     nr_todo += 1
                 else:
                     prescreen_operation.review_manager.logger.warning(
                         "Invalid value in prescreen_inclusion: "
                         f"{prescreened_record.get('presceen_inclusion', '')} "
                         f"({prescreened_record.get('ID', 'NO_ID')})"
                     )
@@ -230,24 +232,24 @@
         self,
         prescreen_operation: colrev.ops.prescreen.Prescreen,
         records: dict,
         split: list,
     ) -> dict:
         """Prescreen records based on screening tables"""
 
-        if "y" == input("create prescreen table [y,n]?"):
+        if input("create prescreen table [y,n]?") == "y":
             self.export_table(
                 prescreen_operation=prescreen_operation, records=records, split=split
             )
 
-        if "y" == input("import prescreen table [y,n]?"):
+        if input("import prescreen table [y,n]?") == "y":
             self.import_table(prescreen_operation=prescreen_operation, records=records)
 
         if prescreen_operation.review_manager.dataset.has_changes():
-            if "y" == input("create commit [y,n]?"):
+            if input("create commit [y,n]?") == "y":
                 prescreen_operation.review_manager.create_commit(
                     msg="Pre-screen (table)",
                     manual_author=True,
                 )
         return records
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/prescreen/scope_prescreen.py` & `colrev-0.8.3/colrev/ops/built_in/prescreen/scope_prescreen.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     colrev.env.package_manager.PrescreenPackageEndpointInterface
 )
 @dataclass
 class ScopePrescreen(JsonSchemaMixin):
 
     """Rule-based prescreen (scope)"""
 
+    settings: ScopePrescreenSettings
     ci_supported: bool = True
 
     @dataclass
     class ScopePrescreenSettings(
         colrev.env.package_manager.DefaultSettings, JsonSchemaMixin
     ):
         """Settings for ScopePrescreen"""
@@ -114,98 +115,102 @@
 
         if filedata:
             for pred_journal in filedata.decode("utf-8").splitlines():
                 predatory_journals[pred_journal.lower()] = pred_journal.lower()
 
         return predatory_journals
 
-    def __conditional_prescreen(
-        self, *, prescreen_operation: colrev.ops.prescreen.Prescreen, record_dict: dict
-    ) -> None:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-nested-blocks
-
-        if record_dict["colrev_status"] != colrev.record.RecordState.md_processed:
-            return
-
-        pad = 50
-
-        # Note : LanguageScope is covered in prep
-        # because dedupe cannot handle merges between languages
-
+    def __conditional_prescreen_entrytypes(self, record: colrev.record.Record) -> None:
         if self.settings.ENTRYTYPEScope:
-            if record_dict["ENTRYTYPE"] not in self.settings.ENTRYTYPEScope:
-                colrev.record.Record(data=record_dict).prescreen_exclude(
-                    reason="not in ENTRYTYPEScope"
-                )
+            if record.data["ENTRYTYPE"] not in self.settings.ENTRYTYPEScope:
+                record.prescreen_exclude(reason="not in ENTRYTYPEScope")
 
+    def __conditional_prescreen_outlets_exclusion(
+        self, record: colrev.record.Record
+    ) -> None:
         if self.settings.OutletExclusionScope:
             if "values" in self.settings.OutletExclusionScope:
                 for resource in self.settings.OutletExclusionScope["values"]:
                     for key, value in resource.items():
-                        if key in record_dict and record_dict.get(key, "") == value:
-                            colrev.record.Record(data=record_dict).prescreen_exclude(
-                                reason="in OutletExclusionScope"
-                            )
+                        if key in record.data and record.data.get(key, "") == value:
+                            record.prescreen_exclude(reason="in OutletExclusionScope")
             if "list" in self.settings.OutletExclusionScope:
                 for resource in self.settings.OutletExclusionScope["list"]:
                     for key, value in resource.items():
-                        if "resource" == key and "predatory_journals_beal" == value:
-                            if "journal" in record_dict:
-                                if (
-                                    record_dict["journal"].lower()
-                                    in self.predatory_journals_beal
-                                ):
-                                    colrev.record.Record(
-                                        data=record_dict
-                                    ).prescreen_exclude(
-                                        reason="predatory_journals_beal"
-                                    )
-
-        if self.settings.TimeScopeFrom:
-            if int(record_dict.get("year", 0)) < self.settings.TimeScopeFrom:
-                colrev.record.Record(data=record_dict).prescreen_exclude(
-                    reason="not in TimeScopeFrom " f"(>{self.settings.TimeScopeFrom})"
-                )
-
-        if self.settings.TimeScopeTo:
-            if int(record_dict.get("year", 5000)) > self.settings.TimeScopeTo:
-                colrev.record.Record(data=record_dict).prescreen_exclude(
-                    reason="not in TimeScopeTo " f"(<{self.settings.TimeScopeTo})"
-                )
+                        if not (
+                            key == "resource" and value == "predatory_journals_beal"
+                        ):
+                            continue
+                        if "journal" not in record.data:
+                            continue
+                        if (
+                            record.data["journal"].lower()
+                            in self.predatory_journals_beal
+                        ):
+                            record.prescreen_exclude(reason="predatory_journals_beal")
 
+    def __conditional_prescreen_outlets_inclusion(
+        self, record: colrev.record.Record
+    ) -> None:
         if self.settings.OutletInclusionScope:
             in_outlet_scope = False
             if "values" in self.settings.OutletInclusionScope:
                 for outlet in self.settings.OutletInclusionScope["values"]:
                     for key, value in outlet.items():
-                        if key in record_dict and record_dict.get(key, "") == value:
+                        if key in record.data and record.data.get(key, "") == value:
                             in_outlet_scope = True
             if not in_outlet_scope:
-                colrev.record.Record(data=record_dict).prescreen_exclude(
-                    reason="not in OutletInclusionScope"
+                record.prescreen_exclude(reason="not in OutletInclusionScope")
+
+    def __conditional_prescreen_timescope(self, record: colrev.record.Record) -> None:
+        if self.settings.TimeScopeFrom:
+            if int(record.data.get("year", 0)) < self.settings.TimeScopeFrom:
+                record.prescreen_exclude(
+                    reason="not in TimeScopeFrom " f"(>{self.settings.TimeScopeFrom})"
                 )
 
+        if self.settings.TimeScopeTo:
+            if int(record.data.get("year", 5000)) > self.settings.TimeScopeTo:
+                record.prescreen_exclude(
+                    reason="not in TimeScopeTo " f"(<{self.settings.TimeScopeTo})"
+                )
+
+    def __conditional_prescreen_complementary_materials(
+        self, record: colrev.record.Record
+    ) -> None:
         if self.settings.ExcludeComplementaryMaterials:
-            if self.settings.ExcludeComplementaryMaterials:
-                if "title" in record_dict:
-                    if (
-                        record_dict["title"].lower()
-                        in self.title_complementary_materials_keywords
-                    ):
-                        colrev.record.Record(data=record_dict).prescreen_exclude(
-                            reason="complementary material"
-                        )
+            if "title" in record.data:
+                if (
+                    record.data["title"].lower()
+                    in self.title_complementary_materials_keywords
+                ):
+                    record.prescreen_exclude(reason="complementary material")
+
+    def __conditional_prescreen(
+        self, *, prescreen_operation: colrev.ops.prescreen.Prescreen, record_dict: dict
+    ) -> None:
+        if record_dict["colrev_status"] != colrev.record.RecordState.md_processed:
+            return
+
+        # Note : LanguageScope is covered in prep
+        # because dedupe cannot handle merges between languages
+        record = colrev.record.Record(data=record_dict)
+
+        self.__conditional_prescreen_entrytypes(record=record)
+        self.__conditional_prescreen_outlets_inclusion(record=record)
+        self.__conditional_prescreen_outlets_exclusion(record=record)
+        self.__conditional_prescreen_timescope(record=record)
+        self.__conditional_prescreen_complementary_materials(record=record)
 
         if (
-            record_dict["colrev_status"]
+            record.data["colrev_status"]
             == colrev.record.RecordState.rev_prescreen_excluded
         ):
             prescreen_operation.review_manager.report_logger.info(
-                f' {record_dict["ID"]}'.ljust(pad, " ")
+                f' {record.data["ID"]}'.ljust(50, " ")
                 + "Prescreen excluded (automatically)"
             )
 
     def run_prescreen(
         self,
         prescreen_operation: colrev.ops.prescreen.Prescreen,
         records: dict,
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/conceptual_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/conceptual_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/critical_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/critical_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/curated_masterdata.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/curated_masterdata.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/descriptive_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/descriptive_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/literature_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/literature_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/meta_analysis.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/meta_analysis.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/narrative_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/narrative_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/qualitative_systematic_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/qualitative_systematic_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/scientometric.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/scientometric.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/scoping_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/scoping_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/review_types/theoretical_review.py` & `colrev-0.8.3/colrev/ops/built_in/review_types/theoretical_review.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/screen/screen_cli.py` & `colrev-0.8.3/colrev/ops/built_in/screen/screen_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,24 +65,143 @@
                 f" - {criterion_name} "
                 f"({color}{criterion_settings.criterion_type}{colors.END}): "
                 f"{criterion_settings.explanation}"
             )
             if criterion_settings.comment != "":
                 print(f"   {criterion_settings.comment}")
 
+    def __screen_with_criteria_print_overall_decision(
+        self, *, record: colrev.record.Record, screen_inclusion: bool
+    ) -> None:
+        if screen_inclusion:
+            print(
+                f"Overall screening decision for {record.data['ID']}: "
+                f"{colors.GREEN}include{colors.END}"
+            )
+        else:
+            print(
+                f"Overall screening decision for {record.data['ID']}: "
+                f"{colors.RED}exclude{colors.END}"
+            )
+
+    def __screen_record_with_criteria(
+        self,
+        *,
+        screen_operation: colrev.ops.screen.Screen,
+        record: colrev.record.Record,
+        abstract_from_tei: bool,
+    ) -> str:
+        decisions = []
+        quit_pressed, skip_pressed = False, False
+
+        for criterion_name, criterion_settings in self.screening_criteria.items():
+            decision, ret = "NA", "NA"
+            while ret not in ["y", "n", "q", "s"]:
+                color = colors.GREEN
+                if (
+                    colrev.settings.ScreenCriterionType.exclusion_criterion
+                    == criterion_settings.criterion_type
+                ):
+                    color = colors.RED
+
+                ret = input(
+                    # is relevant / should be in the sample / should be retained
+                    # ({self.__i}/{self.__stat_len})
+                    f"Record should be included according to"
+                    f" {criterion_settings.criterion_type}"
+                    f" {color}{criterion_name}{colors.END}"
+                    " [y,n,q,s for yes,no,quit,skip to decide later]? "
+                )
+                if ret == "q":
+                    quit_pressed = True
+                elif ret == "s":
+                    skip_pressed = True
+                    continue
+                elif ret in ["y", "n"]:
+                    decision = ret
+
+            if quit_pressed:
+                return "quit"
+            if skip_pressed:
+                return "skip"
+
+            decision = decision.replace("n", "out").replace("y", "in")
+            decisions.append([criterion_name, decision])
+
+        c_field = ""
+        for criterion_name, decision in decisions:
+            c_field += f";{criterion_name}={decision}"
+        c_field = c_field.replace(" ", "").lstrip(";")
+
+        screen_inclusion = all(decision == "in" for _, decision in decisions)
+        self.__screen_with_criteria_print_overall_decision(
+            record=record, screen_inclusion=screen_inclusion
+        )
+
+        if abstract_from_tei:
+            if "abstract" in record.data:
+                del record.data["abstract"]
+
+        screen_operation.screen(
+            record=record,
+            screen_inclusion=screen_inclusion,
+            screening_criteria=c_field,
+            PAD=self.__pad,
+        )
+        return "screened"
+
+    def __screen_record_without_criteria(
+        self,
+        *,
+        screen_operation: colrev.ops.screen.Screen,
+        record: colrev.record.Record,
+        abstract_from_tei: bool,
+    ) -> str:
+        quit_pressed = False
+        decision, ret = "NA", "NA"
+        while ret not in ["y", "n", "q", "s"]:
+            ret = input(
+                f"({self.__i}/{self.__stat_len}) "
+                "Include [y,n,q,s for yes, no, quit, skip/screen later]? "
+            )
+            if ret == "q":
+                quit_pressed = True
+            elif ret == "s":
+                return "skip"
+            elif ret in ["y", "n"]:
+                decision = ret
+
+        if quit_pressed:
+            screen_operation.review_manager.logger.info("Stop screen")
+            return "quit"
+
+        if abstract_from_tei:
+            if "abstract" in record.data:
+                del record.data["abstract"]
+        if decision == "y":
+            screen_operation.screen(
+                record=record,
+                screen_inclusion=True,
+                screening_criteria="NA",
+            )
+        if decision == "n":
+            screen_operation.screen(
+                record=record,
+                screen_inclusion=False,
+                screening_criteria="NA",
+                PAD=self.__pad,
+            )
+        return "screened"
+
     def __screen_record(
         self,
         *,
         screen_operation: colrev.ops.screen.Screen,
         record_dict: dict,
     ) -> str:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
-
         record = colrev.record.Record(data=record_dict)
         abstract_from_tei = False
         if (
             "abstract" not in record.data
             and Path(record.data.get("file", "")).suffix == ".pdf"
         ):
             try:
@@ -92,123 +211,33 @@
                     tei_path=record.get_tei_filename(),
                 )
                 record.data["abstract"] = tei.get_abstract()
             except (colrev_exceptions.ServiceNotAvailableException, XMLSyntaxError):
                 pass
 
         self.__i += 1
-        quit_pressed, skip_pressed = False, False
-
         print("\n\n")
         print(f"Record {self.__i} (of {self.__stat_len})")
         print(record)
 
         if self.criteria_available:
-            decisions = []
-
-            for criterion_name, criterion_settings in self.screening_criteria.items():
-                decision, ret = "NA", "NA"
-                while ret not in ["y", "n", "q", "s"]:
-                    color = colors.GREEN
-                    if (
-                        colrev.settings.ScreenCriterionType.exclusion_criterion
-                        == criterion_settings.criterion_type
-                    ):
-                        color = colors.RED
-
-                    ret = input(
-                        # is relevant / should be in the sample / should be retained
-                        # ({self.__i}/{self.__stat_len})
-                        f"Record should be included according to"
-                        f" {criterion_settings.criterion_type}"
-                        f" {color}{criterion_name}{colors.END}"
-                        " [y,n,q,s for yes,no,quit,skip to decide later]? "
-                    )
-                    if "q" == ret:
-                        quit_pressed = True
-                    elif "s" == ret:
-                        skip_pressed = True
-                        continue
-                    elif ret in ["y", "n"]:
-                        decision = ret
-
-                if quit_pressed:
-                    return "quit"
-                if skip_pressed:
-                    return "skip"
-
-                decision = decision.replace("n", "out").replace("y", "in")
-                decisions.append([criterion_name, decision])
-
-            c_field = ""
-            for criterion_name, decision in decisions:
-                c_field += f";{criterion_name}={decision}"
-            c_field = c_field.replace(" ", "").lstrip(";")
-
-            screen_inclusion = all(decision == "in" for _, decision in decisions)
-
-            if screen_inclusion:
-                print(
-                    f"Overall screening decision for {record_dict['ID']}: "
-                    f"{colors.GREEN}include{colors.END}"
-                )
-            else:
-                print(
-                    f"Overall screening decision for {record_dict['ID']}: "
-                    f"{colors.RED}exclude{colors.END}"
-                )
-
-            if abstract_from_tei:
-                if "abstract" in record.data:
-                    del record.data["abstract"]
-
-            screen_operation.screen(
+            ret = self.__screen_record_with_criteria(
+                screen_operation=screen_operation,
                 record=record,
-                screen_inclusion=screen_inclusion,
-                screening_criteria=c_field,
-                PAD=self.__pad,
+                abstract_from_tei=abstract_from_tei,
             )
 
         else:
-            decision, ret = "NA", "NA"
-            while ret not in ["y", "n", "q", "s"]:
-                ret = input(
-                    f"({self.__i}/{self.__stat_len}) "
-                    "Include [y,n,q,s for yes, no, quit, skip/screen later]? "
-                )
-                if "q" == ret:
-                    quit_pressed = True
-                elif "s" == ret:
-                    skip_pressed = True
-                    return "skip"
-                elif ret in ["y", "n"]:
-                    decision = ret
-
-            if quit_pressed:
-                screen_operation.review_manager.logger.info("Stop screen")
-                return "quit"
-
-            if abstract_from_tei:
-                if "abstract" in record.data:
-                    del record.data["abstract"]
-            if decision == "y":
-                screen_operation.screen(
-                    record=record,
-                    screen_inclusion=True,
-                    screening_criteria="NA",
-                )
-            if decision == "n":
-                screen_operation.screen(
-                    record=record,
-                    screen_inclusion=False,
-                    screening_criteria="NA",
-                    PAD=self.__pad,
-                )
+            ret = self.__screen_record_without_criteria(
+                screen_operation=screen_operation,
+                record=record,
+                abstract_from_tei=abstract_from_tei,
+            )
 
-        return "screened"
+        return ret
 
     def __screen_cli(
         self, screen_operation: colrev.ops.screen.Screen, split: list
     ) -> dict:
         screen_data = screen_operation.get_data()
         self.__pad = screen_data["PAD"]
         self.__stat_len = screen_data["nr_tasks"]
@@ -232,28 +261,28 @@
                 if record_dict["ID"] not in split:
                     continue
 
             ret = self.__screen_record(
                 screen_operation=screen_operation, record_dict=record_dict
             )
 
-            if "skip" == ret:
+            if ret == "skip":
                 continue
-            if "quit" == ret:
+            if ret == "quit":
                 screen_operation.review_manager.logger.info("Stop screen")
                 break
 
         if self.__stat_len == 0:
             screen_operation.review_manager.logger.info("No records to screen")
             return records
 
         screen_operation.review_manager.dataset.add_record_changes()
 
         if self.__i < self.__stat_len:  # if records remain for screening
-            if "y" != input("Create commit (y/n)?"):
+            if input("Create commit (y/n)?") != "y":
                 return records
 
         screen_operation.review_manager.create_commit(
             msg="Screening (manual)", manual_author=True
         )
         return records
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/screen/screen_table.py` & `colrev-0.8.3/colrev/ops/built_in/screen/screen_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,22 +131,22 @@
 
         tbl = self.__create_screening_table(
             screen_operation=screen_operation, records=records, split=split
         )
 
         self.screen_table_path.parents[0].mkdir(parents=True, exist_ok=True)
 
-        if "csv" == export_table_format.lower():
+        if export_table_format.lower() == "csv":
             screen_df = pd.DataFrame(tbl)
             screen_df.to_csv(self.screen_table_path, index=False, quoting=csv.QUOTE_ALL)
             screen_operation.review_manager.logger.info(
                 f"Created {self.screen_table_path}"
             )
 
-        if "xlsx" == export_table_format.lower():
+        if export_table_format.lower() == "xlsx":
             screen_df = pd.DataFrame(tbl)
             screen_df.to_excel(
                 self.screen_table_path.with_suffix(".xlsx"),
                 index=False,
                 sheet_name="screen",
             )
             screen_operation.review_manager.logger.info(
@@ -177,20 +177,25 @@
         screen_df.fillna("", inplace=True)
         screened_records = screen_df.to_dict("records")
 
         screening_criteria = screen_operation.review_manager.settings.screen.criteria
 
         for screened_record in screened_records:
             if screened_record.get("ID", "") in records:
-                record = records[screened_record.get("ID", "")]
+                record_dict = records[screened_record.get("ID", "")]
+                record = colrev.record.Record(data=record_dict)
                 if "screen_inclusion" in screened_record:
-                    if "in" == screened_record["screen_inclusion"]:
-                        record["colrev_status"] = colrev.record.RecordState.rev_included
-                    elif "out" == screened_record["screen_inclusion"]:
-                        record["colrev_status"] = colrev.record.RecordState.rev_excluded
+                    if screened_record["screen_inclusion"] == "in":
+                        record.set_status(
+                            target_state=colrev.record.RecordState.rev_included
+                        )
+                    elif screened_record["screen_inclusion"] == "out":
+                        record.set_status(
+                            target_state=colrev.record.RecordState.rev_excluded
+                        )
                     else:
                         print(
                             f"Invalid choice: {screened_record['screen_inclusion']} "
                             f"({screened_record['ID']})"
                         )
                     continue
                 screening_criteria_field = ""
@@ -199,36 +204,40 @@
                     screening_criteria_field += (
                         screening_criterion
                         + "="
                         + screened_record[screening_criterion]
                         + ";"
                     )
                 screening_criteria_field = screening_criteria_field.rstrip(";")
-                record["screening_criteria"] = screening_criteria_field
+                record.data["screening_criteria"] = screening_criteria_field
                 if "=out" in screening_criteria_field:
-                    record["colrev_status"] = colrev.record.RecordState.rev_excluded
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_excluded
+                    )
                 else:
-                    record["colrev_status"] = colrev.record.RecordState.rev_included
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_included
+                    )
 
         screen_operation.review_manager.dataset.save_records_dict(records=records)
         screen_operation.review_manager.dataset.add_record_changes()
 
     def run_screen(
         self, screen_operation: colrev.ops.screen.Screen, records: dict, split: list
     ) -> dict:
         """Screen records based on screening tables"""
 
-        if "y" == input("create screen table [y,n]?"):
+        if input("create screen table [y,n]?") == "y":
             self.export_table(screen_operation, records, split)
 
-        if "y" == input("import screen table [y,n]?"):
+        if input("import screen table [y,n]?") == "y":
             self.import_table(screen_operation, records)
 
         if screen_operation.review_manager.dataset.has_changes():
-            if "y" == input("create commit [y,n]?"):
+            if input("create commit [y,n]?") == "y":
                 screen_operation.review_manager.create_commit(
                     msg="Screen", manual_author=True
                 )
         return records
 
 
 if __name__ == "__main__":
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/screen/utils.py` & `colrev-0.8.3/colrev/ops/built_in/screen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         screening_criteria = {}
         while "y" == input(
             __get_add_screening_criterion_dialogue(
                 screening_criteria=screening_criteria
             )
         ):
             short_name = input("Provide a short name: ")
-            if "i" == input("Inclusion or exclusion criterion [i,e]?: "):
+            if input("Inclusion or exclusion criterion [i,e]?: ") == "i":
                 criterion_type = colrev.settings.ScreenCriterionType.inclusion_criterion
             else:
                 criterion_type = colrev.settings.ScreenCriterionType.exclusion_criterion
             explanation = input("Provide a short explanation: ")
 
             screening_criteria[short_name] = colrev.settings.ScreenCriterion(
                 explanation=explanation, criterion_type=criterion_type, comment=""
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/abi_inform_proquest.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/abi_inform_proquest.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/acm_digital_library.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/acm_digital_library.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/aisel.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/aisel.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,32 @@
     heuristic_status = colrev.env.package_manager.SearchSourceHeuristicStatus.supported
     short_name = "AIS eLibrary"
     link = (
         "https://github.com/CoLRev-Environment/colrev/blob/main/"
         + "colrev/ops/built_in/search_sources/aisel.md"
     )
 
+    __conference_abbreviations = {
+        "ICIS": "International Conference on Information Systems",
+        "PACIS": "Pacific-Asia Conference on Information Systems",
+        "ECIS": "European Conference on Information Systems",
+        "AMCIS": "Americas Conference on Information Systems",
+        "HICSS": "Hawaii International Conference on System Sciences",
+        "MCIS": "Mediterranean Conference on Information Systems",
+        "ACIS": "Australasian Conference on Information Systems",
+    }
+
+    __link_confs = {
+        "https://aisel.aisnet.org/hicss": "Hawaii International Conference on System Sciences",
+        "https://aisel.aisnet.org/amcis": "Americas Conference on Information Systems",
+        "https://aisel.aisnet.org/pacis": "Pacific-Asia Conference on Information Systems",
+        "https://aisel.aisnet.org/ecis": "European Conference on Information Systems",
+        "https://aisel.aisnet.org/icis": "International Conference on Information Systems",
+    }
+
     def __init__(
         self, *, source_operation: colrev.operation.CheckOperation, settings: dict
     ) -> None:
         self.search_source = from_dict(data_class=self.settings_class, data=settings)
         self.review_manager = source_operation.review_manager
 
     @classmethod
@@ -103,17 +121,17 @@
 
             search_terms = []
             query_parts_merged = []
             parenthesis_expression = ""
             for query_part in query_parts:
                 if query_part not in ["(", ")"] and "" == parenthesis_expression:
                     query_parts_merged.append(query_part)
-                elif "(" == query_part:
+                elif query_part == "(":
                     parenthesis_expression += "("
-                elif ")" == query_part:
+                elif query_part == ")":
                     parenthesis_expression = parenthesis_expression.rstrip().replace(
                         "(", ""
                     )
                     query_parts_merged.append(parenthesis_expression)
                     parenthesis_expression = ""
                 else:
                     parenthesis_expression = parenthesis_expression + query_part + " "
@@ -218,15 +236,15 @@
 
         query_string = (
             "https://aisel.aisnet.org/do/search/results/refer?"
             + "start=0&context=509156&sort=score&facet=&dlt=Export122204"
         )
         query_string = f"{query_string}&q={final_q}"
 
-        response = requests.get(query_string)
+        response = requests.get(query_string, timeout=300)
         response.raise_for_status()
 
         zotero_translation_service = (
             self.review_manager.get_zotero_translation_service()
         )
         zotero_translation_service.start()
 
@@ -387,25 +405,15 @@
         source: colrev.settings.SearchSource,
         records: typing.Dict,
     ) -> dict:
         """Load fixes for AIS electronic Library (AISeL)"""
 
         return records
 
-    def prepare(
-        self, record: colrev.record.PrepRecord, source: colrev.settings.SearchSource
-    ) -> colrev.record.Record:
-        """Source-specific preparation for the AIS electronic Library (AISeL)"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-
-        ais_mapping: dict = {}
-        record.rename_fields_based_on_mapping(mapping=ais_mapping)
-
+    def __fix_entrytype(self, *, record: colrev.record.Record) -> None:
         # Note : simple heuristic
         # but at the moment, AISeLibrary only indexes articles and conference papers
         if (
             record.data.get("volume", "UNKNOWN") != "UNKNOWN"
             or record.data.get("number", "UNKNOWN") != "UNKNOWN"
         ) and not any(
             x in record.data.get("journal", "")
@@ -414,26 +422,28 @@
                 "ICIS",
                 "ECIS",
                 "AMCIS",
                 "Proceedings",
                 "All Sprouts Content",
             ]
         ):
+            # Journal articles
             if (
                 "journal" not in record.data
                 and "title" in record.data
                 and "chapter" in record.data
             ):
                 record.rename_field(key="title", new_key="journal")
                 record.rename_field(key="chapter", new_key="title")
                 record.remove_field(key="publisher")
 
             record.change_entrytype(new_entrytype="article")
-
         else:
+            # Inproceedings
+
             record.remove_field(key="publisher")
 
             if (
                 "booktitle" not in record.data
                 and "title" in record.data
                 and "chapter" in record.data
             ):
@@ -447,115 +457,71 @@
                 "Research Papers",
             ]:
                 if "https://aisel.aisnet.org/ecis" in record.data.get("url", ""):
                     record.update_field(
                         key="booktitle", value="ECIS", source="prep_ais_source"
                     )
 
+    def __unify_container_titles(self, *, record: colrev.record.Record) -> None:
         if record.data.get("journal", "") == "Management Information Systems Quarterly":
             record.update_field(
                 key="journal", value="MIS Quarterly", source="prep_ais_source"
             )
 
-        if "inproceedings" == record.data["ENTRYTYPE"]:
-            if "ICIS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="International Conference on Information Systems",
-                    source="prep_ais_source",
-                )
-            if "PACIS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="Pacific-Asia Conference on Information Systems",
-                    source="prep_ais_source",
-                )
-            if "ECIS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="European Conference on Information Systems",
-                    source="prep_ais_source",
-                )
-            if "AMCIS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="Americas Conference on Information Systems",
-                    source="prep_ais_source",
-                )
-            if "HICSS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="Hawaii International Conference on System Sciences",
-                    source="prep_ais_source",
-                )
-            if "MCIS" in record.data.get("booktitle", ""):
-                record.update_field(
-                    key="booktitle",
-                    value="Mediterranean Conference on Information Systems",
-                    source="prep_ais_source",
-                )
-            if "ACIS" in record.data.get("booktitle", ""):
+        if record.data["ENTRYTYPE"] == "inproceedings":
+            for conf_abbreviation, conf_name in self.__conference_abbreviations.items():
+                if conf_abbreviation in record.data.get("booktitle", ""):
+                    record.update_field(
+                        key="booktitle",
+                        value=conf_name,
+                        source="prep_ais_source",
+                    )
+
+        for link_part, conf_name in self.__link_confs.items():
+            if link_part in record.data.get("url", ""):
                 record.update_field(
                     key="booktitle",
-                    value="Australasian Conference on Information Systems",
+                    value=conf_name,
                     source="prep_ais_source",
                 )
-        if "https://aisel.aisnet.org/hicss" in record.data.get("url", ""):
-            record.update_field(
-                key="booktitle",
-                value="Hawaii International Conference on System Sciences",
-                source="prep_ais_source",
-            )
-        elif "https://aisel.aisnet.org/amcis" in record.data.get("url", ""):
-            record.update_field(
-                key="booktitle",
-                value="Americas Conference on Information Systems",
-                source="prep_ais_source",
-            )
 
-        elif "https://aisel.aisnet.org/pacis" in record.data.get("url", ""):
-            record.update_field(
-                key="booktitle",
-                value="Pacific-Asia Conference on Information Systems",
-                source="prep_ais_source",
-            )
-        elif "https://aisel.aisnet.org/ecis" in record.data.get("url", ""):
-            record.update_field(
-                key="booktitle",
-                value="European Conference on Information Systems",
-                source="prep_ais_source",
-            )
-        elif "https://aisel.aisnet.org/icis" in record.data.get("url", ""):
-            record.update_field(
-                key="booktitle",
-                value="International Conference on Information Systems",
-                source="prep_ais_source",
-            )
-        elif "https://aisel.aisnet.org/bise/" in record.data.get("url", ""):
+        if "https://aisel.aisnet.org/bise/" in record.data.get("url", ""):
             record.update_field(
                 key="journal",
                 value="Business & Information Systems Engineering",
                 source="prep_ais_source",
             )
 
+    def __format_fields(self, *, record: colrev.record.Record) -> None:
         if "abstract" in record.data:
-            if "N/A" == record.data["abstract"]:
+            if record.data["abstract"] == "N/A":
                 record.remove_field(key="abstract")
         if "author" in record.data:
             record.update_field(
                 key="author",
                 value=record.data["author"].replace("\n", " "),
                 source="prep_ais_source",
                 keep_source_if_equal=True,
             )
 
+    def __exclude_complementary_material(self, *, record: colrev.record.Record) -> None:
         if re.match(
             r"MISQ Volume \d{1,2}, Issue \d Table of Contents",
             record.data.get("title", ""),
         ):
             record.prescreen_exclude(reason="complementary material")
 
+    def prepare(
+        self, record: colrev.record.PrepRecord, source: colrev.settings.SearchSource
+    ) -> colrev.record.Record:
+        """Source-specific preparation for the AIS electronic Library (AISeL)"""
+
+        self.__fix_entrytype(record=record)
+        self.__unify_container_titles(record=record)
+        self.__format_fields(record=record)
+        self.__exclude_complementary_material(record=record)
+
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/colrev_project.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/colrev_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         except colrev_exceptions.RepoSetupError as exc:
             search_operation.review_manager.logger.error(
                 f"Error retrieving records from colrev project {project_identifier} ({exc})"
             )
             return
 
         remote_url = project_review_manager.dataset.get_remote_url()
-        if "NA" != remote_url:
+        if remote_url != "NA":
             project_identifier = remote_url.rstrip(".git")
 
         project_review_manager.get_load_operation(
             notify_state_transition_operation=False,
         )
         search_operation.review_manager.logger.info(
             f'Loading records from {self.search_source.search_parameters["scope"]["url"]}'
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/crossref.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/crossref.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from importlib.metadata import version
 from multiprocessing import Lock
 from pathlib import Path
 from sqlite3 import OperationalError
 from typing import Optional
 
 import requests
+import timeout_decorator
 import zope.interface
 from crossref.restful import Etiquette
 from crossref.restful import Journals
 from dacite import from_dict
 from dataclasses_jsonschema import JsonSchemaMixin
 from thefuzz import fuzz
 
@@ -143,28 +144,30 @@
         except (requests.exceptions.RequestException, IndexError) as exc:
             print(exc)
             if not source_operation.force_mode:
                 raise colrev_exceptions.ServiceNotAvailableException(
                     "CROSSREF"
                 ) from exc
 
+    @timeout_decorator.timeout(800, use_signals=False)
     def __query(self, **kwargs) -> typing.Iterator[dict]:  # type: ignore
         """Get records from Crossref based on a bibliographic query"""
 
         # pylint: disable=import-outside-toplevel
         from crossref.restful import Works
 
         works = Works(etiquette=self.etiquette)
         # use facets:
         # https://api.crossref.org/swagger-ui/index.html#/Works/get_works
 
         crossref_query_return = works.query(**kwargs).sort("deposited").order("desc")
         for item in crossref_query_return:
             yield connector_utils.json_to_record(item=item)
 
+    @timeout_decorator.timeout(40, use_signals=False)
     def query_doi(self, *, doi: str) -> colrev.record.PrepRecord:
         """Get records from Crossref based on a doi query"""
 
         # pylint: disable=import-outside-toplevel
         from crossref.restful import Works
 
         works = Works(etiquette=self.etiquette)
@@ -180,14 +183,15 @@
         retrieved_record_dict = connector_utils.json_to_record(
             item=crossref_query_return
         )
         retrieved_record = colrev.record.PrepRecord(data=retrieved_record_dict)
 
         return retrieved_record
 
+    @timeout_decorator.timeout(500, use_signals=False)
     def __query_journal(
         self, *, journal_issn: str, rerun: bool
     ) -> typing.Iterator[dict]:
         """Get records of a selected journal from Crossref"""
 
         # pylint: disable=import-outside-toplevel
 
@@ -283,15 +287,20 @@
     def __prep_crossref_record(
         self,
         *,
         record: colrev.record.Record,
         prep_main_record: bool = True,
         crossref_source: str = "",
     ) -> colrev.record.Record:
-        self.language_service.unify_to_iso_639_3_language_codes(record=record)
+        if "language" in record.data:
+            try:
+                self.language_service.unify_to_iso_639_3_language_codes(record=record)
+            except colrev_exceptions.InvalidLanguageCodeException:
+                del record.data["language"]
+
         doi_connector.DOIConnector.get_link_from_doi(
             review_manager=self.review_manager,
             record=record,
         )
 
         if not prep_main_record:
             # Skip steps for feed records
@@ -311,15 +320,15 @@
 
     def crossref_query(
         self,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         record_input: colrev.record.Record,
         jour_vol_iss_list: bool = False,
-        timeout: int = 10,
+        timeout: int = 40,
     ) -> list:
         """Retrieve records from Crossref based on a query"""
 
         # pylint: disable=too-many-branches
         # pylint: disable=too-many-statements
         # pylint: disable=too-many-locals
 
@@ -385,40 +394,40 @@
 
         if not jour_vol_iss_list:
             if most_similar_record:
                 record_list = [colrev.record.PrepRecord(data=most_similar_record)]
 
         return record_list
 
-    def __check_journal(
-        self,
-        prep_operation: colrev.ops.prep.Prep,
-        record: colrev.record.Record,
-        timeout: int,
-        save_feed: bool,
-    ) -> colrev.record.Record:
-        """When there is no doi, journal names can be checked against crossref"""
-
-        if "article" == record.data["ENTRYTYPE"]:
-            # If type article and doi not in record and
-            # journal name not found in journal-query: notify
-            journals = Journals(etiquette=self.etiquette)
-            # record.data["journal"] = "Information Systems Research"
-            found = False
-            ret = journals.query(record.data["journal"])
-            for rets in ret:
-                if rets["title"]:
-                    found = True
-                    break
-            if not found:
-                record.add_masterdata_provenance_note(
-                    key="journal", note="quality_defect:journal not in crossref"
-                )
+    # def __check_journal(
+    #     self,
+    #     prep_operation: colrev.ops.prep.Prep,
+    #     record: colrev.record.Record,
+    #     timeout: int,
+    #     save_feed: bool,
+    # ) -> colrev.record.Record:
+    #     """When there is no doi, journal names can be checked against crossref"""
+
+    #     if record.data["ENTRYTYPE"] == "article":
+    #         # If type article and doi not in record and
+    #         # journal name not found in journal-query: notify
+    #         journals = Journals(etiquette=self.etiquette)
+    #         # record.data["journal"] = "Information Systems Research"
+    #         found = False
+    #         ret = journals.query(record.data["journal"])
+    #         for rets in ret:
+    #             if rets["title"]:
+    #                 found = True
+    #                 break
+    #         if not found:
+    #             record.add_masterdata_provenance_note(
+    #                 key="journal", note="quality_defect:journal not in crossref"
+    #             )
 
-        return record
+    #     return record
 
     def __get_masterdata_record(
         self,
         prep_operation: colrev.ops.prep.Prep,
         record: colrev.record.Record,
         timeout: int,
         save_feed: bool,
@@ -543,15 +552,15 @@
         return record
 
     def get_masterdata(
         self,
         prep_operation: colrev.ops.prep.Prep,
         record: colrev.record.Record,
         save_feed: bool = True,
-        timeout: int = 10,
+        timeout: int = 30,
     ) -> colrev.record.Record:
         """Retrieve masterdata from Crossref based on similarity with the record provided"""
 
         # To test the metadata provided for a particular DOI use:
         # https://api.crossref.org/works/DOI
 
         # https://github.com/OpenAPC/openapc-de/blob/master/python/import_dois.py
@@ -564,21 +573,22 @@
         record = self.__get_masterdata_record(
             prep_operation=prep_operation,
             record=record,
             timeout=timeout,
             save_feed=save_feed,
         )
 
-        if "doi" not in record.data:
-            record = self.__check_journal(
-                prep_operation=prep_operation,
-                record=record,
-                timeout=timeout,
-                save_feed=save_feed,
-            )
+        # Note: this should be optional
+        # if "doi" not in record.data:
+        #     record = self.__check_journal(
+        #         prep_operation=prep_operation,
+        #         record=record,
+        #         timeout=timeout,
+        #         save_feed=save_feed,
+        #     )
 
         return record
 
     def validate_source(
         self,
         search_operation: colrev.ops.search.Search,
         source: colrev.settings.SearchSource,
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/dblp.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/dblp.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,33 +194,33 @@
     ) -> dict:
         # pylint: disable=too-many-branches
 
         # To test in browser:
         # https://dblp.org/search/publ/api?q=ADD_TITLE&format=json
 
         retrieved_record = {}
-        if "Withdrawn Items" == item["type"]:
-            if "journals" == item["key"][:8]:
+        if item["type"] == "Withdrawn Items":
+            if item["key"][:8] == "journals":
                 item["type"] = "Journal Articles"
-            if "conf" == item["key"][:4]:
+            if item["key"][:4] == "conf":
                 item["type"] = "Conference and Workshop Papers"
             retrieved_record["warning"] = "Withdrawn (according to DBLP)"
-        if "Journal Articles" == item["type"]:
+        if item["type"] == "Journal Articles":
             retrieved_record["ENTRYTYPE"] = "article"
             lpos = item["key"].find("/") + 1
             rpos = item["key"].rfind("/")
             ven_key = item["key"][lpos:rpos]
             retrieved_record["journal"] = self.__get_dblp_venue(
                 session=session,
                 review_manager=review_manager,
                 timeout=timeout,
                 venue_string=ven_key,
                 venue_type="Journal",
             )
-        if "Conference and Workshop Papers" == item["type"]:
+        if item["type"] == "Conference and Workshop Papers":
             retrieved_record["ENTRYTYPE"] = "inproceedings"
             lpos = item["key"].find("/") + 1
             rpos = item["key"].rfind("/")
             ven_key = item["key"][lpos:rpos]
             retrieved_record["booktitle"] = self.__get_dblp_venue(
                 session=session,
                 review_manager=review_manager,
@@ -662,15 +662,15 @@
         return records
 
     def prepare(
         self, record: colrev.record.Record, source: colrev.settings.SearchSource
     ) -> colrev.record.Record:
         """Source-specific preparation for DBLP"""
 
-        if "UNKNOWN" != record.data.get("author", "UNKNOWN"):
+        if record.data.get("author", "UNKNOWN") != "UNKNOWN":
             # DBLP appends identifiers to non-unique authors
             record.update_field(
                 key="author",
                 value=str(re.sub(r"[0-9]{4}", "", record.data["author"])),
                 source="dblp",
                 keep_source_if_equal=True,
             )
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/doi_org.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/doi_org.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     @classmethod
     def retrieve_doi_metadata(
         cls,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         record: colrev.record.PrepRecord,
-        timeout: int = 10,
+        timeout: int = 60,
     ) -> colrev.record.Record:
         """Retrieve the metadata from DOI.org based on a record (similarity)"""
 
         if "doi" not in record.data:
             return record
 
         try:
@@ -96,15 +96,15 @@
 
     @classmethod
     def get_link_from_doi(
         cls,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         record: colrev.record.Record,
-        timeout: int = 10,
+        timeout: int = 30,
     ) -> None:
         """Get the website link from DOI resolution API"""
 
         if "doi" not in record.data:
             return
 
         doi_url = f"https://www.doi.org/{record.data['doi']}"
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/ebsco_host.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/ebsco_host.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/eric.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/eric.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/europe_pmc.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/europe_pmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 #! /usr/bin/env python
 """SearchSource: Europe PMC"""
 from __future__ import annotations
 
 import json
 import typing
-import xml.etree.ElementTree as ET
 from dataclasses import dataclass
 from multiprocessing import Lock
 from pathlib import Path
 from sqlite3 import OperationalError
 from typing import Optional
 from urllib.parse import quote
 from xml.etree.ElementTree import Element
 
+import defusedxml
 import requests
 import zope.interface
 from dacite import from_dict
 from dataclasses_jsonschema import JsonSchemaMixin
+from defusedxml.ElementTree import fromstring
 from thefuzz import fuzz
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.search
 import colrev.record
 import colrev.settings
 
-# pylint: disable=duplicate-code
-
-if False:  # pylint: disable=using-constant-test
-    from typing import TYPE_CHECKING  # pylint: disable=ungrouped-imports
-
-    if TYPE_CHECKING:
-        import colrev.ops.prep
+# defuse std xml lib
+defusedxml.defuse_stdlib()
 
 
+# pylint: disable=duplicate-code
 # pylint: disable=unused-argument
 # pylint: disable=duplicate-code
 
 
 @zope.interface.implementer(
     colrev.env.package_manager.SearchSourcePackageEndpointInterface
 )
@@ -227,15 +224,15 @@
     @classmethod
     def europe_pcmc_query(
         cls,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         record_input: colrev.record.Record,
         most_similar_only: bool = True,
-        timeout: int = 10,
+        timeout: int = 60,
     ) -> list:
         """Retrieve records from Europe PMC based on a query"""
 
         # pylint: disable=too-many-branches
         # pylint: disable=too-many-statements
         # pylint: disable=too-many-locals
 
@@ -259,15 +256,15 @@
                 if ret.status_code != 200:
                     # review_manager.logger.debug(
                     #     f"europe_pmc failed with status {ret.status_code}"
                     # )
                     return []
 
                 most_similar, most_similar_record = 0.0, {}
-                root = ET.fromstring(ret.text)
+                root = fromstring(str.encode(ret.text))
                 result_list = root.findall("resultList")[0]
 
                 for result_item in result_list.findall("result"):
                     retrieved_record = cls.__europe_pmc_xml_to_record(item=result_item)
 
                     if "title" not in retrieved_record.data:
                         continue
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/google_scholar.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/google_scholar.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/ieee.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/ieee.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/jstor.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/jstor.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/local_index.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/local_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -351,195 +351,214 @@
         records: typing.Dict,
     ) -> dict:
         """Load fixes for local-index"""
 
         # Note : to avoid modifying the feed-records
         records = deepcopy(records)
 
-        for record in records.values():
-            curation_url = record["curation_ID"].split("#")[0]
-            record["colrev_masterdata_provenance"] = {
+        for record_dict in records.values():
+            curation_url = record_dict["curation_ID"].split("#")[0]
+            record_dict["colrev_masterdata_provenance"] = {
                 "CURATED": {"source": curation_url, "note": ""}
             }
-            record["colrev_status"] = colrev.record.RecordState.md_prepared
+            record = colrev.record.Record(data=record_dict)
+            record.set_status(target_state=colrev.record.RecordState.md_prepared)
             del curation_url
 
         return records
 
     def prepare(
         self, record: colrev.record.Record, source: colrev.settings.SearchSource
     ) -> colrev.record.Record:
         """Source-specific preparation for local-index"""
 
         return record
 
-    def get_masterdata(
-        self,
-        prep_operation: colrev.ops.prep.Prep,
-        record: colrev.record.Record,
-        save_feed: bool = True,
-        timeout: int = 10,
-    ) -> colrev.record.Record:
-        """Retrieve masterdata from LocalIndex based on similarity with the record provided"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
-        # pylint: disable=too-many-return-statements
-
-        if any(self.origin_prefix in o for o in record.data["colrev_origin"]):
-            # Already linked to a local-index record
-            return record
-
-        retrieved_record_dict = {}
-        added_colrev_pdf_id = False
+    def __add_cpid(self, *, record: colrev.record.Record) -> bool:
         # To enable retrieval based on colrev_pdf_id (as part of the global_ids)
         if "file" in record.data and "colrev_pdf_id" not in record.data:
-            pdf_path = Path(
-                prep_operation.review_manager.path / Path(record.data["file"])
-            )
+            pdf_path = Path(self.review_manager.path / Path(record.data["file"]))
             if pdf_path.is_file():
                 try:
                     record.data.update(
                         colrev_pdf_id=colrev.record.Record.get_colrev_pdf_id(
-                            review_manager=prep_operation.review_manager,
                             pdf_path=pdf_path,
                         )
                     )
-                    added_colrev_pdf_id = True
+                    return True
                 except colrev_exceptions.PDFHashError:
                     pass
+        return False
 
+    def __set_not_in_toc_info(
+        self, *, record: colrev.record.Record, toc_key: str
+    ) -> None:
+        record.set_status(
+            target_state=colrev.record.RecordState.md_needs_manual_preparation
+        )
+        if "journal" in record.data:
+            record.add_masterdata_provenance_note(
+                key="journal", note=f"record_not_in_toc {toc_key}"
+            )
+        elif "booktitle" in record.data:
+            record.add_masterdata_provenance_note(
+                key="booktitle", note=f"record_not_in_toc {toc_key}"
+            )
+
+    def __retrieve_record_from_local_index(
+        self,
+        *,
+        record: colrev.record.Record,
+        added_colrev_pdf_id: bool,
+        retrieval_similarity: float,
+    ) -> colrev.record.Record:
+        retrieved_record_dict = {}
         try:
             retrieved_record_dict = self.local_index.retrieve(
                 record_dict=record.get_data(), include_file=False
             )
         except (
             colrev_exceptions.RecordNotInIndexException,
             colrev_exceptions.NotEnoughDataToIdentifyException,
         ):
             try:
                 # Search within the table-of-content in local_index
                 retrieved_record_dict = self.local_index.retrieve_from_toc(
                     record_dict=record.data,
-                    similarity_threshold=prep_operation.retrieval_similarity,
+                    similarity_threshold=retrieval_similarity,
                     include_file=False,
                 )
             except colrev_exceptions.RecordNotInTOCException as exc:
-                record.set_status(
-                    target_state=colrev.record.RecordState.md_needs_manual_preparation
-                )
-                if "journal" in record.data:
-                    record.add_masterdata_provenance_note(
-                        key="journal", note=f"record_not_in_toc {exc.toc_key}"
-                    )
-                elif "booktitle" in record.data:
-                    record.add_masterdata_provenance_note(
-                        key="booktitle", note=f"record_not_in_toc {exc.toc_key}"
-                    )
+                self.__set_not_in_toc_info(record=record, toc_key=exc.toc_key)
                 return record
 
             except colrev_exceptions.RecordNotInIndexException:
                 try:
                     # Search across table-of-contents in local_index
                     retrieved_record_dict = self.local_index.retrieve_from_toc(
                         record_dict=record.data,
-                        similarity_threshold=prep_operation.retrieval_similarity,
+                        similarity_threshold=retrieval_similarity,
                         include_file=False,
                         search_across_tocs=True,
                     )
                 except colrev_exceptions.RecordNotInTOCException as exc:
-                    record.set_status(
-                        target_state=colrev.record.RecordState.md_needs_manual_preparation
-                    )
-                    if "journal" in record.data:
-                        record.add_masterdata_provenance_note(
-                            key="journal", note=f"record_not_in_toc {exc.toc_key}"
-                        )
-                    elif "booktitle" in record.data:
-                        record.add_masterdata_provenance_note(
-                            key="booktitle", note=f"record_not_in_toc {exc.toc_key}"
-                        )
+                    self.__set_not_in_toc_info(record=record, toc_key=exc.toc_key)
                     return record
                 except (colrev_exceptions.RecordNotInIndexException,):
                     return record
             except colrev_exceptions.NotTOCIdentifiableException:
                 return record
         finally:
             if added_colrev_pdf_id:
                 del record.data["colrev_pdf_id"]
 
-        retrieved_record = colrev.record.PrepRecord(data=retrieved_record_dict)
-        if "colrev_status" in retrieved_record.data:
-            del retrieved_record.data["colrev_status"]
+        if "colrev_status" in retrieved_record_dict:
+            del retrieved_record_dict["colrev_status"]
 
-        # restriction: if we don't restrict to CURATED,
-        # we may have to rethink the LocalIndexSearchFeed.set_ids()
-        if "CURATED" not in retrieved_record.data.get(
-            "colrev_masterdata_provenance", ""
-        ):
-            return record
-
-        default_source = "LOCAL_INDEX"
-        if "colrev_masterdata_provenance" in retrieved_record.data:
-            if "CURATED" in retrieved_record.data["colrev_masterdata_provenance"]:
-                default_source = retrieved_record.data["colrev_masterdata_provenance"][
-                    "CURATED"
-                ]["source"]
+        return colrev.record.PrepRecord(data=retrieved_record_dict)
 
+    def __store_retrieved_record_in_feed(
+        self,
+        *,
+        record: colrev.record.Record,
+        default_source: str,
+        prep_operation: colrev.ops.prep.Prep,
+    ) -> None:
         try:
             # lock: to prevent different records from having the same origin
             self.local_index_lock.acquire(timeout=60)
 
             # Note : need to reload file because the object is not shared between processes
             local_index_feed = self.search_source.get_feed(
-                review_manager=prep_operation.review_manager,
+                review_manager=self.review_manager,
                 source_identifier=self.source_identifier,
                 update_only=False,
             )
 
-            local_index_feed.set_id(record_dict=retrieved_record.data)
-            local_index_feed.add_record(record=retrieved_record)
+            local_index_feed.set_id(record_dict=record.data)
+            local_index_feed.add_record(record=record)
 
-            retrieved_record.remove_field(key="curation_ID")
+            record.remove_field(key="curation_ID")
             record.merge(
-                merging_record=retrieved_record,
+                merging_record=record,
                 default_source=default_source,
             )
             record.set_status(target_state=colrev.record.RecordState.md_prepared)
-            if "retracted" == retrieved_record.data.get("prescreen_exclusion", "NA"):
+            if record.data.get("prescreen_exclusion", "NA") == "retracted":
                 record.prescreen_exclude(reason="retracted")
 
-            git_repo = prep_operation.review_manager.dataset.get_repo()
-            cur_project_source_paths = [str(prep_operation.review_manager.path)]
+            git_repo = self.review_manager.dataset.get_repo()
+            cur_project_source_paths = [str(self.review_manager.path)]
             for remote in git_repo.remotes:
                 if remote.url:
                     shared_url = remote.url
                     shared_url = shared_url.rstrip(".git")
                     cur_project_source_paths.append(shared_url)
                     break
 
             try:
                 local_index_feed.save_feed_file()
                 # extend fields_to_keep (to retrieve all fields from the index)
-                for key in retrieved_record.data.keys():
+                for key in record.data.keys():
                     if key not in prep_operation.fields_to_keep:
                         prep_operation.fields_to_keep.append(key)
 
             except OSError:
                 pass
 
             self.local_index_lock.release()
 
         except (
             colrev_exceptions.InvalidMerge,
             colrev_exceptions.NotFeedIdentifiableException,
         ):
             self.local_index_lock.release()
 
+    def get_masterdata(
+        self,
+        prep_operation: colrev.ops.prep.Prep,
+        record: colrev.record.Record,
+        save_feed: bool = True,
+        timeout: int = 10,
+    ) -> colrev.record.Record:
+        """Retrieve masterdata from LocalIndex based on similarity with the record provided"""
+
+        if any(self.origin_prefix in o for o in record.data["colrev_origin"]):
+            # Already linked to a local-index record
+            return record
+
+        # add colrev_pdf_id
+        added_colrev_pdf_id = self.__add_cpid(record=record)
+
+        retrieved_record = self.__retrieve_record_from_local_index(
+            record=record,
+            added_colrev_pdf_id=added_colrev_pdf_id,
+            retrieval_similarity=prep_operation.retrieval_similarity,
+        )
+
+        # restriction: if we don't restrict to CURATED,
+        # we may have to rethink the LocalIndexSearchFeed.set_ids()
+        if "CURATED" not in retrieved_record.data.get(
+            "colrev_masterdata_provenance", ""
+        ):
+            return record
+
+        default_source = "LOCAL_INDEX"
+        if "colrev_masterdata_provenance" in retrieved_record.data:
+            if "CURATED" in retrieved_record.data["colrev_masterdata_provenance"]:
+                default_source = retrieved_record.data["colrev_masterdata_provenance"][
+                    "CURATED"
+                ]["source"]
+
+        self.__store_retrieved_record_in_feed(
+            record=retrieved_record,
+            default_source=default_source,
+            prep_operation=prep_operation,
+        )
+
         return record
 
     def __get_local_base_repos(self, *, change_itemsets: list) -> dict:
         base_repos = []
         for item in change_itemsets:
             if "CURATED" in item["original_record"].get(
                 "colrev_masterdata_provenance", {}
@@ -601,17 +620,17 @@
                     continue
 
                 # self.review_manager.p_printer.pprint(item["original_record"])
                 colrev.record.Record(
                     data=item["original_record"]
                 ).print_citation_format()
                 for change_item in item["changes"]:
-                    if "change" == change_item[0]:
+                    if change_item[0] == "change":
                         edit_type, field, values = change_item
-                        if "colrev_id" == field:
+                        if field == "colrev_id":
                             continue
                         prefix = f"{edit_type} {field}"
                         print(
                             f"{prefix}"
                             + " " * max(len(prefix), 30 - len(prefix))
                             + f": {values[0]}"
                         )
@@ -620,15 +639,15 @@
                             + f"  {colors.ORANGE}{values[1]}{colors.END}"
                         )
                         print(
                             " " * max(len(prefix), 30)
                             + f"  {print_diff((values[0], values[1]))}"
                         )
 
-                    elif "add" == change_item[0]:
+                    elif change_item[0] == "add":
                         edit_type, field, values = change_item
                         prefix = f"{edit_type} {values[0][0]}"
                         print(
                             prefix
                             + " " * max(len(prefix), 30 - len(prefix))
                             + f": {colors.GREEN}{values[0][1]}{colors.END}"
                         )
@@ -638,21 +657,21 @@
 
             response = ""
             while True:
                 response = input("\nConfirm changes? (y/n)")
                 if response in ["y", "n"]:
                     break
 
-            if "y" == response:
+            if response == "y":
                 self.__apply_correction(
                     source_url=local_base_repos[repo_path],
                     change_list=validated_changes,
                 )
-            elif "n" == response:
-                if "y" == input("Discard all corrections (y/n)?"):
+            elif response == "n":
+                if input("Discard all corrections (y/n)?") == "y":
                     for validated_change in validated_changes:
                         Path(validated_change["file"]).unlink()
 
     def __apply_corrections_precondition(
         self, *, check_operation: colrev.operation.Operation, source_url: str
     ) -> bool:
         git_repo = check_operation.review_manager.dataset.get_repo()
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/open_citations_forward_search.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/open_citations_forward_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def __get_forward_search_records(self, *, record_dict: dict) -> list:
         forward_citations = []
 
         url = f"https://opencitations.net/index/coci/api/v1/citations/{record_dict['doi']}"
         # headers = {"authorization": "YOUR-OPENCITATIONS-ACCESS-TOKEN"}
         headers: typing.Dict[str, str] = {}
 
-        ret = requests.get(url, headers=headers)
+        ret = requests.get(url, headers=headers, timeout=300)
         try:
             items = json.loads(ret.text)
 
             for doi in [x["citing"] for x in items]:
                 retrieved_record = self.crossref_connector.query_doi(doi=doi)
                 # if not crossref_query_return:
                 #     raise colrev_exceptions.RecordNotFoundInPrepSourceException()
@@ -239,15 +239,15 @@
 
     @classmethod
     def add_endpoint(
         cls, search_operation: colrev.ops.search.Search, query: str
     ) -> typing.Optional[colrev.settings.SearchSource]:
         """Add SearchSource as an endpoint (based on query provided to colrev search -a )"""
 
-        if "forwardsearch" == query.replace("_", "").replace("-", ""):
+        if query.replace("_", "").replace("-", "") == "forwardsearch":
             return cls.get_default_source()
 
         return None
 
     def get_masterdata(
         self,
         prep_operation: colrev.ops.prep.Prep,
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/open_library.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/open_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #! /usr/bin/env python
 """Connector to OpenLibrary (API)"""
 from __future__ import annotations
 
 import json
+import typing
 from dataclasses import dataclass
 from multiprocessing import Lock
 from pathlib import Path
 from typing import Optional
 
 import requests
 import zope.interface
@@ -23,14 +24,15 @@
         import colrev.ops.prep
 
 # Note: not (yet) implemented as a full search_source
 # (including SearchSourcePackageEndpointInterface, packages_endpoints.json)
 
 
 # pylint: disable=too-few-public-methods
+# pylint: disable=unused-argument
 
 
 @zope.interface.implementer(
     colrev.env.package_manager.SearchSourcePackageEndpointInterface
 )
 @dataclass
 class OpenLibrarySearchSource(JsonSchemaMixin):
@@ -104,15 +106,15 @@
             requests_headers = {
                 "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) "
                 "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36"
             }
             ret = requests.get(
                 url,
                 headers=requests_headers,
-                timeout=20,
+                timeout=30,
             )
             if ret.status_code != 200:
                 if not source_operation.force_mode:
                     raise colrev_exceptions.ServiceNotAvailableException("OPENLIBRARY")
         except requests.exceptions.RequestException as exc:
             if not source_operation.force_mode:
                 raise colrev_exceptions.ServiceNotAvailableException(
@@ -180,15 +182,15 @@
             url = ""
             if record.data.get("author", "NA").split(",")[0]:
                 url = (
                     base_url
                     + "&author="
                     + record.data.get("author", "NA").split(",")[0]
                 )
-            if "inbook" == record.data["ENTRYTYPE"] and "editor" in record.data:
+            if record.data["ENTRYTYPE"] == "inbook" and "editor" in record.data:
                 if record.data.get("editor", "NA").split(",")[0]:
                     url = (
                         base_url
                         + "&author="
                         + record.data.get("editor", "NA").split(",")[0]
                     )
             if base_url not in url:
@@ -219,20 +221,46 @@
                 raise colrev_exceptions.RecordNotFoundInPrepSourceException()
             item = items[0]
 
         retrieved_record = self.__open_library_json_to_record(item=item, url=url)
 
         return retrieved_record
 
+    @classmethod
+    def heuristic(cls, filename: Path, data: str) -> dict:
+        """Source heuristic for OpenLibrary"""
+
+        result = {"confidence": 0.0}
+
+        return result
+
+    @classmethod
+    def add_endpoint(
+        cls, search_operation: colrev.ops.search.Search, query: str
+    ) -> typing.Optional[colrev.settings.SearchSource]:
+        """Add SearchSource as an endpoint (based on query provided to colrev search -a )"""
+
+    def validate_source(
+        self,
+        search_operation: colrev.ops.search.Search,
+        source: colrev.settings.SearchSource,
+    ) -> None:
+        """Validate the OpenLibrary (parameters etc.)"""
+
+    def run_search(
+        self, search_operation: colrev.ops.search.Search, rerun: bool
+    ) -> None:
+        """Run a search of OpenLibrary"""
+
     def get_masterdata(
         self,
-        *,
         prep_operation: colrev.ops.prep.Prep,
         record: colrev.record.Record,
-        timeout: int = 10,  # pylint: disable=unused-argument
+        save_feed: bool = True,
+        timeout: int = 10,
     ) -> colrev.record.Record:
         """Retrieve masterdata from OpenLibrary based on similarity with the record provided"""
 
         if any(self.origin_prefix in o for o in record.data["colrev_origin"]):
             # Already linked to an open-library record
             return record
 
@@ -268,10 +296,27 @@
             colrev_exceptions.InvalidMerge,
             colrev_exceptions.NotFeedIdentifiableException,
         ):
             self.open_library_lock.release()
 
         return record
 
+    def load_fixes(
+        self,
+        load_operation: colrev.ops.load.Load,
+        source: colrev.settings.SearchSource,
+        records: typing.Dict,
+    ) -> dict:
+        """Load fixes for OpenLibrary"""
+
+        return records
+
+    def prepare(
+        self, record: colrev.record.Record, source: colrev.settings.SearchSource
+    ) -> colrev.record.Record:
+        """Source-specific preparation for OpenLibrary"""
+
+        return record
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/pdf_backward_search.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/pdf_backward_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
     @classmethod
     def add_endpoint(
         cls, search_operation: colrev.ops.search.Search, query: str
     ) -> typing.Optional[colrev.settings.SearchSource]:
         """Add SearchSource as an endpoint (based on query provided to colrev search -a )"""
 
-        if "backwardsearch" == query.replace("_", "").replace("-", ""):
+        if query.replace("_", "").replace("-", "") == "backwardsearch":
             return cls.get_default_source()
 
         return None
 
     def load_fixes(
         self,
         load_operation: colrev.ops.load.Load,
@@ -297,15 +297,15 @@
         if (
             "multimedia appendix"
             in record.data.get("title", "").lower()
             + record.data.get("journal", "").lower()
         ):
             record.prescreen_exclude(reason="grobid-error")
 
-        if "misc" == record.data["ENTRYTYPE"] and "publisher" in record.data:
+        if record.data["ENTRYTYPE"] == "misc" and "publisher" in record.data:
             record.data["ENTRYTYPE"] = "book"
 
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/pdfs_dir.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/pdfs_dir.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pdfminer.pdfparser import PDFParser
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.built_in.search_sources.crossref
 import colrev.ops.built_in.search_sources.pdf_backward_search as bws
 import colrev.ops.search
+import colrev.qm.colrev_pdf_id
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
 
 # pylint: disable=unused-argument
 # pylint: disable=duplicate-code
 
 
@@ -44,14 +45,15 @@
     short_name = "PDF directory"
     link = (
         "https://github.com/CoLRev-Environment/colrev/blob/main/"
         + "colrev/ops/built_in/search_sources/pdfs_dir.md"
     )
 
     __doi_regex = re.compile(r"10\.\d{4,9}/[-._;/:A-Za-z0-9]*")
+    __batch_size = 20
 
     def __init__(
         self, *, source_operation: colrev.operation.CheckOperation, settings: dict
     ) -> None:
         self.search_source = from_dict(data_class=self.settings_class, data=settings)
         self.source_operation = source_operation
 
@@ -72,19 +74,19 @@
         if "subdir_pattern" in self.search_source.search_parameters.get("scope", {}):
             self.subdir_pattern = self.search_source.search_parameters["scope"][
                 "subdir_pattern"
             ]
             source_operation.review_manager.logger.info(
                 f"Activate subdir_pattern: {self.subdir_pattern}"
             )
-            if "year" == self.subdir_pattern:
+            if self.subdir_pattern == "year":
                 self.r_subdir_pattern = re.compile("([1-3][0-9]{3})")
-            if "volume_number" == self.subdir_pattern:
+            if self.subdir_pattern == "volume_number":
                 self.r_subdir_pattern = re.compile("([0-9]{1,3})(_|/)([0-9]{1,2})")
-            if "volume" == self.subdir_pattern:
+            if self.subdir_pattern == "volume":
                 self.r_subdir_pattern = re.compile("([0-9]{1,4})")
         self.crossref_connector = (
             colrev.ops.built_in.search_sources.crossref.CrossrefSearchSource(
                 source_operation=source_operation
             )
         )
 
@@ -112,15 +114,14 @@
                     record_dict["file"]
                 )
                 pdf_path = pdf_fp.parents[0]
                 potential_pdfs = pdf_path.glob("*.pdf")
 
                 for potential_pdf in potential_pdfs:
                     cpid_potential_pdf = colrev.record.Record.get_colrev_pdf_id(
-                        review_manager=search_operation.review_manager,
                         pdf_path=potential_pdf,
                     )
 
                     if cpid == cpid_potential_pdf:
                         record_dict["file"] = str(
                             potential_pdf.relative_to(
                                 search_operation.review_manager.path
@@ -213,38 +214,38 @@
             record_dict["ENTRYTYPE"] = "inproceedings"
 
         if self.subdir_pattern:
             # Note : no file access here (just parsing the patterns)
             # no absolute paths needed
             partial_path = Path(record_dict["file"]).parents[0]
 
-            if "year" == self.subdir_pattern:
+            if self.subdir_pattern == "year":
                 # Note: for year-patterns, we allow subfolders
                 # (eg., conference tracks)
                 match = self.r_subdir_pattern.search(str(partial_path))
                 if match is not None:
                     year = match.group(1)
                     record_dict["year"] = year
 
-            elif "volume_number" == self.subdir_pattern:
+            elif self.subdir_pattern == "volume_number":
                 match = self.r_subdir_pattern.search(str(partial_path))
                 if match is not None:
                     volume = match.group(1)
                     number = match.group(3)
                     record_dict["volume"] = volume
                     record_dict["number"] = number
                 else:
                     # sometimes, journals switch...
                     r_subdir_pattern = re.compile("([0-9]{1,3})")
                     match = r_subdir_pattern.search(str(partial_path))
                     if match is not None:
                         volume = match.group(1)
                         record_dict["volume"] = volume
 
-            elif "volume" == self.subdir_pattern:
+            elif self.subdir_pattern == "volume":
                 match = self.r_subdir_pattern.search(str(partial_path))
                 if match is not None:
                     volume = match.group(1)
                     record_dict["volume"] = volume
 
         return record_dict
 
@@ -446,205 +447,244 @@
         record: colrev.record.Record,
         save_feed: bool = True,
         timeout: int = 10,
     ) -> colrev.record.Record:
         """Not implemented"""
         return record
 
-    def run_search(
-        self, search_operation: colrev.ops.search.Search, rerun: bool
-    ) -> None:
-        """Run a search of a PDF directory (based on GROBID)"""
+    def __index_pdf(
+        self,
+        *,
+        pdf_path: Path,
+        search_operation: colrev.ops.search.Search,
+        pdfs_dir_feed: colrev.ops.search.GeneralOriginFeed,
+        linked_pdf_paths: list,
+        local_index: colrev.env.local_index.LocalIndex,
+    ) -> dict:
+        new_record: dict = {}
 
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+        if self.__is_broken_filepath(pdf_path=pdf_path):
+            return new_record
 
-        # Do not run in continuous-integration environment
-        if search_operation.review_manager.in_ci_environment():
-            return
+        if search_operation.review_manager.force_mode:
+            # i.e., reindex all
+            pass
+        else:
+            # note: for curations, we want all pdfs indexed/merged separately,
+            # in other projects, it is generally sufficient if the pdf is linked
+            if not self.review_manager.settings.is_curated_masterdata_repo():
+                if pdf_path in linked_pdf_paths:
+                    # Otherwise: skip linked PDFs
+                    return new_record
+
+            if pdf_path in [
+                Path(r["file"])
+                for r in pdfs_dir_feed.feed_records.values()
+                if "file" in r
+            ]:
+                return new_record
 
-        # Removing records/origins for which PDFs were removed makes sense for curated repositories
-        # In regular repositories, it may be confusing (e.g., if PDFs are renamed)
-        # In these cases, we may simply print a warning instead of modifying/removing records?
-        if self.review_manager.settings.is_curated_masterdata_repo():
-            self.__remove_records_if_pdf_no_longer_exists(
-                search_operation=search_operation
+        self.review_manager.logger.info(f" extract metadata from {pdf_path}")
+        try:
+            if not self.review_manager.settings.is_curated_masterdata_repo():
+                # retrieve_based_on_colrev_pdf_id
+                colrev_pdf_id = colrev.qm.colrev_pdf_id.get_pdf_hash(
+                    pdf_path=Path(pdf_path),
+                    page_nr=1,
+                    hash_size=32,
+                )
+                new_record = local_index.retrieve_based_on_colrev_pdf_id(
+                    colrev_pdf_id="cpid1:" + colrev_pdf_id
+                )
+                new_record["file"] = str(pdf_path)
+                # Note : an alternative to replacing all data with the curated version
+                # is to just add the curation_ID
+                # (and retrieve the curated metadata separately/non-redundantly)
+            else:
+                new_record = self.__get_grobid_metadata(
+                    search_operation=search_operation, pdf_path=pdf_path
+                )
+        except (
+            colrev_exceptions.PDFHashError,
+            colrev_exceptions.RecordNotInIndexException,
+        ):
+            # otherwise, get metadata from grobid (indexing)
+            new_record = self.__get_grobid_metadata(
+                search_operation=search_operation, pdf_path=pdf_path
             )
 
-        pdfs_dir_feed = self.search_source.get_feed(
-            review_manager=search_operation.review_manager,
-            source_identifier=self.source_identifier,
-            update_only=(not rerun),
-        )
+        new_record = self.__add_md_string(record_dict=new_record)
 
-        records = search_operation.review_manager.dataset.load_records_dict()
-        grobid_service = search_operation.review_manager.get_grobid_service()
-        grobid_service.start()
+        # Note: identical md_string as a heuristic for duplicates
+        potential_duplicates = [
+            r
+            for r in pdfs_dir_feed.feed_records.values()
+            if r["md_string"] == new_record["md_string"]
+            and not r["file"] == new_record["file"]
+        ]
+        if potential_duplicates:
+            self.review_manager.logger.warning(
+                f" {colors.RED}skip record (PDF potential duplicate): "
+                f"{new_record['file']} {colors.END} "
+                f"({','.join([r['file'] for r in potential_duplicates])})"
+            )
+            return new_record
 
-        local_index = search_operation.review_manager.get_local_index()
+        try:
+            pdfs_dir_feed.set_id(record_dict=new_record)
+        except colrev_exceptions.NotFeedIdentifiableException:
+            return new_record
+        return new_record
+
+    def __print_run_search_stats(
+        self, *, records: dict, nr_added: int, nr_changed: int
+    ) -> None:
+        if nr_added > 0:
+            self.review_manager.logger.info(
+                f"{colors.GREEN}Retrieved {nr_added} records{colors.END}"
+            )
+        else:
+            self.review_manager.logger.info(
+                f"{colors.GREEN}No additional records retrieved{colors.END}"
+            )
+
+        if self.review_manager.force_mode:
+            if nr_changed > 0:
+                self.review_manager.logger.info(
+                    f"{colors.GREEN}Updated {nr_changed} records{colors.END}"
+                )
+            else:
+                if records:
+                    self.review_manager.logger.info(
+                        f"{colors.GREEN}Records (data/records.bib) up-to-date{colors.END}"
+                    )
 
+    def __get_pdf_batches(self) -> list:
         pdfs_to_index = [
-            x.relative_to(search_operation.review_manager.path)
+            x.relative_to(self.review_manager.path)
             for x in self.pdfs_path.glob("**/*.pdf")
         ]
 
-        linked_pdf_paths = [Path(r["file"]) for r in records.values() if "file" in r]
-
-        if search_operation.review_manager.force_mode:  # i.e., reindex all
-            search_operation.review_manager.logger.info("Reindex all")
-
-        batch_size = 20
         pdf_batches = [
-            pdfs_to_index[i * batch_size : (i + 1) * batch_size]
-            for i in range((len(pdfs_to_index) + batch_size - 1) // batch_size)
+            pdfs_to_index[i * self.__batch_size : (i + 1) * self.__batch_size]
+            for i in range(
+                (len(pdfs_to_index) + self.__batch_size - 1) // self.__batch_size
+            )
         ]
+        return pdf_batches
+
+    def __run_pdfs_dir_search(
+        self,
+        *,
+        search_operation: colrev.ops.search.Search,
+        records: dict,
+        pdfs_dir_feed: colrev.ops.search.GeneralOriginFeed,
+        local_index: colrev.env.local_index.LocalIndex,
+        linked_pdf_paths: list,
+        rerun: bool,
+    ) -> None:
         nr_added, nr_changed = 0, 0
-        for pdf_batch in pdf_batches:
+        for pdf_batch in self.__get_pdf_batches():
             for record in pdfs_dir_feed.feed_records.values():
                 record = self.__add_md_string(record_dict=record)
 
             for pdf_path in pdf_batch:
-                if self.__is_broken_filepath(pdf_path=pdf_path):
-                    continue
-
-                if search_operation.review_manager.force_mode:
-                    # i.e., reindex all
-                    pass
-                else:
-                    # note: for curations, we want all pdfs indexed/merged separately,
-                    # in other projects, it is generally sufficient if the pdf is linked
-                    if not self.review_manager.settings.is_curated_masterdata_repo():
-                        if pdf_path in linked_pdf_paths:
-                            # Otherwise: skip linked PDFs
-                            continue
-
-                    if pdf_path in [
-                        Path(r["file"])
-                        for r in pdfs_dir_feed.feed_records.values()
-                        if "file" in r
-                    ]:
-                        continue
-
-                search_operation.review_manager.logger.info(
-                    f" extract metadata from {pdf_path}"
+                new_record = self.__index_pdf(
+                    pdf_path=pdf_path,
+                    search_operation=search_operation,
+                    pdfs_dir_feed=pdfs_dir_feed,
+                    linked_pdf_paths=linked_pdf_paths,
+                    local_index=local_index,
                 )
-                try:
-                    if (
-                        not search_operation.review_manager.settings.is_curated_masterdata_repo()
-                    ):
-                        # retrieve_based_on_colrev_pdf_id
-                        pdf_hash_service = (
-                            search_operation.review_manager.get_pdf_hash_service()
-                        )
-                        colrev_pdf_id = pdf_hash_service.get_pdf_hash(
-                            pdf_path=Path(pdf_path),
-                            page_nr=1,
-                            hash_size=32,
-                        )
-                        new_record = local_index.retrieve_based_on_colrev_pdf_id(
-                            colrev_pdf_id="cpid1:" + colrev_pdf_id
-                        )
-                        new_record["file"] = str(pdf_path)
-                        # Note : an alternative to replacing all data with the curated version
-                        # is to just add the curation_ID
-                        # (and retrieve the curated metadata separately/non-redundantly)
-                    else:
-                        new_record = self.__get_grobid_metadata(
-                            search_operation=search_operation, pdf_path=pdf_path
-                        )
-                except (
-                    colrev_exceptions.PDFHashError,
-                    colrev_exceptions.RecordNotInIndexException,
-                ):
-                    # otherwise, get metadata from grobid (indexing)
-                    new_record = self.__get_grobid_metadata(
-                        search_operation=search_operation, pdf_path=pdf_path
-                    )
-
-                new_record = self.__add_md_string(record_dict=new_record)
-
-                # Note: identical md_string as a heuristic for duplicates
-                potential_duplicates = [
-                    r
-                    for r in pdfs_dir_feed.feed_records.values()
-                    if r["md_string"] == new_record["md_string"]
-                    and not r["file"] == new_record["file"]
-                ]
-                if potential_duplicates:
-                    search_operation.review_manager.logger.warning(
-                        f" {colors.RED}skip record (PDF potential duplicate): "
-                        f"{new_record['file']} {colors.END} "
-                        f"({','.join([r['file'] for r in potential_duplicates])})"
-                    )
-                    continue
-
-                try:
-                    pdfs_dir_feed.set_id(record_dict=new_record)
-                except colrev_exceptions.NotFeedIdentifiableException:
+                if new_record == {}:
                     continue
 
-                prev_record_dict_version = {}
-                if new_record["ID"] in pdfs_dir_feed.feed_records:
-                    prev_record_dict_version = pdfs_dir_feed.feed_records[
-                        new_record["ID"]
-                    ]
+                prev_record_dict_version = pdfs_dir_feed.feed_records.get(
+                    new_record["ID"], {}
+                )
 
                 added = pdfs_dir_feed.add_record(
                     record=colrev.record.Record(data=new_record),
                 )
                 if added:
                     nr_added += 1
+                    self.__add_doi_from_pdf_if_not_available(record_dict=new_record)
 
-                    if "doi" not in new_record:
-                        record = colrev.record.Record(data=new_record)
-                        record.set_text_from_pdf(
-                            project_path=search_operation.review_manager.path
-                        )
-                        res = re.findall(self.__doi_regex, record.data["text_from_pdf"])
-                        if res:
-                            record.data["doi"] = res[0].upper()
-                        del record.data["text_from_pdf"]
-
-                elif search_operation.review_manager.force_mode:
+                elif self.review_manager.force_mode:
                     # Note : only re-index/update
-                    changed = search_operation.update_existing_record(
+                    if search_operation.update_existing_record(
                         records=records,
                         record_dict=new_record,
                         prev_record_dict_version=prev_record_dict_version,
                         source=self.search_source,
                         update_time_variant_fields=rerun,
-                    )
-                    if changed:
+                    ):
                         nr_changed += 1
 
             for record in pdfs_dir_feed.feed_records.values():
                 record.pop("md_string")
 
             pdfs_dir_feed.save_feed_file()
 
-        if nr_added > 0:
-            search_operation.review_manager.logger.info(
-                f"{colors.GREEN}Retrieved {nr_added} records{colors.END}"
-            )
-        else:
-            search_operation.review_manager.logger.info(
-                f"{colors.GREEN}No additional records retrieved{colors.END}"
+        self.__print_run_search_stats(
+            records=records, nr_added=nr_added, nr_changed=nr_changed
+        )
+
+    def __add_doi_from_pdf_if_not_available(self, *, record_dict: dict) -> None:
+        if "doi" in record_dict:
+            return
+        record = colrev.record.Record(data=record_dict)
+        record.set_text_from_pdf(project_path=self.review_manager.path)
+        res = re.findall(self.__doi_regex, record.data["text_from_pdf"])
+        if res:
+            record.data["doi"] = res[0].upper()
+        del record.data["text_from_pdf"]
+
+    def run_search(
+        self, search_operation: colrev.ops.search.Search, rerun: bool
+    ) -> None:
+        """Run a search of a PDF directory (based on GROBID)"""
+
+        # Do not run in continuous-integration environment
+        if search_operation.review_manager.in_ci_environment():
+            return
+
+        if search_operation.review_manager.force_mode:  # i.e., reindex all
+            search_operation.review_manager.logger.info("Reindex all")
+
+        # Removing records/origins for which PDFs were removed makes sense for curated repositories
+        # In regular repositories, it may be confusing (e.g., if PDFs are renamed)
+        # In these cases, we may simply print a warning instead of modifying/removing records?
+        if self.review_manager.settings.is_curated_masterdata_repo():
+            self.__remove_records_if_pdf_no_longer_exists(
+                search_operation=search_operation
             )
 
-        if search_operation.review_manager.force_mode:
-            if nr_changed > 0:
-                search_operation.review_manager.logger.info(
-                    f"{colors.GREEN}Updated {nr_changed} records{colors.END}"
-                )
-            else:
-                if records:
-                    search_operation.review_manager.logger.info(
-                        f"{colors.GREEN}Records (data/records.bib) up-to-date{colors.END}"
-                    )
+        grobid_service = self.review_manager.get_grobid_service()
+        grobid_service.start()
+
+        local_index = self.review_manager.get_local_index()
+
+        records = self.review_manager.dataset.load_records_dict()
+        pdfs_dir_feed = self.search_source.get_feed(
+            review_manager=self.review_manager,
+            source_identifier=self.source_identifier,
+            update_only=(not rerun),
+        )
+
+        linked_pdf_paths = [Path(r["file"]) for r in records.values() if "file" in r]
+
+        self.__run_pdfs_dir_search(
+            search_operation=search_operation,
+            records=records,
+            pdfs_dir_feed=pdfs_dir_feed,
+            linked_pdf_paths=linked_pdf_paths,
+            local_index=local_index,
+            rerun=rerun,
+        )
 
     @classmethod
     def heuristic(cls, filename: Path, data: str) -> dict:
         """Source heuristic for PDF directories (GROBID)"""
 
         result = {"confidence": 0.0}
 
@@ -658,15 +698,15 @@
 
     @classmethod
     def add_endpoint(
         cls, search_operation: colrev.ops.search.Search, query: str
     ) -> typing.Optional[colrev.settings.SearchSource]:
         """Add SearchSource as an endpoint (based on query provided to colrev search -a )"""
 
-        if "pdfs" == query:
+        if query == "pdfs":
             filename = search_operation.get_unique_filename(file_path_string="pdfs")
             # pylint: disable=no-value-for-parameter
             add_source = colrev.settings.SearchSource(
                 endpoint="colrev.pdfs_dir",
                 filename=filename,
                 search_type=colrev.settings.SearchType.PDFS,
                 search_parameters={"scope": {"path": "data/pdfs"}},
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/psycinfo.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/psycinfo.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/pubmed.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/pubmed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 #! /usr/bin/env python
 """SearchSource: Pubmed"""
 from __future__ import annotations
 
 import typing
-import xml.etree.ElementTree as ET
 from copy import deepcopy
 from dataclasses import dataclass
 from multiprocessing import Lock
 from pathlib import Path
 from sqlite3 import OperationalError
 from typing import Optional
 from urllib.parse import urlparse
+from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
+import defusedxml
 import requests
 import zope.interface
 from dacite import from_dict
 from dataclasses_jsonschema import JsonSchemaMixin
+from defusedxml.lxml import fromstring
 
 import colrev.env.package_manager
 import colrev.exceptions as colrev_exceptions
 import colrev.ops.search
 import colrev.record
 import colrev.ui_cli.cli_colors as colors
 
+defusedxml.defuse_stdlib()
+
+
 # pylint: disable=unused-argument
 # pylint: disable=duplicate-code
 
 
 @zope.interface.implementer(
     colrev.env.package_manager.SearchSourcePackageEndpointInterface
 )
@@ -111,15 +116,15 @@
 
         host = urlparse(query).hostname
 
         if host and host.endswith("pubmed.ncbi.nlm.nih.gov"):
             query = query.replace("https://pubmed.ncbi.nlm.nih.gov/?term=", "")
 
             filename = search_operation.get_unique_filename(
-                file_path_string=f"pubmed_{query}"
+                file_path_string=f"pubmed_{query.replace('&sort=', '')}"
             )
             query = (
                 "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi?db=pubmed&term="
                 + query
             )
             add_source = colrev.settings.SearchSource(
                 endpoint="colrev.pubmed",
@@ -185,106 +190,104 @@
                     raise colrev_exceptions.ServiceNotAvailableException("Pubmed")
         except (requests.exceptions.RequestException, IndexError) as exc:
             print(exc)
             if not source_operation.force_mode:
                 raise colrev_exceptions.ServiceNotAvailableException("Pubmed") from exc
 
     @classmethod
-    def __pubmed_xml_to_record(cls, *, root: Element) -> dict:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
-        # pylint: disable=too-many-nested-blocks
+    def __get_author_string_from_node(cls, *, author_node: Element) -> str:
+        authors_string = ""
+        author_last_name_node = author_node.find("LastName")
+        if author_last_name_node is not None:
+            if author_last_name_node.text is not None:
+                authors_string += author_last_name_node.text
+        author_fore_name_node = author_node.find("ForeName")
+        if author_fore_name_node is not None:
+            if author_fore_name_node.text is not None:
+                authors_string += ", "
+                authors_string += author_fore_name_node.text
+        return authors_string
+
+    @classmethod
+    def __get_author_string(cls, *, root) -> str:  # type: ignore
+        authors_list = []
+        for author_node in root.xpath(
+            "/PubmedArticleSet/PubmedArticle/MedlineCitation/Article/AuthorList/Author"
+        ):
+            authors_list.append(
+                cls.__get_author_string_from_node(author_node=author_node)
+            )
+        return " and ".join(authors_list)
+
+    @classmethod
+    def __get_title_string(cls, *, root) -> str:  # type: ignore
+        title = root.xpath(
+            "/PubmedArticleSet/PubmedArticle/MedlineCitation/Article/ArticleTitle"
+        )
+        if title:
+            title = title[0].text.strip().rstrip(".")
+        return title
+
+    @classmethod
+    def __get_abstract_string(cls, *, root) -> str:  # type: ignore
+        abstract = root.xpath(
+            "/PubmedArticleSet/PubmedArticle/MedlineCitation/Article/Abstract"
+        )
+        if abstract:
+            return ElementTree.tostring(abstract[0], encoding="unicode")
+        return ""
 
+    @classmethod
+    def __pubmed_xml_to_record(cls, *, root) -> dict:  # type: ignore
         retrieved_record_dict: dict = {"ENTRYTYPE": "misc"}
 
         pubmed_article = root.find("PubmedArticle")
-        item = None
-        if pubmed_article is not None:
-            item = pubmed_article.find("MedlineCitation")
-        if item is not None:
-            article_node = item.find("Article")
-        else:
+        if pubmed_article is None:
+            return {}
+        if pubmed_article.find("MedlineCitation") is None:
             return {}
 
-        authors_string = ""
-        if article_node is not None:
-            author_list_node = article_node.find("AuthorList")
-            if author_list_node is not None:
-                author_nodes = author_list_node.findall("Author")
-                if author_nodes is not None:
-                    for author_node in author_nodes:
-                        if author_node is not None:
-                            author_last_name_node = author_node.find("LastName")
-                            if author_last_name_node is not None:
-                                if author_last_name_node.text is not None:
-                                    authors_string += author_last_name_node.text
-                            author_fore_name_node = author_node.find("ForeName")
-                            if author_fore_name_node is not None:
-                                if author_fore_name_node.text is not None:
-                                    authors_string += ", "
-                                    authors_string += author_fore_name_node.text
-                            authors_string += " and "
-        authors_string = authors_string.rstrip(" and ")
-        retrieved_record_dict.update(author=authors_string)
-
-        if article_node is not None:
-            title_node = article_node.find("ArticleTitle")
-            if title_node is not None:
-                if title_node.text is not None:
-                    retrieved_record_dict.update(title=title_node.text.rstrip("."))
-
-        if article_node is not None:
-            journal_node = article_node.find("Journal")
-            if journal_node is not None:
-                journal_name_node = journal_node.find("ISOAbbreviation")
-                if journal_name_node is not None:
-                    if journal_name_node.text is not None:
-                        retrieved_record_dict.update(journal=journal_name_node.text)
-                        retrieved_record_dict.update(ENTRYTYPE="article")
-                journal_issue_node = journal_node.find("JournalIssue")
-                if journal_issue_node is not None:
-                    journal_volume_node = journal_issue_node.find("Volume")
-                    if journal_volume_node is not None:
-                        if journal_volume_node.text is not None:
-                            retrieved_record_dict.update(
-                                volume=journal_volume_node.text
-                            )
-                    journal_number_node = journal_issue_node.find("Issue")
-                    if journal_number_node is not None:
-                        if journal_number_node.text is not None:
-                            retrieved_record_dict.update(
-                                number=journal_number_node.text
-                            )
-
-                    pubdate_node = journal_issue_node.find("PubDate")
-                    if pubdate_node is not None:
-                        if pubdate_node.text is not None:
-                            retrieved_record_dict.update(year=pubdate_node.text)
-
-        if article_node is not None:
-            abstract_node = article_node.find("Abstract")
-            if abstract_node is not None:
-                if abstract_node.text is not None:
-                    retrieved_record_dict.update(abstract=abstract_node.text)
-
-        if pubmed_article is not None:
-            pubmed_data_node = pubmed_article.find("PubmedData")
-            if pubmed_data_node is not None:
-                article_id_node = pubmed_data_node.find("ArticleIdList")
-                if article_id_node is not None:
-                    for article_id_node_item in article_id_node:
-                        id_type = article_id_node_item.attrib.get("IdType")
-                        id_text = article_id_node_item.text
-                        if id_type is not None and id_text is not None:
-                            if "pubmed" == id_type:
-                                id_type = "pubmedid"
-                            if "doi" == id_type:
-                                id_text = id_text.upper()
-                            retrieved_record_dict[id_type] = id_text
+        retrieved_record_dict.update(title=cls.__get_title_string(root=root))
+        retrieved_record_dict.update(author=cls.__get_author_string(root=root))
+
+        journal_path = "/PubmedArticleSet/PubmedArticle/MedlineCitation/Article/Journal"
+        journal_name = root.xpath(journal_path + "/ISOAbbreviation")
+        if journal_name:
+            retrieved_record_dict.update(ENTRYTYPE="article")
+            retrieved_record_dict.update(journal=journal_name[0].text)
+
+        volume = root.xpath(journal_path + "/JournalIssue/Volume")
+        if volume:
+            retrieved_record_dict.update(volume=volume[0].text)
+
+        number = root.xpath(journal_path + "/JournalIssue/Issue")
+        if number:
+            retrieved_record_dict.update(number=number[0].text)
+
+        year = root.xpath(journal_path + "/JournalIssue/PubDate/Year")
+        if year:
+            retrieved_record_dict.update(year=year[0].text)
+
+        retrieved_record_dict.update(volume=cls.__get_abstract_string(root=root))
+
+        article_id_list = root.xpath(
+            "/PubmedArticleSet/PubmedArticle/PubmedData/ArticleIdList"
+        )
+        for article_id in article_id_list[0]:
+            id_type = article_id.attrib.get("IdType")
+            if article_id.attrib.get("IdType") == "pubmed":
+                retrieved_record_dict.update(pubmedid=article_id.text.upper())
+            elif article_id.attrib.get("IdType") == "doi":
+                retrieved_record_dict.update(doi=article_id.text.upper())
+            else:
+                retrieved_record_dict[id_type] = article_id.text
+
+        retrieved_record_dict = {
+            k: v for k, v in retrieved_record_dict.items() if v != ""
+        }
 
         return retrieved_record_dict
 
     def __get_pubmed_ids(self, query: str, retstart: int) -> typing.List[str]:
         headers = {"user-agent": f"{__name__} (mailto:{self.email})"}
         session = self.review_manager.get_cached_session()
 
@@ -295,27 +298,27 @@
         ret.raise_for_status()
         if ret.status_code != 200:
             # review_manager.logger.debug(
             #     f"crossref_query failed with status {ret.status_code}"
             # )
             return []
 
-        root = ET.fromstring(ret.text)
+        root = fromstring(str.encode(ret.text))
         return [
             x.text
             for x_el in root.findall("IdList")
             for x in x_el
             if x.text is not None
         ]
 
     def __pubmed_query_id(
         self,
         *,
         pubmed_id: str,
-        timeout: int = 10,
+        timeout: int = 60,
     ) -> dict:
         """Retrieve records from Pubmed based on a query"""
 
         try:
             database = "pubmed"
             url = (
                 "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi?"
@@ -328,22 +331,22 @@
             # review_manager.logger.debug(url)
             ret = session.request("GET", url, headers=headers, timeout=timeout)
             ret.raise_for_status()
             if ret.status_code != 200:
                 # review_manager.logger.debug(
                 #     f"crossref_query failed with status {ret.status_code}"
                 # )
-                return {}
+                return {"pubmed_id": pubmed_id}
 
-            root = ET.fromstring(ret.text)
+            root = fromstring(str.encode(ret.text))
             retrieved_record = self.__pubmed_xml_to_record(root=root)
             if not retrieved_record:
-                return {}
+                return {"pubmed_id": pubmed_id}
         except requests.exceptions.RequestException:
-            return {}
+            return {"pubmed_id": pubmed_id}
         # pylint: disable=duplicate-code
         except OperationalError as exc:
             raise colrev_exceptions.ServiceNotAvailableException(
                 "sqlite, required for requests CachedSession "
                 "(possibly caused by concurrent operations)"
             ) from exc
 
@@ -474,15 +477,14 @@
             pubmed_ids = self.__get_pubmed_ids(query=params["query"], retstart=retstart)
             if not pubmed_ids:
                 break
             for pubmed_id in pubmed_ids:
                 yield self.__pubmed_query_id(pubmed_id=pubmed_id)
 
             retstart += 20
-            # input(pubmed_ids)
 
     def __run_parameter_search(
         self,
         *,
         search_operation: colrev.ops.search.Search,
         pubmed_feed: colrev.ops.search.GeneralOriginFeed,
         rerun: bool,
@@ -499,14 +501,17 @@
 
         try:
             for record_dict in self.__get_pubmed_query_return():
                 # Note : discard "empty" records
                 if "" == record_dict.get("author", "") and "" == record_dict.get(
                     "title", ""
                 ):
+                    search_operation.review_manager.logger.warning(
+                        f"Skipped record: {record_dict}"
+                    )
                     continue
                 try:
                     pubmed_feed.set_id(record_dict=record_dict)
                 except colrev_exceptions.NotFeedIdentifiableException:
                     continue
 
                 prev_record_dict_version = {}
@@ -686,33 +691,35 @@
                     record["author"] = " and ".join(author_list)
             if "first_author" in record:
                 del record["first_author"]
             if "citation" in record:
                 del record["citation"]
             if "create_date" in record:
                 del record["create_date"]
-            if "" != record.get("journal", ""):
+            if record.get("journal", "") != "":
                 record["ENTRYTYPE"] = "article"
+            if record.get("pii", "pii").lower() == record.get("doi", "doi").lower():
+                del record["pii"]
 
         return records
 
     def prepare(
         self, record: colrev.record.Record, source: colrev.settings.SearchSource
     ) -> colrev.record.Record:
         """Source-specific preparation for Pubmed"""
 
         if "first_author" in record.data:
             record.remove_field(key="first_author")
         if "journal/book" in record.data:
             record.rename_field(key="journal/book", new_key="journal")
-        if "UNKNOWN" == record.data.get("author") and "authors" in record.data:
+        if record.data.get("author") == "UNKNOWN" and "authors" in record.data:
             record.remove_field(key="author")
             record.rename_field(key="authors", new_key="author")
 
-        if "UNKNOWN" == record.data.get("year"):
+        if record.data.get("year") == "UNKNOWN":
             record.remove_field(key="year")
             if "publication_year" in record.data:
                 record.rename_field(key="publication_year", new_key="year")
 
         if "author" in record.data:
             record.data["author"] = colrev.record.PrepRecord.format_author_field(
                 input_string=record.data["author"]
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/scopus.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/scopus.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/springer_link.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/springer_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,56 +116,59 @@
         source: colrev.settings.SearchSource,
         records: typing.Dict,
     ) -> dict:
         """Load fixes for Springer Link"""
 
         # pylint: disable=too-many-branches
 
-        for record in records.values():
-            if "item_title" in record:
-                record["title"] = record["item_title"]
-                del record["item_title"]
-
-            if "content_type" in record:
-                if "Article" == record["content_type"]:
-                    if "publication_title" in record:
-                        record["journal"] = record["publication_title"]
-                        del record["publication_title"]
+        for record_dict in records.values():
+            if "item_title" in record_dict:
+                record_dict["title"] = record_dict["item_title"]
+                del record_dict["item_title"]
+
+            if "content_type" in record_dict:
+                record = colrev.record.Record(data=record_dict)
+                if record_dict["content_type"] == "Article":
+                    if "publication_title" in record_dict:
+                        record_dict["journal"] = record_dict["publication_title"]
+                        del record_dict["publication_title"]
                     record.change_entrytype(new_entrytype="article")
 
-                if "Book" == record["content_type"]:
-                    if "publication_title" in record:
-                        record["series"] = record["publication_title"]
-                        del record["publication_title"]
+                if record_dict["content_type"] == "Book":
+                    if "publication_title" in record_dict:
+                        record_dict["series"] = record_dict["publication_title"]
+                        del record_dict["publication_title"]
                     record.change_entrytype(new_entrytype="book")
 
-                if "Chapter" == record["content_type"]:
-                    record["chapter"] = record["title"]
-                    if "publication_title" in record:
-                        record["title"] = record["publication_title"]
-                        del record["publication_title"]
+                if record_dict["content_type"] == "Chapter":
+                    record_dict["chapter"] = record_dict["title"]
+                    if "publication_title" in record_dict:
+                        record_dict["title"] = record_dict["publication_title"]
+                        del record_dict["publication_title"]
                     record.change_entrytype(new_entrytype="inbook")
 
-                del record["content_type"]
+                del record_dict["content_type"]
 
-            if "item_doi" in record:
-                record["doi"] = record["item_doi"]
-                del record["item_doi"]
-            if "journal_volume" in record:
-                record["volume"] = record["journal_volume"]
-                del record["journal_volume"]
-            if "journal_issue" in record:
-                record["number"] = record["journal_issue"]
-                del record["journal_issue"]
+            if "item_doi" in record_dict:
+                record_dict["doi"] = record_dict["item_doi"]
+                del record_dict["item_doi"]
+            if "journal_volume" in record_dict:
+                record_dict["volume"] = record_dict["journal_volume"]
+                del record_dict["journal_volume"]
+            if "journal_issue" in record_dict:
+                record_dict["number"] = record_dict["journal_issue"]
+                del record_dict["journal_issue"]
 
             # Fix authors
-            if "author" in record:
+            if "author" in record_dict:
                 # a-bd-z: do not match McDonald
-                record["author"] = re.sub(
-                    r"([a-bd-z]{1})([A-Z]{1})", r"\g<1> and \g<2>", record["author"]
+                record_dict["author"] = re.sub(
+                    r"([a-bd-z]{1})([A-Z]{1})",
+                    r"\g<1> and \g<2>",
+                    record_dict["author"],
                 )
 
         return records
 
     def prepare(
         self, record: colrev.record.Record, source: colrev.settings.SearchSource
     ) -> colrev.record.Record:
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/systematic_review_datasets.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/systematic_review_datasets.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/taylor_and_francis.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/taylor_and_francis.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/trid.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/trid.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/unknown_source.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/unknown_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     short_name = "Unknown Source"
     link = (
         "https://github.com/CoLRev-Environment/colrev/blob/main/"
         + "colrev/ops/built_in/search_sources/unknown_source.md"
     )
 
     HTML_CLEANER = re.compile("<.*?>")
+    __padding = 40
 
     def __init__(
         self, *, source_operation: colrev.operation.CheckOperation, settings: dict
     ) -> None:
         converters = {Path: Path, Enum: Enum}
         self.search_source = from_dict(
             data_class=self.settings_class,
@@ -117,187 +118,173 @@
         source: colrev.settings.SearchSource,
         records: typing.Dict,
     ) -> dict:
         """Load fixes for unknown sources"""
 
         return records
 
-    def prepare(
-        self, record: colrev.record.PrepRecord, source: colrev.settings.SearchSource
-    ) -> colrev.record.Record:
-        """Source-specific preparation for unknown sources"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+    def __heuristically_fix_entrytypes(
+        self, *, record: colrev.record.PrepRecord, source_identifier: str
+    ) -> None:
+        """Prepare the record by heuristically correcting erroneous ENTRYTYPEs"""
 
-        if not record.has_inconsistent_fields() or record.masterdata_is_curated():
-            return record
+        # Journal articles should not have booktitles/series set.
+        if record.data["ENTRYTYPE"] == "article":
+            if "booktitle" in record.data:
+                if "journal" not in record.data:
+                    record.update_field(
+                        key="journal",
+                        value=record.data["booktitle"],
+                        source="unkown_source_prep",
+                    )
+                    record.remove_field(key="booktitle")
+            if "series" in record.data:
+                if "journal" not in record.data:
+                    record.update_field(
+                        key="journal",
+                        value=record.data["series"],
+                        source="unkown_source_prep",
+                    )
+                    record.remove_field(key="series")
 
-        if "colrev.md_to_bib" == source.load_conversion_package_endpoint["endpoint"]:
-            if "misc" == record.data["ENTRYTYPE"] and "publisher" in record.data:
+        if source_identifier == "colrev.md_to_bib":
+            if record.data["ENTRYTYPE"] == "misc" and "publisher" in record.data:
                 record.update_field(
                     key="ENTRYTYPE", value="book", source="unkown_source_prep"
                 )
             if record.data.get("year", "year") == record.data.get("date", "date"):
                 record.remove_field(key="date")
             if (
                 "inbook" == record.data["ENTRYTYPE"]
                 and "chapter" not in record.data
                 and "title" in record.data
             ):
                 record.rename_field(key="title", new_key="chapter")
 
-        if "UNKNOWN" != record.data.get("author", "UNKNOWN"):
-            # fix name format
-            if (1 == len(record.data["author"].split(" ")[0])) or (
-                ", " not in record.data["author"]
-            ):
-                record.update_field(
-                    key="author",
-                    value=colrev.record.PrepRecord.format_author_field(
-                        input_string=record.data["author"]
-                    ),
-                    source="unkown_source_prep",
-                    keep_source_if_equal=True,
-                )
-
-        if "UNKNOWN" != record.data.get("title", "UNKNOWN"):
-            record.format_if_mostly_upper(key="title")
-
-        if "date" in record.data and "year" not in record.data:
-            year = re.search(r"\d{4}", record.data["date"])
-            if year:
-                record.update_field(
-                    key="year",
-                    value=year.group(0),
-                    source="unkown_source_prep",
-                    keep_source_if_equal=True,
-                )
-
-        if "UNKNOWN" != record.data.get("journal", "UNKNOWN"):
-            if len(record.data["journal"]) > 10 and "UNKNOWN" != record.data["journal"]:
-                record.format_if_mostly_upper(key="journal", case="title")
-
-        # Prepare the record by heuristically correcting erroneous ENTRYTYPEs
-        padding = 40
-
         if (
             "dissertation" in record.data.get("fulltext", "NA").lower()
             and record.data["ENTRYTYPE"] != "phdthesis"
         ):
             prior_e_type = record.data["ENTRYTYPE"]
             record.update_field(
                 key="ENTRYTYPE", value="phdthesis", source="unkown_source_prep"
             )
             self.review_manager.report_logger.info(
-                f' {record.data["ID"]}'.ljust(padding, " ")
+                f' {record.data["ID"]}'.ljust(self.__padding, " ")
                 + f"Set from {prior_e_type} to phdthesis "
                 '("dissertation" in fulltext link)'
             )
 
         if (
             "thesis" in record.data.get("fulltext", "NA").lower()
             and record.data["ENTRYTYPE"] != "phdthesis"
         ):
             prior_e_type = record.data["ENTRYTYPE"]
             record.update_field(
                 key="ENTRYTYPE", value="phdthesis", source="unkown_source_prep"
             )
             self.review_manager.report_logger.info(
-                f' {record.data["ID"]}'.ljust(padding, " ")
+                f' {record.data["ID"]}'.ljust(self.__padding, " ")
                 + f"Set from {prior_e_type} to phdthesis "
                 '("thesis" in fulltext link)'
             )
 
         if (
-            "This thesis" in record.data.get("abstract", "NA").lower()
+            "this thesis" in record.data.get("abstract", "NA").lower()
             and record.data["ENTRYTYPE"] != "phdthesis"
         ):
             prior_e_type = record.data["ENTRYTYPE"]
             record.update_field(
                 key="ENTRYTYPE", value="phdthesis", source="unkown_source_prep"
             )
             self.review_manager.report_logger.info(
-                f' {record.data["ID"]}'.ljust(padding, " ")
+                f' {record.data["ID"]}'.ljust(self.__padding, " ")
                 + f"Set from {prior_e_type} to phdthesis "
                 '("thesis" in abstract)'
             )
 
-        # Journal articles should not have booktitles/series set.
-        if "article" == record.data["ENTRYTYPE"]:
-            if "booktitle" in record.data:
-                if "journal" not in record.data:
-                    record.update_field(
-                        key="journal",
-                        value=record.data["booktitle"],
-                        source="unkown_source_prep",
-                    )
-                    record.remove_field(key="booktitle")
-            if "series" in record.data:
-                if "journal" not in record.data:
-                    record.update_field(
-                        key="journal",
-                        value=record.data["series"],
-                        source="unkown_source_prep",
-                    )
-                    record.remove_field(key="series")
+    def __format_inproceedings(self, *, record: colrev.record.PrepRecord) -> None:
+        if record.data.get("booktitle", "UNKNOWN") == "UNKNOWN":
+            return
+        if (
+            "UNKNOWN" != record.data["booktitle"]
+            and "inbook" != record.data["ENTRYTYPE"]
+        ):
+            record.format_if_mostly_upper(key="booktitle", case="title")
 
-        if "article" == record.data["ENTRYTYPE"]:
-            if "journal" not in record.data:
-                if "series" in record.data:
-                    journal_string = record.data["series"]
-                    record.update_field(
-                        key="journal", value=journal_string, source="unkown_source_prep"
-                    )
-                    record.remove_field(key="series")
+            stripped_btitle = re.sub(r"\d{4}", "", record.data["booktitle"])
+            stripped_btitle = re.sub(r"\d{1,2}th", "", stripped_btitle)
+            stripped_btitle = re.sub(r"\d{1,2}nd", "", stripped_btitle)
+            stripped_btitle = re.sub(r"\d{1,2}rd", "", stripped_btitle)
+            stripped_btitle = re.sub(r"\d{1,2}st", "", stripped_btitle)
+            stripped_btitle = re.sub(r"\([A-Z]{3,6}\)", "", stripped_btitle)
+            stripped_btitle = stripped_btitle.replace("Proceedings of the", "").replace(
+                "Proceedings", ""
+            )
+            stripped_btitle = stripped_btitle.lstrip().rstrip()
+            record.update_field(
+                key="booktitle",
+                value=stripped_btitle,
+                source="unkown_source_prep",
+                keep_source_if_equal=True,
+            )
 
-        if "UNKNOWN" != record.data.get("booktitle", "UNKNOWN"):
-            if (
-                "UNKNOWN" != record.data["booktitle"]
-                and "inbook" != record.data["ENTRYTYPE"]
-            ):
-                record.format_if_mostly_upper(key="booktitle", case="title")
+    def __format_article(self, record: colrev.record.PrepRecord) -> None:
+        if record.data.get("journal", "UNKNOWN") != "UNKNOWN":
+            if len(record.data["journal"]) > 10 and "UNKNOWN" != record.data["journal"]:
+                record.format_if_mostly_upper(key="journal", case="title")
+
+        if record.data.get("volume", "UNKNOWN") != "UNKNOWN":
+            record.update_field(
+                key="volume",
+                value=record.data["volume"].replace("Volume ", ""),
+                source="unkown_source_prep",
+                keep_source_if_equal=True,
+            )
+
+    def __format_fields(self, *, record: colrev.record.PrepRecord) -> None:
+        """Format fields"""
 
-                stripped_btitle = re.sub(r"\d{4}", "", record.data["booktitle"])
-                stripped_btitle = re.sub(r"\d{1,2}th", "", stripped_btitle)
-                stripped_btitle = re.sub(r"\d{1,2}nd", "", stripped_btitle)
-                stripped_btitle = re.sub(r"\d{1,2}rd", "", stripped_btitle)
-                stripped_btitle = re.sub(r"\d{1,2}st", "", stripped_btitle)
-                stripped_btitle = re.sub(r"\([A-Z]{3,6}\)", "", stripped_btitle)
-                stripped_btitle = stripped_btitle.replace(
-                    "Proceedings of the", ""
-                ).replace("Proceedings", "")
-                stripped_btitle = stripped_btitle.lstrip().rstrip()
+        if record.data["entrytype"] == "inproceedings":
+            self.__format_inproceedings(record=record)
+        elif record.data["entrytype"] == "article":
+            self.__format_article(record=record)
+
+        if record.data.get("author", "UNKNOWN") != "UNKNOWN":
+            # fix name format
+            if (1 == len(record.data["author"].split(" ")[0])) or (
+                ", " not in record.data["author"]
+            ):
                 record.update_field(
-                    key="booktitle",
-                    value=stripped_btitle,
+                    key="author",
+                    value=colrev.record.PrepRecord.format_author_field(
+                        input_string=record.data["author"]
+                    ),
                     source="unkown_source_prep",
                     keep_source_if_equal=True,
                 )
+            # Replace nicknames in parentheses
+            record.data["author"] = re.sub(r"\([^)]*\)", "", record.data["author"])
+            record.data["author"] = record.data["author"].replace("  ", " ").rstrip()
+
+        if record.data.get("title", "UNKNOWN") != "UNKNOWN":
+            record.format_if_mostly_upper(key="title")
 
-        record.unify_pages_field()
         if "pages" in record.data:
+            record.unify_pages_field()
             if (
                 not re.match(r"^\d*$", record.data["pages"])
                 and not re.match(r"^\d*--\d*$", record.data["pages"])
                 and not re.match(r"^[xivXIV]*--[xivXIV]*$", record.data["pages"])
             ):
                 self.review_manager.report_logger.info(
-                    f' {record.data["ID"]}:'.ljust(padding, " ")
+                    f' {record.data["ID"]}:'.ljust(self.__padding, " ")
                     + f'Unusual pages: {record.data["pages"]}'
                 )
 
-        if "UNKNOWN" != record.data.get("volume", "UNKNOWN"):
-            record.update_field(
-                key="volume",
-                value=record.data["volume"].replace("Volume ", ""),
-                source="unkown_source_prep",
-                keep_source_if_equal=True,
-            )
-
         if "url" in record.data and "fulltext" in record.data:
             if record.data["url"] == record.data["fulltext"]:
                 record.remove_field(key="fulltext")
 
         if "language" in record.data:
             try:
                 self.language_service.unify_to_iso_639_3_language_codes(record=record)
@@ -306,53 +293,78 @@
                     value=record.data["language"],
                     source="unkown_source_prep",
                     keep_source_if_equal=True,
                 )
             except colrev_exceptions.InvalidLanguageCodeException:
                 del record.data["language"]
 
+    def __remove_redundant_fields(self, *, record: colrev.record.PrepRecord) -> None:
+        if record.data["ENTRYTYPE"] == "article":
+            if "journal" in record.data and "booktitle" in record.data:
+                similarity_journal_booktitle = fuzz.partial_ratio(
+                    record.data["journal"].lower(), record.data["booktitle"].lower()
+                )
+                if similarity_journal_booktitle / 100 > 0.9:
+                    record.remove_field(key="booktitle")
+
+        if record.data.get("publisher", "") in ["researchgate.net"]:
+            record.remove_field(key="publisher")
+
+        if record.data["ENTRYTYPE"] == "inproceedings":
+            if "journal" in record.data and "booktitle" in record.data:
+                similarity_journal_booktitle = fuzz.partial_ratio(
+                    record.data["journal"].lower(), record.data["booktitle"].lower()
+                )
+                if similarity_journal_booktitle / 100 > 0.9:
+                    record.remove_field(key="journal")
+
+    def __impute_missing_fields(self, *, record: colrev.record.PrepRecord) -> None:
+        if "date" in record.data and "year" not in record.data:
+            year = re.search(r"\d{4}", record.data["date"])
+            if year:
+                record.update_field(
+                    key="year",
+                    value=year.group(0),
+                    source="unkown_source_prep",
+                    keep_source_if_equal=True,
+                )
+
+    def __unify_special_characters(self, *, record: colrev.record.PrepRecord) -> None:
+        # Remove html entities
         for field in list(record.data.keys()):
-            # Note : some dois (and their provenance) contain html entities
+            # Skip dois (and their provenance), which may contain html entities
             if field in [
                 "colrev_masterdata_provenance",
                 "colrev_data_provenance",
                 "doi",
             ]:
                 continue
             if field in ["author", "title", "journal"]:
                 record.data[field] = re.sub(r"\s+", " ", record.data[field])
                 record.data[field] = re.sub(self.HTML_CLEANER, "", record.data[field])
 
-        if "article" == record.data["ENTRYTYPE"]:
-            if "journal" in record.data and "booktitle" in record.data:
-                if (
-                    fuzz.partial_ratio(
-                        record.data["journal"].lower(), record.data["booktitle"].lower()
-                    )
-                    / 100
-                    > 0.9
-                ):
-                    record.remove_field(key="booktitle")
-        if "inproceedings" == record.data["ENTRYTYPE"]:
-            if "journal" in record.data and "booktitle" in record.data:
-                if (
-                    fuzz.partial_ratio(
-                        record.data["journal"].lower(), record.data["booktitle"].lower()
-                    )
-                    / 100
-                    > 0.9
-                ):
-                    record.remove_field(key="journal")
+    def prepare(
+        self, record: colrev.record.PrepRecord, source: colrev.settings.SearchSource
+    ) -> colrev.record.Record:
+        """Source-specific preparation for unknown sources"""
 
-        if record.data.get("publisher", "") in ["researchgate.net"]:
-            record.remove_field(key="publisher")
+        if not record.has_inconsistent_fields() or record.masterdata_is_curated():
+            return record
 
-        # Replace nicknames in parentheses
-        if "author" in record.data:
-            record.data["author"] = re.sub(r"\([^)]*\)", "", record.data["author"])
-            record.data["author"] = record.data["author"].replace("  ", " ").rstrip()
+        self.__heuristically_fix_entrytypes(
+            record=record,
+            source_identifier=source.load_conversion_package_endpoint["endpoint"],
+        )
+
+        self.__impute_missing_fields(record=record)
+
+        self.__format_fields(record=record)
+
+        self.__remove_redundant_fields(record=record)
+
+        self.__unify_special_characters(record=record)
 
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/utils.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,170 @@
 #! /usr/bin/env python
-"""Connector to doi.org (API)"""
+"""Utility to transform crossref/doi.org items to records"""
 from __future__ import annotations
 
 import html
 import re
 
-import colrev.record
+# pylint: disable=duplicate-code
 
-if False:  # pylint: disable=using-constant-test
-    from typing import TYPE_CHECKING
 
-    if TYPE_CHECKING:
-        import colrev.ops.prep
-
-
-def json_to_record(*, item: dict) -> dict:
-    """Convert a crossref item to a record dict"""
-
-    # pylint: disable=too-many-branches
-    # pylint: disable=too-many-statements
-    # pylint: disable=too-many-locals
-
-    # Note: the format differst between crossref and doi.org
-    record_dict: dict = {}
-
-    # Note : better use the doi-link resolution
-    if "link" in item:
-        fulltext_link_l = [u["URL"] for u in item["link"] if "pdf" in u["content-type"]]
-        if len(fulltext_link_l) == 1:
-            record_dict["fulltext"] = fulltext_link_l.pop()
-    #     item["link"] = [u for u in item["link"] if "pdf" not in u["content-type"]]
-    #     if len(item["link"]) >= 1:
-    #         link = item["link"][0]["URL"]
-    #         if link != record_dict.get("fulltext", ""):
-    #             record_dict["link"] = link
-
-    if "title" in item:
-        retrieved_title = ""
-        if isinstance(item["title"], list):
-            if len(item["title"]) > 0:
-                retrieved_title = str(item["title"][0])
-        elif isinstance(item["title"], str):
-            retrieved_title = item["title"]
-
-        if retrieved_title:
-            retrieved_title = retrieved_title.replace("\n", " ")
-            retrieved_title = retrieved_title.replace("<scp>", "{")
-            retrieved_title = retrieved_title.replace("</scp>", "}")
-            retrieved_title = re.sub(r"<\/?[^>]*>", " ", retrieved_title)
-            retrieved_title = re.sub(r"\s+", " ", retrieved_title).rstrip().lstrip()
-            record_dict.update(title=retrieved_title)
-
-    container_title = ""
-    if "container-title" in item:
-        if isinstance(item["container-title"], list):
-            if len(item["container-title"]) > 0:
-                container_title = item["container-title"][0]
-        elif isinstance(item["container-title"], str):
-            container_title = item["container-title"]
-
-    container_title = container_title.replace("\n", " ")
-    container_title = re.sub(r"\s+", " ", container_title)
-    if "type" in item:
-        if "journal-article" == item.get("type", "NA"):
-            record_dict.update(ENTRYTYPE="article")
-            if container_title is not None:
-                record_dict.update(journal=container_title)
-        if "proceedings-article" == item.get("type", "NA"):
-            record_dict.update(ENTRYTYPE="inproceedings")
-            if container_title is not None:
-                record_dict.update(booktitle=container_title)
-        if "book" == item.get("type", "NA"):
-            record_dict.update(ENTRYTYPE="book")
-            if container_title is not None:
-                record_dict.update(series=container_title)
+def __get_year(*, item: dict) -> str:
+    try:
+        if "published-print" in item:
+            date_parts = item["published-print"]["date-parts"]
+        elif "published" in item:
+            date_parts = item["published"]["date-parts"]
+        elif "published-online" in item:
+            date_parts = item["published-online"]["date-parts"]
+        else:
+            return ""
+        year = str(date_parts[0][0])
+    except KeyError:
+        pass
+    return year
 
-    if "DOI" in item:
-        record_dict.update(doi=item["DOI"].upper())
 
+def __get_authors(*, item: dict) -> str:
     authors_strings = []
     for author in item.get("author", "NA"):
         a_string = ""
-
         if "family" in author:
             a_string += author["family"]
             if "given" in author:
                 a_string += f", {author['given']}"
             authors_strings.append(a_string)
-    authors_string = " and ".join(authors_strings)
-    authors_string = re.sub(r"\s+", " ", authors_string)
-
-    # authors_string = PrepRecord.format_author_field(authors_string)
-    record_dict.update(author=authors_string)
-
-    try:
-        if "published-print" in item:
-            date_parts = item["published-print"]["date-parts"]
-            record_dict.update(year=str(date_parts[0][0]))
-        elif "published" in item:
-            date_parts = item["published"]["date-parts"]
-            record_dict.update(year=str(date_parts[0][0]))
-        elif "published-online" in item:
-            date_parts = item["published-online"]["date-parts"]
-            record_dict.update(year=str(date_parts[0][0]))
-    except KeyError:
-        pass
+    return " and ".join(authors_strings)
 
-    retrieved_pages = item.get("page", "")
-    if retrieved_pages:
-        # DOI data often has only the first page.
-        if (
-            not record_dict.get("pages", "no_pages") in retrieved_pages
-            and "-" in retrieved_pages
-        ):
-            record_dict.update(pages=item["page"])
-            record = colrev.record.PrepRecord(data=record_dict)
-            record.unify_pages_field()
-            record_dict = record.get_data()
-
-    retrieved_volume = item.get("volume", "")
-    if not retrieved_volume == "":
-        record_dict.update(volume=str(retrieved_volume))
 
-    retrieved_number = item.get("issue", "")
+def __get_number(*, item: dict) -> str:
     if "journal-issue" in item:
         if "issue" in item["journal-issue"]:
-            retrieved_number = item["journal-issue"]["issue"]
-    if not retrieved_number == "":
-        record_dict.update(number=str(retrieved_number))
-
-    if "abstract" in item:
-        retrieved_abstract = item["abstract"]
-        if not retrieved_abstract == "":
-            retrieved_abstract = re.sub(r"<\/?jats\:[^>]*>", " ", retrieved_abstract)
-            retrieved_abstract = re.sub(r"\s+", " ", retrieved_abstract)
-            retrieved_abstract = str(retrieved_abstract).replace("\n", "")
-            retrieved_abstract = retrieved_abstract.lstrip().rstrip()
-            record_dict.update(abstract=retrieved_abstract)
+            item["issue"] = item["journal-issue"]["issue"]
+    return str(item.get("issue", ""))
 
-    if "language" in item:
-        record_dict["language"] = item["language"]
 
-    if (
-        not any(x in item for x in ["published-print", "published"])
-        # and "volume" not in record_dict
-        # and "number" not in record_dict
-        and "year" in record_dict
-    ):
-        record_dict.update(published_online=record_dict["year"])
-        record_dict.update(year="forthcoming")
+def __get_fulltext(*, item: dict) -> str:
+    fulltext_link = ""
+    # Note : better use the doi-link resolution
+    fulltext_link_l = [
+        u["URL"] for u in item.get("link", []) if "pdf" in u["content-type"]
+    ]
+    if len(fulltext_link_l) == 1:
+        fulltext_link = fulltext_link_l.pop()
+    return fulltext_link
 
-    if "is-referenced-by-count" in item:
-        record_dict["cited_by"] = item["is-referenced-by-count"]
 
-    if "update-to" in item:
-        for update_item in item["update-to"]:
+def __item_to_record(*, item: dict) -> dict:
+    # Note: the format differst between crossref and doi.org
+
+    if isinstance(item["title"], list):
+        item["title"] = str(item["title"][0])
+    assert isinstance(item["title"], str)
+
+    if isinstance(item.get("container-title", ""), list):
+        item["container-title"] = item["container-title"][0]
+    assert isinstance(item.get("container-title", ""), str)
+
+    item["ENTRYTYPE"] = "misc"
+    if item.get("type", "NA") == "journal-article":
+        item.update(ENTRYTYPE="article")
+        item.update(journal=item.get("container-title", ""))
+    elif item.get("type", "NA") == "proceedings-article":
+        item.update(ENTRYTYPE="inproceedings")
+        item.update(booktitle=item.get("container-title", ""))
+    elif item.get("type", "NA") == "book":
+        item.update(ENTRYTYPE="book")
+        item.update(series=item.get("container-title", ""))
+
+    item.update(author=__get_authors(item=item))
+    item.update(year=__get_year(item=item))
+    item.update(volume=str(item.get("volume", "")))
+    item.update(number=__get_number(item=item))
+    item.update(pages=item.get("page", "").replace("-", "--"))
+    item.update(cited_by=item.get("is-referenced-by-count", ""))
+    item.update(doi=item.get("DOI", "").upper())
+    item.update(fulltext=__get_fulltext(item=item))
+
+    return item
+
+
+def __flag_retracts(*, record_dict: dict) -> dict:
+    if "update-to" in record_dict:
+        for update_item in record_dict["update-to"]:
             if update_item["type"] == "retraction":
                 record_dict["warning"] = "retracted"
     if "(retracted)" in record_dict.get("title", "").lower():
         record_dict["warning"] = "retracted"
+    return record_dict
+
 
+def __format_fields(*, record_dict: dict) -> dict:
     for key, value in record_dict.items():
         record_dict[key] = str(value).replace("{", "").replace("}", "")
         if key in ["colrev_masterdata_provenance", "colrev_data_provenance", "doi"]:
             continue
         # Note : some dois (and their provenance) contain html entities
+        if not isinstance(value, str):
+            continue
+        value = value.replace("<scp>", "{")
+        value = value.replace("</scp>", "}")
         record_dict[key] = html.unescape(str(value))
+        value = value.replace("\n", " ")
+        value = re.sub(r"<\/?[^>]*>", " ", value)
+        value = re.sub(r"<\/?jats\:[^>]*>", " ", value)
+        value = re.sub(r"\s+", " ", value).rstrip().lstrip()
+        record_dict[key] = value
+
+    return record_dict
+
+
+def __set_forthcoming(*, record_dict: dict) -> dict:
+    if (
+        not any(x in record_dict for x in ["published-print", "published"])
+        and "year" in record_dict
+    ):
+        record_dict.update(published_online=record_dict["year"])
+        record_dict.update(year="forthcoming")
+    return record_dict
+
+
+def __remove_fields(*, record_dict: dict) -> dict:
+    # Drop empty and non-supported fields
+    supported_fields = [
+        "ENTRYTYPE",
+        "ID",
+        "title",
+        "author",
+        "year",
+        "journal",
+        "booktitle",
+        "volume",
+        "number",
+        "pages",
+        "doi",
+        "fulltext",
+        "abstract",
+        "warning",
+        "language",
+    ]
+    record_dict = {
+        k: v for k, v in record_dict.items() if k in supported_fields and v != ""
+    }
+
+    return record_dict
+
+
+def json_to_record(*, item: dict) -> dict:
+    """Convert a crossref item to a record dict"""
 
-    if "ENTRYTYPE" not in record_dict:
-        record_dict["ENTRYTYPE"] = "misc"
+    record_dict = __item_to_record(item=item)
+    record_dict = __set_forthcoming(record_dict=record_dict)
+    record_dict = __flag_retracts(record_dict=record_dict)
+    record_dict = __format_fields(record_dict=record_dict)
+    record_dict = __remove_fields(record_dict=record_dict)
 
     return record_dict
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/video_dir.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/video_dir.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/web_of_science.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/web_of_science.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         return records
 
     def prepare(
         self, record: colrev.record.PrepRecord, source: colrev.settings.SearchSource
     ) -> colrev.record.Record:
         """Source-specific preparation for Web of Science"""
 
-        if "UNKNOWN" != record.data.get("title", "UNKNOWN"):
+        if record.data.get("title", "UNKNOWN") != "UNKNOWN":
             record.format_if_mostly_upper(key="title")
 
         return record
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/website.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/website.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,23 +52,23 @@
         record: colrev.record.Record,
         item: dict,
     ) -> None:
         # pylint: disable=too-many-branches
 
         record.data["ID"] = item["key"]
         record.data["ENTRYTYPE"] = "article"  # default
-        if "journalArticle" == item.get("itemType", ""):
+        if item.get("itemType", "") == "journalArticle":
             record.data["ENTRYTYPE"] = "article"
             if "publicationTitle" in item:
                 record.data["journal"] = item["publicationTitle"]
             if "volume" in item:
                 record.data["volume"] = item["volume"]
             if "issue" in item:
                 record.data["number"] = item["issue"]
-        if "conferencePaper" == item.get("itemType", ""):
+        if item.get("itemType", "") == "conferencePaper":
             record.data["ENTRYTYPE"] = "inproceedings"
             if "proceedingsTitle" in item:
                 record.data["booktitle"] = item["proceedingsTitle"]
         if "creators" in item:
             author_str = ""
             for creator in item["creators"]:
                 author_str += (
@@ -141,15 +141,15 @@
                 return
 
             items = json.loads(export.content.decode())
             if len(items) == 0:
                 self.zotero_lock.release()
                 return
             item = items[0]
-            if "Shibboleth Authentication Request" == item["title"]:
+            if item["title"] == "Shibboleth Authentication Request":
                 self.zotero_lock.release()
                 return
 
             self.__update_record(
                 prep_operation=prep_operation, record=record, item=item
             )
```

### Comparing `colrev-0.8.2/colrev/ops/built_in/search_sources/wiley.py` & `colrev-0.8.3/colrev/ops/built_in/search_sources/wiley.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/clone.py` & `colrev-0.8.3/colrev/ops/clone.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/commit.py` & `colrev-0.8.3/colrev/ops/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.colrev_version = f'version {version("colrev")}'
         sys_v = sys.version
         self.python_version = f'version {sys_v[: sys_v.find(" ")]}'
         stream = os.popen("git --version")
         self.git_version = stream.read().replace("git ", "").replace("\n", "")
         stream = os.popen("docker --version")
         self.docker_version = stream.read().replace("Docker ", "").replace("\n", "")
-        if "" == self.docker_version:
+        if self.docker_version == "":
             self.docker_version = "Not installed"
 
         self.ext_script_name = ""
         self.ext_script_version = ""
 
         if script_name != "":
             ext_script = script_name.split(" ")[0]
@@ -91,15 +91,15 @@
                         saved_args_str = saved_args_str + f"     --{key}={value} \\\n"
             # Replace the last backslash (for argument chaining across linebreaks)
             saved_args_str = saved_args_str.rstrip(" \\\n")
 
         return saved_args_str
 
     def __parse_script_name(self, *, script_name: str) -> str:
-        if "MANUAL" == script_name:
+        if script_name == "MANUAL":
             script_name = "Commit created manually or by external script"
         elif " " in script_name:
             script_name = script_name.replace("colrev cli", "colrev").replace(
                 "prescreen_cli", "prescreen"
             )
         return script_name
 
@@ -136,15 +136,15 @@
                 "[('change', 'booktitle',",
             ]
 
             with tempfile.NamedTemporaryFile(
                 dir=self.__temp_path, mode="r+b", delete=False
             ) as temp:
                 with open(self.review_manager.report_path, "r+b") as file:
-                    shutil.copyfileobj(file, temp)
+                    shutil.copyfileobj(file, temp)  # type: ignore
             # self.report_path.rename(temp.name)
             with open(temp.name, encoding="utf8") as reader, open(
                 self.review_manager.report_path, "w", encoding="utf8"
             ) as writer:
                 line = reader.readline()
                 while line:
                     if (
@@ -187,23 +187,24 @@
 
         report = self.__get_commit_report_header()
         report += status_operation.get_review_status_report(colors=False)
         report += self.__get_commit_report_details()
 
         return report
 
-    def create(self) -> bool:
+    def create(self, *, skip_status_yaml: bool = False) -> bool:
         """Create a commit (including the commit message and details)"""
 
         if self.review_manager.dataset.has_changes():
             self.review_manager.logger.debug("Prepare commit: checks and updates")
-            self.review_manager.update_status_yaml()
-            self.review_manager.dataset.add_changes(
-                path=self.review_manager.STATUS_RELATIVE
-            )
+            if not skip_status_yaml:
+                self.review_manager.update_status_yaml()
+                self.review_manager.dataset.add_changes(
+                    path=self.review_manager.STATUS_RELATIVE
+                )
 
             committer, email = self.review_manager.get_committer()
 
             if self.manual_author:
                 git_author = git.Actor(committer, email)
             else:
                 git_author = git.Actor(f"script:{self.script_name}", email)
```

### Comparing `colrev-0.8.2/colrev/ops/correct.py` & `colrev-0.8.3/colrev/ops/correct.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,32 +105,32 @@
         selected_change_items = []
         for change_item in list(changes):
             change_type, key, val = change_item
 
             if not isinstance(key, str):
                 continue
 
-            if "add" != change_type and "" == key:
+            if change_type != "add" and key == "":
                 continue
 
             if key.split(".")[0] in self.keys_to_ignore:
                 continue
 
-            if "add" == change_type:
+            if change_type == "add":
                 for add_item in val:
                     add_item_key, add_item_val = add_item
                     if not isinstance(add_item_key, str):
                         break
                     if add_item_key.split(".")[0] in self.keys_to_ignore:
                         break
                     selected_change_items.append(
                         ("add", "", [(add_item_key, add_item_val)])
                     )
 
-            elif "change" == change_type:
+            elif change_type == "change":
                 selected_change_items.append(change_item)
 
         if len(selected_change_items) == 0:
             return
 
         if len(corrected_record.get("colrev_origin", [])) > len(
             original_record.get("colrev_origin", [])
```

### Comparing `colrev-0.8.2/colrev/ops/data.py` & `colrev-0.8.3/colrev/ops/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     ) -> None:
         super().__init__(
             review_manager=review_manager,
             operations_type=colrev.operation.OperationsType.data,
             notify_state_transition_operation=notify_state_transition_operation,
         )
 
+        self.package_manager = self.review_manager.get_package_manager()
+
     def get_record_ids_for_synthesis(self, records: dict) -> list:
         """Get the IDs of records for the synthesis"""
         return [
             ID
             for ID, record in records.items()
             if record["colrev_status"]
             in [
@@ -221,48 +223,27 @@
         new_data_endpoint = {"endpoint": "custom_data_script"}
 
         self.review_manager.settings.data.data_package_endpoints.append(
             new_data_endpoint
         )
         self.review_manager.save_settings()
 
-    def main(
-        self,
-        *,
-        selection_list: Optional[list] = None,
-        records: Optional[dict] = None,
-        silent_mode: bool = False,
-    ) -> dict:
-        """Data operation (main entrypoint)
-
-        silent_mode: for review_manager checks
-        """
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
-
+    def __pre_data(self, *, records: dict, silent_mode: bool) -> None:
         if not silent_mode:
             self.review_manager.logger.info("Data")
             self.review_manager.logger.info(
                 "The data operation covers different forms of data extraction, "
                 "analysis, and synthesis."
             )
             self.review_manager.logger.info(
                 "See https://colrev.readthedocs.io/en/latest/manual/data/data.html"
             )
-
-        no_endpoints_registered = 0 == len(
-            self.review_manager.settings.data.data_package_endpoints
-        )
-
-        if not records:
-            records = self.review_manager.dataset.load_records_dict()
-
         self.__pad = min((max(len(ID) for ID in list(records.keys()) + [""]) + 2), 35)
 
+    def __get_synthesized_record_status_matrix(self, *, records: dict) -> dict:
         included = self.get_record_ids_for_synthesis(records)
 
         # TBD: do we assume that records are not changed by the processes?
         # records = self.review_manager.dataset.load_records_dict()
 
         # synthesized_record_status_matrix (paper IDs x endpoint):
         # each endpoint sets synthesized = True/False
@@ -273,61 +254,19 @@
             df["endpoint"]: False
             for df in self.review_manager.settings.data.data_package_endpoints
         }
         synthesized_record_status_matrix = {ID: default_row.copy() for ID in included}
 
         # if self.review_manager.verbose_mode:
         #     self.review_manager.p_printer.pprint(synthesized_record_status_matrix)
+        return synthesized_record_status_matrix
 
-        package_manager = self.review_manager.get_package_manager()
-
-        for (
-            data_package_endpoint
-        ) in self.review_manager.settings.data.data_package_endpoints:
-            if selection_list:
-                if not any(
-                    x in data_package_endpoint["endpoint"] for x in selection_list
-                ):
-                    continue
-
-            if not silent_mode:
-                print()
-                self.review_manager.logger.info(
-                    f"Data: {data_package_endpoint['endpoint'].replace('colrev.', '')}"
-                )
-
-            endpoint_dict = package_manager.load_packages(
-                package_type=colrev.env.package_manager.PackageEndpointType.data,
-                selected_packages=[data_package_endpoint],
-                operation=self,
-                only_ci_supported=self.review_manager.in_ci_environment(),
-            )
-
-            if data_package_endpoint["endpoint"] not in endpoint_dict:
-                self.review_manager.logger.info(
-                    f'Skip {data_package_endpoint["endpoint"]} (not available)'
-                )
-                continue
-
-            endpoint = endpoint_dict[data_package_endpoint["endpoint"]]
-
-            endpoint.update_data(  # type: ignore
-                self, records, synthesized_record_status_matrix, silent_mode=silent_mode
-            )
-
-            endpoint.update_record_status_matrix(  # type: ignore
-                self,
-                synthesized_record_status_matrix,
-                data_package_endpoint["endpoint"],
-            )
-
-            if self.review_manager.verbose_mode and not silent_mode:
-                msg = f"Updated {endpoint.settings.endpoint}"  # type: ignore
-                self.review_manager.logger.info(msg)
-
+    def __update_record_status_matrix(
+        self, *, records: dict, synthesized_record_status_matrix: dict
+    ) -> bool:
         records_changed = False
         for (
             record_id,
             individual_status_dict,
         ) in synthesized_record_status_matrix.items():
             if all(x for x in individual_status_dict.values()):
                 if (
@@ -357,33 +296,110 @@
                     colrev.record.RecordState.rev_included
                     != records[record_id]["colrev_status"]
                 ):
                     records[record_id].update(
                         colrev_status=colrev.record.RecordState.rev_included
                     )
                     records_changed = True
+        return records_changed
 
+    def __post_data(self, *, silent_mode: bool) -> None:
         # if self.review_manager.verbose_mode:
         #     self.review_manager.p_printer.pprint(synthesized_record_status_matrix)
 
         if self.review_manager.verbose_mode and not silent_mode:
             print()
 
-        if records_changed:
-            self.review_manager.dataset.save_records_dict(records=records)
-            self.review_manager.dataset.add_record_changes()
-
         if not silent_mode:
             self.review_manager.logger.info(
                 f"{colors.GREEN}Completed data operation{colors.END}"
             )
         if self.review_manager.in_ci_environment():
             print("\n\n")
 
+    def main(
+        self,
+        *,
+        selection_list: Optional[list] = None,
+        records: Optional[dict] = None,
+        silent_mode: bool = False,
+    ) -> dict:
+        """Data operation (main entrypoint)
+
+        silent_mode: for review_manager checks
+        """
+
+        if not records:
+            records = self.review_manager.dataset.load_records_dict()
+
+        self.__pre_data(records=records, silent_mode=silent_mode)
+
+        synthesized_record_status_matrix = self.__get_synthesized_record_status_matrix(
+            records=records
+        )
+
+        for (
+            data_package_endpoint
+        ) in self.review_manager.settings.data.data_package_endpoints:
+            if selection_list:
+                if not any(
+                    x in data_package_endpoint["endpoint"] for x in selection_list
+                ):
+                    continue
+
+            if not silent_mode:
+                print()
+                self.review_manager.logger.info(
+                    f"Data: {data_package_endpoint['endpoint'].replace('colrev.', '')}"
+                )
+
+            endpoint_dict = self.package_manager.load_packages(
+                package_type=colrev.env.package_manager.PackageEndpointType.data,
+                selected_packages=[data_package_endpoint],
+                operation=self,
+                only_ci_supported=self.review_manager.in_ci_environment(),
+            )
+
+            if data_package_endpoint["endpoint"] not in endpoint_dict:
+                self.review_manager.logger.info(
+                    f'Skip {data_package_endpoint["endpoint"]} (not available)'
+                )
+                continue
+
+            endpoint = endpoint_dict[data_package_endpoint["endpoint"]]
+
+            endpoint.update_data(  # type: ignore
+                self, records, synthesized_record_status_matrix, silent_mode=silent_mode
+            )
+
+            endpoint.update_record_status_matrix(  # type: ignore
+                self,
+                synthesized_record_status_matrix,
+                data_package_endpoint["endpoint"],
+            )
+
+            if self.review_manager.verbose_mode and not silent_mode:
+                msg = f"Updated {endpoint.settings.endpoint}"  # type: ignore
+                self.review_manager.logger.info(msg)
+
+        records_status_changed = self.__update_record_status_matrix(
+            records=records,
+            synthesized_record_status_matrix=synthesized_record_status_matrix,
+        )
+        if records_status_changed:
+            self.review_manager.dataset.save_records_dict(records=records)
+            self.review_manager.dataset.add_record_changes()
+
+        self.__post_data(silent_mode=silent_mode)
+
+        no_endpoints_registered = 0 == len(
+            self.review_manager.settings.data.data_package_endpoints
+        )
+
         return {
-            "ask_to_commit": True,
+            "ask_to_commit": self.review_manager.dataset.has_changes(),
             "no_endpoints_registered": no_endpoints_registered,
         }
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/dedupe.py` & `colrev-0.8.3/colrev/ops/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.review_manager
 
+# pylint: disable=too-many-lines
+
 
 class Dedupe(colrev.operation.Operation):
     """Deduplicate records (entity resolution)"""
 
     NON_DUPLICATE_FILE_XLSX = Path("non_duplicates_to_validate.xlsx")
     NON_DUPLICATE_FILE_TXT = Path("non_duplicates_to_validate.txt")
     DUPLICATES_TO_VALIDATE = Path("duplicates_to_validate.xlsx")
@@ -103,14 +105,15 @@
         ]
         for required_field in required_fields:
             if required_field not in records_df:
                 records_df[required_field] = ""
 
         records_df["year"] = records_df["year"].astype(str)
         if "colrev_status" in records_df:
+            # pylint: disable=direct-status-assign
             records_df["colrev_status"] = records_df["colrev_status"].astype(str)
 
         records_df["author"] = records_df["author"].str[:60]
 
         records_df.loc[
             records_df.ENTRYTYPE == "inbook", "container_title"
         ] = records_df.loc[records_df.ENTRYTYPE == "inbook", "title"]
@@ -411,14 +414,16 @@
         records: dict,
         duplicate_id_mappings: dict,
         removed_duplicates: list,
         complete_dedupe: bool,
         set_to_md_processed: list,
     ) -> None:
         for record_id, duplicate_ids in duplicate_id_mappings.items():
+            if record_id not in records:
+                continue
             if (
                 colrev.record.RecordState.md_prepared
                 == records[record_id]["colrev_status"]
             ):
                 if complete_dedupe:
                     self.review_manager.logger.info(
                         f" {colors.GREEN}{record_id} ({','.join(duplicate_ids)})".ljust(
@@ -579,18 +584,24 @@
             if removed_duplicate in records:
                 del records[removed_duplicate]
 
         set_to_md_processed = []
         if complete_dedupe:
             # Set remaining records to md_processed (not duplicate) because all records
             # have been considered by dedupe
-            for record in records.values():
-                if record["colrev_status"] == colrev.record.RecordState.md_prepared:
-                    record["colrev_status"] = colrev.record.RecordState.md_processed
-                    set_to_md_processed.append(record["ID"])
+            for record_dict in records.values():
+                if (
+                    record_dict["colrev_status"]
+                    == colrev.record.RecordState.md_prepared
+                ):
+                    record = colrev.record.Record(data=record_dict)
+                    record.set_status(
+                        target_state=colrev.record.RecordState.md_processed
+                    )
+                    set_to_md_processed.append(record.data["ID"])
 
         self.__print_merge_stats(
             records=records,
             duplicate_id_mappings=duplicate_id_mappings,
             removed_duplicates=removed_duplicates,
             complete_dedupe=complete_dedupe,
             set_to_md_processed=set_to_md_processed,
@@ -706,17 +717,18 @@
                         if record_dict["ID"] in id_list_to_unmerge:
                             # add manual_dedupe/non_dupe decision to the records
                             manual_non_duplicates = id_list_to_unmerge.copy()
                             manual_non_duplicates.remove(record_dict["ID"])
 
                             # The followin may need to be set to the previous state of the
                             # record that was erroneously merged (could be md_prepared)
-                            record_dict[
-                                "colrev_status"
-                            ] = colrev.record.RecordState.md_processed
+                            record = colrev.record.Record(data=record_dict)
+                            record.set_status(
+                                target_state=colrev.record.RecordState.md_processed
+                            )
                             records[record_dict["ID"]] = record_dict
                             self.review_manager.logger.info(
                                 f'Restored {record_dict["ID"]}'
                             )
                     unmerged = True
 
                 if unmerged:
@@ -998,19 +1010,23 @@
         self.review_manager.logger.info(
             f"{colors.GREEN}Completed dedupe operation{colors.END}"
         )
 
         if not self.review_manager.settings.prescreen.prescreen_package_endpoints:
             self.review_manager.logger.info("Skipping prescreen/including all records")
             records = self.review_manager.dataset.load_records_dict()
-            for record in records.values():
-                if colrev.record.RecordState.md_processed == record["colrev_status"]:
-                    record[
-                        "colrev_status"
-                    ] = colrev.record.RecordState.rev_prescreen_included
+            for record_dict in records.values():
+                record = colrev.record.Record(data=record_dict)
+                if (
+                    colrev.record.RecordState.md_processed
+                    == record.data["colrev_status"]
+                ):
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_prescreen_included
+                    )
 
             self.review_manager.dataset.save_records_dict(records=records)
             self.review_manager.dataset.add_record_changes()
             self.review_manager.create_commit(msg="Skip prescreen/include all")
 
         if self.review_manager.in_ci_environment():
             print("\n\n")
```

### Comparing `colrev-0.8.2/colrev/ops/distribute.py` & `colrev-0.8.3/colrev/ops/distribute.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/init.py` & `colrev-0.8.3/colrev/ops/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         with open("data/records.bib", mode="w", encoding="utf-8") as file:
             file.write("\n")
 
         git_repo = self.review_manager.dataset.get_repo()
         git_repo.git.add(all=True)
 
     def __post_commit_edits(self) -> None:
-        if "colrev.curated_masterdata" == self.review_type:
+        if self.review_type == "colrev.curated_masterdata":
             self.review_manager.logger.info("Post-commit edits")
             self.review_manager.settings.project.curation_url = "TODO"
             self.review_manager.settings.project.curated_fields = ["url", "doi", "TODO"]
 
             pdf_source_l = [
                 s
                 for s in self.review_manager.settings.sources
@@ -383,15 +383,15 @@
         ]
         for script_to_call in scripts_to_call:
             try:
                 if script_to_call["description"]:
                     self.logger.debug("%s...", script_to_call["description"])
                 check_call(script_to_call["command"], stdout=DEVNULL, stderr=STDOUT)
             except CalledProcessError:
-                if "pre-commit autoupdate" == " ".join(script_to_call["command"]):
+                if " ".join(script_to_call["command"]) == "pre-commit autoupdate":
                     pass
                 else:
                     self.logger.error(
                         "%sFailed: %s%s",
                         colors.RED,
                         " ".join(script_to_call),
                         colors.END,
```

### Comparing `colrev-0.8.2/colrev/ops/load.py` & `colrev-0.8.3/colrev/ops/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import html
 import itertools
 import re
 import string
 import typing
 from pathlib import Path
 
+import colrev.env.language_service
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.record
 import colrev.settings
 import colrev.ui_cli.cli_colors as colors
 
 # pylint: disable=too-many-lines
@@ -50,14 +51,15 @@
         super().__init__(
             review_manager=review_manager,
             operations_type=colrev.operation.OperationsType.load,
             notify_state_transition_operation=notify_state_transition_operation,
         )
 
         self.package_manager = self.review_manager.get_package_manager()
+        self.language_service = colrev.env.language_service.LanguageService()
 
         if not hide_load_explanation:
             self.review_manager.logger.info("Load")
             self.review_manager.logger.info(
                 "Load converts search results and adds them to the shared data/records.bib."
             )
             self.review_manager.logger.info(
@@ -340,15 +342,15 @@
                         selection = input("select nr")
                     if not selection.isdigit():
                         continue
                     if int(selection) in range(1, len(heuristic_result_list) + 1):
                         heuristic_source = heuristic_result_list[int(selection) - 1]
                         break
 
-            if "colrev.unknown_source" == heuristic_source["source_candidate"].endpoint:
+            if heuristic_source["source_candidate"].endpoint == "colrev.unknown_source":
                 cmd = "Enter the search query (or NA)".ljust(25, " ") + ": "
                 query_input = ""
                 if not skip_query:
                     query_input = input(cmd)
                 if query_input not in ["", "NA"]:
                     heuristic_source["source_candidate"].search_parameters = {
                         "query": query_input
@@ -365,15 +367,15 @@
             if (
                 {}
                 == heuristic_source["source_candidate"].load_conversion_package_endpoint
             ):
                 custom_load_conversion_package_endpoint = input(
                     "provide custom load_conversion_package_endpoint [or NA]:"
                 )
-                if "NA" == custom_load_conversion_package_endpoint:
+                if custom_load_conversion_package_endpoint == "NA":
                     heuristic_source[
                         "source_candidate"
                     ].load_conversion_package_endpoint = {}
                 else:
                     heuristic_source[
                         "source_candidate"
                     ].load_conversion_package_endpoint = {
@@ -585,118 +587,103 @@
                         key=defect_field, note="quality_defect"
                     )
 
         if not record.masterdata_is_curated():
             set_initial_import_provenance(record=record)
             set_initial_non_curated_import_provenance(record=record)
 
-    def __import_record(self, *, record_dict: dict) -> dict:
-        # pylint: disable=too-many-branches
-
-        self.review_manager.logger.debug(
-            f'import_record {record_dict["ID"]}: '
-            # f"\n{self.review_manager.p_printer.pformat(record_dict)}\n\n"
-        )
-
-        if colrev.record.RecordState.md_retrieved == record_dict["colrev_status"]:
-            # Consistently set keys to lower case
-            lower_keys = [k.lower() for k in list(record_dict.keys())]
-            for key, n_key in zip(list(record_dict.keys()), lower_keys):
-                if key in ["ID", "ENTRYTYPE"]:
-                    continue
-                record_dict[n_key] = record_dict.pop(key)
-
-            # pylint: disable=duplicate-code
-            # For better readability of the git diff:
-            fields_to_process = [
-                "author",
-                "year",
-                "title",
-                "journal",
-                "booktitle",
-                "series",
-                "volume",
-                "number",
-                "pages",
-                "doi",
-                "abstract",
-            ]
-
-            for field in fields_to_process:
-                if field in record_dict:
-                    if "\\" in record_dict[field]:
-                        record_dict[field] = self.__unescape_latex(
-                            input_str=record_dict[field]
-                        )
+    def __import_format_fields(self, *, record: colrev.record.Record) -> None:
+        # pylint: disable=duplicate-code
+        # For better readability of the git diff:
+        fields_to_process = [
+            "author",
+            "year",
+            "title",
+            "journal",
+            "booktitle",
+            "series",
+            "volume",
+            "number",
+            "pages",
+            "doi",
+            "abstract",
+        ]
 
-                    if "<" in record_dict[field]:
-                        record_dict[field] = self.__unescape_html(
-                            input_str=record_dict[field]
-                        )
+        for field in fields_to_process:
+            if field in record.data:
+                if "\\" in record.data[field]:
+                    record.data[field] = self.__unescape_latex(
+                        input_str=record.data[field]
+                    )
 
-                    record_dict[field] = (
-                        record_dict[field]
-                        .replace("\n", " ")
-                        .rstrip()
-                        .lstrip()
-                        .replace("{", "")
-                        .replace("}", "")
+                if "<" in record.data[field]:
+                    record.data[field] = self.__unescape_html(
+                        input_str=record.data[field]
                     )
 
-            if "UNKNOWN" != record_dict.get("title", "UNKNOWN"):
-                record_dict["title"] = (
-                    re.sub(r"\s+", " ", record_dict["title"])
-                    .lstrip()
+                record.data[field] = (
+                    record.data[field]
+                    .replace("\n", " ")
                     .rstrip()
-                    .rstrip(".")
+                    .lstrip()
+                    .replace("{", "")
+                    .replace("}", "")
                 )
+        if record.data.get("title", "UNKNOWN") != "UNKNOWN":
+            record.data["title"] = re.sub(r"\s+", " ", record.data["title"]).rstrip(".")
 
-            if "year" in record_dict:
-                if str(record_dict["year"]).endswith(".0"):
-                    record_dict["year"] = str(record_dict["year"])[:-2]
-
-            if "pages" in record_dict:
-                record_dict["pages"] = record_dict["pages"].replace("–", "--")
-                if record_dict["pages"].count("-") == 1:
-                    record_dict["pages"] = record_dict["pages"].replace("-", "--")
-                if "n.pag" == record_dict["pages"].lower():
-                    del record_dict["pages"]
-
-            if "number" not in record_dict and "issue" in record_dict:
-                record_dict.update(number=record_dict["issue"])
-                del record_dict["issue"]
-
-            if record_dict.get("volume", "") == "ahead-of-print":
-                del record_dict["volume"]
-            if record_dict.get("number", "") == "ahead-of-print":
-                del record_dict["number"]
-
-            if "language" in record_dict:
-                if len(record_dict["language"]) > 3:
-                    for long, short in [
-                        ("English", "eng"),
-                        ("Spanish", "esp"),
-                        ("Chinese", "zho"),
-                        ("Portuguese", "por"),
-                        ("German", "deu"),
-                        ("Hungarian", "hun"),
-                        ("French", "fra"),
-                        ("Russian", "rus"),
-                    ]:
-                        record_dict["language"] = record_dict["language"].replace(
-                            long, short
-                        )
+        if "year" in record.data:
+            if str(record.data["year"]).endswith(".0"):
+                record.data["year"] = str(record.data["year"])[:-2]
+
+        if "pages" in record.data:
+            record.data["pages"] = record.data["pages"].replace("–", "--")
+            if record.data["pages"].count("-") == 1:
+                record.data["pages"] = record.data["pages"].replace("-", "--")
+            if record.data["pages"].lower() == "n.pag":
+                del record.data["pages"]
+
+    def __import_process_fields(self, *, record: colrev.record.Record) -> None:
+        # Consistently set keys to lower case
+        lower_keys = [k.lower() for k in list(record.data.keys())]
+        for key, n_key in zip(list(record.data.keys()), lower_keys):
+            if key not in ["ID", "ENTRYTYPE"]:
+                record.data[n_key] = record.data.pop(key)
+
+        self.__import_format_fields(record=record)
+
+        if "number" not in record.data and "issue" in record.data:
+            record.data.update(number=record.data["issue"])
+            del record.data["issue"]
+
+        if record.data.get("volume", "") == "ahead-of-print":
+            del record.data["volume"]
+        if record.data.get("number", "") == "ahead-of-print":
+            del record.data["number"]
+
+        if "language" in record.data:
+            if len(record.data["language"]) != 3:
+                self.language_service.unify_to_iso_639_3_language_codes(record=record)
+
+        if "url" in record.data:
+            if "login?url=https" in record.data["url"]:
+                record.data["url"] = record.data["url"][
+                    record.data["url"].find("login?url=https") + 10 :
+                ]
 
-            if "url" in record_dict:
-                if "login?url=https" in record_dict["url"]:
-                    record_dict["url"] = record_dict["url"][
-                        record_dict["url"].find("login?url=https") + 10 :
-                    ]
+    def __import_record(self, *, record_dict: dict) -> dict:
+        self.review_manager.logger.debug(
+            f'import_record {record_dict["ID"]}: '
+            # f"\n{self.review_manager.p_printer.pformat(record_dict)}\n\n"
+        )
 
         record = colrev.record.Record(data=record_dict)
+        if record.data["colrev_status"] == colrev.record.RecordState.md_retrieved:
+            self.__import_process_fields(record=record)
+
         if "doi" in record.data:
             record.data.update(
                 doi=record.data["doi"].replace("http://dx.doi.org/", "").upper()
             )
 
         self.import_provenance(
             record=record,
@@ -716,15 +703,15 @@
     ) -> list:
         record_list = []
         origin_prefix = source.get_origin_prefix()
         for record in search_records:
             for key in colrev.record.Record.provenance_keys + [
                 "screening_criteria",
             ]:
-                if "colrev_status" == key:
+                if key == "colrev_status":
                     continue
                 if key in record:
                     del record[key]
 
             record.update(colrev_origin=[f"{origin_prefix}/{record['ID']}"])
 
             # Drop empty fields
```

### Comparing `colrev-0.8.2/colrev/ops/merge.py` & `colrev-0.8.3/colrev/ops/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,52 +183,54 @@
                 for r in current_branch_records.values()
                 if other_branch_records[r["ID"]]["colrev_status"] != r["colrev_status"]
             ]
         )
         i = 0
         for (
             current_branch_record_id,
-            current_branch_record,
+            current_branch_record_dict,
         ) in current_branch_records.items():
             other_branch_record = other_branch_records[current_branch_record_id]
 
             if (
-                current_branch_record["colrev_status"]
+                current_branch_record_dict["colrev_status"]
                 != other_branch_record["colrev_status"]
             ):
                 i += 1
                 print(f"{i}/{nr_to_reconcile}")
-                copied_rec = current_branch_record.copy()
+                copied_rec = current_branch_record_dict.copy()
                 copied_rec.pop("colrev_status")
                 print(colrev.record.Record(data=copied_rec).format_bib_style())
                 print(
                     f"1 - {current_branch_author} coded on {current_branch}".ljust(
                         40, " "
                     )
-                    + f": {current_branch_record['colrev_status']}"
+                    + f": {current_branch_record_dict['colrev_status']}"
                 )
                 print(
                     f"2 - {merging_branch_author} coded on {branch}".ljust(40, " ")
                     + f": {other_branch_record['colrev_status']}"
                 )
                 resolution_nr = input("Enter resolution: (1 or 2)")
-                if "1" == resolution_nr:
+                if resolution_nr == "1":
                     self.review_manager.report_logger.info(
                         f"Reconciliation for {current_branch_record_id}: "
-                        f"{current_branch_record['colrev_status']}"
+                        f"{current_branch_record_dict['colrev_status']}"
                     )
-                    resolution = current_branch_record["colrev_status"]
+                    resolution = current_branch_record_dict["colrev_status"]
                 else:
                     self.review_manager.report_logger.info(
                         f"Reconciliation for {current_branch_record_id}: "
                         f"{other_branch_record['colrev_status']}"
                     )
                     resolution = other_branch_record["colrev_status"]
-
-                current_branch_record["colrev_status"] = resolution
+                current_branch_record = colrev.record.Record(
+                    data=current_branch_record_dict
+                )
+                current_branch_record.set_status(target_state=resolution)
                 print("\n\n\n")
 
         self.review_manager.dataset.save_records_dict(records=current_branch_records)
 
         self.review_manager.update_status_yaml(add_to_git=False)
 
         validate_operation = self.review_manager.get_validate_operation()
```

### Comparing `colrev-0.8.2/colrev/ops/pdf_get.py` & `colrev-0.8.3/colrev/ops/pdf_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,20 +91,20 @@
                 record.set_status(target_state=colrev.record.RecordState.pdf_imported)
 
         return record
 
     def get_target_filepath(self, *, record: colrev.record.Record) -> Path:
         """Get the target filepath for a PDF"""
 
-        if "year" == self.filepath_directory_pattern:
+        if self.filepath_directory_pattern == "year":
             target_filepath = self.review_manager.PDF_DIR_RELATIVE / Path(
                 f"{record.data.get('year', 'no_year')}/{record.data['ID']}.pdf"
             )
 
-        elif "volume_number" == self.filepath_directory_pattern:
+        elif self.filepath_directory_pattern == "volume_number":
             if "volume" in record.data and "number" in record.data:
                 target_filepath = self.review_manager.PDF_DIR_RELATIVE / Path(
                     f"{record.data['volume']}/{record.data['number']}/{record.data['ID']}.pdf"
                 )
 
             if "volume" in record.data and "number" not in record.data:
                 target_filepath = self.review_manager.PDF_DIR_RELATIVE / Path(
@@ -221,15 +221,15 @@
     ) -> typing.Dict[str, typing.Dict]:
         # pylint: disable=too-many-branches
 
         # Relink files in source file
         corresponding_origin: str
         source_records: typing.List[typing.Dict] = []
         for source in self.review_manager.settings.sources:
-            if "colrev.pdfs_dir" != source.endpoint:
+            if source.endpoint != "colrev.pdfs_dir":
                 continue
 
             if not source.filename.is_file():
                 continue
 
             corresponding_origin = str(source.filename)
             with open(source.filename, encoding="utf8") as target_db:
@@ -238,17 +238,15 @@
                 )
             source_records = list(source_records_dict.values())
 
             self.review_manager.logger.info("Calculate colrev_pdf_ids")
             pdf_candidates = {
                 pdf_candidate.relative_to(
                     self.review_manager.path
-                ): colrev.record.Record.get_colrev_pdf_id(
-                    review_manager=self.review_manager, pdf_path=pdf_candidate
-                )
+                ): colrev.record.Record.get_colrev_pdf_id(pdf_path=pdf_candidate)
                 for pdf_candidate in list(self.review_manager.pdf_dir.glob("**/*.pdf"))
             }
 
             for record in records.values():
                 if "file" not in record:
                     continue
 
@@ -399,82 +397,96 @@
                 record = records[file.stem]
                 self.link_pdf(record=colrev.record.Record(data=record))
 
         self.review_manager.dataset.save_records_dict(records=records)
 
         return records
 
+    def __rename_pdf(
+        self,
+        *,
+        record_dict: dict,
+        file: Path,
+        new_filename: Path,
+        pdfs_search_file: Path,
+    ) -> None:
+        record_dict["file"] = new_filename
+
+        if "colrev_masterdata_provenance" in record_dict:
+            for value in record_dict["colrev_masterdata_provenance"].values():
+                if str(file) == value.get("source", ""):
+                    value["source"] = str(new_filename)
+
+        if "data_provenance" in record_dict:
+            for value in record_dict["data_provenance"].values():
+                if str(file) == value.get("source", ""):
+                    value["source"] = str(new_filename)
+
+        if pdfs_search_file.is_file():
+            colrev.env.utils.inplace_change(
+                filename=pdfs_search_file,
+                old_string="{" + str(file) + "}",
+                new_string="{" + str(new_filename) + "}",
+            )
+
+        if not file.is_file():
+            corrected_path = Path(str(file).replace("  ", " "))
+            if corrected_path.is_file():
+                file = corrected_path
+
+        if file.is_file():
+            file.rename(new_filename)
+        elif file.is_symlink():
+            os.rename(str(file), str(new_filename))
+
+        record_dict["file"] = str(new_filename)
+        self.review_manager.logger.info(f"rename {file.name} > {new_filename}")
+        if (
+            colrev.record.RecordState.rev_prescreen_included
+            == record_dict["colrev_status"]
+        ):
+            record = colrev.record.Record(data=record_dict)
+            record.set_status(target_state=colrev.record.RecordState.pdf_imported)
+
     def rename_pdfs(self) -> None:
         """Rename the PDFs"""
 
-        # pylint: disable=too-many-branches
-
         self.review_manager.logger.info("Rename PDFs")
 
         records = self.review_manager.dataset.load_records_dict()
 
         # We may use other pdfs_search_files from the sources:
         # review_manager.settings.sources
         pdfs_search_file = Path("data/search/pdfs.bib")
 
-        for record in records.values():
-            if "file" not in record:
+        for record_dict in records.values():
+            if "file" not in record_dict:
                 continue
-            if record[
+            if record_dict[
                 "colrev_status"
             ] not in colrev.record.RecordState.get_post_x_states(
                 state=colrev.record.RecordState.md_processed
             ):
                 continue
 
-            file = Path(record["file"])
-            new_filename = file.parents[0] / Path(f"{record['ID']}{file.suffix}")
+            file = Path(record_dict["file"])
+            new_filename = file.parents[0] / Path(f"{record_dict['ID']}{file.suffix}")
             # Possible option: move to top (pdfs) directory:
             # new_filename = self.review_manager.PDF_DIR_RELATIVE / Path(
             #     f"{record['ID']}.pdf"
             # )
             if str(file) == str(new_filename):
                 continue
 
-            record["file"] = new_filename
-
-            if "colrev_masterdata_provenance" in record:
-                for value in record["colrev_masterdata_provenance"].values():
-                    if str(file) == value.get("source", ""):
-                        value["source"] = str(new_filename)
-
-            if "data_provenance" in record:
-                for value in record["data_provenance"].values():
-                    if str(file) == value.get("source", ""):
-                        value["source"] = str(new_filename)
-
-            if pdfs_search_file.is_file():
-                colrev.env.utils.inplace_change(
-                    filename=pdfs_search_file,
-                    old_string="{" + str(file) + "}",
-                    new_string="{" + str(new_filename) + "}",
-                )
-
-            if not file.is_file():
-                corrected_path = Path(str(file).replace("  ", " "))
-                if corrected_path.is_file():
-                    file = corrected_path
-
-            if file.is_file():
-                file.rename(new_filename)
-            elif file.is_symlink():
-                os.rename(str(file), str(new_filename))
-
-            record["file"] = str(new_filename)
-            self.review_manager.logger.info(f"rename {file.name} > {new_filename}")
-            if (
-                colrev.record.RecordState.rev_prescreen_included
-                == record["colrev_status"]
-            ):
-                record["colrev_status"] = colrev.record.RecordState.pdf_imported
+            self.__rename_pdf(
+                record_dict=record_dict,
+                file=file,
+                new_filename=new_filename,
+                pdfs_search_file=pdfs_search_file,
+            )
 
         self.review_manager.dataset.save_records_dict(records=records)
 
         if pdfs_search_file.is_file():
             self.review_manager.dataset.add_changes(path=pdfs_search_file)
         self.review_manager.dataset.add_record_changes()
 
@@ -541,36 +553,38 @@
             not_retrieved_string += f"{self.not_retrieved}".rjust(6, " ")
             not_retrieved_string += f"{colors.END} PDFs"
 
         self.review_manager.logger.info(retrieved_string)
         self.review_manager.logger.info(not_retrieved_string)
 
     def __set_status_if_file_linked(self, *, records: dict) -> dict:
-        for record in records.values():
-            if record["colrev_status"] in [
+        for record_dict in records.values():
+            if record_dict["colrev_status"] in [
                 colrev.record.RecordState.rev_prescreen_included,
                 colrev.record.RecordState.pdf_needs_manual_retrieval,
             ]:
-                if "file" in record:
+                record = colrev.record.Record(data=record_dict)
+                if "file" in record_dict:
                     if any(
-                        Path(fpath).is_file() for fpath in record["file"].split(";")
+                        Path(fpath).is_file()
+                        for fpath in record.data["file"].split(";")
                     ):
                         if (
                             colrev.record.RecordState.rev_prescreen_included
-                            == record["colrev_status"]
+                            == record.data["colrev_status"]
                         ):
-                            record[
-                                "colrev_status"
-                            ] = colrev.record.RecordState.pdf_imported
+                            record.set_status(
+                                target_state=colrev.record.RecordState.pdf_imported
+                            )
                     else:
                         self.review_manager.logger.warning(
                             "Remove non-existent file link "
-                            f'({record["ID"]}: {record["file"]}'
+                            f'({record_dict["ID"]}: {record_dict["file"]}'
                         )
-                        colrev.record.Record(data=record).remove_field(key="file")
+                        record.remove_field(key="file")
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
 
         return records
 
     def setup_custom_script(self) -> None:
         """Setup a custom pfd-get script"""
```

### Comparing `colrev-0.8.2/colrev/ops/pdf_get_man.py` & `colrev-0.8.3/colrev/ops/pdf_get_man.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,23 @@
                 f"Created {self.missing_pdf_files_csv} with paper details"
             )
 
     def discard(self) -> None:
         """Discard missing PDFs (set to pdf_not_available)"""
 
         records = self.review_manager.dataset.load_records_dict()
-        for record in records.values():
+        for record_dict in records.values():
+            record = colrev.record.Record(data=record_dict)
             if (
-                record["colrev_status"]
+                record.data["colrev_status"]
                 == colrev.record.RecordState.pdf_needs_manual_retrieval
             ):
-                record["colrev_status"] = colrev.record.RecordState.pdf_not_available
+                record.set_status(
+                    target_state=colrev.record.RecordState.pdf_not_available
+                )
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg="Discard missing PDFs", manual_author=True
         )
 
     def get_data(self) -> dict:
```

### Comparing `colrev-0.8.2/colrev/ops/pdf_prep.py` & `colrev-0.8.3/colrev/ops/pdf_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,15 @@
         self, *, record: colrev.record.Record, original_filename: str
     ) -> None:
         record.data.update(colrev_status=colrev.record.RecordState.pdf_prepared)
         pdf_path = self.review_manager.path / Path(record.data["file"])
         if pdf_path.suffix == ".pdf":
             try:
                 record.data.update(
-                    colrev_pdf_id=record.get_colrev_pdf_id(
-                        review_manager=self.review_manager, pdf_path=pdf_path
-                    )
+                    colrev_pdf_id=record.get_colrev_pdf_id(pdf_path=pdf_path)
                 )
             except colrev_exceptions.ServiceNotAvailableException:
                 self.review_manager.logger.error(
                     "Cannot create pdf-hash (Docker service not available)"
                 )
 
         # colrev_status == pdf_imported : means successful
@@ -169,17 +167,17 @@
                 colrev_exceptions.TEIException,
                 requests.exceptions.ReadTimeout,
             ) as err:
                 self.review_manager.logger.error(
                     f'Error for {record.data["ID"]} '  # type: ignore
                     f"(in {endpoint.settings.endpoint} : {err})"  # type: ignore
                 )
-                record.data[
-                    "colrev_status"
-                ] = colrev.record.RecordState.pdf_needs_manual_preparation
+                record.set_status(
+                    target_state=colrev.record.RecordState.pdf_needs_manual_preparation
+                )
 
             failed = (
                 colrev.record.RecordState.pdf_needs_manual_preparation
                 == record.data["colrev_status"]
             )
 
             if failed:
@@ -270,17 +268,15 @@
         self.review_manager.dataset.save_records_dict(records=records)
 
     # Note : no named arguments (multiprocessing)
     def __update_colrev_pdf_ids(self, record_dict: dict) -> dict:
         if "file" in record_dict:
             pdf_path = self.review_manager.path / Path(record_dict["file"])
             record_dict.update(
-                colrev_pdf_id=colrev.record.Record(data=record_dict).get_colrev_pdf_id(
-                    review_manager=self.review_manager, pdf_path=pdf_path
-                )
+                colrev_pdf_id=colrev.record.Record.get_colrev_pdf_id(pdf_path=pdf_path)
             )
         return record_dict
 
     def update_colrev_pdf_ids(self) -> None:
         """Update the colrev-pdf-ids"""
         self.review_manager.logger.info("Update colrev_pdf_ids")
         records = self.review_manager.dataset.load_records_dict()
```

### Comparing `colrev-0.8.2/colrev/ops/pdf_prep_man.py` & `colrev-0.8.3/colrev/ops/pdf_prep_man.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,23 @@
 
         self.verbose = True
 
     def discard(self) -> None:
         """Discard records whose PDFs need manual preparation (set to pdf_not_available)"""
 
         records = self.review_manager.dataset.load_records_dict()
-        for record in records.values():
+        for record_dict in records.values():
             if (
-                record["colrev_status"]
+                record_dict["colrev_status"]
                 == colrev.record.RecordState.pdf_needs_manual_preparation
             ):
-                record["colrev_status"] = colrev.record.RecordState.pdf_not_available
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(
+                    target_state=colrev.record.RecordState.pdf_not_available
+                )
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg="Discard man-prep PDFs", manual_author=True
         )
 
     def get_data(self) -> dict:
@@ -304,19 +307,15 @@
         """Set the PDF to manually prepared"""
 
         record.set_status(target_state=colrev.record.RecordState.pdf_prepared)
         record.reset_pdf_provenance_notes()
 
         pdf_path = Path(self.review_manager.path / Path(record.data["file"]))
         prev_cpid = record.data.get("colrev_pdf_id", "NA")
-        record.data.update(
-            colrev_pdf_id=record.get_colrev_pdf_id(
-                review_manager=self.review_manager, pdf_path=pdf_path
-            )
-        )
+        record.data.update(colrev_pdf_id=record.get_colrev_pdf_id(pdf_path=pdf_path))
         if prev_cpid != record.data.get("colrev_pdf_id", "NA"):
             record.add_data_provenance(key="file", source="manual")
 
         record_dict = record.get_data()
         self.review_manager.dataset.save_records_dict(
             records={record_dict["ID"]: record_dict}, partial=True
         )
```

### Comparing `colrev-0.8.2/colrev/ops/prep.py` & `colrev-0.8.3/colrev/ops/prep.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 class Prep(colrev.operation.Operation):
     """Prepare records (metadata)"""
 
     # pylint: disable=too-many-instance-attributes
 
-    timeout = 10
+    timeout = 30
     max_retries_on_error = 3
 
     retrieval_similarity: float
 
     first_round: bool
     last_round: bool
 
@@ -107,14 +107,17 @@
         "issn",
         "language",
         "howpublished",
         "cited_by",
         "cited_by_file",
     ]
 
+    __cpu = 1
+    __prep_commit_id = "HEAD"
+
     def __init__(
         self,
         *,
         review_manager: colrev.review_manager.ReviewManager,
         notify_state_transition_operation: bool = True,
         retrieval_similarity: float = 1.0,
     ) -> None:
@@ -211,170 +214,206 @@
                 f"{prep_package_endpoint}"
                 f' on {preparation_record.data["ID"]}'
                 " changed: -"
             )
             print("\n")
             time.sleep(0.1)
 
-    # Note : no named arguments for multiprocessing
-    def prepare(self, item: dict) -> dict:
-        """Prepare a record (based on package_endpoints in the settings)"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-
-        record: colrev.record.PrepRecord = item["record"]
+    def __package_prep(
+        self,
+        prep_round_package_endpoint: dict,
+        record: colrev.record.PrepRecord,
+        preparation_record: colrev.record.PrepRecord,
+    ) -> None:
+        try:
+            if (
+                prep_round_package_endpoint["endpoint"].lower()
+                not in self.prep_package_endpoints
+            ):
+                return
+            endpoint = self.prep_package_endpoints[
+                prep_round_package_endpoint["endpoint"].lower()
+            ]
 
-        if not record.status_to_prepare() and not self.polish:
-            return record.get_data()
+            if self.debug_mode:
+                self.review_manager.logger.info(
+                    f"{endpoint.settings.endpoint}(...) called"
+                )
 
-        if self.review_manager.verbose_mode:
-            self.review_manager.logger.info(" prep " + record.data["ID"])
+            prior = preparation_record.copy_prep_rec()
 
-        # preparation_record changes with each endpoint and
-        # eventually replaces record (if md_prepared or endpoint.always_apply_changes)
-        preparation_record = record.copy_prep_rec()
-        prior_state = record.data["colrev_status"]
+            start_time = datetime.now()
+            preparation_record = endpoint.prepare(self, preparation_record)
+            self.__add_stats(
+                start_time=start_time,
+                prep_round_package_endpoint=prep_round_package_endpoint,
+            )
 
-        for prep_round_package_endpoint in deepcopy(
-            item["prep_round_package_endpoints"]
-        ):
-            try:
-                if (
-                    prep_round_package_endpoint["endpoint"].lower()
-                    not in self.prep_package_endpoints
-                ):
-                    continue
-                endpoint = self.prep_package_endpoints[
-                    prep_round_package_endpoint["endpoint"].lower()
-                ]
+            self.__print_diffs_for_debug(
+                prior=prior,
+                preparation_record=preparation_record,
+                prep_package_endpoint=endpoint,
+            )
 
-                if self.debug_mode:
-                    self.review_manager.logger.info(
-                        f"{endpoint.settings.endpoint}(...) called"
-                    )
+            if endpoint.always_apply_changes:
+                record.update_by_record(update_record=preparation_record)
 
-                prior = preparation_record.copy_prep_rec()
+            if preparation_record.preparation_save_condition():
+                record.update_by_record(update_record=preparation_record)
+                if not self.polish:
+                    record.update_masterdata_provenance()
 
-                start_time = datetime.now()
-                preparation_record = endpoint.prepare(self, preparation_record)
-                self.__add_stats(
-                    start_time=start_time,
-                    prep_round_package_endpoint=prep_round_package_endpoint,
+            if preparation_record.preparation_break_condition() and not self.polish:
+                record.update_by_record(update_record=preparation_record)
+                raise colrev_exceptions.PreparationBreak
+        except (timeout_decorator.timeout_decorator.TimeoutError, ReadTimeout):
+            self.__add_stats(
+                start_time=start_time,
+                prep_round_package_endpoint=prep_round_package_endpoint,
+            )
+            if self.review_manager.verbose_mode:
+                self.review_manager.logger.error(
+                    f" {colors.RED}{record.data['ID']}".ljust(45)
+                    + f"{endpoint.settings.endpoint}(...) timed out{colors.END}{colors.END}"
                 )
 
-                self.__print_diffs_for_debug(
-                    prior=prior,
-                    preparation_record=preparation_record,
-                    prep_package_endpoint=endpoint,
-                )
-
-                if endpoint.always_apply_changes:
-                    record.update_by_record(update_record=preparation_record)
-
-                if preparation_record.preparation_save_condition():
-                    record.update_by_record(update_record=preparation_record)
-                    if not self.polish:
-                        record.update_masterdata_provenance()
-
-                if preparation_record.preparation_break_condition() and not self.polish:
-                    record.update_by_record(update_record=preparation_record)
-                    break
-            except (timeout_decorator.timeout_decorator.TimeoutError, ReadTimeout):
+        except colrev_exceptions.ServiceNotAvailableException as exc:
+            if self.review_manager.force_mode:
                 self.__add_stats(
                     start_time=start_time,
                     prep_round_package_endpoint=prep_round_package_endpoint,
                 )
-                if self.review_manager.verbose_mode:
-                    self.review_manager.logger.error(
-                        f" {colors.RED}{record.data['ID']}".ljust(45)
-                        + f"{endpoint.settings.endpoint}(...) timed out{colors.END}{colors.END}"
-                    )
-
-            except colrev_exceptions.ServiceNotAvailableException as exc:
-                if self.review_manager.force_mode:
-                    self.__add_stats(
-                        start_time=start_time,
-                        prep_round_package_endpoint=prep_round_package_endpoint,
-                    )
-                    self.review_manager.logger.error(exc)
-                else:
-                    raise exc
+                self.review_manager.logger.error(exc)
+            else:
+                raise exc
 
-        if not self.review_manager.verbose_mode:
-            # pylint: disable=redefined-outer-name,invalid-name
-            with PREP_COUNTER.get_lock():
-                PREP_COUNTER.value += 1  # type: ignore
-            progress = ""
-            if item["nr_items"] > 100:
-                progress = f"({PREP_COUNTER.value}/{item['nr_items']}) ".rjust(  # type: ignore
-                    12, " "
-                )
+    def __print_post_package_prep_info(
+        self,
+        record: colrev.record.PrepRecord,
+        item: dict,
+        prior_state: colrev.record.RecordState,
+    ) -> None:
+        # pylint: disable=redefined-outer-name,invalid-name
+        with PREP_COUNTER.get_lock():
+            PREP_COUNTER.value += 1  # type: ignore
+        progress = ""
+        if item["nr_items"] > 100:
+            progress = f"({PREP_COUNTER.value}/{item['nr_items']}) ".rjust(  # type: ignore
+                12, " "
+            )
 
-            if record.preparation_break_condition():
-                if (
-                    colrev.record.RecordState.rev_prescreen_excluded
-                    == record.data["colrev_status"]
-                ):
-                    if self.review_manager.verbose_mode:
-                        self.review_manager.logger.info(
-                            f" {colors.RED}{record.data['ID']}".ljust(46)
-                            + f"Detected: {record.data.get('prescreen_exclusion', 'NA')}"
-                            + f"{colors.END}"
-                        )
-                    target_state = "rev_prescreen_excluded"
-                    if self.polish:
-                        target_state = prior_state
+        if record.preparation_break_condition():
+            if (
+                colrev.record.RecordState.rev_prescreen_excluded
+                == record.data["colrev_status"]
+            ):
+                if self.review_manager.verbose_mode:
                     self.review_manager.logger.info(
                         f" {colors.RED}{record.data['ID']}".ljust(46)
-                        + f"{progress}{prior_state} →  {target_state}"
+                        + f"Detected: {record.data.get('prescreen_exclusion', 'NA')}"
                         + f"{colors.END}"
                     )
-                else:
-                    target_state = "md_needs_manual_preparation"
-                    if self.polish:
-                        target_state = prior_state
-                    self.review_manager.logger.info(
-                        f" {colors.ORANGE}{record.data['ID']}".ljust(46)
-                        + f"{progress}{prior_state} →  {target_state}{colors.END}"
-                    )
-
-            elif record.preparation_save_condition():
-                curation_addition = "   "
-                if record.masterdata_is_curated():
-                    curation_addition = " ✔ "
-                target_state = "md_prepared"
+                target_state = colrev.record.RecordState.rev_prescreen_excluded
                 if self.polish:
                     target_state = prior_state
                 self.review_manager.logger.info(
-                    f" {colors.GREEN}{record.data['ID']}".ljust(46)
-                    + f"{progress}{prior_state} →  {target_state}{colors.END}{curation_addition}"
+                    f" {colors.RED}{record.data['ID']}".ljust(46)
+                    + f"{progress}{prior_state} →  {target_state}"
+                    + f"{colors.END}"
                 )
             else:
-                target_state = "md_needs_manual_preparation"
+                target_state = colrev.record.RecordState.md_needs_manual_preparation
                 if self.polish:
                     target_state = prior_state
                 self.review_manager.logger.info(
                     f" {colors.ORANGE}{record.data['ID']}".ljust(46)
                     + f"{progress}{prior_state} →  {target_state}{colors.END}"
                 )
 
+        elif record.preparation_save_condition():
+            curation_addition = "   "
+            if record.masterdata_is_curated():
+                curation_addition = " ✔ "
+            target_state = colrev.record.RecordState.md_prepared
+            if self.polish:
+                target_state = prior_state
+            self.review_manager.logger.info(
+                f" {colors.GREEN}{record.data['ID']}".ljust(46)
+                + f"{progress}{prior_state} →  {target_state}{colors.END}{curation_addition}"
+            )
+        else:
+            target_state = colrev.record.RecordState.md_needs_manual_preparation
+            if self.polish:
+                target_state = prior_state
+            self.review_manager.logger.info(
+                f" {colors.ORANGE}{record.data['ID']}".ljust(46)
+                + f"{progress}{prior_state} →  {target_state}{colors.END}"
+            )
+
+    def __post_package_prep(
+        self,
+        record: colrev.record.PrepRecord,
+        preparation_record: colrev.record.PrepRecord,
+        item: dict,
+        prior_state: colrev.record.RecordState,
+    ) -> None:
+        if not self.review_manager.verbose_mode:
+            self.__print_post_package_prep_info(
+                record=record, item=item, prior_state=prior_state
+            )
+
         if self.last_round and not self.polish:
             if record.status_to_prepare():
                 for key in list(record.data.keys()):
                     if key not in self.fields_to_keep:
                         record.remove_field(key=key)
                     elif record.data[key] in ["", "NA"]:
                         record.remove_field(key=key)
                 record.update_by_record(update_record=preparation_record)
                 # Note: update_masterdata_provenance sets to md_needs_manual_preparation
                 record.update_masterdata_provenance()
 
         if self.polish:
-            record.data["colrev_status"] = prior_state
+            record.set_status(target_state=prior_state)
+
+    # Note : no named arguments for multiprocessing
+    def prepare(self, item: dict) -> dict:
+        """Prepare a record (based on package_endpoints in the settings)"""
+
+        record: colrev.record.PrepRecord = item["record"]
+
+        if not record.status_to_prepare() and not self.polish:
+            return record.get_data()
+
+        if self.review_manager.verbose_mode:
+            self.review_manager.logger.info(" prep " + record.data["ID"])
+
+        # preparation_record changes with each endpoint and
+        # eventually replaces record (if md_prepared or endpoint.always_apply_changes)
+        preparation_record = record.copy_prep_rec()
+        prior_state = record.data["colrev_status"]
+
+        for prep_round_package_endpoint in deepcopy(
+            item["prep_round_package_endpoints"]
+        ):
+            try:
+                self.__package_prep(
+                    prep_round_package_endpoint,
+                    record,
+                    preparation_record,
+                )
+            except colrev_exceptions.PreparationBreak:
+                break
+
+        self.__post_package_prep(
+            record=record,
+            preparation_record=preparation_record,
+            item=item,
+            prior_state=prior_state,
+        )
 
         return record.get_data()
 
     def __select_record_list_for_reset(self, *, record_list: list[dict]) -> list[dict]:
         record_list = [
             rec
             for rec in record_list
@@ -617,15 +656,14 @@
 
     def __get_preparation_data(
         self,
         *,
         prep_round: colrev.settings.PrepRound,
         debug_file: Optional[Path] = None,
         debug_ids: str,
-        max_n: int = 2500,
         polish: bool = False,
     ) -> list:
         if self.debug_mode:
             prepare_data = self.__load_prep_data_for_debug(
                 debug_ids=debug_ids, debug_file=debug_file
             )
             if prepare_data["nr_tasks"] == 0:
@@ -695,20 +733,25 @@
     ) -> dict:
         if debug_file:
             with open(debug_file, encoding="utf8") as target_db:
                 records_dict = self.review_manager.dataset.load_records_dict(
                     load_str=target_db.read()
                 )
 
-            for record in records_dict.values():
-                if colrev.record.RecordState.md_imported != record.get("state", ""):
+            for record_dict in records_dict.values():
+                if colrev.record.RecordState.md_imported != record_dict.get(
+                    "state", ""
+                ):
                     self.review_manager.logger.info(
-                        f"Setting colrev_status to md_imported {record['ID']}"
+                        f"Setting colrev_status to md_imported {record_dict['ID']}"
+                    )
+                    record = colrev.record.Record(data=record_dict)
+                    record.set_status(
+                        target_state=colrev.record.RecordState.md_imported
                     )
-                    record["colrev_status"] = colrev.record.RecordState.md_imported
             debug_ids_list = list(records_dict.keys())
             debug_ids = ",".join(debug_ids_list)
             self.review_manager.logger.info("Imported record (retrieved from file)")
 
         else:
             records = []
             debug_ids_list = debug_ids.split(",")
@@ -822,36 +865,36 @@
                 )
 
     def __log_details(self, *, prepared_records: list) -> None:
         nr_recs = len(
             [
                 record
                 for record in prepared_records
-                if record["colrev_status"] == colrev.record.RecordState.md_prepared
+                if "CURATED" in record["colrev_masterdata_provenance"]
             ]
         )
 
         self.review_manager.logger.info(
-            "Overall md_prepared".ljust(29)
+            "Overall curated (✔)".ljust(29)
             + f"{colors.GREEN}{nr_recs}{colors.END}".rjust(20, " ")
             + " records"
         )
 
         nr_recs = len(
             [
                 record
                 for record in prepared_records
-                if "CURATED" in record["colrev_masterdata_provenance"]
+                if record["colrev_status"] == colrev.record.RecordState.md_prepared
             ]
         )
 
         self.review_manager.logger.info(
-            "Overall curated".ljust(29)
+            "Overall md_prepared".ljust(29)
             + f"{colors.GREEN}{nr_recs}{colors.END}".rjust(20, " ")
-            + " records ( ✔ quality-assured by CoLRev community curators)"
+            + " records"
         )
 
         nr_recs = len(
             [
                 record
                 for record in prepared_records
                 if record["colrev_status"]
@@ -880,35 +923,23 @@
             )
 
     def skip_prep(self) -> None:
         """Skip the preparation"""
 
         records = self.review_manager.dataset.load_records_dict()
 
-        for record in records.values():
-            if colrev.record.RecordState.md_imported == record["colrev_status"]:
-                record["colrev_status"] = colrev.record.RecordState.md_prepared
+        for record_dict in records.values():
+            if colrev.record.RecordState.md_imported == record_dict["colrev_status"]:
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(target_state=colrev.record.RecordState.md_prepared)
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(msg="Skip prep")
 
-    def main(
-        self,
-        *,
-        keep_ids: bool = False,
-        debug_ids: str = "NA",
-        debug_file: Optional[Path] = None,
-        cpu: int = 4,
-        polish: bool = False,
-    ) -> None:
-        """Preparation of records (main entrypoint)"""
-
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+    def __initialize_prep(self, *, polish: bool, debug_ids: str, cpu: int) -> None:
         if not polish:
             self.review_manager.logger.info("Prep")
         else:
             self.review_manager.logger.info("Prep (polish mode)")
         self.review_manager.logger.info(
             "Prep completes and corrects record metadata based on APIs and preparation rules."
         )
@@ -917,33 +948,119 @@
             self.review_manager.logger.info(
                 "Polish mode: consider all records but prevent state transitions."
             )
         self.review_manager.logger.info(
             "See https://colrev.readthedocs.io/en/latest/manual/metadata_retrieval/prep.html"
         )
 
-        # Note: for unit testing, we use a simple loop (instead of parallel)
-        # to ensure that the IDs of feed records don't change
-        __unit_testing = "test_prep" == inspect.stack()[1][3]
-
         if self.debug_mode:
             print("\n\n\n")
             self.review_manager.logger.info("Start debug prep\n")
             self.review_manager.logger.info(
                 "The debugger will replay the preparation procedures"
                 " step-by-step, allow you to identify potential errors, trace them to "
                 "their colrev_origin and correct them."
             )
             input("\nPress Enter to continue")
             print("\n\n")
 
-        if "NA" != debug_ids:
+        if debug_ids != "NA":
             self.debug_mode = True
 
-        prep_commit_id = "HEAD"
+        self.__cpu = cpu
+
+        # Note: for unit testing, we use a simple loop (instead of parallel)
+        # to ensure that the IDs of feed records don't change
+        unit_testing = "test_prep" == inspect.stack()[1][3]
+        if unit_testing or self.debug_mode:
+            self.__cpu = 1
+
+    def __prep_packages_ram_heavy(self, prep_round: colrev.settings.PrepRound) -> bool:
+        prep_pe_names = [r["endpoint"] for r in prep_round.prep_package_endpoints]
+        ram_reavy = "colrev.exclude_languages" in prep_pe_names  # type: ignore
+        self.review_manager.logger.info(
+            "Info: The language detector requires RAM and may take longer"
+        )
+        return ram_reavy
+
+    def __get_prep_pool(
+        self, *, prep_round: colrev.settings.PrepRound
+    ) -> mp.pool.ThreadPool:
+        if self.__prep_packages_ram_heavy(prep_round=prep_round):
+            pool = Pool(mp.cpu_count() // 2)
+        else:
+            # Note : if we use too many CPUS,
+            # a "too many open files" exception is thrown
+            pool = Pool(self.__cpu)
+        self.review_manager.logger.info(
+            "Info: ✔ = quality-assured by CoLRev community curators"
+        )
+        return pool
+
+    def __create_prep_commit(
+        self,
+        *,
+        previous_preparation_data: list,
+        prepared_records: list,
+        prep_round: colrev.settings.PrepRound,
+    ) -> None:
+        self.__log_record_change_scores(
+            preparation_data=previous_preparation_data,
+            prepared_records=prepared_records,
+        )
+
+        if not self.debug_mode:
+            self.review_manager.dataset.save_records_dict(
+                records={r["ID"]: r for r in prepared_records}, partial=True
+            )
+
+            self.__log_details(prepared_records=prepared_records)
+
+            self.review_manager.create_commit(
+                msg=f"Prepare records ({prep_round.name})",
+            )
+            self.__prep_commit_id = (
+                self.review_manager.dataset.get_repo().head.commit.hexsha
+            )
+            if not self.review_manager.high_level_operation:
+                print()
+        self.review_manager.reset_report_logger()
+
+        self.__print_stats()
+
+    def __post_prep(self) -> None:
+        if not self.review_manager.high_level_operation:
+            print()
+
+        self.review_manager.logger.info("To validate the changes, use")
+
+        self.review_manager.logger.info(
+            f"{colors.ORANGE}colrev validate {self.__prep_commit_id}{colors.END}"
+        )
+        if not self.review_manager.high_level_operation:
+            print()
+
+        self.review_manager.logger.info(
+            f"{colors.GREEN}Completed prep operation{colors.END}"
+        )
+        if self.review_manager.in_ci_environment():
+            print("\n\n")
+
+    def main(
+        self,
+        *,
+        keep_ids: bool = False,
+        debug_ids: str = "NA",
+        debug_file: Optional[Path] = None,
+        cpu: int = 4,
+        polish: bool = False,
+    ) -> None:
+        """Preparation of records (main entrypoint)"""
+
+        self.__initialize_prep(polish=polish, debug_ids=debug_ids, cpu=cpu)
 
         try:
             for i, prep_round in enumerate(
                 self.review_manager.settings.prep.prep_rounds
             ):
                 self.__setup_prep_round(i=i, prep_round=prep_round)
 
@@ -956,61 +1073,32 @@
                 previous_preparation_data = deepcopy(preparation_data)
 
                 if len(preparation_data) == 0:
                     self.review_manager.logger.info("No records to prepare.")
                     print()
                     return
 
-                if self.debug_mode or __unit_testing:
+                if self.__cpu == 1:
                     # Note: preparation_data is not turned into a list of records.
                     prepared_records = []
                     for item in preparation_data:
                         record = self.prepare(item)
                         prepared_records.append(record)
                 else:
-                    prep_pe_names = [
-                        r["endpoint"] for r in prep_round.prep_package_endpoints
-                    ]
-                    if "colrev.exclude_languages" in prep_pe_names:  # type: ignore
-                        self.review_manager.logger.info(
-                            "Info: The language detector requires RAM and may take longer"
-                        )
-                        pool = Pool(mp.cpu_count() // 2)
-                    else:
-                        # Note : if we use too many CPUS,
-                        # a "too many open files" exception is thrown
-                        pool = Pool(cpu)
+                    pool = self.__get_prep_pool(prep_round=prep_round)
                     prepared_records = pool.map(self.prepare, preparation_data)
                     pool.close()
                     pool.join()
 
-                self.__log_record_change_scores(
-                    preparation_data=previous_preparation_data,
+                self.__create_prep_commit(
+                    previous_preparation_data=previous_preparation_data,
                     prepared_records=prepared_records,
+                    prep_round=prep_round,
                 )
 
-                if not self.debug_mode:
-                    self.review_manager.dataset.save_records_dict(
-                        records={r["ID"]: r for r in prepared_records}, partial=True
-                    )
-
-                    self.__log_details(prepared_records=prepared_records)
-
-                    self.review_manager.create_commit(
-                        msg=f"Prepare records ({prep_round.name})",
-                    )
-                    prep_commit_id = (
-                        self.review_manager.dataset.get_repo().head.commit.hexsha
-                    )
-                    if not self.review_manager.high_level_operation:
-                        print()
-                self.review_manager.reset_report_logger()
-
-                self.__print_stats()
-
         except requests_ConnectionError as exc:
             if "OSError(24, 'Too many open files" in str(exc):
                 raise colrev_exceptions.ServiceNotAvailableException(
                     "Too many files opened (OSError, Errno24). "
                     "To use a smaller number of parallel processes, run colrev prep --cpu 1"
                 ) from exc
             raise exc
@@ -1024,27 +1112,12 @@
             raise exc
 
         if not keep_ids and not self.debug_mode:
             self.review_manager.logger.info("Set record IDs")
             self.review_manager.dataset.set_ids()
             self.review_manager.create_commit(msg="Set IDs")
 
-        if not self.review_manager.high_level_operation:
-            print()
-
-        self.review_manager.logger.info("To validate the changes, use")
-
-        self.review_manager.logger.info(
-            f"{colors.ORANGE}colrev validate {prep_commit_id}{colors.END}"
-        )
-        if not self.review_manager.high_level_operation:
-            print()
-
-        self.review_manager.logger.info(
-            f"{colors.GREEN}Completed prep operation{colors.END}"
-        )
-        if self.review_manager.in_ci_environment():
-            print("\n\n")
+        self.__post_prep()
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `colrev-0.8.2/colrev/ops/prep_man.py` & `colrev-0.8.3/colrev/ops/prep_man.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         else:
             self.review_manager.logger.info(
                 f"Import language fields from {lang_prep_csv_path}"
             )
             languages_df = pd.read_csv(lang_prep_csv_path)
             language_records = languages_df.to_dict("records")
             for language_record in language_records:
-                if "" == language_record["most_likely_language"]:
+                if language_record["most_likely_language"] == "":
                     continue
                 if language_record["ID"] not in records:
                     # warn
                     continue
                 record_dict = records[language_record["ID"]]
                 record = colrev.record.Record(data=record_dict)
                 record.update_field(
@@ -167,17 +167,17 @@
                         ] = ""
                     if (
                         record.data["colrev_status"]
                         == colrev.record.RecordState.md_needs_manual_preparation
                     ):
                         # by resetting to md_imported,
                         # the prescreen-exclusion based on languages will be reapplied.
-                        record.data[
-                            "colrev_status"
-                        ] = colrev.record.RecordState.md_imported
+                        record.set_status(
+                            target_state=colrev.record.RecordState.md_imported
+                        )
 
             self.review_manager.dataset.save_records_dict(records=records)
 
     def prep_man_stats(self) -> None:
         """Print statistics on prep_man"""
         # pylint: disable=duplicate-code
```

### Comparing `colrev-0.8.2/colrev/ops/prescreen.py` & `colrev-0.8.3/colrev/ops/prescreen.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,31 +84,31 @@
 
     def __prescreen_records(self, *, ids: str, include: bool) -> None:
         records = self.review_manager.dataset.load_records_dict()
         for record_id in ids.split(","):
             if record_id not in records:
                 self.review_manager.logger.info(f" not found: {record_id}")
                 continue
-            record = records[record_id]
+            record = colrev.record.Record(data=records[record_id])
             if (
-                record["colrev_status"] != colrev.record.RecordState.md_processed
+                record.data["colrev_status"] != colrev.record.RecordState.md_processed
                 and not self.review_manager.force_mode
             ):
                 self.review_manager.logger.info(
                     f" record not md_processed / cannot prescreen: {record_id}"
                 )
                 continue
             if include:
-                record[
-                    "colrev_status"
-                ] = colrev.record.RecordState.rev_prescreen_included
+                record.set_status(
+                    target_state=colrev.record.RecordState.rev_prescreen_included
+                )
             else:
-                record[
-                    "colrev_status"
-                ] = colrev.record.RecordState.rev_prescreen_excluded
+                record.set_status(
+                    target_state=colrev.record.RecordState.rev_prescreen_excluded
+                )
 
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
 
         msg = f"Pre-screen (exclude {ids})"
         if include:
             msg = f"Pre-screen (include {ids})"
@@ -179,19 +179,20 @@
             {"endpoint": "custom_prescreen_script"}
         )
         self.review_manager.save_settings()
 
     def __prescreen_include_all(self, *, records: dict) -> None:
         # pylint: disable=duplicate-code
         self.review_manager.logger.info("Prescreen-including all records")
-        for record in records.values():
-            if record["colrev_status"] == colrev.record.RecordState.md_processed:
-                record[
-                    "colrev_status"
-                ] = colrev.record.RecordState.rev_prescreen_included
+        for record_dict in records.values():
+            if record_dict["colrev_status"] == colrev.record.RecordState.md_processed:
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(
+                    target_state=colrev.record.RecordState.rev_prescreen_included
+                )
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg="Pre-screen (include_all)",
             manual_author=False,
         )
```

### Comparing `colrev-0.8.2/colrev/ops/pull.py` & `colrev-0.8.3/colrev/ops/pull.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/push.py` & `colrev-0.8.3/colrev/ops/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         text = (
             "Dear Sir or Madam,\n\nwe have noticed potential corrections and "
             + "would like to share them with you.\nThe potentical changes are:\n\n"
             + f"{corrections}\n\nBest regards\n\n"
         )
 
-        if "colrev.dblp" == source.endpoint:
+        if source.endpoint == "colrev.dblp":
             file_path = Path("dblp-corrections-mail.txt")
             dblp_header = (
                 "Send to: dblp@dagstuhl.de\n\n"
                 + "Subject: Potential correction to DBLP metadata\n\n"
             )
 
             text = dblp_header + text
```

### Comparing `colrev-0.8.2/colrev/ops/remove.py` & `colrev-0.8.3/colrev/ops/remove.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/repare.py` & `colrev-0.8.3/colrev/ops/repare.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,34 +28,69 @@
         review_manager: colrev.review_manager.ReviewManager,
     ) -> None:
         super().__init__(
             review_manager=review_manager,
             operations_type=colrev.operation.OperationsType.check,
             notify_state_transition_operation=False,
         )
+        # fix file no longer available
+        self.local_index = self.review_manager.get_local_index()
+        self.pdf_get_operation = self.review_manager.get_pdf_get_operation()
 
-    def __fix_files(self, *, records: dict) -> None:
-        # pylint: disable=too-many-branches
+    def __fix_broken_symlink_based_on_local_index(
+        self, *, record: colrev.record.Record, full_path: Path
+    ) -> None:
+        """Fix broken symlinks based on local_index"""
 
-        # fix file no longer available
-        local_index = self.review_manager.get_local_index()
-        pdf_get_operation = self.review_manager.get_pdf_get_operation()
+        if os.path.islink(full_path) and not os.path.exists(full_path):
+            self.review_manager.logger.debug(f" remove broken symlink: {full_path}")
+            full_path.unlink()
 
+        try:
+            retrieved_record = self.local_index.retrieve(
+                record_dict=record.data, include_file=True
+            )
+
+            if "file" in retrieved_record:
+                record.update_field(
+                    key="file",
+                    value=str(retrieved_record["file"]),
+                    source="local_index",
+                    append_edit=False,
+                )
+                self.pdf_get_operation.import_file(record=record)
+                if "fulltext" in retrieved_record:
+                    del retrieved_record["fulltext"]
+                self.review_manager.logger.info(
+                    f" fix broken symlink: {record.data['ID']}"
+                )
+            else:
+                self.review_manager.logger.debug(
+                    f" file not linked in retrieved record: {record.data['ID']}"
+                )
+
+        except colrev_exceptions.RecordNotInIndexException:
+            self.review_manager.logger.debug(
+                f" record not in index: {record.data['ID']}"
+            )
+
+    def __fix_files(self, *, records: dict) -> None:
         for record_dict in records.values():
             if "file" not in record_dict:
                 continue
 
             if not record_dict["file"].startswith("data/pdfs/"):
                 record_dict["file"] = f"data/pdfs/{record_dict['ID']}.pdf"
 
             full_path = self.review_manager.path / Path(record_dict["file"])
 
             if full_path.is_file():
                 continue
 
+            # Add .pdf extension if missing
             if Path(str(full_path) + ".pdf").is_file():
                 Path(str(full_path) + ".pdf").rename(full_path)
 
             # Check / replace multiple blanks in file and filename
             try:
                 parent_dir = full_path.parent
                 same_dir_pdfs = [
@@ -70,230 +105,205 @@
                         record_dict["file"] = record_dict["file"].replace("  ", " ")
             except ValueError:
                 pass
 
             full_path = self.review_manager.path / Path(record_dict["file"])
 
             if not full_path.is_file():
-                # Fix broken symlinks based on local_index
-
-                if os.path.islink(full_path) and not os.path.exists(full_path):
-                    self.review_manager.logger.debug(
-                        f" remove broken symlink: {full_path}"
-                    )
-                    full_path.unlink()
-
-                try:
-                    record = colrev.record.Record(data=record_dict)
-                    retrieved_record = local_index.retrieve(
-                        record_dict=record.data, include_file=True
-                    )
-
-                    if "file" in retrieved_record:
-                        record.update_field(
-                            key="file",
-                            value=str(retrieved_record["file"]),
-                            source="local_index",
-                            append_edit=False,
-                        )
-                        pdf_get_operation.import_file(record=record)
-                        if "fulltext" in retrieved_record:
-                            del retrieved_record["fulltext"]
-                        self.review_manager.logger.info(
-                            f" fix broken symlink: {record_dict['ID']}"
-                        )
-                    else:
-                        self.review_manager.logger.debug(
-                            f" file not linked in retrieved record: {record_dict['ID']}"
-                        )
-
-                except colrev_exceptions.RecordNotInIndexException:
-                    self.review_manager.logger.debug(
-                        f" record not in index: {record_dict['ID']}"
-                    )
+                record = colrev.record.Record(data=record_dict)
+                self.__fix_broken_symlink_based_on_local_index(
+                    record=record, full_path=full_path
+                )
 
             if full_path.is_file():
                 continue
 
             record_dict["colrev_status_backup"] = record_dict["colrev_status"]
             del record_dict["file"]
-            record_dict[
-                "colrev_status"
-            ] = colrev.record.RecordState.rev_prescreen_included
-
-    def __fix_provenance(self, *, records: dict) -> None:
-        # pylint: disable=too-many-nested-blocks
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
+            record = colrev.record.Record(data=record_dict)
+            record.set_status(
+                target_state=colrev.record.RecordState.rev_prescreen_included
+            )
 
+    def __get_source_feeds(self) -> dict:
         source_feeds = {}
         for source in self.review_manager.settings.sources:
             source_feeds[
                 str(source.get_corresponding_bib_file()).replace("data/search/", "")
             ] = source.get_feed(
                 review_manager=self.review_manager,
                 source_identifier="NA",
                 update_only=False,
             ).feed_records
+        return source_feeds
 
-        for record_dict in records.values():
-            record = colrev.record.Record(data=record_dict)
-            if "colrev_data_provenance" not in record.data:
-                record.data["colrev_data_provenance"] = {}
-            if "colrev_masterdata_provenance" not in record.data:
-                record.data["colrev_masterdata_provenance"] = {}
-            if "pdf_hash" in record.data:
-                record.data["colrev_pdf_id"] = record.data["pdf_hash"]
-                del record.data["pdf_hash"]
-            if "pdf_prep_hints" in record.data:
-                del record.data["pdf_prep_hints"]
-            if "grobid-version" in record.data:
-                del record.data["grobid-version"]
-
-            mk_to_remove = []
-            for key in record.data["colrev_data_provenance"]:
-                if key not in record.data:
-                    mk_to_remove += [key]
-            for key in mk_to_remove:
+    def __remove_fields(self, *, record: colrev.record.Record) -> None:
+        if "pdf_hash" in record.data:
+            record.data["colrev_pdf_id"] = record.data["pdf_hash"]
+            del record.data["pdf_hash"]
+        if "pdf_prep_hints" in record.data:
+            del record.data["pdf_prep_hints"]
+        if "grobid-version" in record.data:
+            del record.data["grobid-version"]
+
+        mk_to_remove = []
+        for key in record.data["colrev_data_provenance"]:
+            if key not in record.data:
+                mk_to_remove += [key]
+        for key in mk_to_remove:
+            del record.data["colrev_data_provenance"][key]
+
+        mdk_to_remove = []
+        for key in record.data["colrev_masterdata_provenance"]:
+            if (
+                key not in record.data
+                and "CURATED" != key
+                and "not_missing"
+                not in record.data["colrev_masterdata_provenance"][key]["note"]
+            ):
+                mdk_to_remove += [key]
+        for key in mdk_to_remove:
+            del record.data["colrev_masterdata_provenance"][key]
+
+        if self.review_manager.settings.is_curated_masterdata_repo():
+            if "CURATED" in record.data["colrev_masterdata_provenance"]:
+                del record.data["colrev_masterdata_provenance"]["CURATED"]
+
+    def __set_data_provenance_field(
+        self, *, record: colrev.record.Record, key: str, source_feeds: dict
+    ) -> None:
+        if key in record.data["colrev_data_provenance"]:
+            if not any(
+                record.data["colrev_data_provenance"][key]["source"].startswith(sf)
+                for sf in list(source_feeds.keys())
+            ):
                 del record.data["colrev_data_provenance"][key]
+        if key not in record.data["colrev_data_provenance"]:
+            for origin in record.data["colrev_origin"]:
+                origin_source, origin_id = origin.split("/")
+                if key in source_feeds[origin_source][origin_id]:
+                    record.add_data_provenance(key=key, source=origin, note="")
+        if key == "language":
+            record.add_data_provenance(key=key, source="LanguageDetector", note="")
+        if key == "tei_file":
+            record.add_data_provenance(key=key, source="file|grobid", note="")
+        if key == "colrev_pdf_id":
+            record.add_data_provenance(key=key, source="file|pdf_hash", note="")
 
-            mdk_to_remove = []
-            for key in record.data["colrev_masterdata_provenance"]:
-                if (
-                    key not in record.data
-                    and "CURATED" != key
-                    and "not_missing"
-                    not in record.data["colrev_masterdata_provenance"][key]["note"]
-                ):
-                    mdk_to_remove += [key]
-            for key in mdk_to_remove:
-                del record.data["colrev_masterdata_provenance"][key]
+        if key not in record.data["colrev_data_provenance"]:
+            record.add_data_provenance(key=key, source="manual", note="")
 
-            if self.review_manager.settings.is_curated_masterdata_repo():
-                if "CURATED" in record.data["colrev_masterdata_provenance"]:
-                    del record.data["colrev_masterdata_provenance"]["CURATED"]
-
-            for key, value in record.data.items():
-                if key in [
-                    "colrev_status",
-                    "colrev_origin",
-                    "colrev_masterdata_provenance",
-                    "colrev_data_provenance",
-                    "colrev_pdfid",
-                    "colrev_pdf_id",
-                    "colrev_id",
-                    "ID",
-                    "ENTRYTYPE",
-                    "screening_criteria",
-                ]:
-                    continue
-                if key in colrev.record.Record.identifying_field_keys:
-                    if "CURATED" not in record.data["colrev_masterdata_provenance"]:
-                        if key in record.data["colrev_masterdata_provenance"]:
-                            if not any(
-                                record.data["colrev_masterdata_provenance"][key][
-                                    "source"
-                                ].startswith(sf)
-                                for sf in list(source_feeds.keys())
-                            ):
-                                del record.data["colrev_masterdata_provenance"][key]
-                        if key not in record.data["colrev_masterdata_provenance"]:
-                            options = {}
-                            for origin in record.data["colrev_origin"]:
-                                origin_source, origin_id = origin.split("/")
-                                if key in source_feeds[origin_source][origin_id]:
-                                    options[origin_source] = source_feeds[
-                                        origin_source
-                                    ][origin_id][key]
-
-                            source_value = "manual"
-
-                            # Note : simple heuristics:
-                            if value in options.values():
-                                if "md_curated.bib" in options:
-                                    source_origin = "md_curated.bib"
-                                elif "md_crossref.bib" in options:
-                                    source_origin = "md_crossref.bib"
-                                elif "CROSSREF.bib" in options:
-                                    source_origin = "CROSSREF.bib"
-                                elif "md_dblp.bib" in options:
-                                    source_origin = "md_dblp.bib"
-                                elif "DBLP.bib" in options:
-                                    source_origin = "DBLP.bib"
-                                else:
-                                    source_origin = [
-                                        k for k, v in options.items() if v == value
-                                    ][0]
-
-                                for origin in record.data["colrev_origin"]:
-                                    origin_source, origin_id = origin.split("/")
-                                    if source_origin == origin_source:
-                                        source_value = origin
+        for _, prov_details in record.data["colrev_data_provenance"].items():
+            if prov_details["source"] in record.data["colrev_origin"] + ["manual"]:
+                continue
+            # Note : simple heuristic
+            prov_details["source"] = record.data["colrev_origin"][0]
 
-                            record.add_masterdata_provenance(
-                                key=key, source=source_value, note=""
-                            )
+    def __add_missing_masterdata_provenance(
+        self, *, record: colrev.record.Record, key: str, value: str, source_feeds: dict
+    ) -> None:
+        options = {}
+        for origin in record.data["colrev_origin"]:
+            origin_source, origin_id = origin.split("/")
+            if key in source_feeds[origin_source][origin_id]:
+                options[origin_source] = source_feeds[origin_source][origin_id][key]
+
+        source_value = "manual"
+
+        # Note : simple heuristics:
+        if value in options.values():
+            if "md_curated.bib" in options:
+                source_origin = "md_curated.bib"
+            elif "md_crossref.bib" in options:
+                source_origin = "md_crossref.bib"
+            elif "CROSSREF.bib" in options:
+                source_origin = "CROSSREF.bib"
+            elif "md_dblp.bib" in options:
+                source_origin = "md_dblp.bib"
+            elif "DBLP.bib" in options:
+                source_origin = "DBLP.bib"
+            else:
+                source_origin = [k for k, v in options.items() if v == value][0]
+
+            for origin in record.data["colrev_origin"]:
+                origin_source, origin_id = origin.split("/")
+                if source_origin == origin_source:
+                    source_value = origin
 
-                        if key not in record.data["colrev_masterdata_provenance"]:
-                            record.add_masterdata_provenance(
-                                key=key, source="manual", note=""
-                            )
+        record.add_masterdata_provenance(key=key, source=source_value, note="")
 
-                        for _, prov_details in record.data[
-                            "colrev_masterdata_provenance"
-                        ].items():
-                            if prov_details["source"] in record.data[
-                                "colrev_origin"
-                            ] + ["manual"]:
-                                continue
-                            # Note : simple heuristic
-                            prov_details["source"] = record.data["colrev_origin"][0]
-
-                else:
-                    if key in record.data["colrev_data_provenance"]:
-                        if not any(
-                            record.data["colrev_data_provenance"][key][
-                                "source"
-                            ].startswith(sf)
-                            for sf in list(source_feeds.keys())
-                        ):
-                            del record.data["colrev_data_provenance"][key]
-                    if key not in record.data["colrev_data_provenance"]:
-                        for origin in record.data["colrev_origin"]:
-                            origin_source, origin_id = origin.split("/")
-                            if key in source_feeds[origin_source][origin_id]:
-                                record.add_data_provenance(
-                                    key=key, source=origin, note=""
-                                )
-                    if "language" == key:
-                        record.add_data_provenance(
-                            key=key, source="LanguageDetector", note=""
-                        )
-                    if "tei_file" == key:
-                        record.add_data_provenance(
-                            key=key, source="file|grobid", note=""
-                        )
-                    if "colrev_pdf_id" == key:
-                        record.add_data_provenance(
-                            key=key, source="file|pdf_hash", note=""
-                        )
+    def __set_non_curated_masterdata_provenance_field(
+        self, *, record: colrev.record.Record, key: str, value: str, source_feeds: dict
+    ) -> None:
+        if key in record.data["colrev_masterdata_provenance"]:
+            if not any(
+                record.data["colrev_masterdata_provenance"][key]["source"].startswith(
+                    sf
+                )
+                for sf in list(source_feeds.keys())
+            ):
+                del record.data["colrev_masterdata_provenance"][key]
+        if key not in record.data["colrev_masterdata_provenance"]:
+            self.__add_missing_masterdata_provenance(
+                record=record, key=key, value=value, source_feeds=source_feeds
+            )
 
-                    if key not in record.data["colrev_data_provenance"]:
-                        record.add_data_provenance(key=key, source="manual", note="")
+        for prov_details in record.data["colrev_masterdata_provenance"].values():
+            if prov_details["source"] in record.data["colrev_origin"] + ["manual"]:
+                continue
+            # Note : simple heuristic
+            prov_details["source"] = record.data["colrev_origin"][0]
 
-                    for _, prov_details in record.data[
-                        "colrev_data_provenance"
-                    ].items():
-                        if prov_details["source"] in record.data["colrev_origin"] + [
-                            "manual"
-                        ]:
-                            continue
-                        # Note : simple heuristic
-                        prov_details["source"] = record.data["colrev_origin"][0]
+    def __set_provenance_field(
+        self, *, record: colrev.record.Record, key: str, value: str, source_feeds: dict
+    ) -> None:
+        if key in colrev.record.Record.identifying_field_keys:
+            if "CURATED" in record.data["colrev_masterdata_provenance"]:
+                return
+            self.__set_non_curated_masterdata_provenance_field(
+                record=record, key=key, value=value, source_feeds=source_feeds
+            )
+
+        else:
+            self.__set_data_provenance_field(
+                record=record, key=key, source_feeds=source_feeds
+            )
+
+    def __set_provenance(
+        self, *, record: colrev.record.Record, source_feeds: dict
+    ) -> None:
+        if "colrev_data_provenance" not in record.data:
+            record.data["colrev_data_provenance"] = {}
+        if "colrev_masterdata_provenance" not in record.data:
+            record.data["colrev_masterdata_provenance"] = {}
+
+        for key, value in record.data.items():
+            if key in [
+                "colrev_status",
+                "colrev_origin",
+                "colrev_masterdata_provenance",
+                "colrev_data_provenance",
+                "colrev_pdfid",
+                "colrev_pdf_id",
+                "colrev_id",
+                "ID",
+                "ENTRYTYPE",
+                "screening_criteria",
+            ]:
+                continue
+            self.__set_provenance_field(
+                record=record, key=key, value=value, source_feeds=source_feeds
+            )
+
+    def __fix_provenance(self, *, records: dict) -> None:
+        source_feeds = self.__get_source_feeds()
+        for record_dict in records.values():
+            record = colrev.record.Record(data=record_dict)
+            self.__remove_fields(record=record)
+            self.__set_provenance(record=record, source_feeds=source_feeds)
 
     def __fix_curated_sources(self, *, records: dict) -> None:
         local_index = self.review_manager.get_local_index()
         for search_source in self.review_manager.settings.sources:
             if search_source.endpoint != "colrev.local_index":
                 continue
             curation_recs = self.review_manager.dataset.load_records_dict(
@@ -331,18 +341,14 @@
                 records=curation_recs, save_path=search_source.filename
             )
             self.review_manager.dataset.add_changes(path=search_source.filename)
 
     def main(self) -> None:
         """Repare a CoLRev project (main entrypoint)"""
 
-        # pylint: disable=too-many-nested-blocks
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-
         # Try: open settings, except: notify & start repare
 
         # ...
 
         # Try: open records, except: notify & start repare
         try:
             records = self.review_manager.dataset.load_records_dict()
```

### Comparing `colrev-0.8.2/colrev/ops/review_types.py` & `colrev-0.8.3/colrev/ops/review_types.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/screen.py` & `colrev-0.8.3/colrev/ops/screen.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,25 +124,26 @@
 
             self.review_manager.save_settings()
             self.review_manager.dataset.add_setting_changes()
         else:
             print(f"Error: criterion {criterion_name} already in settings")
             return
 
-        for record in records.values():
-            if record["colrev_status"] in [
+        for record_dict in records.values():
+            if record_dict["colrev_status"] in [
                 colrev.record.RecordState.rev_included,
                 colrev.record.RecordState.rev_synthesized,
             ]:
-                record["screening_criteria"] += f";{criterion_name}=TODO"
+                record_dict["screening_criteria"] += f";{criterion_name}=TODO"
                 # Note : we set the status to pdf_prepared because the screening
                 # decisions have to be updated (resulting in inclusion or exclusion)
-                record["colrev_status"] = colrev.record.RecordState.pdf_prepared
-            if record["colrev_status"] == colrev.record.RecordState.rev_excluded:
-                record["screening_criteria"] += f";{criterion_name}=TODO"
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(target_state=colrev.record.RecordState.pdf_prepared)
+            if record_dict["colrev_status"] == colrev.record.RecordState.rev_excluded:
+                record_dict["screening_criteria"] += f";{criterion_name}=TODO"
                 # Note : no change in colrev_status
                 # because at least one of the other criteria led to exclusion decision
 
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg=f"Add screening criterion: {criterion_name}",
@@ -156,47 +157,50 @@
             del self.review_manager.settings.screen.criteria[criterion_to_delete]
             self.review_manager.save_settings()
             self.review_manager.dataset.add_setting_changes()
         else:
             print(f"Error: criterion {criterion_to_delete} not in settings")
             return
 
-        for record in records.values():
-            if record["colrev_status"] in [
+        for record_dict in records.values():
+            if record_dict["colrev_status"] in [
                 colrev.record.RecordState.rev_included,
                 colrev.record.RecordState.rev_synthesized,
             ]:
-                record["screening_criteria"] = (
-                    record["screening_criteria"]
+                record_dict["screening_criteria"] = (
+                    record_dict["screening_criteria"]
                     .replace(f"{criterion_to_delete}=TODO", "")
                     .replace(f"{criterion_to_delete}=in", "")
                     .replace(f"{criterion_to_delete}=out", "")
                     .replace(";;", ";")
                     .lstrip(";")
                     .rstrip(";")
                 )
                 # Note : colrev_status does not change
                 # because the other screening criteria do not change
 
-            if record["colrev_status"] in [colrev.record.RecordState.rev_excluded]:
-                record["screening_criteria"] = (
-                    record["screening_criteria"]
+            if record_dict["colrev_status"] in [colrev.record.RecordState.rev_excluded]:
+                record_dict["screening_criteria"] = (
+                    record_dict["screening_criteria"]
                     .replace(f"{criterion_to_delete}=TODO", "")
                     .replace(f"{criterion_to_delete}=in", "")
                     .replace(f"{criterion_to_delete}=out", "")
                     .replace(";;", ";")
                     .lstrip(";")
                     .rstrip(";")
                 )
 
                 if (
-                    "=out" not in record["screening_criteria"]
-                    and "=TODO" not in record["screening_criteria"]
+                    "=out" not in record_dict["screening_criteria"]
+                    and "=TODO" not in record_dict["screening_criteria"]
                 ):
-                    record["colrev_status"] = colrev.record.RecordState.rev_included
+                    record = colrev.record.Record(data=record_dict)
+                    record.set_status(
+                        target_state=colrev.record.RecordState.rev_included
+                    )
 
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg=f"Removed screening criterion: {criterion_to_delete}",
         )
 
@@ -236,17 +240,18 @@
         self.review_manager.settings.screen.screen_package_endpoints.append(
             {"endpoint": "custom_screen_script"}
         )
         self.review_manager.save_settings()
 
     def __screen_include_all(self, *, records: dict) -> None:
         self.review_manager.logger.info("Screen: Include all records")
-        for record in records.values():
-            if record["colrev_status"] == colrev.record.RecordState.pdf_prepared:
-                record["colrev_status"] = colrev.record.RecordState.rev_included
+        for record_dict in records.values():
+            if record_dict["colrev_status"] == colrev.record.RecordState.pdf_prepared:
+                record = colrev.record.Record(data=record_dict)
+                record.set_status(target_state=colrev.record.RecordState.rev_included)
         self.review_manager.dataset.save_records_dict(records=records)
         self.review_manager.dataset.add_record_changes()
         self.review_manager.create_commit(
             msg="Screen (include_all)",
             manual_author=False,
         )
 
@@ -269,15 +274,15 @@
             return
 
         print()
         self.review_manager.logger.info("Statistics")
         for record_dict in records.values():
             if record_dict["ID"] in screen_excluded:
                 reasons = record_dict.get("screening_criteria", "NA")
-                if "NA" == reasons:
+                if reasons == "NA":
                     reasons = ""
                 else:
                     reasons = f"({reasons})"
                 self.review_manager.logger.info(
                     f" {record_dict['ID']}".ljust(40)
                     + f"pdf_prepared → rev_excluded {colors.RED}{reasons}{colors.END}"
                 )
```

### Comparing `colrev-0.8.2/colrev/ops/search.py` & `colrev-0.8.3/colrev/ops/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 from copy import deepcopy
 from pathlib import Path
 from random import randint
 from typing import Optional
 
 import requests
+import timeout_decorator
 from pybtex.database.input import bibtex
 
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.settings
 import colrev.ui_cli.cli_colors as colors
 
@@ -106,15 +107,15 @@
             )
 
     def __get_search_sources(
         self, *, selection_str: Optional[str] = None
     ) -> list[colrev.settings.SearchSource]:
         sources_selected = self.sources
         if selection_str:
-            if "all" != selection_str:
+            if selection_str != "all":
                 sources_selected = [
                     f
                     for f in self.sources
                     if str(f.filename) in selection_str.split(",")
                 ]
             if len(sources_selected) == 0:
                 available_options = [str(f.filename) for f in self.sources]
@@ -163,148 +164,178 @@
                 continue
             if key not in record_a:
                 return True
             if record_a[key] != value:
                 return True
         return changed
 
-    def update_existing_record(
+    def __get_record_based_on_origin(self, origin: str, records: dict) -> dict:
+        for main_record_dict in records.values():
+            if origin in main_record_dict["colrev_origin"]:
+                return main_record_dict
+        return {}
+
+    def __update_existing_record_retract(
+        self, *, record: colrev.record.Record, main_record_dict: dict
+    ) -> bool:
+        if record.check_potential_retracts():
+            self.review_manager.logger.info(
+                f"{colors.GREEN}Found paper retract: "
+                f"{main_record_dict['ID']}{colors.END}"
+            )
+            main_record = colrev.record.Record(data=main_record_dict)
+            main_record.prescreen_exclude(reason="retracted", print_warning=True)
+            main_record.remove_field(key="warning")
+            return True
+        return False
+
+    def __update_existing_record_forthcoming(
+        self, *, record: colrev.record.Record, main_record_dict: dict
+    ) -> None:
+        if "forthcoming" == main_record_dict.get(
+            "year", ""
+        ) and "forthcoming" != record.data.get("year", ""):
+            self.review_manager.logger.info(
+                f"{colors.GREEN}Update published forthcoming paper: "
+                f"{record.data['ID']}{colors.END}"
+            )
+            # prepared_record = crossref_prep.prepare(prep_operation, record)
+            main_record_dict["year"] = record.data["year"]
+            record = colrev.record.PrepRecord(data=main_record_dict)
+
+    def __update_existing_record_fields(
         self,
         *,
-        records: dict,
         record_dict: dict,
+        main_record_dict: dict,
         prev_record_dict_version: dict,
-        source: colrev.settings.SearchSource,
         update_time_variant_fields: bool,
-    ) -> bool:
-        """Convenience function to update existing records (main data/records.bib)"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-
-        changed = False
+        origin: str,
+        source: colrev.settings.SearchSource,
+    ) -> None:
+        for key, value in record_dict.items():
+            if (
+                not update_time_variant_fields
+                and key in colrev.record.Record.time_variant_fields
+            ):
+                continue
 
-        origin = f"{source.get_origin_prefix()}/{record_dict['ID']}"
-        for main_record_dict in records.values():
-            if origin not in main_record_dict["colrev_origin"]:
+            if key in ["curation_ID"]:
                 continue
 
-            # TBD: in curated masterdata repositories?
+            if key in colrev.record.Record.provenance_keys + ["ID"]:
+                continue
 
-            record = colrev.record.Record(data=record_dict)
-            if record.check_potential_retracts():
-                self.review_manager.logger.info(
-                    f"{colors.GREEN}Found paper retract: "
-                    f"{main_record_dict['ID']}{colors.END}"
-                )
+            if key not in main_record_dict:
+                if key in main_record_dict.get("colrev_masterdata_provenance", {}):
+                    if (
+                        main_record_dict["colrev_masterdata_provenance"][key]["source"]
+                        == "colrev_curation.masterdata_restrictions"
+                        and main_record_dict["colrev_masterdata_provenance"][key][
+                            "note"
+                        ]
+                        == "not_missing"
+                    ):
+                        continue
                 main_record = colrev.record.Record(data=main_record_dict)
-                main_record.prescreen_exclude(reason="retracted", print_warning=True)
-                main_record.remove_field(key="warning")
-                changed = True
-
-            if "forthcoming" == main_record_dict.get(
-                "year", ""
-            ) and "forthcoming" != record_dict.get("year", ""):
-                self.review_manager.logger.info(
-                    f"{colors.GREEN}Update published forthcoming paper: "
-                    f"{record.data['ID']}{colors.END}"
+                main_record.update_field(
+                    key=key,
+                    value=value,
+                    source=origin,
+                    keep_source_if_equal=True,
+                    append_edit=False,
                 )
-                # prepared_record = crossref_prep.prepare(prep_operation, record)
-                main_record_dict["year"] = record_dict["year"]
-                record = colrev.record.PrepRecord(data=main_record_dict)
-
-            if (
-                "CURATED" in main_record_dict.get("colrev_masterdata_provenance", {})
-                and "md_curated.bib" != source.get_origin_prefix()
-            ):
-                continue
-
-            similarity_score = colrev.record.Record.get_record_similarity(
-                record_a=colrev.record.Record(data=record_dict),
-                record_b=colrev.record.Record(data=prev_record_dict_version),
-            )
-            dict_diff = colrev.record.Record(data=record_dict).get_diff(
-                other_record=colrev.record.Record(data=prev_record_dict_version)
-            )
-
-            for key, value in record_dict.items():
-                if (
-                    not update_time_variant_fields
-                    and key in colrev.record.Record.time_variant_fields
+            else:
+                if source.get_origin_prefix() != "md_curated.bib":
+                    if prev_record_dict_version.get(key, "NA") != main_record_dict.get(
+                        key, "OTHER"
+                    ):
+                        continue
+                main_record = colrev.record.Record(data=main_record_dict)
+                if value.replace(" - ", ": ") == main_record.data[key].replace(
+                    " - ", ": "
                 ):
                     continue
+                main_record.update_field(
+                    key=key,
+                    value=value,
+                    source=origin,
+                    keep_source_if_equal=True,
+                    append_edit=False,
+                )
 
-                if key in ["curation_ID"]:
-                    continue
+    def update_existing_record(
+        self,
+        *,
+        records: dict,
+        record_dict: dict,
+        prev_record_dict_version: dict,
+        source: colrev.settings.SearchSource,
+        update_time_variant_fields: bool,
+    ) -> bool:
+        """Convenience function to update existing records (main data/records.bib)"""
 
-                if key in colrev.record.Record.provenance_keys + ["ID"]:
-                    continue
+        origin = f"{source.get_origin_prefix()}/{record_dict['ID']}"
+        main_record_dict = self.__get_record_based_on_origin(
+            origin=origin, records=records
+        )
 
-                if key not in main_record_dict:
-                    if key in main_record_dict.get("colrev_masterdata_provenance", {}):
-                        if (
-                            main_record_dict["colrev_masterdata_provenance"][key][
-                                "source"
-                            ]
-                            == "colrev_curation.masterdata_restrictions"
-                            and main_record_dict["colrev_masterdata_provenance"][key][
-                                "note"
-                            ]
-                            == "not_missing"
-                        ):
-                            continue
-                    main_record = colrev.record.Record(data=main_record_dict)
-                    main_record.update_field(
-                        key=key,
-                        value=value,
-                        source=origin,
-                        keep_source_if_equal=True,
-                        append_edit=False,
-                    )
-                else:
-                    if "md_curated.bib" != source.get_origin_prefix():
-                        if prev_record_dict_version.get(
-                            key, "NA"
-                        ) != main_record_dict.get(key, "OTHER"):
-                            continue
-                    main_record = colrev.record.Record(data=main_record_dict)
-                    if value.replace(" - ", ": ") == main_record.data[key].replace(
-                        " - ", ": "
-                    ):
-                        continue
-                    main_record.update_field(
-                        key=key,
-                        value=value,
-                        source=origin,
-                        keep_source_if_equal=True,
-                        append_edit=False,
-                    )
-            if self.__have_changed(
-                record_a_orig=main_record_dict, record_b_orig=prev_record_dict_version
-            ):
-                changed = True
+        if main_record_dict == {}:
+            self.review_manager.logger.debug(f"Could not update {record_dict['ID']}")
+            return False
+
+        # TBD: in curated masterdata repositories?
+
+        record = colrev.record.Record(data=record_dict)
+        changed = self.__update_existing_record_retract(
+            record=record, main_record_dict=main_record_dict
+        )
+        self.__update_existing_record_forthcoming(
+            record=record, main_record_dict=main_record_dict
+        )
 
-            if self.__have_changed(
-                record_a_orig=record_dict, record_b_orig=prev_record_dict_version
-            ):
-                # Note : not (yet) in the main records but changed
-                changed = True
-            if changed:
-                if similarity_score > 0.98:
-                    self.review_manager.logger.info(f" check/update {origin}")
-                else:
-                    self.review_manager.logger.info(
-                        f" {colors.RED} check/update {origin} leads to substantial changes "
-                        f"({similarity_score}) in {main_record_dict['ID']}:{colors.END}"
-                    )
-                    self.review_manager.p_printer.pprint(
-                        [x for x in dict_diff if "change" == x[0]]
-                    )
+        if (
+            "CURATED" in main_record_dict.get("colrev_masterdata_provenance", {})
+            and "md_curated.bib" != source.get_origin_prefix()
+        ):
+            return False
+
+        similarity_score = colrev.record.Record.get_record_similarity(
+            record_a=colrev.record.Record(data=record_dict),
+            record_b=colrev.record.Record(data=prev_record_dict_version),
+        )
+        dict_diff = colrev.record.Record(data=record_dict).get_diff(
+            other_record=colrev.record.Record(data=prev_record_dict_version)
+        )
+
+        self.__update_existing_record_fields(
+            record_dict=record_dict,
+            main_record_dict=main_record_dict,
+            prev_record_dict_version=prev_record_dict_version,
+            update_time_variant_fields=update_time_variant_fields,
+            origin=origin,
+            source=source,
+        )
 
-            break
+        if self.__have_changed(
+            record_a_orig=main_record_dict, record_b_orig=prev_record_dict_version
+        ) or self.__have_changed(  # Note : not (yet) in the main records but changed
+            record_a_orig=record_dict, record_b_orig=prev_record_dict_version
+        ):
+            changed = True
+            if similarity_score > 0.98:
+                self.review_manager.logger.info(f" check/update {origin}")
+            else:
+                self.review_manager.logger.info(
+                    f" {colors.RED} check/update {origin} leads to substantial changes "
+                    f"({similarity_score}) in {main_record_dict['ID']}:{colors.END}"
+                )
+                self.review_manager.p_printer.pprint(
+                    [x for x in dict_diff if "change" == x[0]]
+                )
 
         return changed
 
     def main(
         self,
         *,
         selection_str: Optional[str] = None,
@@ -359,15 +390,18 @@
                 print()
             self.review_manager.logger.info(
                 f"search [{source.endpoint} > data/search/{source.filename.name}]"
             )
 
             try:
                 endpoint.run_search(search_operation=self, rerun=rerun)  # type: ignore
-            except requests.exceptions.ConnectionError as exc:
+            except (
+                requests.exceptions.ConnectionError,
+                timeout_decorator.timeout_decorator.TimeoutError,
+            ) as exc:
                 raise colrev_exceptions.ServiceNotAvailableException(
                     source.endpoint
                 ) from exc
 
             if source.filename.is_file():
                 if not self.review_manager.settings.search.retrieve_forthcoming:
                     self.__remove_forthcoming(source=source)
@@ -499,15 +533,15 @@
 
                     search_operation.review_manager.dataset.add_changes(
                         path=self.feed_file
                     )
                     break
                 except (FileExistsError, OSError, json.decoder.JSONDecodeError):
                     search_operation.review_manager.logger.debug("Wait for git")
-                    time.sleep(randint(1, 15))
+                    time.sleep(randint(1, 15))  # nosec
 
     def set_id(self, *, record_dict: dict) -> dict:
         """Set incremental record ID
         If self.source_identifier is in record_dict, it is updated, otherwise added as a new record.
         """
 
         if self.source_identifier not in record_dict:
```

### Comparing `colrev-0.8.2/colrev/ops/search_sources.py` & `colrev-0.8.3/colrev/ops/search_sources.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ops/status.py` & `colrev-0.8.3/colrev/ops/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             self.record_links += len([o for o in origin if not o.startswith("md_")])
 
         criteria = list(review_manager.settings.screen.criteria.keys())
         self.screening_statistics = {crit: 0 for crit in criteria}
         for screening_case in self.screening_criteria:
             for criterion in screening_case.split(";"):
                 criterion_name, decision = criterion.split("=")
-                if "out" == decision:
+                if decision == "out":
                     self.screening_statistics[criterion_name] += 1
 
         self.currently = self.StatusStatsCurrently(status_stats=self)
         self.overall = self.StatusStatsOverall(status_stats=self)
 
         self.completed_atomic_steps = 0
         self.nr_incomplete = 0
@@ -269,15 +269,15 @@
                         # ignore _man versions to avoid double-counting:
                         if "_man" not in predecessors[0]["trigger"]:
                             self.completed_atomic_steps += getattr(
                                 self.overall, str(predecessor["dest"])
                             )
                         # Note : load is not a predecessor so we need to
                         # correct for a missing step (same number like prep)
-                        if "prep" == predecessors[0]["trigger"]:
+                        if predecessors[0]["trigger"] == "prep":
                             self.completed_atomic_steps += getattr(
                                 self.overall, str(predecessor["dest"])
                             )
 
             atomic_step_number += 1
             # Note : the following does not consider multiple parallel steps.
             for trans_for_completeness in [
```

### Comparing `colrev-0.8.2/colrev/ops/sync.py` & `colrev-0.8.3/colrev/ops/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                     "number",
                     "pages",
                     "editor",
                 ]
 
                 for ordered_field in field_order:
                     if ordered_field in record_dict:
-                        if "" == record_dict[ordered_field]:
+                        if record_dict[ordered_field] == "":
                             continue
                         if isinstance(record_dict[ordered_field], (list, dict)):
                             continue
                         bibtex_str += format_field(
                             ordered_field, record_dict[ordered_field]
                         )
```

### Comparing `colrev-0.8.2/colrev/ops/trace.py` & `colrev-0.8.3/colrev/ops/trace.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,33 +51,33 @@
                         time.gmtime(commit.committed_date),
                     )
                     + f" {commit} ".ljust(40, " ")
                     + f" {commit_message_first_line} (by {commit.author.name})"
                 )
 
             for diff in diffs:
-                if "add" == diff[0]:
+                if diff[0] == "add":
                     print(
                         colors.GREEN
                         + self.__lpad_multiline(
                             s=self.review_manager.p_printer.pformat(diff),
                             lpad=5,
                         )
                         + colors.END
                     )
-                if "change" == diff[0]:
+                if diff[0] == "change":
                     print(
                         colors.ORANGE
                         + self.__lpad_multiline(
                             s=self.review_manager.p_printer.pformat(diff),
                             lpad=5,
                         )
                         + colors.END
                     )
-                if "delete" == diff[0]:
+                if diff[0] == "delete":
                     print(
                         colors.RED
                         + self.__lpad_multiline(
                             s=self.review_manager.p_printer.pformat(diff),
                             lpad=5,
                         )
                         + colors.END
```

### Comparing `colrev-0.8.2/colrev/ops/upgrade.py` & `colrev-0.8.3/colrev/ops/upgrade.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import shutil
 import typing
 from importlib.metadata import version
 from pathlib import Path
 
 import git
+from tqdm import tqdm
 
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
 import colrev.operation
 import colrev.ui_cli.cli_colors as colors
 
 if False:  # pylint: disable=using-constant-test
@@ -82,62 +83,73 @@
         if settings_version < CoLRevVersion("0.7.0"):
             settings_version = CoLRevVersion("0.7.0")
         installed_colrev_version = CoLRevVersion(version("colrev"))
 
         if installed_colrev_version == settings_version:
             return
 
+        # version: indicates from which version on the migration should be applied
         migration_scripts: typing.List[typing.Dict[str, typing.Any]] = [
             {
                 "version": CoLRevVersion("0.7.0"),
                 "script": self.__migrate_0_7_0,
                 "released": True,
             },
             {
                 "version": CoLRevVersion("0.7.1"),
                 "script": self.__migrate_0_7_1,
                 "released": True,
             },
             # Note : we may add a flag to update to pre-released versions
             {
                 "version": CoLRevVersion("0.8.0"),
+                "target_version": CoLRevVersion("0.8.1"),
                 "script": self.__migrate_0_8_0,
                 "released": True,
             },
             {
                 "version": CoLRevVersion("0.8.1"),
+                "target_version": CoLRevVersion("0.8.2"),
                 "script": self.__migrate_0_8_1,
                 "released": True,
             },
+            {
+                "version": CoLRevVersion("0.8.2"),
+                "target_version": CoLRevVersion("0.8.3"),
+                "script": self.__migrate_0_8_2,
+                "released": True,
+            },
         ]
 
         # Note: we should always update the colrev_version in settings.json because the
         # checker.__check_software requires the settings version and
         # the installed version to be identical
 
         # skipping_versions_before_settings_version = True
         run_migration = False
         while migration_scripts:
             migrator = migration_scripts.pop(0)
-
-            # Activate run_migration after the current settings_version
-            if migrator["version"] == settings_version:
+            # Activate run_migration for the current settings_version
+            if (
+                settings_version == migrator["version"]
+            ):  # settings_version == migrator["version"] or
                 run_migration = True
-                continue
             if not run_migration:
                 continue
 
             migration_script = migrator["script"]
+            self.review_manager.logger.info(
+                "Upgrade to: %s", migrator["target_version"]
+            )
+            if migrator["released"]:
+                self.__print_release_notes(selected_version=migrator["target_version"])
 
             updated = migration_script()
             if not updated:
                 continue
-            self.review_manager.logger.info("Update to: %s", migrator["version"])
-            if migrator["released"]:
-                self.__print_release_notes(selected_version=migrator["version"])
 
         settings = self.__load_settings_dict()
         settings["project"]["colrev_version"] = str(installed_colrev_version)
         self.__save_settings(settings)
 
         if self.repo.is_dirty():
             msg = f"Upgrade to CoLRev {installed_colrev_version}"
@@ -155,15 +167,15 @@
         active, printed = False, False
         if filedata:
             for line in filedata.decode("utf-8").split("\n"):
                 if str(selected_version) in line:
                     active = True
                     print(f"{colors.ORANGE}Release notes v{selected_version}")
                     continue
-                if "## [" in line:
+                if line.startswith("## "):
                     active = False
                 if active:
                     print(line)
                     printed = True
         if not printed:
             print(f"{colors.ORANGE}No release notes")
         print(f"{colors.END}")
@@ -255,14 +267,34 @@
 
         settings = self.__load_settings_dict()
         settings["project"]["auto_upgrade"] = True
         self.__save_settings(settings)
 
         return self.repo.is_dirty()
 
+    def __migrate_0_8_2(self) -> bool:
+        records = self.review_manager.dataset.load_records_dict()
+
+        for record_dict in tqdm(records.values()):
+            if "colrev_pdf_id" not in record_dict:
+                continue
+            if not record_dict["colrev_pdf_id"].startswith("cpid1:"):
+                continue
+            if not Path(record_dict.get("file", "")).is_file():
+                continue
+
+            pdf_path = Path(record_dict["file"])
+            colrev_pdf_id = colrev.record.Record.get_colrev_pdf_id(pdf_path=pdf_path)
+            record_dict["colrev_pdf_id"] = colrev_pdf_id
+
+        self.review_manager.dataset.save_records_dict(records=records)
+        self.review_manager.dataset.add_record_changes()
+
+        return self.repo.is_dirty()
+
 
 class CoLRevVersion:
     """Class for handling the CoLRev version"""
 
     def __init__(self, version_string: str) -> None:
         if "+" in version_string:
             version_string = version_string[: version_string.find("+")]
```

### Comparing `colrev-0.8.2/colrev/ops/validate.py` & `colrev-0.8.3/colrev/ops/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                         file.write("\n")
                         file.write(comp_rec.format_bib_style())
                         file.write("\n")
                         file.write(
                             f"colrev dedupe -m {ref_rec_dict['ID']},{comp_rec_dict['ID']}\n\n"
                         )
 
-        if "" == merge_candidates_file.read_text(encoding="utf-8"):
+        if merge_candidates_file.read_text(encoding="utf-8") == "":
             merge_candidates_file.unlink()
 
         # sort according to similarity
         change_diff.sort(key=lambda x: x["change_score"], reverse=True)
 
         return change_diff
 
@@ -433,15 +433,15 @@
             except ValueError:
                 for commit_candidate in git_repo.iter_commits():
                     if str(commit_candidate.tree) == scope:
                         commit = commit_candidate.hexsha
                         break
                     valid_options.append(str(commit_candidate.tree))
 
-                if "" == commit:
+                if commit == "":
                     # pylint: disable=raise-missing-from
                     raise colrev_exceptions.ParameterError(
                         parameter="validate.scope", value=scope, options=valid_options
                     )
 
         if not re.match(r"[0-9a-f]{5,40}", commit):
             raise colrev_exceptions.ParameterError(
@@ -536,19 +536,19 @@
         validation_details: typing.Dict[str, typing.Any] = {}
         if properties:
             validation_details["properties"] = self.validate_properties(
                 commit=target_commit
             )
             return validation_details
 
-        if "all" == filter_setting:
+        if filter_setting == "all":
             filter_setting = self.__set_scope_based_on_target_commit(
                 target_commit=target_commit
             )
-        if "general" == filter_setting:
+        if filter_setting == "general":
             validation_details["general"] = {
                 "commit": target_commit,
                 "commit_relative": self.__get_relative_commit(
                     target_commit=target_commit
                 ),
             }
             return validation_details
```

### Comparing `colrev-0.8.2/colrev/record.py` & `colrev-0.8.3/colrev/record.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from pdfminer.pdfparser import PDFSyntaxError
 from PyPDF2 import PdfFileReader
 from PyPDF2 import PdfFileWriter
 from thefuzz import fuzz
 
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
+import colrev.qm.colrev_id
+import colrev.qm.colrev_pdf_id
 import colrev.ui_cli.cli_colors as colors
 
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.review_manager
@@ -172,25 +174,25 @@
         # pylint: disable=too-many-branches
 
         diff = []
         if identifying_fields_only:
             for selected_tuple in list(
                 dictdiffer.diff(self.get_data(), other_record.get_data())
             ):
-                if "change" == selected_tuple[0]:
+                if selected_tuple[0] == "change":
                     if selected_tuple[1] in self.identifying_field_keys:
                         diff.append(selected_tuple)
-                if "add" == selected_tuple[0]:
+                if selected_tuple[0] == "add":
                     addition_list: typing.Tuple = ("add", "", [])
                     for addition_item in selected_tuple[2]:
                         if addition_item[0] in self.identifying_field_keys:
                             addition_list[2].append(addition_item)
                     if addition_list[2]:
                         diff.append(addition_list)
-                if "remove" == selected_tuple[0]:
+                if selected_tuple[0] == "remove":
                     removal_list: typing.Tuple = ("remove", "", [])
                     for removal_item in selected_tuple[2]:
                         if removal_item[0] in self.identifying_field_keys:
                             removal_list[2].append(removal_item)
                     if removal_list[2]:
                         diff.append(removal_list)
         else:
@@ -215,23 +217,23 @@
             + self.data.get("number", "")
         )
         return bib_formatted
 
     def __save_field_dict(self, *, input_dict: dict, input_key: str) -> list:
         list_to_return = []
         assert input_key in ["colrev_masterdata_provenance", "colrev_data_provenance"]
-        if "colrev_masterdata_provenance" == input_key:
+        if input_key == "colrev_masterdata_provenance":
             for key, value in input_dict.items():
                 if isinstance(value, dict):
                     formated_node = ",".join(
                         sorted(e for e in value["note"].split(",") if "" != e)
                     )
                     list_to_return.append(f"{key}:{value['source']};{formated_node};")
 
-        elif "colrev_data_provenance" == input_key:
+        elif input_key == "colrev_data_provenance":
             for key, value in input_dict.items():
                 if isinstance(value, dict):
                     list_to_return.append(f"{key}:{value['source']};{value['note']};")
 
         return list_to_return
 
     def get_data(self, *, stringify: bool = False) -> dict:
@@ -245,15 +247,15 @@
 
             for key in self.list_fields_keys:
                 if key in data_copy:
                     if key in ["colrev_origin"]:
                         data_copy[key] = sorted(list(set(data_copy[key])))
                     for ind, val in enumerate(data_copy[key]):
                         if len(val) > 0:
-                            if ";" != val[-1]:
+                            if val[-1] != ";":
                                 data_copy[key][ind] = val + ";"
                     data_copy[key] = list_to_str(val=data_copy[key])
 
             for key in self.dict_fields_keys:
                 if key in data_copy:
                     if isinstance(data_copy[key], dict):
                         data_copy[key] = self.__save_field_dict(
@@ -282,14 +284,17 @@
     def set_status(self, *, target_state: RecordState) -> None:
         """Set the record status"""
         if RecordState.md_prepared == target_state:
             # Note : must be after import provenance
             # masterdata_is_complete() relies on "missing" notes/"UNKNOWN" fields
             if not self.masterdata_is_complete():
                 target_state = RecordState.md_needs_manual_preparation
+            if self.has_quality_defects():
+                target_state = RecordState.md_needs_manual_preparation
+        # pylint: disable=direct-status-assign
         self.data["colrev_status"] = target_state
 
     def shares_origins(self, *, other_record: Record) -> bool:
         """Check at least one origin is shared with the other record"""
         return any(
             x in other_record.data.get("colrev_origin", [])
             for x in self.data.get("colrev_origin", [])
@@ -389,21 +394,21 @@
     def change_entrytype(self, *, new_entrytype: str) -> None:
         """Change the ENTRYTYPE"""
         for value in self.data.get("colrev_masterdata_provenance", {}).values():
             if "inconsistent with entrytype" in value["note"]:
                 value["note"] = ""
         self.data["ENTRYTYPE"] = new_entrytype
         if new_entrytype in ["inproceedings", "proceedings"]:
-            if "UNKNOWN" == self.data.get("volume", ""):
+            if self.data.get("volume", "") == "UNKNOWN":
                 self.remove_field(key="volume")
-            if "UNKNOWN" == self.data.get("number", ""):
+            if self.data.get("number", "") == "UNKNOWN":
                 self.remove_field(key="number")
             if "journal" in self.data and "booktitle" not in self.data:
                 self.rename_field(key="journal", new_key="booktitle")
-        elif "article" == new_entrytype:
+        elif new_entrytype == "article":
             if "booktitle" in self.data:
                 self.rename_field(key="booktitle", new_key="journal")
         else:
             raise colrev_exceptions.MissingRecordQualityRuleSpecification(
                 f"No ENTRYTYPE specification ({new_entrytype})"
             )
 
@@ -479,24 +484,24 @@
         if "colrev_masterdata_provenance" not in self.data:
             self.data["colrev_masterdata_provenance"] = {}
         md_p_dict = self.data["colrev_masterdata_provenance"]
 
         for identifying_field_key in self.identifying_field_keys:
             if identifying_field_key in ["author", "title", "year"]:
                 continue
-            if "UNKNOWN" == self.data.get(identifying_field_key, "NA"):
+            if self.data.get(identifying_field_key, "NA") == "UNKNOWN":
                 del self.data[identifying_field_key]
             if identifying_field_key in md_p_dict:
                 note = md_p_dict[identifying_field_key]["note"]
                 if "missing" in note and "not_missing" not in note:
                     md_p_dict[identifying_field_key]["note"] = note.replace(
                         "missing", ""
                     )
 
-        if "article" == self.data["ENTRYTYPE"]:
+        if self.data["ENTRYTYPE"] == "article":
             if "volume" not in self.data:
                 if "volume" in self.data["colrev_masterdata_provenance"]:
                     self.data["colrev_masterdata_provenance"]["volume"][
                         "note"
                     ] = "not_missing"
                     if replace_source:
                         self.data["colrev_masterdata_provenance"]["volume"][
@@ -623,22 +628,22 @@
 
     def __merge_status(self, *, merging_record: Record) -> None:
         """Merge the status with the merging_record"""
 
         if "colrev_status" in merging_record.data:
             # Set both status to the latter in the state model
             if self.data["colrev_status"] < merging_record.data["colrev_status"]:
-                self.data["colrev_status"] = merging_record.data["colrev_status"]
+                self.set_status(target_state=merging_record.data["colrev_status"])
             else:
-                merging_record.data["colrev_status"] = self.data["colrev_status"]
+                merging_record.set_status(target_state=self.data["colrev_status"])
 
     def __get_merging_val(self, *, merging_record: Record, key: str) -> str:
         val = merging_record.data.get(key, "")
 
-        if "" == val:
+        if val == "":
             return ""
         if not val:
             return ""
 
         # do not override provenance, ID, ... fields
         if key in [
             "ID",
@@ -716,15 +721,15 @@
             # and we iterate over the curated record (merging_record) in the next step
             for k in list(self.data.keys()):
                 if k in Record.identifying_field_keys and k != "pages":
                     del self.data[k]
 
         for key in list(merging_record.data.keys()):
             val = self.__get_merging_val(merging_record=merging_record, key=key)
-            if "" == val:
+            if val == "":
                 continue
 
             field_provenance = merging_record.get_field_provenance(
                 key=key, default_source=default_source
             )
             source = field_provenance["source"]
             note = field_provenance["note"]
@@ -826,23 +831,37 @@
                 x in merging_record_a_prov["author"]["source"]
                 for x in preferred_sources
             ):
                 return merging_record.data["author"]
         return record.data["author"]
 
     @classmethod
-    def __select_best_pages(cls, *, default: str, candidate: str) -> str:
-        best_pages = default
-        if "--" in candidate and "--" not in default:
-            best_pages = candidate
+    def __select_best_pages(
+        cls,
+        *,
+        record: Record,
+        merging_record: Record,
+        preferred_sources: list,  # pylint: disable=unused-argument
+    ) -> str:
+        best_pages = record.data["pages"]
+        if "--" in merging_record.data["pages"] and "--" not in record.data["pages"]:
+            best_pages = merging_record.data["pages"]
         return best_pages
 
     @classmethod
-    def __select_best_title(cls, *, default: str, candidate: str) -> str:
-        best_title = default
+    def __select_best_title(
+        cls,
+        *,
+        record: Record,
+        merging_record: Record,
+        preferred_sources: list,  # pylint: disable=unused-argument
+    ) -> str:
+        default = record.data["title"]
+        candidate = merging_record.data["title"]
+        best_title = record.data["title"]
 
         # Note : avoid switching titles
         if default.replace(" - ", ": ") == candidate.replace(" - ", ": "):
             return default
 
         default_upper = colrev.env.utils.percent_upper_chars(default)
         candidate_upper = colrev.env.utils.percent_upper_chars(candidate)
@@ -851,14 +870,38 @@
             # Relatively simple rule...
             # catches cases when default is all upper or title case
             if default_upper > candidate_upper:
                 best_title = candidate
         return best_title
 
     @classmethod
+    def __select_best_journal(
+        cls,
+        *,
+        record: Record,
+        merging_record: Record,
+        preferred_sources: list,  # pylint: disable=unused-argument
+    ) -> str:
+        return cls.__select_best_container_title(
+            default=record.data["journal"], candidate=merging_record.data["journal"]
+        )
+
+    @classmethod
+    def __select_best_booktitle(
+        cls,
+        *,
+        record: Record,
+        merging_record: Record,
+        preferred_sources: list,  # pylint: disable=unused-argument
+    ) -> str:
+        return cls.__select_best_container_title(
+            default=record.data["booktitle"], candidate=merging_record.data["booktitle"]
+        )
+
+    @classmethod
     def __select_best_container_title(cls, *, default: str, candidate: str) -> str:
         best_journal = default
 
         default_upper = colrev.env.utils.percent_upper_chars(default)
         candidate_upper = colrev.env.utils.percent_upper_chars(candidate)
 
         # Simple heuristic to avoid abbreviations
@@ -878,110 +921,60 @@
         val: str,
         source: str,
         note: str,  # pylint: disable=unused-argument
     ) -> None:
         # Note : the assumption is that we need masterdata_provenance notes
         # only for authors
 
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
+        custom_field_selectors = {
+            "author": self.__select_best_author,
+            "pages": self.__select_best_pages,
+            "title": self.__select_best_title,
+            "journal": self.__select_best_journal,
+            "booktitle": self.__select_best_booktitle,
+        }
 
-        if "author" == key:
+        if key in custom_field_selectors:
             if key in self.data:
-                best_author = self.__select_best_author(
+                best_value = custom_field_selectors[key](
                     record=self,
                     merging_record=merging_record,
                     preferred_sources=self.preferred_sources,
                 )
-                if self.data[key] != best_author:
+                if self.data[key] != best_value:
                     self.update_field(
-                        key=key, value=best_author, source=source, append_edit=False
+                        key=key, value=best_value, source=source, append_edit=False
                     )
             else:
                 self.update_field(key=key, value=val, source=source, append_edit=False)
 
-        elif "pages" == key:
-            if key in self.data:
-                best_pages = self.__select_best_pages(
-                    default=self.data[key], candidate=merging_record.data[key]
-                )
-                if self.data[key] != best_pages:
-                    self.update_field(
-                        key=key, value=best_pages, source=source, append_edit=False
-                    )
-
-            else:
-                self.update_field(key=key, value=val, source=source, append_edit=False)
-
-        elif "title" == key:
-            if key in self.data:
-                best_title = self.__select_best_title(
-                    default=self.data[key], candidate=merging_record.data[key]
-                )
-                if self.data[key] != best_title:
-                    self.update_field(
-                        key=key, value=best_title, source=source, append_edit=False
-                    )
-
-            else:
-                self.update_field(key=key, value=val, source=source, append_edit=False)
-
-        elif "journal" == key:
-            if key in self.data:
-                best_journal = self.__select_best_container_title(
-                    default=self.data[key],
-                    candidate=merging_record.data[key],
-                )
-                if self.data[key] != best_journal:
-                    self.update_field(
-                        key=key, value=best_journal, source=source, append_edit=False
-                    )
-            else:
-                self.update_field(key=key, value=val, source=source)
-
-        elif "booktitle" == key:
-            if key in self.data:
-                best_booktitle = self.__select_best_container_title(
-                    default=self.data[key],
-                    candidate=merging_record.data[key],
-                )
-                if self.data[key] != best_booktitle:
-                    # TBD: custom select_best_booktitle?
-                    self.update_field(
-                        key=key, value=best_booktitle, source=source, append_edit=False
-                    )
-
-            else:
-                self.update_field(key=key, value=val, source=source, append_edit=False)
-
-        elif "file" == key:
+        elif key == "file":
             if key in self.data:
                 self.data[key] = self.data[key] + ";" + merging_record.data.get(key, "")
             else:
                 self.data[key] = merging_record.data[key]
         elif key in ["url", "link"]:
-            if key in self.data:
-                if self.data[key].rstrip("/") != merging_record.data[key].rstrip("/"):
-                    if "https" not in self.data[key]:
-                        self.update_field(
-                            key=key, value=val, source=source, append_edit=False
-                        )
+            if (
+                key in self.data
+                and self.data[key].rstrip("/") != merging_record.data[key].rstrip("/")
+                and "https" not in self.data[key]
+            ):
+                self.update_field(key=key, value=val, source=source, append_edit=False)
 
         elif "UNKNOWN" == self.data.get(
             key, ""
         ) and "UNKNOWN" != merging_record.data.get(key, ""):
             self.data[key] = merging_record.data[key]
-
             if key in self.identifying_field_keys:
                 self.add_masterdata_provenance(key=key, source=source)
             else:
                 self.add_data_provenance(key=key, source=source)
 
-        elif "UNKNOWN" == merging_record.data.get(key, "UNKNOWN"):
-            pass
+        # elif merging_record.data.get(key, "UNKNOWN") == "UNKNOWN":
+        #     pass
         # Note : the following is deactivated to avoid frequent changes in merged records
         # else:
         #     try:
         #         if key in self.identifying_field_keys:
         #             source = merging_record.data["colrev_masterdata_provenance"][key][
         #                 "source"
         #             ]
@@ -1236,20 +1229,28 @@
                 self.data["colrev_masterdata_provenance"][key]["note"] += f",{note}"
         else:
             self.data["colrev_masterdata_provenance"][key] = {
                 "source": "ORIGINAL",
                 "note": note,
             }
 
+        existing_note = self.data["colrev_masterdata_provenance"][key]["note"]
+        if "quality_defect" in existing_note and any(
+            x in existing_note for x in ["missing", "disagreement"]
+        ):
+            self.data["colrev_masterdata_provenance"][key]["note"] = (
+                existing_note.replace("quality_defect", "").rstrip(",").lstrip(",")
+            )
+
     def add_data_provenance_note(self, *, key: str, note: str) -> None:
         """Add a data provenance note (based on a key)"""
         if "colrev_data_provenance" not in self.data:
             self.data["colrev_data_provenance"] = {}
         if key in self.data["colrev_data_provenance"]:
-            if "" == self.data["colrev_data_provenance"][key]["note"]:
+            if self.data["colrev_data_provenance"][key]["note"] == "":
                 self.data["colrev_data_provenance"][key]["note"] = note
             elif note not in self.data["colrev_data_provenance"][key]["note"].split(
                 ","
             ):
                 self.data["colrev_data_provenance"][key]["note"] += f",{note}"
         else:
             self.data["colrev_data_provenance"][key] = {
@@ -1262,15 +1263,15 @@
     ) -> None:
         """Add a masterdata provenance, including source and note (based on a key)"""
         if "colrev_masterdata_provenance" not in self.data:
             self.data["colrev_masterdata_provenance"] = {}
         md_p_dict = self.data["colrev_masterdata_provenance"]
 
         if key in md_p_dict:
-            if "" == md_p_dict[key]["note"] or "" == note:
+            if md_p_dict[key]["note"] == "" or "" == note:
                 md_p_dict[key]["note"] = note
             elif "missing" == note and "not_missing" in md_p_dict[key]["note"].split(
                 ","
             ):
                 md_p_dict[key]["note"] = "missing"
             elif note not in md_p_dict[key]["note"].split(","):
                 md_p_dict[key]["note"] += f",{note}"
@@ -1306,15 +1307,15 @@
 
     def add_data_provenance(self, *, key: str, source: str, note: str = "") -> None:
         """Add a data provenance, including source and note (based on a key)"""
         if "colrev_data_provenance" not in self.data:
             self.data["colrev_data_provenance"] = {}
         md_p_dict = self.data["colrev_data_provenance"]
         if key in md_p_dict:
-            if "" != note:
+            if note != "":
                 md_p_dict[key]["note"] += f",{note}"
             else:
                 md_p_dict[key]["note"] = ""
             md_p_dict[key]["source"] = source
         else:
             md_p_dict[key] = {"source": source, "note": f"{note}"}
 
@@ -1347,88 +1348,103 @@
         """Get the list of incomplete fields"""
         incomplete_field_keys = set()
         for key in self.data.keys():
             if key in ["title", "journal", "booktitle", "author"]:
                 if self.data[key].endswith("...") or self.data[key].endswith("…"):
                     incomplete_field_keys.add(key)
 
-            if "author" == key:
+            if key == "author":
                 if (
                     self.data[key].endswith("and others")
                     or self.data[key].endswith("et al.")
                     # heuristics for missing first names:
                     or ", and " in self.data[key]
                     or self.data[key].rstrip().endswith(",")
                 ):
                     incomplete_field_keys.add(key)
 
         return incomplete_field_keys
 
     def get_quality_defects(self) -> list:
         """Get the fields (keys) with quality defects"""
 
-        # pylint: disable=too-many-branches
-
-        defect_field_keys = []
-        for key in self.data.keys():
-            if "UNKNOWN" == self.data[key]:
-                continue
-            if "author" == key:
-                sanitized_authors = re.sub(
-                    "[^a-zA-Z, ;1]+",
-                    "",
-                    colrev.env.utils.remove_accents(input_str=self.data[key]),
-                ).split(" and ")
-                if not all(
-                    re.findall(
-                        r"^[\w .'’-]*, [\w .'’-]*$",
-                        sanitized_author,
-                        re.UNICODE,
-                    )
-                    for sanitized_author in sanitized_authors
-                ):
-                    defect_field_keys.append(key)
-                # At least two capital letters per name
-                elif not all(
-                    re.findall(
-                        r"[A-Z]+",
-                        author_part,
-                        re.UNICODE,
-                    )
-                    for sanitized_author in sanitized_authors
-                    for author_part in sanitized_author.split(",")
-                ):
-                    defect_field_keys.append(key)
+        def get_author_quality_defects(*, defect_field_keys: list) -> None:
+            sanitized_authors = re.sub(
+                "[^a-zA-Z, ;1]+",
+                "",
+                colrev.env.utils.remove_accents(input_str=self.data["author"]),
+            ).split(" and ")
+            if not all(
+                re.findall(
+                    r"^[\w .'’-]*, [\w .'’-]*$",
+                    sanitized_author,
+                    re.UNICODE,
+                )
+                for sanitized_author in sanitized_authors
+            ):
+                defect_field_keys.append("author")
+            # At least two capital letters per name
+            elif not all(
+                re.findall(
+                    r"[A-Z]+",
+                    author_part,
+                    re.UNICODE,
+                )
+                for sanitized_author in sanitized_authors
+                for author_part in sanitized_author.split(",")
+            ):
+                defect_field_keys.append("author")
 
-                # Note : patterns like "I N T R O D U C T I O N"
-                # that may result from grobid imports
-                elif re.search(r"[A-Z] [A-Z] [A-Z] [A-Z]", self.data[key]):
-                    defect_field_keys.append(key)
-                elif len(self.data[key]) < 5:
-                    defect_field_keys.append(key)
-                elif any(x in str(self.data[key]) for x in ["�", "http", "University"]):
-                    defect_field_keys.append(key)
+            # Note : patterns like "I N T R O D U C T I O N"
+            # that may result from grobid imports
+            elif re.search(r"[A-Z] [A-Z] [A-Z] [A-Z]", self.data["author"]):
+                defect_field_keys.append("author")
+            elif len(self.data["author"]) < 5:
+                defect_field_keys.append("author")
+            elif any(
+                x in str(self.data["author"]) for x in ["�", "http", "University", "™"]
+            ):
+                defect_field_keys.append("author")
 
-            if "title" == key:
-                # Note : titles that have no space and special characters
-                # like _ . or digits.
-                if " " not in self.data[key] and (
-                    any(x in self.data[key] for x in ["_", "."])
-                    or any(char.isdigit() for char in self.data[key])
-                ):
-                    defect_field_keys.append(key)
-                if "�" in str(self.data[key]):
-                    defect_field_keys.append(key)
+        def get_title_quality_defects(*, defect_field_keys: list) -> None:
+            # Note : titles that have no space and special characters
+            # like _ . or digits.
+            if " " not in self.data["title"] and (
+                any(x in self.data["title"] for x in ["_", "."])
+                or any(char.isdigit() for char in self.data["title"])
+            ):
+                defect_field_keys.append("title")
+            if "�" in str(self.data["title"]):
+                defect_field_keys.append("title")
 
+        def get_general_quality_defects(*, key: str, defect_field_keys: list) -> None:
             if key in ["title", "author", "journal", "booktitle"]:
                 if colrev.env.utils.percent_upper_chars(self.data[key]) > 0.8:
                     defect_field_keys.append(key)
                 if "�" in str(self.data[key]):
                     defect_field_keys.append(key)
 
+        defect_field_keys: typing.List[str] = []
+        for key in self.data.keys():
+            if self.data[key] == "UNKNOWN":
+                continue
+
+            if key == "author":
+                get_author_quality_defects(defect_field_keys=defect_field_keys)
+
+            if key == "title":
+                get_title_quality_defects(defect_field_keys=defect_field_keys)
+
+            get_general_quality_defects(key=key, defect_field_keys=defect_field_keys)
+
+        if "colrev_masterdata_provenance" in self.data:
+            for field, provenance in self.data["colrev_masterdata_provenance"].items():
+                if any(x in provenance["note"] for x in ["disagreement", "missing"]):
+                    defect_field_keys.append(field)
+
         return list(set(defect_field_keys))
 
     def has_quality_defects(self) -> bool:
         """Check whether a record has quality defects"""
         return len(self.get_quality_defects()) > 0
 
     def remove_quality_defect_notes(self) -> None:
@@ -1443,205 +1459,42 @@
 
     def get_container_title(self) -> str:
         """Get the record's container title (journal name, booktitle, etc.)"""
         container_title = "NA"
         if "ENTRYTYPE" not in self.data:
             container_title = self.data.get("journal", self.data.get("booktitle", "NA"))
         else:
-            if "article" == self.data["ENTRYTYPE"]:
+            if self.data["ENTRYTYPE"] == "article":
                 container_title = self.data.get("journal", "NA")
-            if "inproceedings" == self.data["ENTRYTYPE"]:
+            if self.data["ENTRYTYPE"] == "inproceedings":
                 container_title = self.data.get("booktitle", "NA")
-            if "book" == self.data["ENTRYTYPE"]:
+            if self.data["ENTRYTYPE"] == "book":
                 container_title = self.data.get("title", "NA")
-            if "inbook" == self.data["ENTRYTYPE"]:
+            if self.data["ENTRYTYPE"] == "inbook":
                 container_title = self.data.get("booktitle", "NA")
         return container_title
 
     def create_colrev_id(
         self,
         *,
         also_known_as_record: Optional[dict] = None,
         assume_complete: bool = False,
     ) -> str:
         """Returns the colrev_id of the Record.
         If a also_known_as_record is provided, it returns the colrev_id of the
         also_known_as_record (using the Record as the reference to decide whether
         required fields are missing)"""
-
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
-
         if also_known_as_record is None:
             also_known_as_record = {}
 
-        def format_author_field_for_cid(input_string: str) -> str:
-            input_string = input_string.replace("\n", " ").replace("'", "")
-            names = input_string.replace("; ", " and ").split(" and ")
-            author_list = []
-            for name in names:
-                if "," == name.rstrip()[-1:]:
-                    # if last-names only (eg, "Webster, and Watson, ")
-                    if len(name[:-2]) > 1:
-                        author_list.append(str(name.rstrip()[:-1]))
-                else:
-                    parsed_name = HumanName(name)
-
-                    if "" == parsed_name.last and "" != parsed_name.first:
-                        author_list.append(parsed_name.first)
-                        continue
-
-                    # Note: do not set parsed_name.string_format as a global constant
-                    # to preserve consistent creation of identifiers
-                    parsed_name.string_format = "{last} "
-                    if len(parsed_name.middle) > 0:
-                        parsed_name.middle = parsed_name.middle[:1]
-                    if len(parsed_name.first) > 0:
-                        parsed_name.first = parsed_name.first[:1]
-                    if len(parsed_name.nickname) > 0:
-                        parsed_name.nickname = ""
-
-                    if len(str(parsed_name)) > 1:
-                        author_list.append(str(parsed_name))
-
-            return " ".join(author_list)
-
-        def get_container_title(*, record_dict: dict) -> str:
-            # Note: custom get_container_title for the colrev_id
-
-            # school as the container title for theses
-            if record_dict["ENTRYTYPE"] in ["phdthesis", "masterthesis"]:
-                container_title = record_dict["school"]
-            # for technical reports
-            elif "techreport" == record_dict["ENTRYTYPE"]:
-                container_title = record_dict["institution"]
-            elif "inproceedings" == record_dict["ENTRYTYPE"]:
-                container_title = record_dict["booktitle"]
-            elif "article" == record_dict["ENTRYTYPE"]:
-                container_title = record_dict["journal"]
-            elif "series" in record_dict:
-                container_title = record_dict["series"]
-            elif "url" in record_dict:
-                container_title = record_dict["url"]
-            else:
-                raise KeyError
-
-            return container_title
-
-        def robust_append(*, input_string: str, to_append: str) -> str:
-            input_string = str(input_string)
-            to_append = str(to_append).replace("\n", " ").replace("/", " ")
-            to_append = to_append.rstrip().lstrip().replace("–", " ")
-            to_append = to_append.replace("emph{", "")
-            to_append = to_append.replace("&amp;", "and")
-            to_append = to_append.replace(" & ", " and ")
-            to_append = colrev.env.utils.remove_accents(input_str=to_append)
-            to_append = re.sub("[^0-9a-zA-Z -]+", "", to_append)
-            to_append = re.sub(r"\s+", "-", to_append)
-            to_append = re.sub(r"-+", "-", to_append)
-            to_append = to_append.lower()
-            if len(to_append) > 1:
-                to_append = to_append.rstrip("-")
-            input_string = input_string + "|" + to_append
-            return input_string
-
-        if not assume_complete:
-            if self.data.get("colrev_status", "NA") in [
-                RecordState.md_imported,
-                RecordState.md_needs_manual_preparation,
-            ]:
-                if len(also_known_as_record) != 0:
-                    raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                        msg="cannot determine field requirements "
-                        "(e.g., volume/number for journal articles)",
-                        missing_fields=["colrev_status/field_requirements"],
-                    )
-            # Make sure that colrev_ids are not generated when
-            # identifying_field_keys are UNKNOWN but possibly required
-            for identifying_field_key in self.identifying_field_keys:
-                if "UNKNOWN" == self.data.get(identifying_field_key, ""):
-                    raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                        msg=f"{identifying_field_key} unknown (maybe required)",
-                        missing_fields=[identifying_field_key],
-                    )
-
-        if len(also_known_as_record) == 0:
-            record_dict = self.data
-        else:
-            required_fields_keys = self.record_field_requirements["other"]
-            if self.data["ENTRYTYPE"] in self.record_field_requirements:
-                required_fields_keys = self.record_field_requirements[
-                    self.data["ENTRYTYPE"]
-                ]
-
-            missing_field_keys = [
-                f for f in required_fields_keys if f not in also_known_as_record
-            ]
-            if len(missing_field_keys) > 0:
-                raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                    msg="Missing fields:" + ",".join(missing_field_keys),
-                    missing_fields=missing_field_keys,
-                )
-            record_dict = also_known_as_record
-
-        try:
-            # Including the version of the identifier prevents cases
-            # in which almost all identifiers are identical
-            # (and very few identifiers change)
-            # when updating the identifier function function
-            # (this may look like an anomaly and be hard to identify)
-            srep = "colrev_id1:"
-            if "article" == record_dict["ENTRYTYPE"].lower():
-                srep = robust_append(input_string=srep, to_append="a")
-            elif "inproceedings" == record_dict["ENTRYTYPE"].lower():
-                srep = robust_append(input_string=srep, to_append="p")
-            else:
-                srep = robust_append(
-                    input_string=srep, to_append=record_dict["ENTRYTYPE"].lower()
-                )
-            srep = robust_append(
-                input_string=srep,
-                to_append=get_container_title(record_dict=record_dict),
-            )
-            if "article" == record_dict["ENTRYTYPE"]:
-                # Note: volume/number may not be required.
-                srep = robust_append(
-                    input_string=srep, to_append=record_dict.get("volume", "-")
-                )
-                srep = robust_append(
-                    input_string=srep, to_append=record_dict.get("number", "-")
-                )
-            srep = robust_append(input_string=srep, to_append=record_dict["year"])
-            author = format_author_field_for_cid(record_dict["author"])
-            if "" == author.replace("-", ""):
-                raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                    msg="Missing field:", missing_fields=["author"]
-                )
-            srep = robust_append(input_string=srep, to_append=author)
-            srep = robust_append(input_string=srep, to_append=record_dict["title"])
-
-            # Note : pages not needed.
-            # pages = record_dict.get("pages", "")
-            # srep = robust_append(srep, pages)
-        except KeyError as exc:
-            if "ENTRYTYPE" in str(exc):
-                print(f"Missing ENTRYTYPE in {record_dict['ID']}")
-            raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                msg="Missing field:" + str(exc), missing_fields=["ENTRYTYPE"]
-            )
-
-        srep = srep.replace(";", "")  # ";" is the separator in colrev_id list
-
-        # Safeguard against titles that are rarely distinct
-        if any(x in srep for x in ["|minitrack-introduction|"]):
-            raise colrev_exceptions.NotEnoughDataToIdentifyException(
-                msg="Title typically non-distinct", missing_fields=["title"]
-            )
-
-        return srep
+        return colrev.qm.colrev_id.create_colrev_id(
+            record=self,
+            also_known_as_record=also_known_as_record,
+            assume_complete=assume_complete,
+        )
 
     def prescreen_exclude(self, *, reason: str, print_warning: bool = False) -> None:
         """Prescreen-exclude a record"""
         # Warn when setting rev_synthesized/rev_included to prescreen_excluded
         # Especially in cases in which the prescreen-exclusion decision
         # is revised (e.g., because a paper was retracted)
         # In these cases, the paper may already be in the data extraction/synthesis
@@ -1650,15 +1503,15 @@
             RecordState.rev_included,
         ]:
             print(
                 f"\n{colors.RED}Warning: setting paper to prescreen_excluded. Please check and "
                 f"remove from synthesis: {self.data['ID']}{colors.END}\n"
             )
 
-        self.data["colrev_status"] = RecordState.rev_prescreen_excluded
+        self.set_status(target_state=RecordState.rev_prescreen_excluded)
 
         if (
             "retracted" not in self.data.get("prescreen_exclusion", "")
             and "retracted" == reason
             and print_warning
         ):
             print(
@@ -1667,15 +1520,15 @@
             )
 
         self.data["prescreen_exclusion"] = reason
 
         # Note: when records are prescreen-excluded during prep:
         to_drop = []
         for key, value in self.data.items():
-            if "UNKNOWN" == value:
+            if value == "UNKNOWN":
                 to_drop.append(key)
         for key in to_drop:
             self.remove_field(key=key)
 
     def extract_text_by_page(
         self, *, pages: Optional[list] = None, project_path: Path
     ) -> str:
@@ -1759,25 +1612,19 @@
             with open(save_to_path / filepath.name, "wb") as outfile:
                 writer_cp.write(outfile)
 
     @classmethod
     def get_colrev_pdf_id(
         cls,
         *,
-        review_manager: colrev.review_manager.ReviewManager,
         pdf_path: Path,
     ) -> str:  # pragma: no cover
         """Generate the colrev_pdf_id"""
-        pdf_hash_service = review_manager.get_pdf_hash_service()
-        cpid1 = "cpid1:" + pdf_hash_service.get_pdf_hash(
-            pdf_path=pdf_path,
-            page_nr=1,
-            hash_size=32,
-        )
-        return cpid1
+
+        return colrev.qm.colrev_pdf_id.create_colrev_pdf_id(pdf_path=pdf_path)
 
     def apply_fields_keys_requirements(self) -> None:
         """Apply the field key requirements"""
 
         required_fields_keys = self.record_field_requirements["other"]
         if self.data["ENTRYTYPE"] in self.record_field_requirements:
             required_fields_keys = self.record_field_requirements[
@@ -1793,15 +1640,15 @@
                     append_edit=False,
                 )
 
     def get_toc_key(self) -> str:
         """Get the record's toc-key"""
 
         try:
-            if "article" == self.data["ENTRYTYPE"]:
+            if self.data["ENTRYTYPE"] == "article":
                 toc_key = (
                     self.data["journal"]
                     .replace(" ", "-")
                     .replace("\\", "")
                     .replace("&", "and")
                     .lower()
                 )
@@ -1812,15 +1659,15 @@
                 )
                 toc_key += (
                     f"|{self.data['number']}"
                     if ("UNKNOWN" != self.data.get("number", "UNKNOWN"))
                     else "|-"
                 )
 
-            elif "inproceedings" == self.data["ENTRYTYPE"]:
+            elif self.data["ENTRYTYPE"] == "inproceedings":
                 toc_key = (
                     self.data["booktitle"]
                     .replace(" ", "-")
                     .replace("\\", "")
                     .replace("&", "and")
                     .lower()
                     + f"|{self.data.get('year', '')}"
@@ -1909,86 +1756,58 @@
             del self.data["text_from_pdf"]
         if "pages_in_file" in self.data:
             del self.data["pages_in_file"]
 
     def apply_restrictions(self, *, restrictions: dict) -> None:
         """Apply masterdata restrictions to the record"""
 
-        # pylint: disable=too-many-branches
-
-        if "ENTRYTYPE" in restrictions:
-            if restrictions["ENTRYTYPE"] != self.data["ENTRYTYPE"]:
-                self.data["ENTRYTYPE"] = restrictions["ENTRYTYPE"]
-
-        if "author" not in self.data:
-            self.data[
-                "colrev_status"
-            ] = colrev.record.RecordState.md_needs_manual_preparation
-            colrev.record.Record(data=self.data).add_masterdata_provenance(
-                key="author",
-                source="colrev_curation.masterdata_restrictions",
-                note="missing",
-            )
-        if "title" not in self.data:
-            self.data[
-                "colrev_status"
-            ] = colrev.record.RecordState.md_needs_manual_preparation
-            colrev.record.Record(data=self.data).add_masterdata_provenance(
-                key="title",
-                source="colrev_curation.masterdata_restrictions",
-                note="missing",
+        for required_field in ["author", "title", "year"]:
+            if required_field in self.data:
+                continue
+            self.set_status(
+                target_state=colrev.record.RecordState.md_needs_manual_preparation
             )
-        if "year" not in self.data:
-            self.data[
-                "colrev_status"
-            ] = colrev.record.RecordState.md_needs_manual_preparation
             colrev.record.Record(data=self.data).add_masterdata_provenance(
-                key="year",
+                key=required_field,
                 source="colrev_curation.masterdata_restrictions",
                 note="missing",
             )
 
-        if "journal" in restrictions:
-            if restrictions["journal"] != self.data.get("journal", ""):
-                self.data["journal"] = restrictions["journal"]
-
-        if "booktitle" in restrictions:
-            if restrictions["booktitle"] != self.data.get("booktitle", ""):
-                self.data["booktitle"] = restrictions["booktitle"]
+        for exact_match in ["ENTRYTYPE", "journal", "booktitle"]:
+            if exact_match in restrictions:
+                if restrictions[exact_match] != self.data.get(exact_match, ""):
+                    self.data[exact_match] = restrictions[exact_match]
 
         if "volume" in restrictions:
-            if restrictions["volume"]:
-                if "volume" not in self.data:
-                    self.data[
-                        "colrev_status"
-                    ] = colrev.record.RecordState.md_needs_manual_preparation
-                    colrev.record.Record(data=self.data).add_masterdata_provenance(
-                        key="volume",
-                        source="colrev_curation.masterdata_restrictions",
-                        note="missing",
-                    )
+            if restrictions["volume"] and "volume" not in self.data:
+                self.set_status(
+                    target_state=colrev.record.RecordState.md_needs_manual_preparation
+                )
+                colrev.record.Record(data=self.data).add_masterdata_provenance(
+                    key="volume",
+                    source="colrev_curation.masterdata_restrictions",
+                    note="missing",
+                )
 
         if "number" in restrictions:
-            if restrictions["number"]:
-                if "number" not in self.data:
-                    self.data[
-                        "colrev_status"
-                    ] = colrev.record.RecordState.md_needs_manual_preparation
-                    colrev.record.Record(data=self.data).add_masterdata_provenance(
-                        key="number",
-                        source="colrev_curation.masterdata_restrictions",
-                        note="missing",
-                    )
-            else:
-                if "number" in self.data:
-                    self.remove_field(
-                        key="number",
-                        not_missing_note=True,
-                        source="colrev_curation.masterdata_restrictions",
-                    )
+            if restrictions["number"] and "number" not in self.data:
+                self.set_status(
+                    target_state=colrev.record.RecordState.md_needs_manual_preparation
+                )
+                colrev.record.Record(data=self.data).add_masterdata_provenance(
+                    key="number",
+                    source="colrev_curation.masterdata_restrictions",
+                    note="missing",
+                )
+            elif "number" in self.data:
+                self.remove_field(
+                    key="number",
+                    not_missing_note=True,
+                    source="colrev_curation.masterdata_restrictions",
+                )
 
     def update_masterdata_provenance(
         self, *, masterdata_restrictions: Optional[dict] = None
     ) -> None:
         """Update the masterdata provenance"""
         # pylint: disable=too-many-branches
 
@@ -2020,15 +1839,15 @@
                     missing_fields.remove(not_missing_field)
             except colrev_exceptions.MissingRecordQualityRuleSpecification:
                 pass
 
             if masterdata_restrictions:
                 self.apply_restrictions(restrictions=masterdata_restrictions)
 
-            if "forthcoming" == self.data.get("year", ""):
+            if self.data.get("year", "") == "forthcoming":
                 source = "NA"
                 if "year" in self.data["colrev_masterdata_provenance"]:
                     source = self.data["colrev_masterdata_provenance"]["year"]["source"]
                 if "volume" in missing_fields:
                     missing_fields.remove("volume")
                     self.data["colrev_masterdata_provenance"]["volume"] = {
                         "source": source,
@@ -2095,22 +1914,22 @@
         """Print the record for prescreen operations"""
 
         ret_str = f"  ID: {self.data['ID']} ({self.data['ENTRYTYPE']})"
         ret_str += (
             f"\n  {colors.GREEN}{self.data.get('title', 'no title')}{colors.END}"
             f"\n  {self.data.get('author', 'no-author')}"
         )
-        if "article" == self.data["ENTRYTYPE"]:
+        if self.data["ENTRYTYPE"] == "article":
             ret_str += (
                 f"\n  {self.data.get('journal', 'no-journal')} "
                 f"({self.data.get('year', 'no-year')}) "
                 f"{self.data.get('volume', 'no-volume')}"
                 f"({self.data.get('number', '')})"
             )
-        elif "inproceedings" == self.data["ENTRYTYPE"]:
+        elif self.data["ENTRYTYPE"] == "inproceedings":
             ret_str += f"\n  {self.data.get('booktitle', 'no-booktitle')}"
         if "abstract" in self.data:
             lines = textwrap.wrap(self.data["abstract"], 100, break_long_words=False)
             if lines:
                 ret_str += f"\n  Abstract: {lines.pop(0)}\n"
                 ret_str += "\n  ".join(lines) + ""
 
@@ -2143,29 +1962,29 @@
         if "title_not_in_first_pages" in pdf_prep_note["note"]:
             ret_str += f"{colors.RED}{self.data.get('title', 'no title')}{colors.END}\n"
         else:
             ret_str += (
                 f"{colors.GREEN}{self.data.get('title', 'no title')}{colors.END}\n"
             )
 
-        if "article" == self.data["ENTRYTYPE"]:
+        if self.data["ENTRYTYPE"] == "article":
             ret_str += (
                 f"{self.data.get('journal', 'no-journal')} "
                 f"({self.data.get('year', 'no-year')}) "
                 f"{self.data.get('volume', 'no-volume')}"
                 f"({self.data.get('number', '')})"
             )
             if "pages" in self.data:
                 if "nr_pages_not_matching" in pdf_prep_note["note"]:
                     ret_str += f", {colors.RED}pp.{self.data['pages']}{colors.END}\n"
                 else:
                     ret_str += f", pp.{colors.GREEN}{self.data['pages']}{colors.END}\n"
             else:
                 ret_str += "\n"
-        elif "inproceedings" == self.data["ENTRYTYPE"]:
+        elif self.data["ENTRYTYPE"] == "inproceedings":
             ret_str += f"{self.data.get('booktitle', 'no-booktitle')}\n"
         if "abstract" in self.data:
             lines = textwrap.wrap(self.data["abstract"], 100, break_long_words=False)
             ret_str += f"\nAbstract: {lines.pop(0)}\n"
             ret_str += "\n".join(lines) + "\n"
 
         if "url" in self.data:
@@ -2278,24 +2097,20 @@
                 return True
             if self.data["booktitle"].isupper():
                 return True
         # add heuristics? (e.g., Hawaii Int Conf Syst Sci)
         return False
 
     @classmethod
-    def get_retrieval_similarity(
+    def __abbreviate_container_titles(
         cls,
         *,
-        record_original: Record,
-        retrieved_record_original: Record,
-        same_record_type_required: bool = True,
-    ) -> float:
-        """Get the retrieval similarity between the record and a retrieved record"""
-        # pylint: disable=too-many-branches
-
+        record: colrev.record.PrepRecord,
+        retrieved_record: colrev.record.PrepRecord,
+    ) -> None:
         def abbreviate_container(*, record: colrev.record.Record, min_len: int) -> None:
             if "journal" in record.data:
                 record.data["journal"] = " ".join(
                     [x[:min_len] for x in record.data["journal"].split(" ")]
                 )
 
         def get_abbrev_container_min_len(*, record: colrev.record.Record) -> int:
@@ -2306,32 +2121,34 @@
                 )
             if "booktitle" in record.data:
                 min_len = min(
                     len(x) for x in record.data["booktitle"].replace(".", "").split(" ")
                 )
             return min_len
 
-        if same_record_type_required:
-            if record_original.data.get(
-                "ENTRYTYPE", "a"
-            ) != retrieved_record_original.data.get("ENTRYTYPE", "b"):
-                return 0.0
-
-        record = record_original.copy_prep_rec()
-        retrieved_record = retrieved_record_original.copy_prep_rec()
-
         if record.container_is_abbreviated():
             min_len = get_abbrev_container_min_len(record=record)
             abbreviate_container(record=retrieved_record, min_len=min_len)
             abbreviate_container(record=record, min_len=min_len)
         if retrieved_record.container_is_abbreviated():
             min_len = get_abbrev_container_min_len(record=retrieved_record)
             abbreviate_container(record=record, min_len=min_len)
             abbreviate_container(record=retrieved_record, min_len=min_len)
 
+    @classmethod
+    def __prep_records_for_similarity(
+        cls,
+        *,
+        record: colrev.record.PrepRecord,
+        retrieved_record: colrev.record.PrepRecord,
+    ) -> None:
+        cls.__abbreviate_container_titles(
+            record=record, retrieved_record=retrieved_record
+        )
+
         if "title" in record.data:
             record.data["title"] = record.data["title"][:90]
         if "title" in retrieved_record.data:
             retrieved_record.data["title"] = retrieved_record.data["title"][:90]
 
         if "author" in record.data:
             cls.__format_authors_string_for_comparison(record=record)
@@ -2352,22 +2169,45 @@
         elif not (
             "--" in record.data["pages"] and "--" in retrieved_record.data["pages"]
         ):
             record.data["pages"] = "nan"
             retrieved_record.data["pages"] = "nan"
 
         if "year" in record.data and "year" in retrieved_record.data:
-            if "forthcoming" == record.data["year"]:
+            if record.data["year"] == "forthcoming":
                 record.data["year"] = retrieved_record.data["year"]
-            if "forthcoming" == retrieved_record.data["year"]:
+            if retrieved_record.data["year"] == "forthcoming":
                 retrieved_record.data["year"] = record.data["year"]
 
+    @classmethod
+    def get_retrieval_similarity(
+        cls,
+        *,
+        record_original: Record,
+        retrieved_record_original: Record,
+        same_record_type_required: bool = True,
+    ) -> float:
+        """Get the retrieval similarity between the record and a retrieved record"""
+
+        if same_record_type_required:
+            if record_original.data.get(
+                "ENTRYTYPE", "a"
+            ) != retrieved_record_original.data.get("ENTRYTYPE", "b"):
+                return 0.0
+
+        record = record_original.copy_prep_rec()
+        retrieved_record = retrieved_record_original.copy_prep_rec()
+
+        cls.__prep_records_for_similarity(
+            record=record, retrieved_record=retrieved_record
+        )
+
         if "editorial" in record.data.get("title", "NA").lower():
             if not all(x in record.data for x in ["volume", "number"]):
-                return 0
+                return 0.0
 
         similarity = Record.get_record_similarity(
             record_a=record, record_b=retrieved_record
         )
 
         return similarity
 
@@ -2375,17 +2215,17 @@
         """Format the field if it is mostly in upper case"""
         # if not re.match(r"^[a-zA-Z\"\{\} ]+$", self.data[key]):
         #     return
 
         self.data[key] = self.data[key].replace("\n", " ")
 
         if colrev.env.utils.percent_upper_chars(self.data[key]) > 0.8:
-            if "capitalize" == case:
+            if case == "capitalize":
                 self.data[key] = self.data[key].capitalize()
-            if "title" == case:
+            if case == "title":
                 self.data[key] = (
                     self.data[key]
                     .title()
                     .replace(" Of ", " of ")
                     .replace(" For ", " for ")
                     .replace(" The ", " the ")
                     .replace("Ieee", "IEEE")
```

### Comparing `colrev-0.8.2/colrev/review_manager.py` & `colrev-0.8.3/colrev/review_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 import pprint
 import typing
 from dataclasses import asdict
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
+import git
 import requests_cache
 import yaml
 
 import colrev.checker
 import colrev.dataset
 import colrev.env.utils
 import colrev.exceptions as colrev_exceptions
 import colrev.logger
 import colrev.operation
 import colrev.record
 import colrev.settings
+import colrev.ui_cli.cli_colors as colors
 from colrev.exit_codes import ExitCodes
 
 
 class ReviewManager:
     """Class for managing individual CoLRev review project (repositories)"""
 
     # pylint: disable=too-many-instance-attributes
@@ -135,14 +137,21 @@
             # run update before settings/data (which may require changes/fail without update)
             if not skip_upgrade:
                 self.__check_update()
             self.settings = self.load_settings()
             self.dataset = colrev.dataset.Dataset(review_manager=self)
 
         except Exception as exc:  # pylint: disable=broad-except
+            if (self.path / Path(".git")).is_dir():
+                if git.Repo().active_branch.name == "gh-pages":
+                    raise colrev_exceptions.RepoSetupError(
+                        msg="Currently on gh-pages branch. Switch to main: "
+                        + f"{colors.ORANGE}git switch main{colors.END}"
+                    )
+
             if force_mode:
                 if debug_mode:
                     self.logger.debug(exc)
             else:
                 raise exc
 
     def __check_update(self) -> None:
@@ -305,29 +314,30 @@
     def create_commit(
         self,
         *,
         msg: str,
         manual_author: bool = False,
         script_call: str = "",
         saved_args: Optional[dict] = None,
+        skip_status_yaml: bool = False,
     ) -> bool:
         """Create a commit (including a commit report)"""
         import colrev.ops.commit
 
         if self.exact_call and script_call == "":
             script_call = self.exact_call
 
         commit = colrev.ops.commit.Commit(
             review_manager=self,
             msg=msg,
             manual_author=manual_author,
             script_name=script_call,
             saved_args=saved_args,
         )
-        ret = commit.create()
+        ret = commit.create(skip_status_yaml=skip_status_yaml)
         return ret
 
     def get_upgrade(self) -> colrev.ops.upgrade.Upgrade:
         """Get an upgrade object"""
 
         import colrev.ops.upgrade
 
@@ -457,20 +467,14 @@
 
     def get_screenshot_service(self) -> colrev.env.screenshot_service.ScreenshotService:
         """Get the screenshot-service object"""
         import colrev.env.screenshot_service
 
         return colrev.env.screenshot_service.ScreenshotService(review_manager=self)
 
-    def get_pdf_hash_service(self) -> colrev.env.pdf_hash_service.PDFHashService:
-        """Get the pdf-hash-service object"""
-        import colrev.env.pdf_hash_service
-
-        return colrev.env.pdf_hash_service.PDFHashService(logger=self.logger)
-
     @classmethod
     def get_resources(cls) -> colrev.env.resources.Resources:
         """Get a resources object"""
         import colrev.env.resources
 
         return colrev.env.resources.Resources()
```

### Comparing `colrev-0.8.2/colrev/service.py` & `colrev-0.8.3/colrev/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         for instruction in instructions:
             if "cmd" in instruction:
                 cmd = instruction["cmd"]
                 if "priority" in instruction:
                     # Note : colrev load can always be called but we are only interested
                     # in it if data in the search directory changes.
-                    if "colrev load" == cmd and "data/search/" not in event.src_path:
+                    if cmd == "colrev load" and "data/search/" not in event.src_path:
                         return
                     self.service.service_queue.put(
                         {"name": cmd, "cmd": cmd, "priority": "yes"}
                     )
 
 
 class Service:
@@ -171,15 +171,15 @@
 
         item = self.service_queue.get()
         item["cmd"] = item["cmd"].replace("_", "-")
 
         self.previous_command = item["cmd"]
 
         print()
-        if "colrev retrieve" == item["cmd"]:
+        if item["cmd"] == "colrev retrieve":
             search_operation = self.review_manager.get_search_operation()
             search_operation.main(rerun=False)
 
             load_operation = self.review_manager.get_load_operation()
             new_sources = load_operation.get_new_sources(skip_query=True)
             load_operation = self.review_manager.get_load_operation()
             load_operation.main(
@@ -188,74 +188,74 @@
 
             prep_operation = self.review_manager.get_prep_operation()
             prep_operation.main()
 
             dedupe_operation = self.review_manager.get_dedupe_operation()
             dedupe_operation.main()
 
-        elif "colrev search" == item["cmd"]:
+        elif item["cmd"] == "colrev search":
             search_operation = self.review_manager.get_search_operation()
             search_operation.main(selection_str=None, rerun=False)
 
-        elif "colrev load" == item["cmd"]:
+        elif item["cmd"] == "colrev load":
             if len(list(self.review_manager.search_dir.glob("*"))) > 0:
                 self.logger.info("Running %s", item["name"])
 
                 load_operation = self.review_manager.get_load_operation()
                 print()
 
                 new_sources = load_operation.get_new_sources(skip_query=True)
                 load_operation.main(
                     new_sources=new_sources, keep_ids=False, combine_commits=False
                 )
             else:
                 self.service_queue.task_done()
                 return
 
-        elif "colrev prep" == item["cmd"]:
+        elif item["cmd"] == "colrev prep":
             self.logger.info("Running %s", item["name"])
             preparation_operation = self.review_manager.get_prep_operation()
             preparation_operation.main()
-        elif "colrev dedupe" == item["cmd"]:
+        elif item["cmd"] == "colrev dedupe":
             self.logger.info("Running %s", item["name"])
 
             # Note : settings should be
             # simple_dedupe
             # merge_threshold=0.5,
             # partition_threshold=0.8,
             dedupe_operation = self.review_manager.get_dedupe_operation()
             dedupe_operation.main()
 
-        elif "colrev prescreen" == item["cmd"]:
+        elif item["cmd"] == "colrev prescreen":
             self.logger.info("Running %s", item["name"])
             prescreen_operation = self.review_manager.get_prescreen_operation()
             prescreen_operation.include_all_in_prescreen(persist=False)
 
-        elif "colrev pdf-get" == item["cmd"]:
+        elif item["cmd"] == "colrev pdf-get":
             self.logger.info("Running %s", item["name"])
             pdf_get_operation = self.review_manager.get_pdf_get_operation()
             pdf_get_operation.main()
 
-        elif "colrev pdf-prep" == item["cmd"]:
+        elif item["cmd"] == "colrev pdf-prep":
             # this may be solved more elegantly,
             # but we need colrev to link existing pdfs (file field)
 
             self.logger.info("Running %s", item["name"])
             pdf_get_operation = self.review_manager.get_pdf_get_operation()
             pdf_get_operation.main()
 
             pdf_preparation_operation = self.review_manager.get_pdf_prep_operation()
             pdf_preparation_operation.main(batch_size=0)
 
-        elif "colrev screen" == item["cmd"]:
+        elif item["cmd"] == "colrev screen":
             self.logger.info("Running %s", item["name"])
             screen_operation = self.review_manager.get_screen_operation()
             screen_operation.include_all_in_screen(persist=False)
 
-        elif "colrev data" == item["cmd"]:
+        elif item["cmd"] == "colrev data":
             self.logger.info("Running %s", item["name"])
             data_operation = self.review_manager.get_data_operation()
             data_operation.main()
             input("Waiting for synthesis (press enter to continue)")
 
         elif item["cmd"] in [
             '"colrev man-prep"',
```

### Comparing `colrev-0.8.2/colrev/settings.py` & `colrev-0.8.3/colrev/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 class PrescreenSettings(JsonSchemaMixin):
     """Prescreen settings"""
 
     explanation: str
     prescreen_package_endpoints: list
 
     def __str__(self) -> str:
-        return "Prescreen package endoints: " + ",".join(
+        return "- " + ",".join(
             [s["endpoint"] for s in self.prescreen_package_endpoints]
         )
 
 
 # PDF get
 
 
@@ -402,15 +402,15 @@
     pdf_get_package_endpoints: list
 
     pdf_get_man_package_endpoints: list
 
     def __str__(self) -> str:
         return (
             f" - pdf_path_type: {self.pdf_path_type}"
-            + " - "
+            + "\n - "
             + ",".join([s["endpoint"] for s in self.pdf_get_package_endpoints])
         )
 
 
 # PDF prep
 
 
@@ -421,15 +421,15 @@
     keep_backup_of_pdfs: bool
 
     pdf_prep_package_endpoints: list
 
     pdf_prep_man_package_endpoints: list
 
     def __str__(self) -> str:
-        return " - " + ",".join(
+        return "- " + "\n- ".join(
             [s["endpoint"] for s in self.pdf_prep_package_endpoints]
         )
 
 
 # Screen
 
 
@@ -538,15 +538,15 @@
         return False
 
     def __str__(self) -> str:
         return (
             str(self.project)
             + "\nSearch\n"
             + str(self.search)
-            + "\nSources\n"
+            + "\nSources\n- "
             + "\n- ".join([str(s) for s in self.sources])
             + "\nLoad\n"
             + str(self.load)
             + "\nPreparation\n"
             + str(self.prep)
             + "\nDedupe\n"
             + str(self.dedupe)
```

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_data_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_data_script.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_pdf_get_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_pdf_get_script.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_pdf_prep_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_pdf_prep_script.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,14 @@
         self,
         pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep,  # pylint: disable=unused-argument
         record: colrev.record.Record,
         pad: int,  # pylint: disable=unused-argument
     ) -> colrev.record.Record:
         """Prepare the PDF"""
 
-        if random.random() < 0.8:
+        if random.random() < 0.8:  # nosec
             record.add_data_provenance_note(key="file", note="custom_issue_detected")
             record.data.update(
                 colrev_status=colrev.record.RecordState.pdf_needs_manual_preparation
             )
 
         return record
```

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_prep_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_prep_script.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 
 import zope.interface
 from dacite import from_dict
 
 import colrev.operation
 
-# import timeout_decorator
 
 if False:  # pylint: disable=using-constant-test
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         import colrev.ops.prep
 
@@ -30,25 +29,23 @@
         self,
         *,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         settings: dict,
     ) -> None:
         self.settings = from_dict(data_class=self.settings_class, data=settings)
 
-    # Use timeout decorator to limit the execution time of functions
-    # @timeout_decorator.timeout(60, use_signals=False)
     def prepare(
         self,
         prep_operation: colrev.ops.prep.Prep,  # pylint: disable=unused-argument
         record: colrev.record.Record,
     ) -> colrev.record.Record:
         """Update record (metadata)"""
 
         if "journal" in record.data:
-            if "MISQ" == record.data["journal"]:
+            if record.data["journal"] == "MISQ":
                 record.update_field(
                     key="journal", value="MIS Quarterly", source="custom_prep"
                 )
 
         return record
```

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_prescreen_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_prescreen_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         prescreen_operation: colrev.ops.prescreen.Prescreen,
         records: dict,
         split: list,  # pylint: disable=unused-argument
     ) -> dict:
         """Prescreen the record"""
 
         for record in records.values():
-            if random.random() < 0.5:
+            if random.random() < 0.5:  # nosec
                 prescreen_operation.prescreen(
                     record=colrev.record.Record(data=record), prescreen_inclusion=True
                 )
 
             else:
                 prescreen_operation.prescreen(
                     record=colrev.record.Record(data=record), prescreen_inclusion=False
```

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_screen_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_screen_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         for record_dict in screen_data["items"]:
             if len(split) > 0:
                 if record_dict["ID"] not in split:
                     continue
 
             record = colrev.record.Record(data=record_dict)
 
-            if random.random() < 0.5:
+            if random.random() < 0.5:  # nosec
                 if screening_criteria_available:
                     # record criteria
                     pass
                 screen_operation.screen(
                     record=record,
                     screen_inclusion=True,
                     screening_criteria="...",
```

### Comparing `colrev-0.8.2/colrev/template/custom_scripts/custom_search_source_script.py` & `colrev-0.8.3/colrev/template/custom_scripts/custom_search_source_script.py`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/example/30_example_records.bib` & `colrev-0.8.3/colrev/template/example/30_example_records.bib`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/github_pages/index.html` & `colrev-0.8.3/colrev/template/github_pages/index.html`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/init/LICENSE-CC-BY-4.0.txt` & `colrev-0.8.3/colrev/template/init/LICENSE-CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/init/colrev_update.yml` & `colrev-0.8.3/colrev/template/init/colrev_update.yml`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/init/colrev_update_curation.yml` & `colrev-0.8.3/colrev/template/init/colrev_update_curation.yml`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/init/pre-commit-config.yaml` & `colrev-0.8.3/colrev/template/init/pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -27,12 +27,7 @@
         stages: [prepare-commit-msg]
     -   id: colrev-hooks-share
         name: "CoLRev ReviewManager: share"
         entry: colrev-hooks-share
         language: python
         stages: [push]
         pass_filenames: false
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
-    hooks:
-    -   id: check-yaml
-        stages: [commit]
```

### Comparing `colrev-0.8.2/colrev/template/init/settings.json` & `colrev-0.8.3/colrev/template/init/settings.json`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/ops/commit_report_details.txt` & `colrev-0.8.3/colrev/template/ops/commit_report_details.txt`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/ops/predatory_journals_beall.csv` & `colrev-0.8.3/colrev/template/ops/predatory_journals_beall.csv`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/ops/prep_man_curation.ipynb` & `colrev-0.8.3/colrev/template/ops/prep_man_curation.ipynb`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/ops/status.txt` & `colrev-0.8.3/colrev/template/ops/status.txt`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/package_status.json` & `colrev-0.8.3/colrev/template/package_status.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8691620879120878%*

 * *Differences: {"'data'": "{0: {'status': 'MATURING'}, 1: {'package_endpoint_identifier': "*

 * *           "'colrev.structuEXPERIMENTAL', 'status': 'EXPERIMENTAL'}, 2: {'status': 'MATURING'}, 3: "*

 * *           "{'status': 'EXPERIMENTAL'}, 4: {'status': 'MATURING'}, 5: {'status': 'EXPERIMENTAL'}, "*

 * *           "6: {'status': 'MATURING'}, insert: [(7, OrderedDict([('package_endpoint_identifier', "*

 * *           "'colrev.structured'), ('status', 'EXPERIMENTAL')]))]}",*

 * * "'dedupe'": "{0: {'status': 'MATURING'}, 1: {'status': 'EXPERIMENT […]*

```diff
@@ -1,424 +1,432 @@
 {
     "data": [
         {
             "package_endpoint_identifier": "colrev.paper_md",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
-            "package_endpoint_identifier": "colrev.structured",
-            "status": "RED"
+            "package_endpoint_identifier": "colrev.structuEXPERIMENTAL",
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.bibliography_export",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.prisma",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.github_pages",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.obsidian",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.colrev_curation",
-            "status": "ORANGE"
+            "status": "MATURING"
+        },
+        {
+            "package_endpoint_identifier": "colrev.structured",
+            "status": "EXPERIMENTAL"
         }
     ],
     "dedupe": [
         {
             "package_endpoint_identifier": "colrev.simple_dedupe",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.active_learning_training",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.active_learning_automated",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.curation_full_outlet_dedupe",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.curation_missing_dedupe",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ],
     "load_conversion": [
         {
             "package_endpoint_identifier": "colrev.bibtex",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.csv",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.excel",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.zotero_translate",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.md_to_bib",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.bibutils",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "pdf_get": [
         {
             "package_endpoint_identifier": "colrev.unpaywall",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.local_index",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.website_screenshot",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ],
     "pdf_get_man": [
         {
             "package_endpoint_identifier": "colrev.colrev_cli_pdf_get_man",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "pdf_prep": [
         {
             "package_endpoint_identifier": "colrev.pdf_check_ocr",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.remove_coverpage",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.remove_last_page",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.validate_pdf_metadata",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.validate_completeness",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.create_tei",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "pdf_prep_man": [
         {
             "package_endpoint_identifier": "colrev.colrev_cli_pdf_prep_man",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "prep": [
         {
             "package_endpoint_identifier": "colrev.source_specific_prep",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.exclude_complementary_materials",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.exclude_non_latin_alphabets",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.exclude_languages",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.exclude_collections",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.remove_urls_with_500_errors",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.remove_broken_ids",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.global_ids_consistency_check",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.resolve_crossrefs",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_doi_from_sem_scholar",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.get_doi_from_urls",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_doi",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_crossref",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_pubmed",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_europe_pmc",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_dblp",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_open_library",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_citeas",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.get_year_from_vol_iss_jour",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.get_masterdata_from_local_index",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.update_metadata_status",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.general_polish",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.curation_prep",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ],
     "prep_man": [
         {
             "package_endpoint_identifier": "colrev.export_man_prep",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.prep_man_curation_jupyter",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ],
     "prescreen": [
         {
             "package_endpoint_identifier": "colrev.scope_prescreen",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.colrev_cli_prescreen",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.asreview_prescreen",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.conditional_prescreen",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.prescreen_table",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "review_type": [
         {
             "package_endpoint_identifier": "colrev.conceptual_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.curated_masterdata",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.literature_review",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.narrative_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.descriptive_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.scoping_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.critical_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.theoretical_review",
-            "status": "ORANGE"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.qualitative_systematic_review",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.meta_analysis",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.scientometric",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ],
     "screen": [
         {
             "package_endpoint_identifier": "colrev.colrev_cli_screen",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.screen_table",
-            "status": "ORANGE"
+            "status": "MATURING"
         }
     ],
     "search_source": [
         {
+            "package_endpoint_identifier": "colrev.open_library",
+            "status": "EXPERIMENTAL"
+        },
+        {
             "package_endpoint_identifier": "colrev.unknown_source",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.abi_inform_proquest",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.systematic_review_datasets",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.taylor_and_francis",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.ebsco_host",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.crossref",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.dblp",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.europe_pmc",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.acm_digital_library",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.pubmed",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.wiley",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.ieee",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.psycinfo",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.jstor",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.eric",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.springer_link",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.ais_library",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.google_scholar",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.web_of_science",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.scopus",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.pdfs_dir",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.video_dir",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         },
         {
             "package_endpoint_identifier": "colrev.pdf_backward_search",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.open_citations_forward_search",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.colrev_project",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.local_index",
-            "status": "ORANGE"
+            "status": "MATURING"
         },
         {
             "package_endpoint_identifier": "colrev.trid",
-            "status": "RED"
+            "status": "EXPERIMENTAL"
         }
     ]
 }
```

### Comparing `colrev-0.8.2/colrev/template/paper_md/APA-7.docx` & `colrev-0.8.3/colrev/template/paper_md/APA-7.docx`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/paper_md/paper.md` & `colrev-0.8.3/colrev/template/paper_md/paper.md`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/prisma/PRISMA.csv` & `colrev-0.8.3/colrev/template/prisma/PRISMA.csv`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/prisma/PRISMA_original.csv` & `colrev-0.8.3/colrev/template/prisma/PRISMA_original.csv`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/prisma/prisma-refs.bib` & `colrev-0.8.3/colrev/template/prisma/prisma-refs.bib`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/review_type/curated_masterdata/curations_github_colrev_update.yml` & `colrev-0.8.3/colrev/template/review_type/curated_masterdata/curations_github_colrev_update.yml`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/template/review_type/meta_analysis/paper.md` & `colrev-0.8.3/colrev/template/review_type/meta_analysis/paper.md`

 * *Files identical despite different names*

### Comparing `colrev-0.8.2/colrev/ui_cli/add_packages.py` & `colrev-0.8.3/colrev/ui_cli/add_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
     search_source = package_manager.load_packages(
         package_type=colrev.env.package_manager.PackageEndpointType.search_source,
         selected_packages=[{"endpoint": package_identifier}],
         operation=search_operation,
         instantiate_objects=False,
     )
-
-    add_source = search_source[package_identifier].add_endpoint(search_operation, query)  # type: ignore
+    s_obj = search_source[package_identifier]
+    add_source = s_obj.add_endpoint(search_operation, query)  # type: ignore
     search_operation.add_source(add_source=add_source)
 
 
 def add_data(
     *,
     data_operation: colrev.ops.data.Data,
     add: str,
@@ -76,25 +76,25 @@
             selected_packages=[{"endpoint": add}],
             operation=data_operation,
         )
         endpoint = package_endpoints[add]
 
         default_endpoint_conf = endpoint.get_default_setup()  # type: ignore
 
-        if "colrev.paper_md" == add:
-            if "y" == input("Select a custom word template (y/n)?"):
+        if add == "colrev.paper_md":
+            if input("Select a custom word template (y/n)?") == "y":
                 template_name = input(
                     'Please copy the word template to " \
                 "the project directory and enter the filename.'
                 )
                 default_endpoint_conf["word_template"] = template_name
             else:
                 print("Adding APA as a default")
 
-            if "y" == input("Select a custom citation stlye (y/n)?"):
+            if input("Select a custom citation stlye (y/n)?") == "y":
                 print(
                     "Citation stlyes are available at: \n"
                     "https://github.com/citation-style-language/styles"
                 )
                 csl_link = input("Please select a citation style and provide the link.")
                 ret = requests.get(csl_link, allow_redirects=True, timeout=30)
                 with open(Path(csl_link).name, "wb") as file:
```

### Comparing `colrev-0.8.2/colrev/ui_cli/cli.py` & `colrev-0.8.3/colrev/ui_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
     local_pdf_collection: bool,
     verbose: bool,
     force: bool,
 ) -> None:
     """Initialize (define review objectives and type)"""
     # pylint: disable=import-outside-toplevel
     import colrev.ops.init
-    import colrev.ui_web.settings_editor
 
     try:
         colrev.review_manager.get_init_operation(
             review_type=type,
             example=example,
             light=light,
             local_pdf_collection=local_pdf_collection,
@@ -1320,50 +1319,49 @@
     assert Path(cover).suffix == ".pdf"
     record = colrev.record.Record(data={"file": cover})
     record.extract_pages(
         pages=[0], project_path=Path(cover).parent, save_to_path=cp_path
     )
 
 
-def __print_pdf_hashes(
-    *, pdf_prep_operation: colrev.ops.pdf_prep.PDFPrep, pdf_hash: Path
-) -> None:
+def __print_pdf_hashes(*, pdf_path: Path) -> None:
     # pylint: disable=import-outside-toplevel
     from PyPDF2 import PdfFileReader
+    import colrev.qm.colrev_pdf_id
 
-    assert Path(pdf_hash).suffix == ".pdf"
+    try:
+        pdf_reader = PdfFileReader(str(pdf_path), strict=False)
+    except ValueError:
+        print("Could not read PDF")
+        return
 
-    pdf_hash_service = pdf_prep_operation.review_manager.get_pdf_hash_service()
+    assert Path(pdf_path).suffix == ".pdf"
 
-    first_page_average_hash_16 = pdf_hash_service.get_pdf_hash(
-        pdf_path=Path(pdf_hash),
+    first_page_average_hash_16 = colrev.qm.colrev_pdf_id.get_pdf_hash(
+        pdf_path=Path(pdf_path),
         page_nr=1,
         hash_size=16,
     )
     print(f"first page: {first_page_average_hash_16}")
-    first_page_average_hash_32 = pdf_hash_service.get_pdf_hash(
-        pdf_path=Path(pdf_hash),
+    first_page_average_hash_32 = colrev.qm.colrev_pdf_id.get_pdf_hash(
+        pdf_path=Path(pdf_path),
         page_nr=1,
         hash_size=32,
     )
     print(f"first page: {first_page_average_hash_32}")
 
-    try:
-        pdf_reader = PdfFileReader(str(pdf_hash), strict=False)
-    except ValueError:
-        return
     last_page_nr = len(pdf_reader.pages)
-    last_page_average_hash_16 = pdf_hash_service.get_pdf_hash(
-        pdf_path=Path(pdf_hash),
+    last_page_average_hash_16 = colrev.qm.colrev_pdf_id.get_pdf_hash(
+        pdf_path=Path(pdf_path),
         page_nr=last_page_nr,
         hash_size=16,
     )
     print(f"last page: {last_page_average_hash_16}")
-    last_page_average_hash_32 = pdf_hash_service.get_pdf_hash(
-        pdf_path=Path(pdf_hash),
+    last_page_average_hash_32 = colrev.qm.colrev_pdf_id.get_pdf_hash(
+        pdf_path=Path(pdf_path),
         page_nr=last_page_nr,
         hash_size=32,
     )
     print(f"last page: {last_page_average_hash_32}")
 
 
 @main.command(help_priority=14)
@@ -1444,15 +1442,15 @@
     try:
         review_manager = colrev.review_manager.ReviewManager(
             force_mode=force, verbose_mode=verbose, exact_call=EXACT_CALL
         )
         pdf_prep_operation = review_manager.get_pdf_prep_operation(reprocess=reprocess)
 
         if pdf_hash:
-            __print_pdf_hashes(pdf_prep_operation=pdf_prep_operation, pdf_hash=pdf_hash)
+            __print_pdf_hashes(pdf_path=pdf_hash)
 
         elif update_colrev_pdf_ids:
             pdf_prep_operation.update_colrev_pdf_ids()
 
         elif setup_custom_script:
             pdf_prep_operation.setup_custom_script()
             print("Activated custom_pdf_prep_script.py.")
@@ -1483,15 +1481,15 @@
                 )
                 pdf_prep_man_operation.extract_coverpage(filepath=pdf_path)
                 pdf_prep_man_operation.set_pdf_man_prepared(
                     record=colrev.record.Record(data=record_dict)
                 )
             else:
                 print("no file in record")
-        if "n" == input("Extract coverpage from another PDF? (y/n)"):
+        if input("Extract coverpage from another PDF? (y/n)") == "n":
             break
         record_id = input("ID of next PDF for coverpage extraction:")
 
 
 @main.command(help_priority=15)
 @click.option(
     "-dfp",
@@ -1665,15 +1663,15 @@
         if data_operation.review_manager.in_ci_environment():
             if ret["ask_to_commit"]:
                 review_manager.create_commit(
                     msg="Data and synthesis", manual_author=True
                 )
         else:
             if ret["ask_to_commit"]:
-                if "y" == input("Create commit (y/n)?"):
+                if input("Create commit (y/n)?") == "y":
                     review_manager.create_commit(
                         msg="Data and synthesis", manual_author=True
                     )
             if ret["no_endpoints_registered"]:
                 print(
                     "No data format not specified. "
                     "To register a data endpoint, "
@@ -1878,15 +1876,15 @@
     review_manager: colrev.review_manager.ReviewManager,
 ) -> None:
     environment_manager = review_manager.get_environment_manager()
     environment_details = environment_manager.get_environment_details()
 
     print("\nCoLRev environment status\n")
     print("Index\n")
-    if "up" == environment_details["index"]["status"]:
+    if environment_details["index"]["status"] == "up":
         print(f" - Status: {colors.GREEN}up{colors.END}")
         print(f' - Path          : {environment_details["index"]["path"]}')
         print(f' - Size          : {environment_details["index"]["size"]} records')
         print(f' - Last modified : {environment_details["index"]["last_modified"]}')
     else:
         print(f" - Status: {colors.RED}down{colors.END}")
 
@@ -2183,23 +2181,23 @@
         with open("settings.json", "w", encoding="utf-8") as outfile:
             json.dump(project_settings, outfile, indent=4)
 
         review_manager.dataset.add_changes(path=Path("settings.json"))
         review_manager.create_commit(msg="Change settings", manual_author=True)
         return
 
-    import colrev.ui_web.settings_editor
+    # import colrev_ui.ui_web.settings_editor
 
-    review_manager = colrev.review_manager.ReviewManager(
-        force_mode=True, verbose_mode=verbose
-    )
-    settings_operation = colrev.ui_web.settings_editor.SettingsEditor(
-        review_manager=review_manager
-    )
-    settings_operation.open_settings_editor()
+    # review_manager = colrev.review_manager.ReviewManager(
+    #     force_mode=True, verbose_mode=verbose
+    # )
+    # settings_operation = colrev.ui_web.settings_editor.SettingsEditor(
+    #     review_manager=review_manager
+    # )
+    # settings_operation.open_settings_editor()
 
 
 @main.command(help_priority=22)
 @click.option(
     "-v",
     "--verbose",
     is_flag=True,
@@ -2239,18 +2237,18 @@
                 print("\n")
                 print(f"1: {v_1}")
                 print("      " + val[0].data.get("source_url", ""))
                 print("")
                 print(f"2: {v_2}")
                 print("      " + val[1].data.get("source_url", ""))
                 user_selection = input("Import version 1 or 2 (or skip)?")
-                if "1" == user_selection:
+                if user_selection == "1":
                     sync_operation.add_to_records_to_import(record=val[0])
                     continue
-                if "2" == user_selection:
+                if user_selection == "2":
                     sync_operation.add_to_records_to_import(record=val[1])
                     continue
 
     sync_operation.add_to_bib()
 
 
 @main.command(help_priority=23)
@@ -2413,15 +2411,15 @@
         )
         review_manager.get_service_operation()
 
     except KeyboardInterrupt:
         print("\nPressed ctrl-c. Shutting down service")
 
     if review_manager.dataset.has_changes():
-        if "y" == input("Commit current changes (y/n)?"):
+        if input("Commit current changes (y/n)?") == "y":
             review_manager.create_commit(msg="Update (using CoLRev service)")
     else:
         print("No changes to commit")
 
 
 def __validate_show(ctx: click.core.Context, param: str, value: str) -> None:
     if value not in ["sample", "settings", "prisma", "venv"]:
@@ -2455,34 +2453,34 @@
     """Show aspects (sample, ...)"""
     # pylint: disable=too-many-locals
 
     # pylint: disable=import-outside-toplevel
     import colrev.operation
     import colrev.ui_cli.show_printer
 
-    if "venv" == keyword:
+    if keyword == "venv":
         colrev.ui_cli.show_printer.print_venv_notes()
         return
 
     review_manager = colrev.review_manager.ReviewManager(
         force_mode=force, verbose_mode=verbose
     )
 
-    if "sample" == keyword:
+    if keyword == "sample":
         colrev.ui_cli.show_printer.print_sample(review_manager=review_manager)
 
-    elif "settings" == keyword:
+    elif keyword == "settings":
         print(f"Settings:\n{review_manager.settings}")
 
-    elif "prisma" == keyword:
+    elif keyword == "prisma":
         status_operation = review_manager.get_status_operation()
         stats_report = status_operation.get_review_status_report()
         print(stats_report)
 
-    elif "cmd_history" == keyword:
+    elif keyword == "cmd_history":
         cmds = []
         colrev.operation.CheckOperation(review_manager=review_manager)
         revlist = review_manager.dataset.get_repo().iter_commits()
 
         for commit in reversed(list(revlist)):
             try:
                 cmsg = str(commit.message)
@@ -2518,47 +2516,47 @@
         for cmd in cmds:
             print(
                 f"{cmd['date']} ({cmd['committer']}, {cmd['commit_id']}):    "
                 f"{colors.ORANGE}{cmd['cmd']}{colors.END}"
             )
 
 
-@main.command(help_priority=28)
-@click.option(
-    "-v",
-    "--verbose",
-    is_flag=True,
-    default=False,
-    help="Verbose: printing more infos",
-)
-@click.option(
-    "-f",
-    "--force",
-    is_flag=True,
-    default=False,
-    help="Force mode",
-)
-@click.pass_context
-def web(
-    ctx: click.core.Context,
-    verbose: bool,
-    force: bool,
-) -> None:
-    """CoLRev web interface."""
-
-    # pylint: disable=import-outside-toplevel
-    import colrev.ui_web.settings_editor
-
-    review_manager = colrev.review_manager.ReviewManager(
-        force_mode=force, verbose_mode=verbose
-    )
-    se_instance = colrev.ui_web.settings_editor.SettingsEditor(
-        review_manager=review_manager
-    )
-    se_instance.open_settings_editor()
+# @main.command(help_priority=28)
+# @click.option(
+#     "-v",
+#     "--verbose",
+#     is_flag=True,
+#     default=False,
+#     help="Verbose: printing more infos",
+# )
+# @click.option(
+#     "-f",
+#     "--force",
+#     is_flag=True,
+#     default=False,
+#     help="Force mode",
+# )
+# @click.pass_context
+# def web(
+#     ctx: click.core.Context,
+#     verbose: bool,
+#     force: bool,
+# ) -> None:
+#     """CoLRev web interface."""
+
+#     # pylint: disable=import-outside-toplevel
+#     import colrev.ui_web.settings_editor
+
+#     review_manager = colrev.review_manager.ReviewManager(
+#         force_mode=force, verbose_mode=verbose
+#     )
+#     se_instance = colrev.ui_web.settings_editor.SettingsEditor(
+#         review_manager=review_manager
+#     )
+#     se_instance.open_settings_editor()
 
 
 @main.command(hidden=True, help_priority=29)
 @click.option(
     "--disable_auto",
     is_flag=True,
     default=False,
@@ -2773,15 +2771,15 @@
 ) -> None:
     """Undo operations."""
 
     review_manager = colrev.review_manager.ReviewManager(
         force_mode=force, verbose_mode=verbose
     )
 
-    if "commit" == selection:
+    if selection == "commit":
         colrev.operation.CheckOperation(review_manager=review_manager)
         git_repo = review_manager.dataset.get_repo()
         git_repo.git.reset("--hard", "HEAD~1")
 
 
 @main.command(help_priority=35)
 @click.pass_context
```

### Comparing `colrev-0.8.2/colrev/ui_cli/cli_status_printer.py` & `colrev-0.8.3/colrev/ui_cli/cli_status_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,29 +73,29 @@
                 return
 
     print("Versioning and collaboration")
 
     if "status" in collaboration_instructions:
         if "title" in collaboration_instructions["status"]:
             title = collaboration_instructions["status"]["title"]
-            if "WARNING" == collaboration_instructions["status"].get("level", "NA"):
+            if collaboration_instructions["status"].get("level", "NA") == "WARNING":
                 print(f"  {colors.RED}{title}{colors.END}")
-            elif "SUCCESS" == collaboration_instructions["status"].get("level", "NA"):
+            elif collaboration_instructions["status"].get("level", "NA") == "SUCCESS":
                 print(f"  {colors.GREEN}{title}{colors.END}")
             else:
                 print("  " + title)
         if "msg" in collaboration_instructions["status"]:
             print(f'  {collaboration_instructions["status"]["msg"]}')
 
     for item in collaboration_instructions["items"]:
         if "title" in item:
             if "level" in item:
-                if "WARNING" == item["level"]:
+                if item["level"] == "WARNING":
                     print(f'  {colors.RED}{item["title"]}{colors.END}')
-                elif "SUCCESS" == item["level"]:
+                elif item["level"] == "SUCCESS":
                     print(f'  {colors.GREEN}{item["title"]}{colors.END}')
             else:
                 print("  " + item["title"])
 
         if "msg" in item:
             print("  " + item["msg"])
         if "cmd_after" in item:
```

### Comparing `colrev-0.8.2/colrev/ui_cli/cli_validation.py` & `colrev-0.8.3/colrev/ui_cli/cli_validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,22 +43,22 @@
                 validation_item["prior_record_b"],
             ],
             keys=keys,
         )
 
         user_selection = input("Validate [y,n,q for yes, no (undo), or quit]?")
 
-        if "n" == user_selection:
+        if user_selection == "n":
             dedupe_operation.unmerge_records(
                 current_record_ids=validation_item["record"]["ID"]
             )
 
-        if "q" == user_selection:
+        if user_selection == "q":
             break
-        if "y" == user_selection:
+        if user_selection == "y":
             continue
 
 
 def __validate_prep(
     *,
     validate_operation: colrev.operation.Operation,
     validation_details: list,
@@ -74,17 +74,14 @@
     print("Prescreen excluded:")
     for i, validation_detail in enumerate(prescreen_excluded_to_validate):
         print(i)
         colrev.record.Record(
             data=validation_detail["record_dict"]
         ).print_citation_format()
 
-    # TODO : print all, allow users to undo (-> needs_manual_preparation)
-    # by selecting number of record
-
     displayed = False
     for validation_element in validation_details:
         if validation_element["change_score"] < threshold:
             continue
         displayed = True
         # Escape sequence to clear terminal output for each new comparison
         os.system("cls" if os.name == "nt" else "clear")
@@ -109,27 +106,27 @@
                 validation_element["record_dict"],
             ],
             keys=keys,
         )
 
         user_selection = input("Validate [y,n,q for yes, no (undo), or quit]?")
 
-        if "n" == user_selection:
+        if user_selection == "n":
             validate_operation.review_manager.dataset.save_records_dict(
                 records={
                     validation_element["prior_record_dict"]["ID"]: validation_element[
                         "prior_record_dict"
                     ]
                 },
                 partial=True,
             )
 
-        if "q" == user_selection:
+        if user_selection == "q":
             break
-        if "y" == user_selection:
+        if user_selection == "y":
             continue
 
     if not displayed:
         validate_operation.review_manager.logger.info(
             "No preparation changes above threshold"
         )
 
@@ -139,40 +136,40 @@
     validate_operation: colrev.operation.Operation,
     validation_details: dict,
     threshold: float,
 ) -> None:
     """Validate details in the cli"""
 
     for key, details in validation_details.items():
-        if "prep" == key:
+        if key == "prep":
             __validate_prep(
                 validate_operation=validate_operation,
                 validation_details=details,
                 threshold=threshold,
             )
-        elif "dedupe" == key:
+        elif key == "dedupe":
             __validate_dedupe(
                 validate_operation=validate_operation,
                 validation_details=details,
                 threshold=threshold,
             )
-        elif "properties" == key:
+        elif key == "properties":
             validate_operation.review_manager.logger.info(
                 " Traceability of records".ljust(32, " ")
                 + str(details["record_traceability"])
             )
             validate_operation.review_manager.logger.info(
                 " Consistency (based on hooks)".ljust(32, " ")
                 + str(details["consistency"])
             )
             validate_operation.review_manager.logger.info(
                 " Completeness of iteration".ljust(32, " ")
                 + str(details["completeness"])
             )
-        elif "contributor_commits" == key:
+        elif key == "contributor_commits":
             validate_operation.review_manager.logger.info(
                 "Showing commits in which the contributor was involved as the author or committer."
             )
 
             print()
             print("Commits to validate:")
             print()
@@ -185,15 +182,15 @@
                     )
                     print(
                         f"  committer {item_values['committer']} ({item_values['committer_email']})"
                     )
                     print(f"  {colors.ORANGE}{item_values['validate']}{colors.END}")
 
             print()
-        elif "general" == key:
+        elif key == "general":
             validate_operation.review_manager.logger.info("Start general validation")
             validate_operation.review_manager.logger.info(
                 "Next, an interface will open and "
                 "display the changes introduced in the selected commit."
             )
             validate_operation.review_manager.logger.info(
                 "To undo minor changes, edit the corresponding files directly and run "
```

### Comparing `colrev-0.8.2/colrev/ui_cli/show_printer.py` & `colrev-0.8.3/colrev/ui_cli/show_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,37 +28,37 @@
         colrev.record.Record(data=sample_r).print_citation_format()
 
 
 def print_venv_notes() -> None:
     """Print the virtual environment details on cli"""
 
     current_platform = platform.system()
-    if "Linux" == current_platform:
+    if current_platform == "Linux":
         print("Detected platform: Linux")
         if not Path("venv").is_dir():
             print("To create virtualenv, run")
             print(f"  {colors.ORANGE}python3 -m venv venv{colors.END}")
         print("To activate virtualenv, run")
         print(f"  {colors.ORANGE}source venv/bin/activate{colors.END}")
         print("To install colrev/colrev, run")
         print(f"  {colors.ORANGE}python -m pip install colrev{colors.END}")
         print("To deactivate virtualenv, run")
         print(f"  {colors.ORANGE}deactivate{colors.END}")
-    elif "Darwin" == current_platform:
+    elif current_platform == "Darwin":
         print("Detected platform: MacOS")
         if not Path("venv").is_dir():
             print("To create virtualenv, run")
             print(f"  {colors.ORANGE}python3 -m venv venv{colors.END}")
         print("To activate virtualenv, run")
         print(f"  {colors.ORANGE}source venv/bin/activate{colors.END}")
         print("To install colrev/colrev, run")
         print(f"  {colors.ORANGE}python -m pip install colrev{colors.END}")
         print("To deactivate virtualenv, run")
         print(f"  {colors.ORANGE}deactivate{colors.END}")
-    elif "Windows" == current_platform:
+    elif current_platform == "Windows":
         print("Detected platform: Windows")
         if not Path("venv").is_dir():
             print("To create virtualenv, run")
             print(f"  {colors.ORANGE}python -m venv venv{colors.END}")
         print("To activate virtualenv, run")
         print(f"  {colors.ORANGE}venv\\Scripts\\Activate.ps1{colors.END}")
         print("To install colrev/colrev, run")
```

### Comparing `colrev-0.8.2/pyproject.toml` & `colrev-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "colrev"
-version = "0.8.2"
+version = "0.8.3"
 description = "CoLRev: An open-source environment for collaborative reviews"
 authors = ["Gerit Wagner <gerit.wagner@hec.ca>", "Julian Prester <julian.prester@sydney.edu.au>"]
 license = "MIT"
 readme = "README.md"
 homepage="https://colrev.readthedocs.io/en/latest/"
 repository = "https://github.com/CoLRev-Environment/colrev"
 documentation = "https://colrev.readthedocs.io/en/latest/"
@@ -68,14 +68,19 @@
 pre-commit = "^2.20.0"
 Jinja2 = "^3.1.2"
 dataclasses-jsonschema = "^2.15.3"
 Flask = "^2.2.2"
 Flask-Cors = "^3.0.10"
 watchdog = "^2.2.1"
 openpyxl = "^3.1.2"
+pylint = "^2.17.2"
+pymupdf = "^1.22.0"
+imagehash = "^4.3.1"
+defusedxml = "^0.7.1"
+asreview = "^1.2"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.2.3"
 sphinx-autodoc-typehints = "^1.19.4"
 sphinx-click = "^4.3.0"
 sphinx-rtd-theme = "^1.1.1"
 "sphinxcontrib.datatemplates" = "^0.9.2"
```

### Comparing `colrev-0.8.2/PKG-INFO` & `colrev-0.8.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colrev
-Version: 0.8.2
+Version: 0.8.3
 Summary: CoLRev: An open-source environment for collaborative reviews
 Home-page: https://colrev.readthedocs.io/en/latest/
 License: MIT
 Keywords: research,reproducible research,open science,literature,literature review,systematic review,systematic literature review
 Author: Gerit Wagner
 Author-email: gerit.wagner@hec.ca
 Requires-Python: >=3.8,<4
@@ -27,37 +27,42 @@
 Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: GitPython (>=3.1.29,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyPDF2 (>=1.28.6,<2.0.0)
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: alphabet-detector (>=0.0.7,<0.0.8)
+Requires-Dist: asreview (>=1.2,<2.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click8 (>=8.0.1,<9.0.0)
 Requires-Dist: click_completion (>=0.5.2,<0.6.0)
 Requires-Dist: crossrefapi (>=1.5.0,<2.0.0)
 Requires-Dist: cx-Freeze (>=6.11.1,<7.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: daff (>=1.3.46,<2.0.0)
 Requires-Dist: dataclasses-jsonschema (>=2.15.3,<3.0.0)
 Requires-Dist: dedupe (>=2.0.20,<3.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: docker (==6.0.0)
 Requires-Dist: glom (>=22.1.0,<23.0.0)
+Requires-Dist: imagehash (>=4.3.1,<5.0.0)
 Requires-Dist: lingua-language-detector (>1.3)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: nameparser (>=1.1.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pandasql (>=0.7.3,<0.8.0)
 Requires-Dist: pdfminer.six (>=20220524,<20220525)
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0)
 Requires-Dist: psutil (>=5.9.2,<6.0.0)
 Requires-Dist: pybtex (>=0.24.0,<0.25.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: pylint (>=2.17.2,<3.0.0)
+Requires-Dist: pymupdf (>=1.22.0,<2.0.0)
 Requires-Dist: python-Levenshtein (>=0.12.2,<0.13.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.6,<0.10.0)
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: transitions (>=0.8.11,<0.9.0)
@@ -80,43 +85,44 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/colrev)
 [![License](https://img.shields.io/github/license/CoLRev-Ecosystem/colrev.svg)](https://github.com/CoLRev-Environment/colrev/releases/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Documentation Status](https://readthedocs.org/projects/colrev/badge/?version=latest)](https://colrev.readthedocs.io/en/latest/?badge=latest)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Ecosystem/colrev/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/CoLRev-Ecosystem/colrev/main.svg)](https://results.pre-commit.ci/latest/github/CoLRev-Ecosystem/colrev/main)
 ![Coverage](https://raw.githubusercontent.com/CoLRev-Ecosystem/colrev/main/tests/coverage.svg)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bd4e44c6cda646e4b9e494c4c4d9487b)](https://app.codacy.com/gh/CoLRev-Environment/colrev/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 ![GitHub last commit](https://img.shields.io/github/last-commit/CoLRev-Ecosystem/colrev)
 [![Downloads](https://static.pepy.tech/badge/colrev/month)](https://pepy.tech/project/colrev)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7148/badge)](https://bestpractices.coreinfrastructure.org/projects/7148)
 [![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/CoLRev-Environment/colrev/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/CoLRev-Environment/colrev/)
 <!-- ![PyPI](https://img.shields.io/pypi/v/colrev) -->
 <!-- [![](https://img.shields.io/badge/-documentation-green)](https://colrev.readthedocs.io/) -->
 
 </div>
 
 ## Summary
 
-CoLRev is an open-source environment for collaborative literature reviews. It takes care of the data, integrates with differerent synthesis tools, and facilitates Git-based collaboration.
+CoLRev is an open-source environment for collaborative literature reviews. It integrates with differerent synthesis tools, takes care of the data, and facilitates Git-based collaboration.
 
 To accomplish these goals, CoLRev advances the design of review technology at the intersection of methods, design, cognition, and community building.
 The following features stand out:
 
 - An open and extensible environment based on shared data and process standards
 - Builds on git and its transparent collaboration model for the entire literature review process
 - Offers a self-explanatory, fault-tolerant, and configurable user workflow
-- Operates a model for data quality, record identification, content curation, and reuse
+- Operates a model for data quality, content curation, and reuse
 - Enables typological and methodological pluralism throughout the process
 
-See the [statements of development status](https://colrev.readthedocs.io/en/latest/foundations/roadmap.html) and [documentation](https://colrev.readthedocs.io/en/latest/) for more details. A brief overview presented at ESMARConf2023 is available on [YouTube](https://www.youtube.com/watch?v=yfGGraQC6vs).
+See the [statements of development status](https://colrev.readthedocs.io/en/latest/foundations/dev_status.html) and [documentation](https://colrev.readthedocs.io/en/latest/) for more details. A brief overview presented at ESMARConf2023 is available on [YouTube](https://www.youtube.com/watch?v=yfGGraQC6vs).
 
 ## Contributing, changes, and releases
 
 Contributions, code and features are always welcome
 
-- See [contributing guidelines](CONTRIBUTING.md), [help page](docs/build/user_resources/help.html), and [github repository](https://github.com/CoLRev-Environment/colrev).
+- See [contributing guidelines](CONTRIBUTING.md), [help page](https://colrev.readthedocs.io/en/latest/manual/help.html), and [github repository](https://github.com/CoLRev-Environment/colrev).
 - Bug reports or feedback? Please use the [issue tracker](https://github.com/CoLRev-Environment/colrev/issues) and let us know.
 - To get your work included, fork the repository, implement your changes, and create a [pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 For further information, see [tests](tests/readme.md), [changes](CHANGELOG.md), and [releases](https://github.com/CoLRev-Environment/colrev/releases).
 
 ## License
```

