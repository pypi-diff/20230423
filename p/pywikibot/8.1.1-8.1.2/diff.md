# Comparing `tmp/pywikibot-8.1.1.tar.gz` & `tmp/pywikibot-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.1.1.tar", last modified: Fri Apr 21 08:21:51 2023, max compression
+gzip compressed data, was "pywikibot-8.1.2.tar", last modified: Sun Apr 23 07:55:56 2023, max compression
```

## Comparing `pywikibot-8.1.1.tar` & `pywikibot-8.1.2.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.591101 pywikibot-8.1.1/
--rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.1/LICENSE
--rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14586 2023-04-21 08:21:51.589108 pywikibot-8.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.1/README.rst
--rw-rw-rw-   0        0        0     6351 2023-04-16 15:04:28.000000 pywikibot-8.1.1/make_dist.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.974750 pywikibot-8.1.1/pywikibot/
--rw-rw-rw-   0        0        0    55820 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-04-21 07:37:30.000000 pywikibot-8.1.1/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/backports.py
--rw-rw-rw-   0        0        0    96117 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.998685 pywikibot-8.1.1/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    19597 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46527 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/config.py
--rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.005666 pywikibot-8.1.1/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.012647 pywikibot-8.1.1/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.1/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    52512 2023-04-16 16:10:48.000000 pywikibot-8.1.1/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96940 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/date.py
--rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2042 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/editor.py
--rw-rw-rw-   0        0        0    21221 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.047566 pywikibot-8.1.1/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-04-16 15:09:16.000000 pywikibot-8.1.1/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1742 2023-04-18 14:17:02.000000 pywikibot-8.1.1/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10737 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-04-21 05:58:04.000000 pywikibot-8.1.1/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.1/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3843 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2414 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    37565 2023-04-18 14:17:02.000000 pywikibot-8.1.1/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/flow.py
--rw-rw-rw-   0        0        0    30038 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22781 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.066504 pywikibot-8.1.1/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86912 2023-04-17 14:18:54.000000 pywikibot-8.1.1/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    86375 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.071504 pywikibot-8.1.1/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29164 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48967 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.084456 pywikibot-8.1.1/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    12032 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20029 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.086450 pywikibot-8.1.1/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.538241 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18491 2023-04-20 07:19:22.000000 pywikibot-8.1.1/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.558189 pywikibot-8.1.1/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   112506 2023-04-16 16:10:48.000000 pywikibot-8.1.1/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15858 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    93641 2023-04-17 14:52:33.000000 pywikibot-8.1.1/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1667 2023-04-18 14:53:43.000000 pywikibot-8.1.1/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4868 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11156 2023-04-21 07:28:37.000000 pywikibot-8.1.1/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.565171 pywikibot-8.1.1/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.577140 pywikibot-8.1.1/pywikibot/tools/
--rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.587112 pywikibot-8.1.1/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22100 2023-04-16 15:04:28.000000 pywikibot-8.1.1/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.1/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:50.995694 pywikibot-8.1.1/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    14586 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10447 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 08:21:50.000000 pywikibot-8.1.1/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 08:21:51.591101 pywikibot-8.1.1/setup.cfg
--rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:21:51.588110 pywikibot-8.1.1/tests/
--rw-rw-rw-   0        0        0     2814 2023-04-16 15:04:28.000000 pywikibot-8.1.1/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.433088 pywikibot-8.1.2/
+-rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.2/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    14626 2023-04-23 07:55:56.432156 pywikibot-8.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.2/README.rst
+-rw-rw-rw-   0        0        0     6351 2023-04-16 15:04:28.000000 pywikibot-8.1.2/make_dist.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.307106 pywikibot-8.1.2/pywikibot/
+-rw-rw-rw-   0        0        0    55820 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-23 07:34:55.000000 pywikibot-8.1.2/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    96117 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.382276 pywikibot-8.1.2/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    19597 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46527 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.393057 pywikibot-8.1.2/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.404032 pywikibot-8.1.2/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-04-22 08:48:04.000000 pywikibot-8.1.2/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.2/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    52512 2023-04-16 16:10:48.000000 pywikibot-8.1.2/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96940 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2042 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    21221 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.459884 pywikibot-8.1.2/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-04-16 15:09:16.000000 pywikibot-8.1.2/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1742 2023-04-18 14:17:02.000000 pywikibot-8.1.2/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1832 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10737 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-04-21 05:58:04.000000 pywikibot-8.1.2/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.2/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     3850 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2414 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    37565 2023-04-18 14:17:02.000000 pywikibot-8.1.2/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    30038 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22781 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.482845 pywikibot-8.1.2/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86912 2023-04-17 14:18:54.000000 pywikibot-8.1.2/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    86375 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.490821 pywikibot-8.1.2/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29164 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48967 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.504819 pywikibot-8.1.2/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12032 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20029 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.515767 pywikibot-8.1.2/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.346323 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18384 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.384219 pywikibot-8.1.2/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112506 2023-04-16 16:10:48.000000 pywikibot-8.1.2/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15858 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    93641 2023-04-17 14:52:33.000000 pywikibot-8.1.2/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1667 2023-04-18 14:53:43.000000 pywikibot-8.1.2/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4868 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11156 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.392197 pywikibot-8.1.2/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.414139 pywikibot-8.1.2/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27376 2023-04-23 07:41:13.000000 pywikibot-8.1.2/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25547 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-04-22 12:39:46.000000 pywikibot-8.1.2/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4084 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    11075 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4021 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9745 2023-04-22 12:39:48.000000 pywikibot-8.1.2/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7334 2023-04-22 12:39:48.000000 pywikibot-8.1.2/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.427106 pywikibot-8.1.2/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22100 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.375086 pywikibot-8.1.2/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    14626 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10447 2023-04-23 07:55:55.000000 pywikibot-8.1.2/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 07:55:56.433444 pywikibot-8.1.2/setup.cfg
+-rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.430478 pywikibot-8.1.2/tests/
+-rw-rw-rw-   0        0        0     2814 2023-04-16 15:04:28.000000 pywikibot-8.1.2/tests/tests_tests.py
```

### Comparing `pywikibot-8.1.1/AUTHORS.rst` & `pywikibot-8.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/LICENSE` & `pywikibot-8.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/PKG-INFO` & `pywikibot-8.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.1
+Version: 8.1.2
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,17 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for fatwikipedia (T335021)
-* Add support for kcgwiktionary (T334742)
-* Update for wowwiki family
+* Add support for guwwikinews (T334461)
+* Add support for kbdwiktionary (T333271)
+* Fix tools.chars.url2stringparsing for multiple encodings (T335224)
 
 
 Deprecations
 ------------
 
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
```

### Comparing `pywikibot-8.1.1/README.rst` & `pywikibot-8.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/make_dist.py` & `pywikibot-8.1.2/make_dist.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/__init__.py` & `pywikibot-8.1.2/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/__metadata__.py` & `pywikibot-8.1.2/pywikibot/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.1.1'
+__version__ = '8.1.2'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.1.1/pywikibot/_wbtypes.py` & `pywikibot-8.1.2/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/backports.py` & `pywikibot-8.1.2/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/bot.py` & `pywikibot-8.1.2/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/bot_choice.py` & `pywikibot-8.1.2/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/comms/eventstreams.py` & `pywikibot-8.1.2/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/comms/http.py` & `pywikibot-8.1.2/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/config.py` & `pywikibot-8.1.2/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/cosmetic_changes.py` & `pywikibot-8.1.2/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/daemonize.py` & `pywikibot-8.1.2/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/api/__init__.py` & `pywikibot-8.1.2/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/api/_generators.py` & `pywikibot-8.1.2/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/api/_optionset.py` & `pywikibot-8.1.2/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.1.2/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/api/_requests.py` & `pywikibot-8.1.2/pywikibot/data/api/_requests.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/memento.py` & `pywikibot-8.1.2/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/mysql.py` & `pywikibot-8.1.2/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/sparql.py` & `pywikibot-8.1.2/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/data/wikistats.py` & `pywikibot-8.1.2/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/date.py` & `pywikibot-8.1.2/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/diff.py` & `pywikibot-8.1.2/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/echo.py` & `pywikibot-8.1.2/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/editor.py` & `pywikibot-8.1.2/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/exceptions.py` & `pywikibot-8.1.2/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/commons_family.py` & `pywikibot-8.1.2/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/lingualibre_family.py` & `pywikibot-8.1.2/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/meta_family.py` & `pywikibot-8.1.2/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/osm_family.py` & `pywikibot-8.1.2/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/vikidia_family.py` & `pywikibot-8.1.2/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikibooks_family.py` & `pywikibot-8.1.2/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikidata_family.py` & `pywikibot-8.1.2/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikihow_family.py` & `pywikibot-8.1.2/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikimania_family.py` & `pywikibot-8.1.2/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.1.2/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikinews_family.py` & `pywikibot-8.1.2/pywikibot/families/wikinews_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Family module for Wikinews."""
 #
-# (C) Pywikibot team, 2005-2022
+# (C) Pywikibot team, 2005-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 
 
 # The Wikimedia family that is known as Wikinews
@@ -18,15 +18,15 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/closed.dblist
         'bg', 'hu', 'sd', 'th', 'tr',
     ]
 
     languages_by_size = [
         'ru', 'sr', 'pt', 'fr', 'en', 'pl', 'zh', 'de', 'es', 'it', 'ar', 'cs',
         'ca', 'nl', 'el', 'ta', 'li', 'sv', 'uk', 'fa', 'fi', 'ro', 'ja', 'eo',
-        'sq', 'no', 'ko', 'bs', 'he',
+        'sq', 'no', 'ko', 'bs', 'he', 'guw',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'fa': ('الگو:رده بهتر',),
         'no': ('Kategoriomdirigering',),
```

### Comparing `pywikibot-8.1.1/pywikibot/families/wikipedia_family.py` & `pywikibot-8.1.2/pywikibot/families/wikipedia_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,32 @@
         'ast', 'zh-yue', 'lld', 'lv', 'tg', 'af', 'my', 'mg', 'bs', 'mr', 'sq',
         'oc', 'nds', 'ml', 'be-tarask', 'te', 'ky', 'br', 'sw', 'jv', 'new',
         'vec', 'pnb', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
         'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
         'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'bar', 'scn', 'bpy',
         'ha', 'crh', 'qu', 'nv', 'mn', 'xmf', 'si', 'ban', 'ps', 'frr',
         'bat-smg', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'sd', 'ilo',
-        'am', 'nap', 'mzn', 'li', 'ig', 'gor', 'fo', 'hsb', 'map-bms', 'mai',
+        'am', 'nap', 'mzn', 'ig', 'li', 'gor', 'fo', 'hsb', 'map-bms', 'mai',
         'bcl', 'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'as', 'ie',
         'lij', 'zu', 'mhr', 'hyw', 'hif', 'sn', 'mrj', 'tum', 'bjn', 'mni',
         'km', 'hak', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se',
         'myv', 'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab',
-        'tk', 'ary', 'gan', 'dag', 'co', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
+        'tk', 'dag', 'ary', 'gan', 'co', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
         'skr', 'ug', 'zea', 'frp', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn',
         'smn', 'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang',
         'fur', 'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln',
-        'dty', 'kaa', 'pap', 'cbk-zam', 'dv', 'mdf', 'ksh', 'tw', 'ks', 'gag',
+        'dty', 'kaa', 'pap', 'cbk-zam', 'mdf', 'dv', 'ksh', 'tw', 'ks', 'gag',
         'bxr', 'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay',
         'blk', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw',
-        'jam', 'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'ki', 'nqo',
-        'anp', 'bi', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'om', 'kg',
+        'jam', 'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'anp', 'ki',
+        'nqo', 'bi', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'om', 'kg',
         'lbe', 'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr',
         'ltg', 'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'rmy', 'ami', 'bm',
         'ff', 've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt',
-        'ady', 'guc', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
+        'guc', 'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
         'fat', 'cr',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
```

### Comparing `pywikibot-8.1.1/pywikibot/families/wikiquote_family.py` & `pywikibot-8.1.2/pywikibot/families/wikiquote_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikisource_family.py` & `pywikibot-8.1.2/pywikibot/families/wikisource_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikiversity_family.py` & `pywikibot-8.1.2/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.1.2/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/families/wiktionary_family.py` & `pywikibot-8.1.2/pywikibot/families/wiktionary_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         'lv', 'sq', 'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue',
         'sa', 'kk', 'km', 'ckb', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm',
         'hsb', 'ks', 'shy', 'su', 'bcl', 'gd', 'ga', 'an', 'gom', 'mr', 'wo',
         'mni', 'bjn', 'ia', 'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie',
         'ha', 'mi', 'csb', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
         'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'kcg',
         'am', 'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti',
-        'tn',
+        'tn', 'kbd',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'zh': ('分类重定向',),
     }
```

### Comparing `pywikibot-8.1.1/pywikibot/families/wowwiki_family.py` & `pywikibot-8.1.2/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/family.py` & `pywikibot-8.1.2/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/fixes.py` & `pywikibot-8.1.2/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/flow.py` & `pywikibot-8.1.2/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/i18n.py` & `pywikibot-8.1.2/pywikibot/i18n.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/interwiki_graph.py` & `pywikibot-8.1.2/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/logentries.py` & `pywikibot-8.1.2/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/logging.py` & `pywikibot-8.1.2/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/login.py` & `pywikibot-8.1.2/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/__init__.py` & `pywikibot-8.1.2/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_basepage.py` & `pywikibot-8.1.2/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_category.py` & `pywikibot-8.1.2/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_collections.py` & `pywikibot-8.1.2/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_decorators.py` & `pywikibot-8.1.2/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_filepage.py` & `pywikibot-8.1.2/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_links.py` & `pywikibot-8.1.2/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_page.py` & `pywikibot-8.1.2/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_revision.py` & `pywikibot-8.1.2/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_toolforge.py` & `pywikibot-8.1.2/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_user.py` & `pywikibot-8.1.2/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/page/_wikibase.py` & `pywikibot-8.1.2/pywikibot/page/_wikibase.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.1.2/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.1.2/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.1.2/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.1.2/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/plural.py` & `pywikibot-8.1.2/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/proofreadpage.py` & `pywikibot-8.1.2/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/__init__.py` & `pywikibot-8.1.2/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.1.2/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.1.2/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/login.py` & `pywikibot-8.1.2/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/preload_sites.py` & `pywikibot-8.1.2/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/shell.py` & `pywikibot-8.1.2/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/version.py` & `pywikibot-8.1.2/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/scripts/wrapper.py` & `pywikibot-8.1.2/pywikibot/scripts/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,14 @@
             str(wrapper_dir.joinpath('generate_user_files.py')), [])
         # because we have loaded pywikibot without user-config.py loaded,
         # we need to re-start the entire process. Ask the user to do so.
         print('Now, you have to re-execute the command to start your script.')
         sys.exit(1)
 except ImportError as e:  # raised in textlib
     sys.exit(e)
-except SyntaxError as e:  # pragma: no cover
-    sys.exit(str(e) + '\nProbably outdated Python version')
 
 
 def find_alternates(filename, script_paths):
     """Search for similar filenames in the given script paths."""
     from pywikibot import config, error, info, input_choice, warning
     from pywikibot.bot import QuitKeyboardInterrupt, ShowingListOption
```

### Comparing `pywikibot-8.1.1/pywikibot/site/__init__.py` & `pywikibot-8.1.2/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_apisite.py` & `pywikibot-8.1.2/pywikibot/site/_apisite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_basesite.py` & `pywikibot-8.1.2/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_datasite.py` & `pywikibot-8.1.2/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_decorators.py` & `pywikibot-8.1.2/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_extensions.py` & `pywikibot-8.1.2/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_generators.py` & `pywikibot-8.1.2/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_interwikimap.py` & `pywikibot-8.1.2/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_namespace.py` & `pywikibot-8.1.2/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_obsoletesites.py` & `pywikibot-8.1.2/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_siteinfo.py` & `pywikibot-8.1.2/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_tokenwallet.py` & `pywikibot-8.1.2/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site/_upload.py` & `pywikibot-8.1.2/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/site_detect.py` & `pywikibot-8.1.2/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/specialbots/_unlink.py` & `pywikibot-8.1.2/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/specialbots/_upload.py` & `pywikibot-8.1.2/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/textlib.py` & `pywikibot-8.1.2/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/throttle.py` & `pywikibot-8.1.2/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/time.py` & `pywikibot-8.1.2/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/titletranslate.py` & `pywikibot-8.1.2/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/__init__.py` & `pywikibot-8.1.2/pywikibot/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Miscellaneous helper functions (not wiki-dependent)."""
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
+import abc
 import bz2
 import gzip
 import hashlib
 import ipaddress
 import lzma
 import os
 import re
