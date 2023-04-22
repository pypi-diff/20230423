# Comparing `tmp/tagstr-0.0.1.tar.gz` & `tmp/tagstr-0.1.0.tar.gz`

## Comparing `tagstr-0.0.1.tar` & `tagstr-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,154 @@
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 tagstr-0.0.1/temp.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr.pth
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/decorator.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/importer.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/tokenizer.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/transform.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tagstr-0.0.1/tagstr/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tagstr-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 tagstr-0.0.1/tests/case_utils.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 tagstr-0.0.1/tests/test_transform.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 tagstr-0.0.1/tests/cases/transform.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tagstr-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tagstr-0.0.1/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tagstr-0.0.1/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 tagstr-0.0.1/hatch.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tagstr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tagstr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tagstr-0.1.0/temp.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 tagstr-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1202fd3817ee8abe
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/12e653c2cc8b713b
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/16ce0992725e7c99
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1a3f3a94f182d98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1a9be57c5988a68e
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1b09e8d5534476ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1c013fcb5cc738da
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1d75279975891254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/21a2d50da587646a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/21d71b3f3a93829e
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/2341cf1e5946409b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/245d3838a84d1f0d
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/266ac9dcb2a917d3
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/27811028d704c6dc
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/27c5b6fdeba5b7ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/28ba20d8130bc981
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/29b747fe319f3777
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/2fb7e82c318c343b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/30c0fd9ab36ae7bf
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/32b441a8aac0cf4d
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/33344ab4632fffe3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3385489d09b32bc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/36fdc51d203ffca2
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/38df0e9f6de8d029
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/39c329b1df4a32dc
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3b244ec237a19c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3c61c1cdf4ba0e63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e13dc3fa7e13b8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e62ffaafef90d4c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e7426aee801e771
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3fcc684d6dfed26e
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4197cbc369ca1e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/428d4324098031a9
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/42a93bc19bd61f5b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/43416d462caa1fcb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/43e86f39ac064e7f
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4cbb8f887305a1df
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4cfe6a27ce54d44
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4d8867984beffb14
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/50d67579f5cab43f
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/52d2b1c7e14a2ec1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/55b948d7f4ae828b
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/5810920ecddb0d55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/5a66575126fa05ed
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/61f496d82ce99454
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6304bb1f9620b3ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/645eddb2cf3fddd
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6545ffff0952bf2d
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/664c859e0aae0a20
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/66712d58b28d9e32
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/675043ab6278d320
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6853ecaed51fc9cd
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6a2ba283404ca374
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6b02b2ba7a92df26
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6b0d9aea501453e7
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6c549a9787be1e33
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6f8561c81fa54afb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/715b236edbd49e36
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/72b4201b626ff8eb
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7b1d68a8b1cbced5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7e310898b4d4b55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7e81d7d55cc63f63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/804207c459a53f60
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/80d3ae37a5fa9e17
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8148ea1ef8f6d144
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/83907ccb56b539c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/85e7e087c05a9362
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/85fea8713d811823
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/88dac8158c303086
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8aa6519d8d62ed53
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8add245186a0b55e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9211b78fec2ce010
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9228807ce7870a24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/93003edc8ca546c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/94ff10896f94f1e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/96160b841e5b28b1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9764fd4dcd5b66d
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9b11259f9ce28217
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9ba39e9875d3697
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9d371d6b54954c2e
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9ef909f97faedc23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a1b6eeabe36ab1fb
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a472d58082639e5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a625cbbc8778b4d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a6c468410e5aedd9
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a845e6fdb39e199b
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a96cd35c46eb9c8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a98857b51534a9ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ae84286265f9ee63
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/aea3e8c4b5fc68df
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b10fa97d4b462364
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b33f91249c322634
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b6bc86e562ee72d
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b7695d0f2bcd40b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b865b8e6af8bd1e5
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b9583e55d182ceee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/baaa7127908ac1fd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/bb8b64ef50f76867
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/bfbd92fb5d0b4a8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/c6a73143aa527759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/cf5249c8f3e3b1d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d04e2e28866d6219
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d1f94f80a7aa473e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d3866544a2d61dcf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d521ac457c4419d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d7d962891d453308
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d8170825e811e0f9
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d89feb8d30129dc4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/daa7b455394ab040
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dc2de1bca0ba0bc5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dcb3545fc211fb66
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dcf4672b52977830
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ddb845997320023d
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dddf49b53830f171
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/df48c1b44d24756c
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e0751dbc4c0c1e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e31eb0145ab1b3e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e7145fe6e2786e58
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ec29a3884ae9399b
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ed32a4005c3b40ed
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ee12d3323a728899
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f1c6bcd7640579f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f1ed93c6f6981943
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f241e50fbb067a72
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f29e6b327684303c
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f466ece879291fd1
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5537e6fc46b6c71
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5b4c0f80798dd5
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5eeb30888472a10
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f80a89ebefeebbd2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f8f0ff85963c19cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/faec6021ef8ffc2a
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/fbd3d3dd5e077779
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr.pth
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/decorator.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/importer.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/tokenizer.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/transform.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/types.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/case_utils.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/test_transform.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/cases/transform.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tagstr-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tagstr-0.1.0/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tagstr-0.1.0/README.md
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 tagstr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tagstr-0.1.0/PKG-INFO
```

### Comparing `tagstr-0.0.1/tagstr/decorator.py` & `tagstr-0.1.0/tagstr/decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
-from typing import Generic, TypeVar, Protocol
 
