# Comparing `tmp/bycon-1.0.8.tar.gz` & `tmp/bycon-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bycon-1.0.8.tar", last modified: Thu Feb  2 19:21:13 2023, max compression
+gzip compressed data, was "bycon-1.0.9.tar", last modified: Thu Feb  2 19:25:55 2023, max compression
```

## Comparing `bycon-1.0.8.tar` & `bycon-1.0.9.tar`

### file list

```diff
@@ -1,774 +1,774 @@
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.843694 bycon-1.0.8/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.511703 bycon-1.0.8/.github/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.559749 bycon-1.0.8/.github/workflows/
--rw-r--r--   0 mbaudis    (501) staff       (20)      485 2023-01-25 09:18:51.000000 bycon-1.0.8/.github/workflows/mkdocs-bycon.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      241 2023-01-27 12:34:37.000000 bycon-1.0.8/.gitignore
--rw-r--r--   0 mbaudis    (501) staff       (20)     7048 2023-01-16 07:33:33.000000 bycon-1.0.8/LICENSE
--rw-r--r--   0 mbaudis    (501) staff       (20)       56 2023-02-02 17:40:18.000000 bycon-1.0.8/MANIFEST.in
--rw-r--r--   0 mbaudis    (501) staff       (20)     1777 2023-02-02 19:21:13.844017 bycon-1.0.8/PKG-INFO
--rw-r--r--   0 mbaudis    (501) staff       (20)      535 2023-01-16 07:33:33.000000 bycon-1.0.8/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.533315 bycon-1.0.8/bycon/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1147 2023-02-02 11:47:39.000000 bycon-1.0.8/bycon/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.561456 bycon-1.0.8/bycon/beaconServer/
--rw-r--r--   0 mbaudis    (501) staff       (20)      118 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/README.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.8/bycon/beaconServer/__init__.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     5400 2023-02-02 11:58:23.000000 bycon-1.0.8/bycon/beaconServer/aggregator.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2239 2023-02-02 11:58:30.000000 bycon-1.0.8/bycon/beaconServer/beacon.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2602 2023-02-02 17:41:55.000000 bycon-1.0.8/bycon/beaconServer/cohorts.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.562559 bycon-1.0.8/bycon/beaconServer/config/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6259 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/config/aggregator.yaml
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1292 2023-02-02 12:08:18.000000 bycon-1.0.8/bycon/beaconServer/configuration.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2714 2023-02-02 12:08:30.000000 bycon-1.0.8/bycon/beaconServer/datasets.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.563831 bycon-1.0.8/bycon/beaconServer/doc/
--rw-r--r--   0 mbaudis    (501) staff       (20)      255 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/doc/beacon_v2.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      415 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/doc/bycon.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     1299 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/doc/handovers.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1438 2023-02-02 12:08:39.000000 bycon-1.0.8/bycon/beaconServer/entryTypes.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1246 2023-02-02 12:08:58.000000 bycon-1.0.8/bycon/beaconServer/filteringTerms.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1615 2023-02-02 12:09:06.000000 bycon-1.0.8/bycon/beaconServer/info.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1251 2023-02-02 12:09:16.000000 bycon-1.0.8/bycon/beaconServer/map.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     3064 2023-02-02 12:09:23.000000 bycon-1.0.8/bycon/beaconServer/retriever.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1191 2023-02-02 12:09:30.000000 bycon-1.0.8/bycon/beaconServer/service_info.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.566994 bycon-1.0.8/bycon/beaconServer/tests/
--rw-r--r--   0 mbaudis    (501) staff       (20)      945 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/GET-examples.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      756 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      934 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      540 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      552 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      668 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      826 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      619 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      806 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1067 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/beaconServer/tests/terminal-examples.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.572900 bycon-1.0.8/bycon/config/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:01.000000 bycon-1.0.8/bycon/config/.DS_Store
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.8/bycon/config/__init__.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3575 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/argument_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6984 2023-01-26 08:19:43.000000 bycon-1.0.8/bycon/config/beacon_defaults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5088 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/beacon_mappings.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3731 2023-01-26 10:40:49.000000 bycon-1.0.8/bycon/config/config.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1539 2023-01-27 12:32:43.000000 bycon-1.0.8/bycon/config/dataset_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     8827 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/datatable_mappings.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9312 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/filter_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1770 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/geoloc_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6661 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/handover_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1990 2023-01-25 11:54:56.000000 bycon-1.0.8/bycon/config/interval_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9142 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/remap_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4715 2023-01-26 10:41:30.000000 bycon-1.0.8/bycon/config/services_defaults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2367 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/services_mappings.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    11215 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/config/variant_definitions.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.549081 bycon-1.0.8/bycon/lib/
--rw-r--r--   0 mbaudis    (501) staff       (20)        0 2023-02-02 08:40:12.000000 bycon-1.0.8/bycon/lib/__init__.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     7844 2023-01-27 08:55:12.000000 bycon-1.0.8/bycon/lib/aggregator_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1488 2023-01-27 08:55:19.000000 bycon-1.0.8/bycon/lib/args_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    16967 2023-01-27 08:56:48.000000 bycon-1.0.8/bycon/lib/cgi_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    12978 2023-01-23 11:47:53.000000 bycon-1.0.8/bycon/lib/cytoband_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1872 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/data_retrieval.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     8758 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/datatable_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    14137 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/export_file_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3273 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/filter_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     7747 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/geomap_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     9608 2023-01-27 15:16:41.000000 bycon-1.0.8/bycon/lib/handover_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    11089 2023-01-30 22:24:42.000000 bycon-1.0.8/bycon/lib/interval_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     4481 2023-01-27 08:43:31.000000 bycon-1.0.8/bycon/lib/publication_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    13817 2023-01-27 15:15:36.000000 bycon-1.0.8/bycon/lib/query_execution.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    15646 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/query_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3844 2023-01-27 08:55:38.000000 bycon-1.0.8/bycon/lib/read_specs.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    10731 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/response_remapping.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3282 2023-01-27 08:57:34.000000 bycon-1.0.8/bycon/lib/schema_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    24644 2023-01-30 22:33:27.000000 bycon-1.0.8/bycon/lib/service_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    11128 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/lib/variant_parsing.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.574611 bycon-1.0.8/bycon/rsrc/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:06.000000 bycon-1.0.8/bycon/rsrc/.DS_Store
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.8/bycon/rsrc/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.575117 bycon-1.0.8/bycon/rsrc/genomes/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2023-01-26 21:36:47.000000 bycon-1.0.8/bycon/rsrc/genomes/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.575559 bycon-1.0.8/bycon/rsrc/genomes/grch38/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30914 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.576100 bycon-1.0.8/bycon/rsrc/genomes/hg16/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30743 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.576438 bycon-1.0.8/bycon/rsrc/genomes/hg17/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.576789 bycon-1.0.8/bycon/rsrc/genomes/hg18/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.577162 bycon-1.0.8/bycon/rsrc/genomes/hg19/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30754 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.577526 bycon-1.0.8/bycon/rsrc/genomes/mSarHar1.11/
--rw-r--r--   0 mbaudis    (501) staff       (20)      543 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.577865 bycon-1.0.8/bycon/rsrc/genomes/mm8/
--rw-r--r--   0 mbaudis    (501) staff       (20)    13771 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.578305 bycon-1.0.8/bycon/rsrc/genomes/mm9/
--rw-r--r--   0 mbaudis    (501) staff       (20)    13786 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.578748 bycon-1.0.8/bycon/rsrc/genomes/zf7/
--rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.579777 bycon-1.0.8/bycon/schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:16.000000 bycon-1.0.8/bycon/schemas/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.581214 bycon-1.0.8/bycon/schemas/ProgenetixLinkML/
--rw-r--r--   0 mbaudis    (501) staff       (20)     7431 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/ProgenetixLinkML/Publication.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3935 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/ProgenetixLinkML/Publication.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      587 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/ProgenetixLinkML/README.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     2654 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/ProgenetixLinkML/testpub.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      346 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/README.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.8/bycon/schemas/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.582006 bycon-1.0.8/bycon/schemas/bin/
--rw-r--r--   0 mbaudis    (501) staff       (20)     7312 2023-01-27 12:05:43.000000 bycon-1.0.8/bycon/schemas/bin/beaconYamler.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.582584 bycon-1.0.8/bycon/schemas/bin/config/
--rw-r--r--   0 mbaudis    (501) staff       (20)      550 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/bin/config/beaconYamler.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1181 2023-01-27 12:05:43.000000 bycon-1.0.8/bycon/schemas/bin/yamlerRunner.sh
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.583292 bycon-1.0.8/bycon/schemas/framework/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-01-26 21:36:47.000000 bycon-1.0.8/bycon/schemas/framework/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.583860 bycon-1.0.8/bycon/schemas/framework/json/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.586002 bycon-1.0.8/bycon/schemas/framework/json/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      572 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/basicElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    11759 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/beaconCommonComponents.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      566 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/elementWithDescription.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.588307 bycon-1.0.8/bycon/schemas/framework/json/common/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      125 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/basicElement-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1936 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      197 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/elementWithDescription-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      346 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/ontologizedElement-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      127 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/ontologyTerm-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      336 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      239 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      697 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/ontologizedElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      933 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/ontologyTerm.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1017 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/referenceToAnSchema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.588672 bycon-1.0.8/bycon/schemas/framework/json/common/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2011 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.591534 bycon-1.0.8/bycon/schemas/framework/json/configuration/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3213 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4791 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/beaconMapSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3992 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/entryTypeDefinition.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      764 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/entryTypesSchema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.594354 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2281 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      540 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      223 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconMap-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      588 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1318 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      561 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3152 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/configuration/filteringTermsSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.595585 bycon-1.0.8/bycon/schemas/framework/json/requests/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2238 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/beaconRequestBody.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      874 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/beaconRequestMeta.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.596249 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      830 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      114 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MIN-example.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.597396 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      231 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-sections/beaconRequestMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      495 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-sections/filteringTerms-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      386 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/examples-sections/requestParameters-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4850 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      452 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/requestParameters.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.597782 bycon-1.0.8/bycon/schemas/framework/json/requests/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4243 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/requests/validation/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.602537 bycon-1.0.8/bycon/schemas/framework/json/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1231 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconBooleanResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1818 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      727 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1277 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconCountResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      681 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      645 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconErrorResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      664 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconInfoResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconMapResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1454 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.606490 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      745 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2451 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      782 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2832 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1533 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2452 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1164 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1183 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1279 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      538 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1522 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      767 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.610200 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)       85 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconBooleanResponseSection-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      115 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconCountResponseSection-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      166 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconInformationalResponseMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      656 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      214 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsetEmpty-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1070 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      526 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       87 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5381 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.614194 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      522 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      730 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3545 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4676 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      896 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2688 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1801 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2414 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconResultsets.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.615254 bycon-1.0.8/bycon/schemas/framework/src/
--rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.617581 bycon-1.0.8/bycon/schemas/framework/src/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      393 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/basicElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9293 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/beaconCommonComponents.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      356 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/elementWithDescription.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.619980 bycon-1.0.8/bycon/schemas/framework/src/common/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)       96 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/basicElement-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1305 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      159 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/elementWithDescription-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      272 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/ontologizedElement-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       98 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/ontologyTerm-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      201 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      462 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/ontologizedElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/ontologyTerm.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      717 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/referenceToAnSchema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.620282 bycon-1.0.8/bycon/schemas/framework/src/common/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1459 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.623590 bycon-1.0.8/bycon/schemas/framework/src/configuration/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2395 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3917 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3395 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.627505 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1545 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      312 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconConfigurationFilteringTerms-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      152 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconMap-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      810 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      396 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_MIN_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1014 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      440 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/entryTypeDefinition-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2412 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.630222 bycon-1.0.8/bycon/schemas/framework/src/requests/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1678 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/beaconRequestBody.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      693 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.632061 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      449 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       80 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MIN-example.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.633511 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      153 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-sections/beaconRequestMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      284 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-sections/filteringTerms-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/examples-sections/requestParameters-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3254 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      340 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/requestParameters.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.633836 bycon-1.0.8/bycon/schemas/framework/src/requests/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2786 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.641043 bycon-1.0.8/bycon/schemas/framework/src/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)      996 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1326 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      565 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1042 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconCountResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      517 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      481 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconErrorResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconFilteringTermsResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      554 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      545 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconMapResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1157 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.646421 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      418 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconBooleanResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1323 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      432 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1834 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      954 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1579 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      586 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      675 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1035 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      433 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.655206 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)       67 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconBooleanResponseSection-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       90 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconCountResponseSection-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      130 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconInformationalResponseMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      380 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      137 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResponseMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResultsetEmpty-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      582 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       69 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4108 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.659144 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      424 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconBooleanResponseSection.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      579 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2403 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3084 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      679 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2269 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1472 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1572 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      558 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.660093 bycon-1.0.8/bycon/schemas/models/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 21:24:56.000000 bycon-1.0.8/bycon/schemas/models/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.525015 bycon-1.0.8/bycon/schemas/models/json/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.662442 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.664312 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2544 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.665934 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      399 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/analyses-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/analyses-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6428 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/beaconConfiguration.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7195 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/beaconMap.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.667327 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     9989 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.668021 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      498 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/biosample-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      305 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/biosample-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.669958 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)    13006 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    14684 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.671697 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      161 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.678555 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      408 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/age.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      515 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/ageRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6182 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/commonDefinitions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1714 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/complexValue.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2629 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/dataUseConditions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3702 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/disease.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1659 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/doseInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1066 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/evidence.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1724 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/exposure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      968 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/externalReference.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/gestationalAge.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2245 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/measurement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5373 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/pedigree.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3561 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/phenotypicFeature.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2078 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/procedure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      721 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/quantity.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      961 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/referenceRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      939 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/timeElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      835 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/timeInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1909 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/treatment.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      427 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/value.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.679725 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    19610 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.680614 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      825 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-Max-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.683289 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)    25855 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.684716 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3469 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      647 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      275 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6279 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParameters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2722 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParametersComponents.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.686287 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3291 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.692026 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/pedigree-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.697031 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4034 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.699391 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      178 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.699658 bycon-1.0.8/bycon/schemas/models/json/framework/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/framework/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.701682 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8307 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6852 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxCallset.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6140 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2872 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3492 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.702834 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.703819 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2622 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.704470 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      399 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7254 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7602 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/beaconMap.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.705835 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     7855 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.706433 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      498 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      305 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.707799 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)    12858 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    14684 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.709528 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      161 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.722310 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)     5664 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      408 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/age.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      515 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ageRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      939 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ancestry.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5647 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1632 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/complexValue.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2465 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3142 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/disease.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/doseInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      984 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/evidence.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1642 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/exposure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      968 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/externalReference.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1260 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/file.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2039 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/measurement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      925 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/metaData.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      933 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5291 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/pedigree.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3428 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1824 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/procedure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      923 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/provenance.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      721 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/quantity.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      961 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/referenceRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1150 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/resource.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      857 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/timeElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      835 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/timeInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1745 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/treatment.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      511 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/update.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      345 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/value.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1525 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.723482 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    19610 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.724182 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      825 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.726363 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)    25281 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.728237 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3469 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      647 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      275 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6066 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2700 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.729772 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4967 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.731649 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.733696 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/phenopackets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    15893 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.735085 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3807 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.735662 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      178 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.743922 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2415 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoJSONgeometry.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3268 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoLabels.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2357 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoLocation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1757 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2397 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1999 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      370 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/OntologyClassGroup.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1292 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3202 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1773 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4982 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Publication.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2348 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2914 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      808 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/cytobandMapping.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1479 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      748 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseMeta.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1306 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseSummary.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.744390 bycon-1.0.8/bycon/schemas/models/src/
--rw-r--r--   0 mbaudis    (501) staff       (20)      294 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.746627 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.747813 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1701 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.748417 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/analyses-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/analyses-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4623 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/beaconConfiguration.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4861 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/beaconMap.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.749360 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6759 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.751229 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/biosample-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/biosample-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.753137 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8764 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     8407 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.754055 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.765864 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/age.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/ageRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4070 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/commonDefinitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/complexValue.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1324 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/dataUseConditions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2215 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/disease.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1259 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/doseInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      784 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/evidence.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1176 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/exposure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      735 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/externalReference.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/gestationalAge.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1536 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/measurement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3198 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/pedigree.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2555 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/phenotypicFeature.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1417 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/procedure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/quantity.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/referenceRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      684 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/timeElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/timeInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1272 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/treatment.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      311 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/value.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.767696 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    11341 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.768576 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-Max-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.771694 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)    16741 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.773774 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5427 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParameters.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2492 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParametersComponents.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.775707 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.777723 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/pedigree-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.779076 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2703 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.779832 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/runs-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/runs-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.780161 bycon-1.0.8/bycon/schemas/models/src/framework/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/framework/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.782165 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     5372 2023-01-30 13:05:19.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4217 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxCallset.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4175 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2108 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.783179 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.784183 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1581 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.784721 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5059 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5216 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/beaconMap.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.785641 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8221 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.786193 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.787281 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8616 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     8407 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.795551 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.806874 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4265 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/age.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/ageRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      585 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      747 2023-02-02 08:40:12.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3893 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1015 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1160 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/disease.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1177 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/evidence.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1094 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/exposure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      735 2023-01-30 13:02:56.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      875 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/file.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1281 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/measurement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      553 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/metaData.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3116 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1175 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/procedure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1018 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/provenance.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/quantity.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      701 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/resource.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      601 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/treatment.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      362 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/update.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      229 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/value.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1200 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.808373 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    11341 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.809475 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.811489 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)    16007 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.812971 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5744 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2481 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.814677 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3080 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.815957 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.816875 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/phenopackets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1301 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9236 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.818162 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2476 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.819082 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.825718 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1542 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoJSONgeometry.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2419 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoLabels.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1696 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoLocation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1194 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1394 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      257 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/OntologyClassGroup.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      859 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1700 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3262 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1830 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2118 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      660 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/cytobandMapping.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      986 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      483 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseMeta.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      839 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseSummary.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.558876 bycon-1.0.8/bycon/services/
--rw-r--r--   0 mbaudis    (501) staff       (20)       14 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/__init__.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     4747 2023-02-02 12:09:45.000000 bycon-1.0.8/bycon/services/collations.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.831584 bycon-1.0.8/bycon/services/config/
--rw-r--r--   0 mbaudis    (501) staff       (20)      367 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/Readme.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      771 2023-01-31 22:06:53.000000 bycon-1.0.8/bycon/services/config/collations.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      361 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/dbstats.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/genespans.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      328 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/geolocations.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1716 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/ids.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      239 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/interval_frequencies.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      503 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/ontologymaps.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2170 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/publications.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       21 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/config/uploader.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3812 2023-02-02 12:09:50.000000 bycon-1.0.8/bycon/services/cytomapper.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1982 2023-02-02 12:09:55.000000 bycon-1.0.8/bycon/services/dbstats.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.837348 bycon-1.0.8/bycon/services/doc/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1013 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/collations.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     2920 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/cytomapper.md
--rw-r--r--   0 mbaudis    (501) staff       (20)       42 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/dbstats.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      389 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/genespans.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      906 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/geolocations.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/ids.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     2845 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/intervalFrequencies.md
--rw-r--r--   0 mbaudis    (501) staff       (20)       46 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/ontolgymaps.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      559 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/phenopackets.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      654 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/publications.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     2698 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/doc/services.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     1813 2023-02-02 12:10:03.000000 bycon-1.0.8/bycon/services/endpoints.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     4446 2023-02-02 16:14:02.000000 bycon-1.0.8/bycon/services/genespans.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3536 2023-02-02 16:14:09.000000 bycon-1.0.8/bycon/services/geolocations.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     2121 2023-02-02 16:14:24.000000 bycon-1.0.8/bycon/services/ids.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     4545 2023-02-02 12:10:48.000000 bycon-1.0.8/bycon/services/intervalFrequencies.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.559392 bycon-1.0.8/bycon/services/lib/
--rw-r--r--   0 mbaudis    (501) staff       (20)       14 2023-01-16 07:33:33.000000 bycon-1.0.8/bycon/services/lib/__init__.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3522 2023-02-02 12:10:58.000000 bycon-1.0.8/bycon/services/ontologymaps.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     6095 2023-02-02 12:11:07.000000 bycon-1.0.8/bycon/services/publications.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1893 2023-02-02 12:11:19.000000 bycon-1.0.8/bycon/services/schemas.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     2408 2023-02-02 12:11:32.000000 bycon-1.0.8/bycon/services/services.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     2130 2023-02-02 16:14:36.000000 bycon-1.0.8/bycon/services/uploader.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.561209 bycon-1.0.8/bycon.egg-info/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1777 2023-02-02 19:21:13.000000 bycon-1.0.8/bycon.egg-info/PKG-INFO
--rw-r--r--   0 mbaudis    (501) staff       (20)    44230 2023-02-02 19:21:13.000000 bycon-1.0.8/bycon.egg-info/SOURCES.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)        1 2023-02-02 19:21:13.000000 bycon-1.0.8/bycon.egg-info/dependency_links.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)       88 2023-02-02 19:21:13.000000 bycon-1.0.8/bycon.egg-info/requires.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)        6 2023-02-02 19:21:13.000000 bycon-1.0.8/bycon.egg-info/top_level.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.841030 bycon-1.0.8/docs/
--rw-r--r--   0 mbaudis    (501) staff       (20)       20 2023-01-16 07:33:33.000000 bycon-1.0.8/docs/CNAME
--rw-r--r--   0 mbaudis    (501) staff       (20)      265 2023-01-16 07:33:33.000000 bycon-1.0.8/docs/bugs-todo.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.841608 bycon-1.0.8/docs/css/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2834 2022-11-09 11:53:14.000000 bycon-1.0.8/docs/css/extra.css
--rw-r--r--   0 mbaudis    (501) staff       (20)      906 2023-01-19 22:58:34.000000 bycon-1.0.8/docs/handovers.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:21:13.843049 bycon-1.0.8/docs/img/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8070 2021-10-27 14:32:20.000000 bycon-1.0.8/docs/img/site-logo-main.png
--rw-r--r--   0 mbaudis    (501) staff       (20)     6264 2021-10-27 14:32:20.000000 bycon-1.0.8/docs/img/site-logo-topright.png
--rw-r--r--   0 mbaudis    (501) staff       (20)     2849 2023-01-25 08:47:50.000000 bycon-1.0.8/docs/index.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     4830 2023-01-16 07:33:33.000000 bycon-1.0.8/docs/tests.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2775 2023-02-02 08:40:12.000000 bycon-1.0.8/install.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1625 2023-01-25 09:14:58.000000 bycon-1.0.8/mkdocs.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      156 2023-01-27 12:06:55.000000 bycon-1.0.8/requirements.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)       74 2023-02-02 19:21:13.845236 bycon-1.0.8/setup.cfg
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2707 2023-02-02 19:20:49.000000 bycon-1.0.8/setup.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.734305 bycon-1.0.9/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.317615 bycon-1.0.9/.github/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.375234 bycon-1.0.9/.github/workflows/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      485 2023-01-25 09:18:51.000000 bycon-1.0.9/.github/workflows/mkdocs-bycon.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      241 2023-01-27 12:34:37.000000 bycon-1.0.9/.gitignore
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7048 2023-01-16 07:33:33.000000 bycon-1.0.9/LICENSE
+-rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-02-02 19:25:24.000000 bycon-1.0.9/MANIFEST.in
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1777 2023-02-02 19:25:55.734590 bycon-1.0.9/PKG-INFO
+-rw-r--r--   0 mbaudis    (501) staff       (20)      535 2023-01-16 07:33:33.000000 bycon-1.0.9/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.347069 bycon-1.0.9/bycon/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1147 2023-02-02 11:47:39.000000 bycon-1.0.9/bycon/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.377098 bycon-1.0.9/bycon/beaconServer/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      118 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/README.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.9/bycon/beaconServer/__init__.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     5400 2023-02-02 11:58:23.000000 bycon-1.0.9/bycon/beaconServer/aggregator.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2239 2023-02-02 11:58:30.000000 bycon-1.0.9/bycon/beaconServer/beacon.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2602 2023-02-02 17:41:55.000000 bycon-1.0.9/bycon/beaconServer/cohorts.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.378224 bycon-1.0.9/bycon/beaconServer/config/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6259 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/config/aggregator.yaml
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1292 2023-02-02 12:08:18.000000 bycon-1.0.9/bycon/beaconServer/configuration.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2714 2023-02-02 12:08:30.000000 bycon-1.0.9/bycon/beaconServer/datasets.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.379946 bycon-1.0.9/bycon/beaconServer/doc/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      255 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/doc/beacon_v2.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      415 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/doc/bycon.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1299 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/doc/handovers.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1438 2023-02-02 12:08:39.000000 bycon-1.0.9/bycon/beaconServer/entryTypes.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1246 2023-02-02 12:08:58.000000 bycon-1.0.9/bycon/beaconServer/filteringTerms.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1615 2023-02-02 12:09:06.000000 bycon-1.0.9/bycon/beaconServer/info.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1251 2023-02-02 12:09:16.000000 bycon-1.0.9/bycon/beaconServer/map.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     3064 2023-02-02 12:09:23.000000 bycon-1.0.9/bycon/beaconServer/retriever.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1191 2023-02-02 12:09:30.000000 bycon-1.0.9/bycon/beaconServer/service_info.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.386323 bycon-1.0.9/bycon/beaconServer/tests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      945 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/GET-examples.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      756 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      934 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      540 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      552 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      668 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      826 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      619 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      806 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1067 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/beaconServer/tests/terminal-examples.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.392355 bycon-1.0.9/bycon/config/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:01.000000 bycon-1.0.9/bycon/config/.DS_Store
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.9/bycon/config/__init__.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3575 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/argument_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6984 2023-01-26 08:19:43.000000 bycon-1.0.9/bycon/config/beacon_defaults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5088 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/beacon_mappings.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3731 2023-01-26 10:40:49.000000 bycon-1.0.9/bycon/config/config.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1539 2023-01-27 12:32:43.000000 bycon-1.0.9/bycon/config/dataset_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8827 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/datatable_mappings.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9312 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/filter_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1770 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/geoloc_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6661 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/handover_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1990 2023-01-25 11:54:56.000000 bycon-1.0.9/bycon/config/interval_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9142 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/remap_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4715 2023-01-26 10:41:30.000000 bycon-1.0.9/bycon/config/services_defaults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2367 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/services_mappings.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11215 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/config/variant_definitions.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.366724 bycon-1.0.9/bycon/lib/
+-rw-r--r--   0 mbaudis    (501) staff       (20)        0 2023-02-02 08:40:12.000000 bycon-1.0.9/bycon/lib/__init__.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7844 2023-01-27 08:55:12.000000 bycon-1.0.9/bycon/lib/aggregator_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1488 2023-01-27 08:55:19.000000 bycon-1.0.9/bycon/lib/args_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16967 2023-01-27 08:56:48.000000 bycon-1.0.9/bycon/lib/cgi_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    12978 2023-01-23 11:47:53.000000 bycon-1.0.9/bycon/lib/cytoband_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1872 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/data_retrieval.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8758 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/datatable_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    14137 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/export_file_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3273 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/filter_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7747 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/geomap_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9608 2023-01-27 15:16:41.000000 bycon-1.0.9/bycon/lib/handover_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11089 2023-01-30 22:24:42.000000 bycon-1.0.9/bycon/lib/interval_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4481 2023-01-27 08:43:31.000000 bycon-1.0.9/bycon/lib/publication_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13817 2023-01-27 15:15:36.000000 bycon-1.0.9/bycon/lib/query_execution.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15646 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/query_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3844 2023-01-27 08:55:38.000000 bycon-1.0.9/bycon/lib/read_specs.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    10731 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/response_remapping.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3282 2023-01-27 08:57:34.000000 bycon-1.0.9/bycon/lib/schema_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    24644 2023-01-30 22:33:27.000000 bycon-1.0.9/bycon/lib/service_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11128 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/lib/variant_parsing.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.394300 bycon-1.0.9/bycon/rsrc/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:06.000000 bycon-1.0.9/bycon/rsrc/.DS_Store
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.9/bycon/rsrc/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.394826 bycon-1.0.9/bycon/rsrc/genomes/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2023-01-26 21:36:47.000000 bycon-1.0.9/bycon/rsrc/genomes/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.395630 bycon-1.0.9/bycon/rsrc/genomes/grch38/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30914 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.396256 bycon-1.0.9/bycon/rsrc/genomes/hg16/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30743 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.396660 bycon-1.0.9/bycon/rsrc/genomes/hg17/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.397241 bycon-1.0.9/bycon/rsrc/genomes/hg18/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.397905 bycon-1.0.9/bycon/rsrc/genomes/hg19/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30754 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.398317 bycon-1.0.9/bycon/rsrc/genomes/mSarHar1.11/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      543 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.398746 bycon-1.0.9/bycon/rsrc/genomes/mm8/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13771 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.399259 bycon-1.0.9/bycon/rsrc/genomes/mm9/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13786 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.399757 bycon-1.0.9/bycon/rsrc/genomes/zf7/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.400739 bycon-1.0.9/bycon/schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 22:17:16.000000 bycon-1.0.9/bycon/schemas/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.402167 bycon-1.0.9/bycon/schemas/ProgenetixLinkML/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7431 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/ProgenetixLinkML/Publication.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3935 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/ProgenetixLinkML/Publication.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      587 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/ProgenetixLinkML/README.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2654 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/ProgenetixLinkML/testpub.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      346 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/README.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-02-02 12:12:07.000000 bycon-1.0.9/bycon/schemas/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.402973 bycon-1.0.9/bycon/schemas/bin/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7312 2023-01-27 12:05:43.000000 bycon-1.0.9/bycon/schemas/bin/beaconYamler.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.403389 bycon-1.0.9/bycon/schemas/bin/config/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      550 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/bin/config/beaconYamler.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1181 2023-01-27 12:05:43.000000 bycon-1.0.9/bycon/schemas/bin/yamlerRunner.sh
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.403853 bycon-1.0.9/bycon/schemas/framework/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-01-26 21:36:47.000000 bycon-1.0.9/bycon/schemas/framework/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.404438 bycon-1.0.9/bycon/schemas/framework/json/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.407137 bycon-1.0.9/bycon/schemas/framework/json/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      572 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/basicElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11759 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/beaconCommonComponents.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      566 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/elementWithDescription.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.410855 bycon-1.0.9/bycon/schemas/framework/json/common/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      125 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/basicElement-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1936 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      197 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/elementWithDescription-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      346 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/ontologizedElement-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      127 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/ontologyTerm-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      336 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      239 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      697 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/ontologizedElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      933 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/ontologyTerm.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1017 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/referenceToAnSchema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.411239 bycon-1.0.9/bycon/schemas/framework/json/common/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2011 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.413763 bycon-1.0.9/bycon/schemas/framework/json/configuration/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3213 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4791 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/beaconMapSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3992 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/entryTypeDefinition.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      764 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/entryTypesSchema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.417259 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2281 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      540 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      223 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconMap-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      588 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1318 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      561 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3152 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/configuration/filteringTermsSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.422266 bycon-1.0.9/bycon/schemas/framework/json/requests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2238 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/beaconRequestBody.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      874 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/beaconRequestMeta.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.424098 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      830 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      114 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MIN-example.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.427567 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      231 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-sections/beaconRequestMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      495 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-sections/filteringTerms-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      386 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/examples-sections/requestParameters-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4850 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      452 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/requestParameters.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.427876 bycon-1.0.9/bycon/schemas/framework/json/requests/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4243 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/requests/validation/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.434793 bycon-1.0.9/bycon/schemas/framework/json/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1231 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconBooleanResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1818 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      727 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1277 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconCountResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      681 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      645 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconErrorResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      664 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconInfoResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconMapResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1454 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.444666 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      745 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2451 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      782 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2832 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1533 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2452 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1164 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1183 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1279 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      538 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1522 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      767 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.452217 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       85 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconBooleanResponseSection-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      115 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconCountResponseSection-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      166 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconInformationalResponseMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      656 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      214 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsetEmpty-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1070 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      526 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       87 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5381 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.460184 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      522 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      730 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3545 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4676 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      896 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2688 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1801 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2414 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconResultsets.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.461144 bycon-1.0.9/bycon/schemas/framework/src/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.468643 bycon-1.0.9/bycon/schemas/framework/src/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      393 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/basicElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9293 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/beaconCommonComponents.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      356 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/elementWithDescription.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.472434 bycon-1.0.9/bycon/schemas/framework/src/common/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       96 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/basicElement-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1305 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      159 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/elementWithDescription-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      272 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/ontologizedElement-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       98 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/ontologyTerm-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      201 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      462 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/ontologizedElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/ontologyTerm.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      717 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/referenceToAnSchema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.474118 bycon-1.0.9/bycon/schemas/framework/src/common/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1459 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.476683 bycon-1.0.9/bycon/schemas/framework/src/configuration/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2395 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3917 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3395 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.482467 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1545 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      312 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconConfigurationFilteringTerms-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      152 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconMap-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      810 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      396 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_MIN_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1014 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      440 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/entryTypeDefinition-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2412 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.485339 bycon-1.0.9/bycon/schemas/framework/src/requests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1678 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/beaconRequestBody.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      693 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.486517 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      449 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       80 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MIN-example.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.487974 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      153 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-sections/beaconRequestMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      284 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-sections/filteringTerms-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/examples-sections/requestParameters-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3254 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      340 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/requestParameters.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.488520 bycon-1.0.9/bycon/schemas/framework/src/requests/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2786 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.501140 bycon-1.0.9/bycon/schemas/framework/src/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      996 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1326 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      565 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1042 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconCountResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      517 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      481 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconErrorResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconFilteringTermsResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      554 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      545 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconMapResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1157 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.509733 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      418 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconBooleanResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1323 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      432 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1834 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      954 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1579 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      586 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      675 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1035 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      433 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.514400 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       67 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconBooleanResponseSection-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       90 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconCountResponseSection-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      130 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconInformationalResponseMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      380 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      137 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResponseMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResultsetEmpty-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      582 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       69 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4108 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.519304 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      424 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconBooleanResponseSection.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      579 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2403 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3084 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      679 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2269 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1472 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1572 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      558 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.519644 bycon-1.0.9/bycon/schemas/models/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-02-01 21:24:56.000000 bycon-1.0.9/bycon/schemas/models/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.336051 bycon-1.0.9/bycon/schemas/models/json/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.520883 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.522023 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2544 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.522604 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      399 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/analyses-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/examples/analyses-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6428 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/beaconConfiguration.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7195 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/beaconMap.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.523967 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9989 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.525373 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      498 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/biosample-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      305 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/examples/biosample-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.526605 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13006 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    14684 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.528451 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      161 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.542766 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      408 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/age.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      515 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/ageRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6182 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/commonDefinitions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1714 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/complexValue.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2629 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/dataUseConditions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3702 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/disease.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1659 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/doseInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1066 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/evidence.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1724 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/exposure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      968 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/externalReference.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/gestationalAge.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2245 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/measurement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5373 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/pedigree.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3561 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/phenotypicFeature.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2078 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/procedure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      721 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/quantity.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      961 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/referenceRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      939 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/timeElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      835 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/timeInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1909 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/treatment.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      427 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/value.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.545093 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    19610 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.546255 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      825 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-Max-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.549355 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    25855 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.551152 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3469 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      647 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      275 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6279 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParameters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2722 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParametersComponents.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.553704 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3291 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.559072 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/pedigree-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.563020 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4034 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.564021 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      178 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.564836 bycon-1.0.9/bycon/schemas/models/json/framework/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/framework/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.571210 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8307 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6852 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxCallset.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6140 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2872 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3492 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.574562 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.577408 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2622 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.578946 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      399 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      180 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7254 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7602 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/beaconMap.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.580861 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7855 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.583848 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      498 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      305 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.585966 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    12858 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    14684 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.587888 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      161 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.607504 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5664 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      408 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/age.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      515 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ageRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      939 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ancestry.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5647 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1632 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/complexValue.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2465 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3142 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/disease.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/doseInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      984 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/evidence.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1642 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/exposure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      968 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/externalReference.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1260 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/file.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2039 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/measurement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      925 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/metaData.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      933 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5291 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/pedigree.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3428 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1824 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/procedure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      923 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/provenance.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      721 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/quantity.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      961 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/referenceRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1150 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/resource.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      857 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/timeElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      835 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/timeInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1745 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/treatment.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      511 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/update.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      345 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/value.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1525 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.608508 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    19610 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.609026 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      825 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      288 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.610798 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    25281 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.612817 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3469 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      707 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      647 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      275 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6066 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2700 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.614890 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4967 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.617747 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.618559 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/phenopackets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15893 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.619909 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3807 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.620700 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      178 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.626307 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2415 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoJSONgeometry.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3268 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoLabels.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2357 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoLocation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1757 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2397 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1999 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      370 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/OntologyClassGroup.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1292 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3202 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1773 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4982 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Publication.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2348 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2914 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      808 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/cytobandMapping.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1479 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      748 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseMeta.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1306 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseSummary.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.626654 bycon-1.0.9/bycon/schemas/models/src/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      294 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.628252 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.629296 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1701 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.630097 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/analyses-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/examples/analyses-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4623 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/beaconConfiguration.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4861 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/beaconMap.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.631999 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6759 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.632937 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/biosample-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/examples/biosample-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.634169 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8764 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8407 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.635491 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.643355 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/age.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/ageRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4070 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/commonDefinitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/complexValue.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1324 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/dataUseConditions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2215 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/disease.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1259 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/doseInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      784 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/evidence.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1176 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/exposure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      735 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/externalReference.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/gestationalAge.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1536 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/measurement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3198 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/pedigree.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2555 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/phenotypicFeature.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1417 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/procedure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/quantity.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/referenceRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      684 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/timeElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/timeInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1272 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/treatment.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      311 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/value.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.645147 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11341 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.645653 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-Max-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.647086 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16741 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.648086 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5427 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParameters.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2492 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParametersComponents.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.649126 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.650910 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/pedigree-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.651870 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2703 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.652568 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/runs-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/examples/runs-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.653060 bycon-1.0.9/bycon/schemas/models/src/framework/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/framework/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.656286 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5372 2023-01-30 13:05:19.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4217 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxCallset.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4175 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2108 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.657731 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.659841 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1581 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.662708 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5059 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5216 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/beaconMap.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.665566 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8221 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.666627 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.668046 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8616 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8407 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.669649 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.687261 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4265 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/age.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/ageRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      585 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      747 2023-02-02 08:40:12.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3893 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1015 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1160 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/disease.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1177 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/evidence.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1094 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/exposure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      735 2023-01-30 13:02:56.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      875 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/file.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1281 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/measurement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      553 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/metaData.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3116 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1175 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/procedure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1018 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/provenance.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/quantity.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      701 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/resource.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      601 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/treatment.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      362 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/update.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      229 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/value.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1200 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.688506 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11341 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.689146 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.690924 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16007 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.692169 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5744 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2481 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.693084 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3080 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.694597 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.695321 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/phenopackets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1301 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9236 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.699076 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2476 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.699809 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.706559 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1542 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoJSONgeometry.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2419 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoLabels.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1696 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoLocation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1194 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1394 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      257 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/OntologyClassGroup.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      859 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1700 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3262 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1830 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2118 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      660 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/cytobandMapping.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      986 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      483 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseMeta.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      839 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseSummary.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.374559 bycon-1.0.9/bycon/services/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       14 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/__init__.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4747 2023-02-02 12:09:45.000000 bycon-1.0.9/bycon/services/collations.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.712714 bycon-1.0.9/bycon/services/config/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      367 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/Readme.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      771 2023-01-31 22:06:53.000000 bycon-1.0.9/bycon/services/config/collations.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      361 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/dbstats.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/genespans.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      328 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/geolocations.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1716 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/ids.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      239 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/interval_frequencies.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      503 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/ontologymaps.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2170 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/publications.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       21 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/config/uploader.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3812 2023-02-02 12:09:50.000000 bycon-1.0.9/bycon/services/cytomapper.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1982 2023-02-02 12:09:55.000000 bycon-1.0.9/bycon/services/dbstats.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.717543 bycon-1.0.9/bycon/services/doc/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1013 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/collations.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2920 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/cytomapper.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)       42 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/dbstats.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      389 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/genespans.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      906 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/geolocations.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      160 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/ids.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2845 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/intervalFrequencies.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)       46 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/ontolgymaps.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      559 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/phenopackets.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      654 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/publications.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2698 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/doc/services.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1813 2023-02-02 12:10:03.000000 bycon-1.0.9/bycon/services/endpoints.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4446 2023-02-02 16:14:02.000000 bycon-1.0.9/bycon/services/genespans.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3536 2023-02-02 16:14:09.000000 bycon-1.0.9/bycon/services/geolocations.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2121 2023-02-02 16:14:24.000000 bycon-1.0.9/bycon/services/ids.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4545 2023-02-02 12:10:48.000000 bycon-1.0.9/bycon/services/intervalFrequencies.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.374897 bycon-1.0.9/bycon/services/lib/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       14 2023-01-16 07:33:33.000000 bycon-1.0.9/bycon/services/lib/__init__.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3522 2023-02-02 12:10:58.000000 bycon-1.0.9/bycon/services/ontologymaps.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6095 2023-02-02 12:11:07.000000 bycon-1.0.9/bycon/services/publications.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1893 2023-02-02 12:11:19.000000 bycon-1.0.9/bycon/services/schemas.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2408 2023-02-02 12:11:32.000000 bycon-1.0.9/bycon/services/services.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2130 2023-02-02 16:14:36.000000 bycon-1.0.9/bycon/services/uploader.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.376797 bycon-1.0.9/bycon.egg-info/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1777 2023-02-02 19:25:54.000000 bycon-1.0.9/bycon.egg-info/PKG-INFO
+-rw-r--r--   0 mbaudis    (501) staff       (20)    44230 2023-02-02 19:25:55.000000 bycon-1.0.9/bycon.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)        1 2023-02-02 19:25:54.000000 bycon-1.0.9/bycon.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)       88 2023-02-02 19:25:54.000000 bycon-1.0.9/bycon.egg-info/requires.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)        6 2023-02-02 19:25:54.000000 bycon-1.0.9/bycon.egg-info/top_level.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.731526 bycon-1.0.9/docs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       20 2023-01-16 07:33:33.000000 bycon-1.0.9/docs/CNAME
+-rw-r--r--   0 mbaudis    (501) staff       (20)      265 2023-01-16 07:33:33.000000 bycon-1.0.9/docs/bugs-todo.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.732698 bycon-1.0.9/docs/css/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2834 2022-11-09 11:53:14.000000 bycon-1.0.9/docs/css/extra.css
+-rw-r--r--   0 mbaudis    (501) staff       (20)      906 2023-01-19 22:58:34.000000 bycon-1.0.9/docs/handovers.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2023-02-02 19:25:55.733796 bycon-1.0.9/docs/img/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8070 2021-10-27 14:32:20.000000 bycon-1.0.9/docs/img/site-logo-main.png
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6264 2021-10-27 14:32:20.000000 bycon-1.0.9/docs/img/site-logo-topright.png
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2849 2023-01-25 08:47:50.000000 bycon-1.0.9/docs/index.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4830 2023-01-16 07:33:33.000000 bycon-1.0.9/docs/tests.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2775 2023-02-02 08:40:12.000000 bycon-1.0.9/install.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1625 2023-01-25 09:14:58.000000 bycon-1.0.9/mkdocs.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      156 2023-01-27 12:06:55.000000 bycon-1.0.9/requirements.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)       74 2023-02-02 19:25:55.735087 bycon-1.0.9/setup.cfg
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2707 2023-02-02 19:25:36.000000 bycon-1.0.9/setup.py
```

### Comparing `bycon-1.0.8/LICENSE` & `bycon-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/PKG-INFO` & `bycon-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bycon
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python-based environment for the Beacon v2 genomics API
 Home-page: https://github.com/progenetix/bycon
 Author: Michael Baudis
 Author-email: contact@progenetix.org
 Project-URL: Bug Reports, https://github.com/progenetix/bycon/issues
 Project-URL: Source, https://github.com/progenetix/bycon/
 Keywords: genomics,Beacon