@@ -112,15 +113,15 @@
     """
     try:
         m = import_module(module)
     except ImportError:
         return False
     if version:
         if not hasattr(m, '__version__'):
-            return False
+            return False  # pragma: no cover
 
         required_version = pkg_resources.parse_version(version)
         module_version = pkg_resources.parse_version(m.__version__)
 
         if module_version < required_version:
             warn('Module version {} is lower than requested version {}'
                  .format(module_version, required_version), ImportWarning)
@@ -222,21 +223,30 @@
         def suppressed_func(*args, **kwargs):
             with self:
                 return func(*args, **kwargs)
         return suppressed_func
 
 
 # From http://python3porting.com/preparing.html
-class ComparableMixin:
+class ComparableMixin(abc.ABC):
 
     """Mixin class to allow comparing to other objects which are comparable.
 
     .. versionadded:: 3.0
     """
 
+    @abc.abstractmethod
+    def _cmpkey(self) -> Any:
+        """Abstract method to return key for comparison of objects.
+
+        This ensures that ``_cmpkey`` method is defined in subclass.
+
+        .. versionadded:: 8.1.2
+        """
+
     def __lt__(self, other):
         """Compare if self is less than other."""
         return other > self._cmpkey()
 
     def __le__(self, other):
         """Compare if self is less equals other."""
         return other >= self._cmpkey()
```

### Comparing `pywikibot-8.1.1/pywikibot/tools/_deprecate.py` & `pywikibot-8.1.2/pywikibot/tools/_deprecate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 only one arg, and that arg be a callable, as it will be detected as
 a deprecator without any arguments.
 
 .. versionchanged:: 6.4
    deprecation decorators moved to _deprecate submodule
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import collections
 import inspect
 import re
 import sys
@@ -153,15 +153,15 @@
         if (len(outer_args) == 1 and not outer_kwargs
                 and callable(outer_args[0])):
             add_decorated_full_name(outer_args[0])
             return obj(outer_args[0])
         return inner_wrapper
 
     if not __debug__:
-        return obj
+        return obj  # pragma: no cover
 
     return outer_wrapper
 
 
 def _build_msg_string(instead: str, since: str) -> str:
     """Build a deprecation warning message format string.
 
