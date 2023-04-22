# Comparing `tmp/tagstr-0.1.0.tar.gz` & `tmp/tagstr-0.2.0.tar.gz`

## Comparing `tagstr-0.1.0.tar` & `tagstr-0.2.0.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tagstr-0.1.0/temp.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 tagstr-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1202fd3817ee8abe
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/12e653c2cc8b713b
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/16ce0992725e7c99
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1a3f3a94f182d98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1a9be57c5988a68e
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1b09e8d5534476ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1c013fcb5cc738da
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/1d75279975891254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/21a2d50da587646a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/21d71b3f3a93829e
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/2341cf1e5946409b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/245d3838a84d1f0d
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/266ac9dcb2a917d3
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/27811028d704c6dc
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/27c5b6fdeba5b7ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/28ba20d8130bc981
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/29b747fe319f3777
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/2fb7e82c318c343b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/30c0fd9ab36ae7bf
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/32b441a8aac0cf4d
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/33344ab4632fffe3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3385489d09b32bc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/36fdc51d203ffca2
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/38df0e9f6de8d029
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/39c329b1df4a32dc
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3b244ec237a19c48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3c61c1cdf4ba0e63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e13dc3fa7e13b8a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e62ffaafef90d4c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3e7426aee801e771
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/3fcc684d6dfed26e
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4197cbc369ca1e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/428d4324098031a9
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/42a93bc19bd61f5b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/43416d462caa1fcb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/43e86f39ac064e7f
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4cbb8f887305a1df
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4cfe6a27ce54d44
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/4d8867984beffb14
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/50d67579f5cab43f
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/52d2b1c7e14a2ec1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/55b948d7f4ae828b
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/5810920ecddb0d55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/5a66575126fa05ed
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/61f496d82ce99454
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6304bb1f9620b3ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/645eddb2cf3fddd
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6545ffff0952bf2d
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/664c859e0aae0a20
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/66712d58b28d9e32
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/675043ab6278d320
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6853ecaed51fc9cd
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6a2ba283404ca374
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6b02b2ba7a92df26
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6b0d9aea501453e7
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6c549a9787be1e33
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/6f8561c81fa54afb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/715b236edbd49e36
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/72b4201b626ff8eb
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7b1d68a8b1cbced5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7e310898b4d4b55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/7e81d7d55cc63f63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/804207c459a53f60
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/80d3ae37a5fa9e17
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8148ea1ef8f6d144
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/83907ccb56b539c7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/85e7e087c05a9362
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/85fea8713d811823
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/88dac8158c303086
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8aa6519d8d62ed53
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/8add245186a0b55e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9211b78fec2ce010
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9228807ce7870a24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/93003edc8ca546c6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/94ff10896f94f1e6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/96160b841e5b28b1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9764fd4dcd5b66d
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9b11259f9ce28217
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9ba39e9875d3697
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9d371d6b54954c2e
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/9ef909f97faedc23
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a1b6eeabe36ab1fb
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a472d58082639e5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a625cbbc8778b4d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a6c468410e5aedd9
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a845e6fdb39e199b
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a96cd35c46eb9c8a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/a98857b51534a9ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ae84286265f9ee63
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/aea3e8c4b5fc68df
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b10fa97d4b462364
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b33f91249c322634
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b6bc86e562ee72d
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b7695d0f2bcd40b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b865b8e6af8bd1e5
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/b9583e55d182ceee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/baaa7127908ac1fd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/bb8b64ef50f76867
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/bfbd92fb5d0b4a8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/c6a73143aa527759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/cf5249c8f3e3b1d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d04e2e28866d6219
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d1f94f80a7aa473e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d3866544a2d61dcf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d521ac457c4419d0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d7d962891d453308
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d8170825e811e0f9
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/d89feb8d30129dc4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/daa7b455394ab040
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dc2de1bca0ba0bc5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dcb3545fc211fb66
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dcf4672b52977830
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ddb845997320023d
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/dddf49b53830f171
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/df48c1b44d24756c
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e0751dbc4c0c1e10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e31eb0145ab1b3e8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/e7145fe6e2786e58
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ec29a3884ae9399b
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ed32a4005c3b40ed
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/ee12d3323a728899
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f1c6bcd7640579f1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f1ed93c6f6981943
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f241e50fbb067a72
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f29e6b327684303c
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f466ece879291fd1
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5537e6fc46b6c71
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5b4c0f80798dd5
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f5eeb30888472a10
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f80a89ebefeebbd2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/f8f0ff85963c19cd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/faec6021ef8ffc2a
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tagstr-0.1.0/.ruff_cache/content/fbd3d3dd5e077779
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr.pth
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/decorator.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/importer.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/tokenizer.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/transform.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/types.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 tagstr-0.1.0/tagstr/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/case_utils.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/test_transform.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 tagstr-0.1.0/tests/cases/transform.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tagstr-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tagstr-0.1.0/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tagstr-0.1.0/README.md
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 tagstr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tagstr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 tagstr-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1202fd3817ee8abe
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/12e653c2cc8b713b
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/16ce0992725e7c99
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1a3f3a94f182d98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1a9be57c5988a68e
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1b09e8d5534476ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1c013fcb5cc738da
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/1d75279975891254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/21a2d50da587646a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/21d71b3f3a93829e
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/2341cf1e5946409b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/245d3838a84d1f0d
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/266ac9dcb2a917d3
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/27811028d704c6dc
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/27c5b6fdeba5b7ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/28ba20d8130bc981
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/29b747fe319f3777
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/2fb7e82c318c343b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/30c0fd9ab36ae7bf
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/32b441a8aac0cf4d
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/33344ab4632fffe3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3385489d09b32bc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/36fdc51d203ffca2
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/38df0e9f6de8d029
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/39c329b1df4a32dc
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3b244ec237a19c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3c61c1cdf4ba0e63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3e13dc3fa7e13b8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3e62ffaafef90d4c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3e7426aee801e771
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/3fcc684d6dfed26e
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/4197cbc369ca1e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/428d4324098031a9
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/42a93bc19bd61f5b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/43416d462caa1fcb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/43e86f39ac064e7f
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/4cbb8f887305a1df
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/4cfe6a27ce54d44
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/4d8867984beffb14
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/50d67579f5cab43f
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/52d2b1c7e14a2ec1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/55b948d7f4ae828b
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/5810920ecddb0d55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/5a66575126fa05ed
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/61f496d82ce99454
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6304bb1f9620b3ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/645eddb2cf3fddd
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6545ffff0952bf2d
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/664c859e0aae0a20
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/66712d58b28d9e32
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/675043ab6278d320
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6853ecaed51fc9cd
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6a2ba283404ca374
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6b02b2ba7a92df26
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6b0d9aea501453e7
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6c549a9787be1e33
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/6f8561c81fa54afb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/715b236edbd49e36
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/72b4201b626ff8eb
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/7b1d68a8b1cbced5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/7e310898b4d4b55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/7e81d7d55cc63f63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/804207c459a53f60
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/80d3ae37a5fa9e17
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/8148ea1ef8f6d144
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/83907ccb56b539c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/85e7e087c05a9362
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/85fea8713d811823
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/88dac8158c303086
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/8aa6519d8d62ed53
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/8add245186a0b55e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9211b78fec2ce010
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9228807ce7870a24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/93003edc8ca546c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/94ff10896f94f1e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/96160b841e5b28b1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9764fd4dcd5b66d
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9b11259f9ce28217
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9ba39e9875d3697
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9d371d6b54954c2e
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/9ef909f97faedc23
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a1b6eeabe36ab1fb
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a472d58082639e5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a625cbbc8778b4d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a6c468410e5aedd9
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a845e6fdb39e199b
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a96cd35c46eb9c8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/a98857b51534a9ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/ae84286265f9ee63
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/aea3e8c4b5fc68df
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b10fa97d4b462364
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b33f91249c322634
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b6bc86e562ee72d
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b7695d0f2bcd40b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b865b8e6af8bd1e5
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/b9583e55d182ceee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/baaa7127908ac1fd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/bb8b64ef50f76867
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/bfbd92fb5d0b4a8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/c6a73143aa527759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/cf5249c8f3e3b1d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d04e2e28866d6219
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d1f94f80a7aa473e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d3866544a2d61dcf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d521ac457c4419d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d7d962891d453308
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d8170825e811e0f9
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/d89feb8d30129dc4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/daa7b455394ab040
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/dc2de1bca0ba0bc5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/dcb3545fc211fb66
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/dcf4672b52977830
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/ddb845997320023d
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/dddf49b53830f171
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/df48c1b44d24756c
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/e0751dbc4c0c1e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/e31eb0145ab1b3e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/e7145fe6e2786e58
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/ec29a3884ae9399b
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/ed32a4005c3b40ed
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/ee12d3323a728899
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f1c6bcd7640579f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f1ed93c6f6981943
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f241e50fbb067a72
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f29e6b327684303c
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f466ece879291fd1
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f5537e6fc46b6c71
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f5b4c0f80798dd5
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f5eeb30888472a10
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f80a89ebefeebbd2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/f8f0ff85963c19cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/faec6021ef8ffc2a
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tagstr-0.2.0/.ruff_cache/content/fbd3d3dd5e077779
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr.pth
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/decorator.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/importer.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/tokenizer.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/transform.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/types.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 tagstr-0.2.0/tagstr/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tagstr-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tagstr-0.2.0/tests/case_utils.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 tagstr-0.2.0/tests/test_transform.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 tagstr-0.2.0/tests/cases/transform.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tagstr-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tagstr-0.2.0/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tagstr-0.2.0/README.md
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 tagstr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tagstr-0.2.0/PKG-INFO
```

### Comparing `tagstr-0.1.0/.github/workflows/test.yml` & `tagstr-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/12e653c2cc8b713b` & `tagstr-0.2.0/.ruff_cache/content/12e653c2cc8b713b`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/266ac9dcb2a917d3` & `tagstr-0.2.0/.ruff_cache/content/266ac9dcb2a917d3`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/3b244ec237a19c48` & `tagstr-0.2.0/.ruff_cache/content/3b244ec237a19c48`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/4197cbc369ca1e1d` & `tagstr-0.2.0/.ruff_cache/content/4197cbc369ca1e1d`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/4cbb8f887305a1df` & `tagstr-0.2.0/.ruff_cache/content/4cbb8f887305a1df`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/4cfe6a27ce54d44` & `tagstr-0.2.0/.ruff_cache/content/4cfe6a27ce54d44`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/52d2b1c7e14a2ec1` & `tagstr-0.2.0/.ruff_cache/content/52d2b1c7e14a2ec1`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/5810920ecddb0d55` & `tagstr-0.2.0/.ruff_cache/content/5810920ecddb0d55`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/6853ecaed51fc9cd` & `tagstr-0.2.0/.ruff_cache/content/6853ecaed51fc9cd`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/6b0d9aea501453e7` & `tagstr-0.2.0/.ruff_cache/content/6b0d9aea501453e7`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/8148ea1ef8f6d144` & `tagstr-0.2.0/.ruff_cache/content/8148ea1ef8f6d144`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/9b11259f9ce28217` & `tagstr-0.2.0/.ruff_cache/content/9b11259f9ce28217`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/a845e6fdb39e199b` & `tagstr-0.2.0/.ruff_cache/content/a845e6fdb39e199b`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/a96cd35c46eb9c8a` & `tagstr-0.2.0/.ruff_cache/content/a96cd35c46eb9c8a`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/b10fa97d4b462364` & `tagstr-0.2.0/.ruff_cache/content/b10fa97d4b462364`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/b9583e55d182ceee` & `tagstr-0.2.0/.ruff_cache/content/b9583e55d182ceee`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/d1f94f80a7aa473e` & `tagstr-0.2.0/.ruff_cache/content/d1f94f80a7aa473e`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/d89feb8d30129dc4` & `tagstr-0.2.0/.ruff_cache/content/d89feb8d30129dc4`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/dddf49b53830f171` & `tagstr-0.2.0/.ruff_cache/content/dddf49b53830f171`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/e0751dbc4c0c1e10` & `tagstr-0.2.0/.ruff_cache/content/e0751dbc4c0c1e10`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/f5537e6fc46b6c71` & `tagstr-0.2.0/.ruff_cache/content/f5537e6fc46b6c71`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/f5eeb30888472a10` & `tagstr-0.2.0/.ruff_cache/content/f5eeb30888472a10`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.ruff_cache/content/fbd3d3dd5e077779` & `tagstr-0.2.0/.ruff_cache/content/fbd3d3dd5e077779`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tagstr/decorator.py` & `tagstr-0.2.0/tagstr/decorator.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tagstr/importer.py` & `tagstr-0.2.0/tagstr/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
-import os.path as os_path
+import re
 import sys
 from importlib.abc import MetaPathFinder, PathEntryFinder
 from importlib.machinery import FileFinder, ModuleSpec, PathFinder, SourceFileLoader
+from os import path as os_path
 from token import COMMENT, NAME, NL, STRING
 from tokenize import TokenInfo, detect_encoding, generate_tokens
 from types import CodeType, ModuleType
 from typing import Iterator, Sequence, TextIO
 
 from tagstr.transform import transform_stream
 
 
 class TagStrPathHook(PathEntryFinder):
     def __init__(self, path: str) -> None:
-        if not os_path.isfile(path):
-            raise ImportError("Only files are supported")
+        if not os_path.isfile(path) or os_path.splitext(path)[1] != ".py":
+            raise ImportError("Only .py files are supported")
         self.entry_file = path
         self.file_finder = FileFinder(
             os_path.dirname(path), (TagStrSourceFileLoader, [".py"])
         )
         sys.meta_path.insert(0, TagStrMetaFinder(path))
 
     def invalidate_caches(self) -> None:
@@ -41,14 +42,16 @@
         fullname: str,
         path: Sequence[str] | None,
         target: ModuleType | None = None,
     ) -> ModuleSpec | None:
         if fullname == "__main__":
             loader = TagStrSourceFileLoader(fullname, self.entry_file)
             return ModuleSpec(fullname, loader, is_package=False)
+        elif path is None:
+            return None
 
         for finder in sys.meta_path:
             if finder is not self:
                 spec = finder.find_spec(fullname, path, target)
                 if spec is not None:
                     break
         else:
@@ -78,16 +81,21 @@
 
     with open(file, "r", encoding="utf-8") as f:
         return should_transform(f)
 
 
 def should_transform(stream: TextIO) -> bool:
     for line in iter_token_lines(stream):
-        if not line:
-            continue
+        # check if line is a comment with `# tagstr: on`
+        if len(line) == 1 and line[0].type == COMMENT:
+            match = TAGSTR_COMMENT_PATTERN.match(line[0].string)
+            if match:
+                comment_value = match.group("value")
+                if comment_value.lower() == "on":
+                    return True
 
         # check if line is an `import tagstr` statement
         if (
             len(line) >= 2
             and line[0].type == NAME
             and line[0].string == "import"
             and line[1].type == NAME
@@ -104,14 +112,18 @@
     return False
 
 
 def iter_token_lines(stream: TextIO) -> Iterator[list[TokenInfo]]:
     line: list[TokenInfo] = []
     for token in generate_tokens(stream.readline):
         if token.type == NL:
-            yield line
-            line = []
+            if line:  # only yield non-empty lines
+                yield line
+                line = []
         else:
             line.append(token)
 
 
+TAGSTR_COMMENT_PATTERN = re.compile(r"\s*#\s+tagstr\s*:\s*(?P<value>[\w-]+).*$")
+
+
 sys.path_hooks.insert(0, TagStrPathHook)
```

### Comparing `tagstr-0.1.0/tagstr/tokenizer.py` & `tagstr-0.2.0/tagstr/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tagstr/types.py` & `tagstr-0.2.0/tagstr/types.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tagstr/utils.py` & `tagstr-0.2.0/tagstr/utils.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tests/case_utils.py` & `tagstr-0.2.0/tests/case_utils.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/tests/cases/transform.py` & `tagstr-0.2.0/tests/cases/transform.py`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/.gitignore` & `tagstr-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/LICENSE` & `tagstr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tagstr-0.1.0/pyproject.toml` & `tagstr-0.2.0/pyproject.toml`

 * *Files identical despite different names*