-from tagstr.utils import Thunk
+from typing import Generic, TypeVar
+
+from tagstr.types import TagFunc, Thunk
 
 T = TypeVar("T")
 
 
 class tagfunc(Generic[T]):
     def __init__(self, func: TagFunc[T]) -> None:
         self.func = func
@@ -14,12 +15,7 @@
         raise NotImplementedError(
             "Usages of `tag @ f'string'` must be transpiled - is there an "
             "`import tagstr` statement placed at the top of your file?"
         )
 
     def __call__(self, *args: str | Thunk) -> T:
         return self.func(*args)
-
-
-class TagFunc(Protocol[T]):
-    def __call__(self, *args: Thunk) -> T:
-        ...
```

### Comparing `tagstr-0.0.1/tagstr/tokenizer.py` & `tagstr-0.1.0/tagstr/tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from io import StringIO
+from __future__ import annotations
+
 import ast
+from io import StringIO
 from tokenize import (
-    TokenInfo,
-    Untokenizer,
+    COMMA,
     NAME,
-    OP,
-    STRING,
     NEWLINE,
     NL,
-    COMMA,
+    OP,
+    STRING,
+    TokenInfo,
+    Untokenizer,
     generate_tokens,
 )
-from typing import Callable, Iterable, Iterator
+from typing import Callable, Iterable, Iterator, cast
 
 
 def tagstr_untokenize(tokens: Iterator[TokenInfo]) -> str:
     return Untokenizer().untokenize(tokens)
 
 
 def tagstr_tokenize(readline: Callable[[], str]) -> Iterator[TokenInfo]:
@@ -24,68 +26,69 @@
 
 class TransformedTokenStream:
     """Token stream that can be transformed mid-stream."""
 
     def __init__(
         self,
         readline: Callable[[], str],
-        transform: Callable[[Iterator[TokenInfo]], Iterable[TokenInfo] | None],
+        transform: Callable[[RewindableStream], Iterable[TokenInfo] | None],
     ) -> None:
         self._transform = transform
         self._readline = readline
 
     def __iter__(self) -> Iterator[TokenInfo]:
-        buffer: list[TokenInfo] = []
-
-        def make_stream():
-            for token in generate_tokens(self._readline):
-                buffer.append(token)
-                yield token
-
-        stream = make_stream()
+        stream = RewindableStream(generate_tokens(self._readline))
         last_position = (0, 0)
         while True:
             try:
                 changed = self._transform(stream)
+                consumed = stream.consumed(clear=True)
                 if changed is not None:
                     changed = list(changed)
                     yield from changed
                     last_position = changed[-1].end
                 else:
-                    for token in buffer:
+                    for token in consumed:
                         last_line, last_column = last_position
                         start_line, start_column = token.start
                         if start_line == last_line and start_column <= last_column:
                             token = move(token, (0, last_column - start_column))
                         yield token
                     last_position = token.end
-                buffer.clear()
             except StopIteration:
                 break
 
 
-def move(token: TokenInfo, shift: tuple[int, int]) -> tuple[int, int]:
+def move(token: TokenInfo, shift: tuple[int, int]) -> TokenInfo:
     new_start = (token.start[0] + shift[0], token.start[1] + shift[1])
     new_end = (token.end[0] + shift[0], token.end[1] + shift[1])
     return TokenInfo(token.type, token.string, new_start, new_end, token.line)
 
 
-def tagstr_token_stream_transform(
-    stream: Iterator[TokenInfo],
-) -> list[TokenInfo] | None:
-    token = next(stream)
-    if token.type != NAME:
-        return None
-    name = token
+def tagstr_token_stream_transform(stream: RewindableStream) -> list[TokenInfo] | None:
+    # find the last possible NAME token
+    name = None
+    for token in stream:
+        if token.type == NAME:
+            name = token
+        elif name and token.type != NL:
+            stream.rewind()
+            break
+        else:
+            return None
+    assert name is not None
 
     for token in stream:
         if token.type == OP and token.string == "@":
             break
         elif token.type in (NEWLINE, NL):
             pass
+        elif token.type == NAME:
+            stream.rewind()
+            return None
         else:
             return None
 
     depth = 0
     for token in stream:
         if token.type == STRING and token.string.startswith("f"):
             break
@@ -116,50 +119,54 @@
         name,
         move(TokenInfo(OP, "(", (0, 1), (0, 2), name.line), name.end),
         *args,
         move(TokenInfo(OP, ")", (0, 1), (0, 2), end.line), end.end),
     ]
 
 