```

### Comparing `bycon-1.0.8/README.md` & `bycon-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/__init__.py` & `bycon-1.0.9/bycon/__init__.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/aggregator.py` & `bycon-1.0.9/bycon/beaconServer/aggregator.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/beacon.py` & `bycon-1.0.9/bycon/beaconServer/beacon.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/cohorts.py` & `bycon-1.0.9/bycon/beaconServer/cohorts.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/config/aggregator.yaml` & `bycon-1.0.9/bycon/beaconServer/config/aggregator.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/configuration.py` & `bycon-1.0.9/bycon/beaconServer/configuration.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/datasets.py` & `bycon-1.0.9/bycon/beaconServer/datasets.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/doc/handovers.md` & `bycon-1.0.9/bycon/beaconServer/doc/handovers.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/entryTypes.py` & `bycon-1.0.9/bycon/beaconServer/entryTypes.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/filteringTerms.py` & `bycon-1.0.9/bycon/beaconServer/filteringTerms.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/info.py` & `bycon-1.0.9/bycon/beaconServer/info.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/map.py` & `bycon-1.0.9/bycon/beaconServer/map.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/retriever.py` & `bycon-1.0.9/bycon/beaconServer/retriever.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/service_info.py` & `bycon-1.0.9/bycon/beaconServer/service_info.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/GET-examples.md` & `bycon-1.0.9/bycon/beaconServer/tests/GET-examples.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json` & `bycon-1.0.9/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/beaconServer/tests/terminal-examples.md` & `bycon-1.0.9/bycon/beaconServer/tests/terminal-examples.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/.DS_Store` & `bycon-1.0.9/bycon/config/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/argument_definitions.yaml` & `bycon-1.0.9/bycon/config/argument_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/beacon_defaults.yaml` & `bycon-1.0.9/bycon/config/beacon_defaults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/beacon_mappings.yaml` & `bycon-1.0.9/bycon/config/beacon_mappings.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/config.yaml` & `bycon-1.0.9/bycon/config/config.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/dataset_definitions.yaml` & `bycon-1.0.9/bycon/config/dataset_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/datatable_mappings.yaml` & `bycon-1.0.9/bycon/config/datatable_mappings.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/filter_definitions.yaml` & `bycon-1.0.9/bycon/config/filter_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/geoloc_definitions.yaml` & `bycon-1.0.9/bycon/config/geoloc_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/handover_definitions.yaml` & `bycon-1.0.9/bycon/config/handover_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/interval_definitions.yaml` & `bycon-1.0.9/bycon/config/interval_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/remap_definitions.yaml` & `bycon-1.0.9/bycon/config/remap_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/services_defaults.yaml` & `bycon-1.0.9/bycon/config/services_defaults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/services_mappings.yaml` & `bycon-1.0.9/bycon/config/services_mappings.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/config/variant_definitions.yaml` & `bycon-1.0.9/bycon/config/variant_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/aggregator_utils.py` & `bycon-1.0.9/bycon/lib/aggregator_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/args_parsing.py` & `bycon-1.0.9/bycon/lib/args_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/cgi_parsing.py` & `bycon-1.0.9/bycon/lib/cgi_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/cytoband_utils.py` & `bycon-1.0.9/bycon/lib/cytoband_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/data_retrieval.py` & `bycon-1.0.9/bycon/lib/data_retrieval.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/datatable_utils.py` & `bycon-1.0.9/bycon/lib/datatable_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/export_file_generation.py` & `bycon-1.0.9/bycon/lib/export_file_generation.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/filter_parsing.py` & `bycon-1.0.9/bycon/lib/filter_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/geomap_utils.py` & `bycon-1.0.9/bycon/lib/geomap_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/handover_generation.py` & `bycon-1.0.9/bycon/lib/handover_generation.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/interval_utils.py` & `bycon-1.0.9/bycon/lib/interval_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/publication_utils.py` & `bycon-1.0.9/bycon/lib/publication_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/query_execution.py` & `bycon-1.0.9/bycon/lib/query_execution.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/query_generation.py` & `bycon-1.0.9/bycon/lib/query_generation.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/read_specs.py` & `bycon-1.0.9/bycon/lib/read_specs.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/response_remapping.py` & `bycon-1.0.9/bycon/lib/response_remapping.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/schema_parsing.py` & `bycon-1.0.9/bycon/lib/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/service_utils.py` & `bycon-1.0.9/bycon/lib/service_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/lib/variant_parsing.py` & `bycon-1.0.9/bycon/lib/variant_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/.DS_Store` & `bycon-1.0.9/bycon/rsrc/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/.DS_Store` & `bycon-1.0.9/bycon/rsrc/genomes/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt` & `bycon-1.0.9/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/.DS_Store` & `bycon-1.0.9/bycon/schemas/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/ProgenetixLinkML/Publication.json` & `bycon-1.0.9/bycon/schemas/ProgenetixLinkML/Publication.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/ProgenetixLinkML/Publication.yaml` & `bycon-1.0.9/bycon/schemas/ProgenetixLinkML/Publication.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/ProgenetixLinkML/README.md` & `bycon-1.0.9/bycon/schemas/ProgenetixLinkML/README.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/ProgenetixLinkML/testpub.json` & `bycon-1.0.9/bycon/schemas/ProgenetixLinkML/testpub.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/bin/beaconYamler.py` & `bycon-1.0.9/bycon/schemas/bin/beaconYamler.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/bin/config/beaconYamler.yaml` & `bycon-1.0.9/bycon/schemas/bin/config/beaconYamler.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/bin/yamlerRunner.sh` & `bycon-1.0.9/bycon/schemas/bin/yamlerRunner.sh`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/.DS_Store` & `bycon-1.0.9/bycon/schemas/framework/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/basicElement.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/basicElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/beaconCommonComponents.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/beaconCommonComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/elementWithDescription.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/elementWithDescription.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/ontologizedElement.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/ontologizedElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/ontologyTerm.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/ontologyTerm.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/referenceToAnSchema.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/referenceToAnSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json` & `bycon-1.0.9/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/beaconMapSchema.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/beaconMapSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/entryTypeDefinition.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/entryTypeDefinition.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/entryTypesSchema.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/entryTypesSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/configuration/filteringTermsSchema.json` & `bycon-1.0.9/bycon/schemas/framework/json/configuration/filteringTermsSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/endpoints.json` & `bycon-1.0.9/bycon/schemas/framework/json/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/requests/beaconRequestBody.json` & `bycon-1.0.9/bycon/schemas/framework/json/requests/beaconRequestBody.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/requests/beaconRequestMeta.json` & `bycon-1.0.9/bycon/schemas/framework/json/requests/beaconRequestMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/requests/filteringTerms.json` & `bycon-1.0.9/bycon/schemas/framework/json/requests/filteringTerms.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/requests/validation/filteringTerms.json` & `bycon-1.0.9/bycon/schemas/framework/json/requests/validation/filteringTerms.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconBooleanResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconBooleanResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconCountResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconCountResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconErrorResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconErrorResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconInfoResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconInfoResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconMapResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconMapResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconResultsets.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconResultsets.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json` & `bycon-1.0.9/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/common/beaconCommonComponents.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/common/beaconCommonComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/common/ontologyTerm.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/common/ontologyTerm.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/common/referenceToAnSchema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/common/referenceToAnSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/requests/beaconRequestBody.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/requests/beaconRequestBody.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/requests/filteringTerms.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/requests/filteringTerms.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconCountResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconCountResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconMapResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconMapResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml` & `bycon-1.0.9/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/.DS_Store` & `bycon-1.0.9/bycon/schemas/models/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/analyses/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/analyses/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/beaconConfiguration.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/beaconConfiguration.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/beaconMap.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/beaconMap.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/biosamples/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/biosamples/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/ageRange.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/ageRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/commonDefinitions.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/commonDefinitions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/complexValue.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/complexValue.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/dataUseConditions.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/dataUseConditions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/disease.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/disease.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/doseInterval.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/doseInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/evidence.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/evidence.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/exposure.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/exposure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/externalReference.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/externalReference.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/gestationalAge.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/gestationalAge.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/measurement.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/measurement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/pedigree.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/pedigree.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/phenotypicFeature.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/phenotypicFeature.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/procedure.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/procedure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/quantity.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/quantity.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/referenceRange.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/referenceRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/timeElement.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/timeElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/timeInterval.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/timeInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/common/treatment.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/common/treatment.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-Max-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/datasets/examples/dataset-Max-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParameters.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParameters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParametersComponents.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/genomicVariations/requestParametersComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/pedigree-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/individuals/examples/pedigree-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MAX-example.json` & `bycon-1.0.9/bycon/schemas/models/json/beacon-v2-default-model/runs/examples/runs-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/framework/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/framework/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxCallset.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxCallset.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/beaconMap.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/beaconMap.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ageRange.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ageRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ancestry.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ancestry.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/complexValue.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/complexValue.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/disease.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/disease.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/doseInterval.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/doseInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/evidence.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/evidence.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/exposure.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/exposure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/externalReference.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/externalReference.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/file.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/file.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/measurement.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/measurement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/metaData.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/metaData.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/pedigree.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/pedigree.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/procedure.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/procedure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/provenance.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/provenance.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/quantity.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/quantity.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/referenceRange.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/referenceRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/resource.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/resource.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/timeElement.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/timeElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/timeInterval.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/timeInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/treatment.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/treatment.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/endpoints.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoJSONgeometry.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoJSONgeometry.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoLabels.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoLabels.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/GeoLocation.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/GeoLocation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/Publication.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/Publication.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/cytobandMapping.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/cytobandMapping.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponse.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseMeta.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseSummary.json` & `bycon-1.0.9/bycon/schemas/models/json/progenetix-service-schemas/progenetixServiceResponseSummary.json`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/analyses/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/analyses/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/beaconConfiguration.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/beaconConfiguration.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/beaconMap.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/beaconMap.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/biosamples/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/biosamples/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/cohorts/examples/cohorts-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/commonDefinitions.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/commonDefinitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/complexValue.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/complexValue.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/dataUseConditions.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/dataUseConditions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/disease.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/disease.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/doseInterval.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/doseInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/evidence.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/evidence.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/exposure.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/exposure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/externalReference.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/externalReference.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/gestationalAge.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/gestationalAge.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/measurement.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/measurement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/pedigree.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/pedigree.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/phenotypicFeature.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/phenotypicFeature.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/procedure.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/procedure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/referenceRange.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/referenceRange.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/timeElement.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/timeElement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/timeInterval.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/timeInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/common/treatment.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/common/treatment.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-Max-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/datasets/examples/dataset-Max-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/examples/genomicVariant-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParameters.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParameters.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParametersComponents.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/genomicVariations/requestParametersComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/individual-with-pedigree-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/pedigree-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/individuals/examples/pedigree-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/beacon-v2-default-model/runs/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/beacon-v2-default-model/runs/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/framework/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/framework/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxCallset.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxCallset.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/beaconMap.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/beaconMap.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/disease.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/disease.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/evidence.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/evidence.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/exposure.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/exposure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/file.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/file.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/measurement.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/measurement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/metaData.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/metaData.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/procedure.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/procedure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/provenance.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/provenance.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/resource.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/resource.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/treatment.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/treatment.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoJSONgeometry.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoJSONgeometry.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoLabels.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoLabels.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/GeoLocation.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/GeoLocation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/cytobandMapping.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/cytobandMapping.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponse.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseSummary.yaml` & `bycon-1.0.9/bycon/schemas/models/src/progenetix-service-schemas/progenetixServiceResponseSummary.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/collations.py` & `bycon-1.0.9/bycon/services/collations.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/config/collations.yaml` & `bycon-1.0.9/bycon/services/config/collations.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/config/genespans.yaml` & `bycon-1.0.9/bycon/services/config/genespans.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/config/ids.yaml` & `bycon-1.0.9/bycon/services/config/ids.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/config/publications.yaml` & `bycon-1.0.9/bycon/services/config/publications.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/cytomapper.py` & `bycon-1.0.9/bycon/services/cytomapper.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/dbstats.py` & `bycon-1.0.9/bycon/services/dbstats.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/collations.md` & `bycon-1.0.9/bycon/services/doc/collations.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/cytomapper.md` & `bycon-1.0.9/bycon/services/doc/cytomapper.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/geolocations.md` & `bycon-1.0.9/bycon/services/doc/geolocations.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/intervalFrequencies.md` & `bycon-1.0.9/bycon/services/doc/intervalFrequencies.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/phenopackets.md` & `bycon-1.0.9/bycon/services/doc/phenopackets.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/publications.md` & `bycon-1.0.9/bycon/services/doc/publications.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/doc/services.md` & `bycon-1.0.9/bycon/services/doc/services.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/endpoints.py` & `bycon-1.0.9/bycon/services/endpoints.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/genespans.py` & `bycon-1.0.9/bycon/services/genespans.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/geolocations.py` & `bycon-1.0.9/bycon/services/geolocations.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/ids.py` & `bycon-1.0.9/bycon/services/ids.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/intervalFrequencies.py` & `bycon-1.0.9/bycon/services/intervalFrequencies.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/ontologymaps.py` & `bycon-1.0.9/bycon/services/ontologymaps.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/publications.py` & `bycon-1.0.9/bycon/services/publications.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/schemas.py` & `bycon-1.0.9/bycon/services/schemas.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/services.py` & `bycon-1.0.9/bycon/services/services.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon/services/uploader.py` & `bycon-1.0.9/bycon/services/uploader.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/bycon.egg-info/PKG-INFO` & `bycon-1.0.9/bycon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bycon
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python-based environment for the Beacon v2 genomics API
 Home-page: https://github.com/progenetix/bycon
 Author: Michael Baudis
 Author-email: contact@progenetix.org
 Project-URL: Bug Reports, https://github.com/progenetix/bycon/issues
 Project-URL: Source, https://github.com/progenetix/bycon/
 Keywords: genomics,Beacon
```

### Comparing `bycon-1.0.8/bycon.egg-info/SOURCES.txt` & `bycon-1.0.9/bycon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/css/extra.css` & `bycon-1.0.9/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/handovers.md` & `bycon-1.0.9/docs/handovers.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/img/site-logo-main.png` & `bycon-1.0.9/docs/img/site-logo-main.png`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/img/site-logo-topright.png` & `bycon-1.0.9/docs/img/site-logo-topright.png`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/index.md` & `bycon-1.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/docs/tests.md` & `bycon-1.0.9/docs/tests.md`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/install.py` & `bycon-1.0.9/install.py`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/mkdocs.yaml` & `bycon-1.0.9/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.0.8/setup.py` & `bycon-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="bycon",
-    version="1.0.8",
+    version="1.0.9",
     description="A Python-based environment for the Beacon v2 genomics API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/progenetix/bycon",
     author="Michael Baudis",
     author_email="contact@progenetix.org",
     classifiers=[
```