@@ -250,15 +250,15 @@
                 deprecation_notice += '; use ' + instead + ' instead'
             deprecation_notice += '.\n\n'
             if wrapper.__doc__:  # Append old docstring after the notice
                 wrapper.__doc__ = deprecation_notice + wrapper.__doc__
             else:
                 wrapper.__doc__ = deprecation_notice
 
-        if not __debug__:
+        if not __debug__:  # pragma: no cover
             return obj
 
         manage_wrapping(wrapper, obj)
 
         # Regular expression to find existing deprecation notices
         deprecated_notice = re.compile(r'(^|\s)DEPRECATED[.:;,]',
                                        re.IGNORECASE)
@@ -286,15 +286,15 @@
         instead = args[0]
     else:
         instead = False
 
     # When called as @deprecated, return a replacement function
     if without_parameters:
         if not __debug__:
-            return args[0]
+            return args[0]  # pragma: no cover
 
         return decorator(args[0])
 
     # Otherwise return a decorator, which returns a replacement function
     return decorator
 
 
@@ -392,15 +392,15 @@
                          .format_map(output_args),
                          cls, depth)
                 del __kw[old_arg]
 
             return obj(*__args, **__kw)
 
         if not __debug__:
-            return obj
+            return obj  # pragma: no cover
 
         manage_wrapping(wrapper, obj)
 
         if wrapper.__signature__:
             # Build a new signature with deprecated args added.
             params = collections.OrderedDict()
             for param in wrapper.__signature__.parameters.values():