-def transform_fstr_token(fstr_token: TokenInfo) -> list[TokenInfo]:
-    joined_str: ast.JoinedStr = ast.parse(fstr_token.string).body[0].value
-    joined_str_values: list[ast.Constant | ast.FormattedValue] = joined_str.values
+def transform_fstr_token(token: TokenInfo) -> list[TokenInfo]:
+    assert token.type == STRING and token.string.startswith("f"), f"{token} is not fstr"
+    body = cast(ast.Expr, ast.parse(token.string).body[0])
+    joined_str = cast(ast.JoinedStr, body.value)
+    joined_str_values = cast(
+        "list[ast.Constant | ast.FormattedValue]", joined_str.values
+    )
 
     token_type_and_string: list[tuple[int, str]] = []
     for v in joined_str_values:
         if isinstance(v, ast.Constant):
             token_type_and_string += [(STRING, repr(v.s))]
         elif isinstance(v, ast.FormattedValue):
             token_type_and_string += make_thunk_tokens_from_formatted_value(v)
         else:
             raise NotImplementedError(f"Unexpected type: {type(v)}")
         token_type_and_string.append((COMMA, ","))
 
     tokens = []
-    start = fstr_token.start
+    start = token.start
     for token_type, token_string in token_type_and_string:
         token = move(
             TokenInfo(
                 token_type,
                 token_string,
                 (0, 0),
                 (0, len(token_string)),
-                fstr_token.line,
+                token.line,
             ),
             start,
         )
         tokens.append(token)
         start = token.end
 
     return tokens
 
 
 def make_thunk_tokens_from_formatted_value(
     value: ast.FormattedValue,
-) -> list[TokenInfo]:
+) -> list[tuple[int, str]]:
     string_literal = ast.unparse(value.value)
     string_token = (STRING, repr(string_literal))
 
     getvalue_expr_tokens = list(generate_tokens(StringIO(string_literal).readline))[:-2]
     getvalue_tokens = (
         (NAME, "lambda"),
         (OP, ":"),
@@ -181,7 +188,34 @@
         string_token,
         (COMMA, ","),
         conv_token,
         (COMMA, ","),
         spec_token,
         (OP, ")"),
     ]
+
+
+class RewindableStream:
+    def __init__(self, stream: Iterator[TokenInfo]) -> None:
+        self._stream = stream
+        self._consumed: list[TokenInfo] = []
+        self._buffer: list[TokenInfo] = []
+
+    def __iter__(self) -> Iterator[TokenInfo]:
+        return self
+
+    def __next__(self) -> TokenInfo:
+        if self._buffer:
+            token = self._buffer.pop()
+        else:
+            token = next(self._stream)
+        self._consumed.append(token)
+        return token
+
+    def rewind(self) -> None:
+        self._buffer.append(self._consumed.pop())
+
+    def consumed(self, clear: bool = False) -> list[TokenInfo]:
+        consumed = self._consumed[:]
+        if clear:
+            self._consumed.clear()
+        return consumed
```

### Comparing `tagstr-0.0.1/tests/case_utils.py` & `tagstr-0.1.0/tests/case_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,35 +31,44 @@
             loc[target_1] = (
                 (node.value.lineno, node.value.col_offset),
                 (node.value.end_lineno, node.value.end_col_offset),
             )
 
         elif isinstance(node, ast.Assert):
             assert "actual" in loc and "expected" in loc, "Missing actual or expected"
+            assert isinstance(node.test, ast.Str)
+            message = node.test.s
+
             a_start, a_end = loc["actual"]
             a_start_line, a_start_col = a_start
             a_end_line, a_end_col = a_end
 
             a_lines = source_lines[a_start_line - 1 : a_end_line]
-            a_slice_end = len(a_lines[-1]) - a_end_col or None
+            a_slice_end = a_end_col - len(a_lines[-1]) or None
             actual_src = "\n".join(a_lines)[a_start_col:a_slice_end]
 
             e_start, e_end = loc["expected"]
             e_start_line, e_start_col = e_start
             e_end_line, e_end_col = e_end
 
             e_lines = source_lines[e_start_line - 1 : e_end_line]
-            e_slice_end = len(e_lines[-1]) - e_end_col or None
-            expected_src = "\n".join(e_lines)[e_start_col:e_slice_end]
+            e_slice_end = e_end_col - len(e_lines[-1]) or None
+
+            if e_lines[-1][-1] != "\\":
+                expected_src = "\n".join(e_lines)[e_start_col:e_slice_end]
+            else:
+                # handle case of line continuations
+                e_lines = source_lines[e_start_line - 1 : node.lineno - 1]
+                expected_src = "\n".join(e_lines)[e_start_col:].rstrip()
 
             cases.append(
                 {
                     "actual": actual_src,
                     "expected": expected_src,
-                    "message": node.msg.s,
+                    "message": message,
                 }
             )
             loc = {}
     return cases
 
 
 class _CaseLoc(TypedDict, total=False):
```

### Comparing `tagstr-0.0.1/.gitignore` & `tagstr-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tagstr-0.0.1/LICENSE` & `tagstr-0.1.0/LICENSE`

 * *Files identical despite different names*