```

### Comparing `pywikibot-8.1.1/pywikibot/tools/_logging.py` & `pywikibot-8.1.2/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/_unidata.py` & `pywikibot-8.1.2/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/chars.py` & `pywikibot-8.1.2/pywikibot/tools/chars.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Character based helper functions (not wiki-dependent)."""
 #
-# (C) Pywikibot team, 2015-2022
+# (C) Pywikibot team, 2015-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import re
 import sys
 from contextlib import suppress
 from typing import Union
 from urllib.parse import unquote_to_bytes
 
-from pywikibot.backports import List, Tuple
+from pywikibot.backports import Iterable
 from pywikibot.tools._unidata import _category_cf
 
 
 # This is a set of all invisible characters
 # At the moment we've only added the characters from the Cf category
 _invisible_chars = _category_cf
 
@@ -41,14 +41,23 @@
 
     return INVISIBLE_REGEX.sub(replace, text)
 
 
 def string_to_ascii_html(string: str) -> str:
     """Convert unicode chars of str to HTML entities if chars are not ASCII.
 
+    **Example:**
+
+    >>> string_to_ascii_html('Python')
+    'Python'
+    >>> string_to_ascii_html("Pywikibot's API")
+    "Pywikibot's API"
+    >>> string_to_ascii_html('Eetße Joohunndot füür Kreůßtůß')
+    'Eet&#223;e Joohunndot f&#252;&#252;r Kre&#367;&#223;t&#367;&#223;'
+
     :param string: String to update
     """
     html = []
     for c in string:
         cord = ord(c)
         if 31 < cord < 127:
             html.append(c)
@@ -60,46 +69,68 @@
 def string2html(string: str, encoding: str) -> str:
     """Convert unicode string to requested HTML encoding.
 
     Attempt to encode the string into the desired format; if that work
     return it unchanged. Otherwise encode the non-ASCII characters into
     HTML &#; entities.
 
+    **Example:**
+
+    >>> string2html('Referências', 'utf-8')
+    'Referências'
+    >>> string2html('Referências', 'ascii')
+    'Refer&#234;ncias'
+    >>> string2html('脚注', 'euc_jp')
+    '脚注'
+    >>> string2html('脚注', 'iso-8859-1')
+    '&#33050;&#27880;'
+
     :param string: String to update
     :param encoding: Encoding to use
     """
     with suppress(UnicodeError):
         string.encode(encoding)
         return string
 
     return string_to_ascii_html(string)
 
 
-def url2string(
-    title: str,
-    encodings: Union[str, List[str], Tuple[str, ...]] = 'utf-8'
-) -> str:
+def url2string(title: str,
+               encodings: Union[str, Iterable[str]] = 'utf-8') -> str:
     """Convert URL-encoded text to unicode using several encoding.
 
     Uses the first encoding that doesn't cause an error.
 
+    **Example:**
+
+    >>> url2string('/El%20Ni%C3%B1o/')
+    '/El Niño/'
+    >>> url2string('/El%20Ni%C3%B1o/', 'ascii')
+    Traceback (most recent call last):
+    ...
+    UnicodeDecodeError: 'ascii' codec can't decode byte 0xc3 in position 6:...
+    >>> url2string('/El%20Ni%C3%B1o/', ['ascii', 'utf-8'])
+    '/El Niño/'
+
     :param title: URL-encoded character data to convert
     :param encodings: Encodings to attempt to use during conversion.
 
     :raise UnicodeError: Could not convert using any encoding.
+    :raise LookupError: unknown encoding
     """
     if isinstance(encodings, str):
         encodings = [encodings]
 
     first_exception = None
     for enc in encodings:
         try:
             t = title.encode(enc)
             t = unquote_to_bytes(t)
+            result = t.decode(enc)
         except UnicodeError as e:
             if not first_exception:
                 first_exception = e
         else:
-            return t.decode(enc)
+            return result
 
     # Couldn't convert, raise the first exception
     raise first_exception
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywikibot-8.1.1/pywikibot/tools/collections.py` & `pywikibot-8.1.2/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/djvu.py` & `pywikibot-8.1.2/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/formatter.py` & `pywikibot-8.1.2/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/itertools.py` & `pywikibot-8.1.2/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/tools/threading.py` & `pywikibot-8.1.2/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/gui.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.1.2/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/version.py` & `pywikibot-8.1.2/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot/xmlreader.py` & `pywikibot-8.1.2/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.1.2/pywikibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.1
+Version: 8.1.2
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,17 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for fatwikipedia (T335021)
-* Add support for kcgwiktionary (T334742)
-* Update for wowwiki family
+* Add support for guwwikinews (T334461)
+* Add support for kbdwiktionary (T333271)
+* Fix tools.chars.url2stringparsing for multiple encodings (T335224)
 
 
 Deprecations
 ------------
 
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
```

### Comparing `pywikibot-8.1.1/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.1.2/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/pywikibot.egg-info/requires.txt` & `pywikibot-8.1.2/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/setup.py` & `pywikibot-8.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.1/tests/tests_tests.py` & `pywikibot-8.1.2/tests/tests_tests.py`

 * *Files identical despite different names*

