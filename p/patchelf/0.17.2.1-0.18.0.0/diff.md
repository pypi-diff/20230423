# Comparing `tmp/patchelf-0.17.2.1.tar.gz` & `tmp/patchelf-0.18.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchelf-0.17.2.1.tar", last modified: Sun Feb 26 15:37:49 2023, max compression
+gzip compressed data, was "patchelf-0.18.0.0.tar", last modified: Sun Apr 23 14:40:33 2023, max compression
```

## Comparing `patchelf-0.17.2.1.tar` & `patchelf-0.18.0.0.tar`

### file list

```diff
@@ -1,131 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.802638 patchelf-0.17.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.802638 patchelf-0.17.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     4877 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.798638 patchelf-0.17.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.806638 patchelf-0.17.2.1/src/patchelf-upstream/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/BUGS
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)       68 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/bors.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/configure.ac
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/default.nix
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/flake.lock
--rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/flake.nix
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.806638 patchelf-0.17.2.1/src/patchelf-upstream/m4/
--rw-r--r--   0 runner    (1001) docker     (122)    21126 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/m4/ax_cxx_compile_stdcxx.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4466 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/patchelf.1
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/patchelf.nix
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/patchelf.spec.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.806638 patchelf-0.17.2.1/src/patchelf-upstream/src/
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/src/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (122)   187901 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/src/elf.h
--rw-r--r--   0 runner    (1001) docker     (122)    79523 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/src/patchelf.cc
--rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/src/patchelf.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.818638 patchelf-0.17.2.1/src/patchelf-upstream/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4629 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/Makefile.am
--rwxr-xr-x   0 runner    (1001) docker     (122)      729 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/add-debug-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      604 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/add-rpath.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      538 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/args-from-file.sh
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/bar.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      154 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/basic-flags.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      686 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/big-dynstr.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1428 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/build-id.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      930 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/change-abi.sh
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/contiguous-note-sections.ld
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/contiguous-note-sections.s
--rwxr-xr-x   0 runner    (1001) docker     (122)      392 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/contiguous-note-sections.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      984 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/empty-note
--rwxr-xr-x   0 runner    (1001) docker     (122)      386 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/empty-note.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.818638 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.818638 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64/
--rwxr-xr-x   0 runner    (1001) docker     (122)    66736 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64/libtest.so
--rwxr-xr-x   0 runner    (1001) docker     (122)    66920 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64/main
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.818638 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64le/
--rwxr-xr-x   0 runner    (1001) docker     (122)    66736 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64le/libtest.so
--rwxr-xr-x   0 runner    (1001) docker     (122)    66920 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64le/main
--rwxr-xr-x   0 runner    (1001) docker     (122)      750 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness.sh
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/foo.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      745 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/force-rpath.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      364 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/grow-file.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.822638 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/
--rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-phdr-offset
--rw-r--r--   0 runner    (1001) docker     (122)   111801 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shdr-name
--rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-idx
--rw-r--r--   0 runner    (1001) docker     (122)   111289 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-nonterm
--rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-size
--rw-r--r--   0 runner    (1001) docker     (122)   111680 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-zero
--rwxr-xr-x   0 runner    (1001) docker     (122)     1031 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf.sh
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/main.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      120 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-dynamic-section.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      349 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-gnu-hash.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1645 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-pie-powerpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/
--rwxr-xr-x   0 runner    (1001) docker     (122)     9514 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-amd64
--rwxr-xr-x   0 runner    (1001) docker     (122)     7516 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armel
--rwxr-xr-x   0 runner    (1001) docker     (122)     7451 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armhf
--rwxr-xr-x   0 runner    (1001) docker     (122)     7508 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-hurd-i386
--rwxr-xr-x   0 runner    (1001) docker     (122)     7328 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-i386
--rwxr-xr-x   0 runner    (1001) docker     (122)    10745 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-ia64
--rwxr-xr-x   0 runner    (1001) docker     (122)     9526 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-amd64
--rwxr-xr-x   0 runner    (1001) docker     (122)     7296 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-i386
--rwxr-xr-x   0 runner    (1001) docker     (122)     8198 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mips
--rwxr-xr-x   0 runner    (1001) docker     (122)     8202 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mipsel
--rwxr-xr-x   0 runner    (1001) docker     (122)    68704 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-pie-powerpc
--rwxr-xr-x   0 runner    (1001) docker     (122)     7746 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-powerpc
--rwxr-xr-x   0 runner    (1001) docker     (122)     7308 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-s390
--rwxr-xr-x   0 runner    (1001) docker     (122)     7223 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sh4
--rwxr-xr-x   0 runner    (1001) docker     (122)     7197 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sparc
--rwxr-xr-x   0 runner    (1001) docker     (122)     1018 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild.sh
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      558 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1048 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/output-flag.sh
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/phdr-corruption.ld
--rwxr-xr-x   0 runner    (1001) docker     (122)      587 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/phdr-corruption.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)       41 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/plain-fail.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      646 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/plain-needed.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      120 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/plain-run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1002 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/replace-add-needed.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      816 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/replace-needed.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      200 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-empty-rpath.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      903 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-interpreter-long.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      416 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-interpreter-short.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1589 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-rpath-library.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      966 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-rpath-rel-map.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      664 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/set-rpath.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1358 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/shrink-rpath-with-allowed-prefixes.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      685 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/shrink-rpath.sh
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/simple.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      987 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/soname.sh
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/too-many-strtab.c
--rwxr-xr-x   0 runner    (1001) docker     (122)      567 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/too-many-strtab.sh
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/too-many-strtab2.s
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/tests/void.c
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-26 15:37:35.000000 patchelf-0.17.2.1/src/patchelf-upstream/version
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/src/patchelf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-02-26 15:37:49.000000 patchelf-0.17.2.1/src/patchelf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-02-26 15:37:49.000000 patchelf-0.17.2.1/src/patchelf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-26 15:37:49.000000 patchelf-0.17.2.1/src/patchelf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-02-26 15:37:49.000000 patchelf-0.17.2.1/src/patchelf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-26 15:37:49.000000 patchelf-0.17.2.1/src/patchelf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-26 15:37:49.826638 patchelf-0.17.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-02-26 15:37:34.000000 patchelf-0.17.2.1/tests/test_patchelf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.375194 patchelf-0.18.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.355193 patchelf-0.18.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.355193 patchelf-0.18.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     4877 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3395 2023-04-23 14:40:33.375194 patchelf-0.18.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-23 14:40:33.375194 patchelf-0.18.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.355193 patchelf-0.18.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.359194 patchelf-0.18.0.0/src/patchelf-upstream/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/BUGS
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)       68 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/bors.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.355193 patchelf-0.18.0.0/src/patchelf-upstream/completions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.359194 patchelf-0.18.0.0/src/patchelf-upstream/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/completions/zsh/_patchelf
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/default.nix
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/flake.nix
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.359194 patchelf-0.18.0.0/src/patchelf-upstream/m4/
+-rw-r--r--   0 runner    (1001) docker     (122)    21126 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/m4/ax_cxx_compile_stdcxx.m4
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/patchelf.1
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/patchelf.nix
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/patchelf.spec.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.359194 patchelf-0.18.0.0/src/patchelf-upstream/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/src/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (122)   187901 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/src/elf.h
+-rw-r--r--   0 runner    (1001) docker     (122)    97983 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/src/patchelf.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9236 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/src/patchelf.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.367194 patchelf-0.18.0.0/src/patchelf-upstream/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6061 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/Makefile.am
+-rwxr-xr-x   0 runner    (1001) docker     (122)      743 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/add-debug-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      652 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/add-rpath.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      571 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/args-from-file.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/bar.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)      154 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/basic-flags.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      732 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/big-dynstr.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1441 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/build-id.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      829 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/change-abi.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/contiguous-note-sections.ld
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/contiguous-note-sections.s
+-rwxr-xr-x   0 runner    (1001) docker     (122)      396 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/contiguous-note-sections.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      984 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/empty-note
+-rwxr-xr-x   0 runner    (1001) docker     (122)      402 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/empty-note.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.367194 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.367194 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    66736 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64/libtest.so
+-rwxr-xr-x   0 runner    (1001) docker     (122)    66920 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64/main
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.367194 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64le/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    66736 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64le/libtest.so
+-rwxr-xr-x   0 runner    (1001) docker     (122)    66920 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64le/main
+-rwxr-xr-x   0 runner    (1001) docker     (122)      775 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/foo.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)      824 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/force-rpath.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      380 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/grow-file.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.371194 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/
+-rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-phdr-offset
+-rw-r--r--   0 runner    (1001) docker     (122)   111801 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shdr-name
+-rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-idx
+-rw-r--r--   0 runner    (1001) docker     (122)   111289 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-nonterm
+-rw-r--r--   0 runner    (1001) docker     (122)    80176 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-size
+-rw-r--r--   0 runner    (1001) docker     (122)   111680 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-zero
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1037 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/main.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5538 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/modify-execstack.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      120 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-dynamic-section.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      361 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-gnu-hash.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1650 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-pie-powerpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.371194 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9514 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-amd64
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7516 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armel
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7451 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armhf
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7508 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-hurd-i386
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7328 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-i386
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10745 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-ia64
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9526 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-amd64
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7296 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-i386
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8198 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mips
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8202 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mipsel
+-rwxr-xr-x   0 runner    (1001) docker     (122)    68704 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-pie-powerpc
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7746 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-powerpc
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7308 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-s390
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7223 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sh4
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7197 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sparc
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1050 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)      574 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1104 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/output-flag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)   227896 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/overlapping-segments-after-rounding
+-rwxr-xr-x   0 runner    (1001) docker     (122)      593 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/overlapping-segments-after-rounding.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/phdr-corruption.ld
+-rwxr-xr-x   0 runner    (1001) docker     (122)      586 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/phdr-corruption.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)       41 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/plain-fail.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      654 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/plain-needed.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      120 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/plain-run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      546 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/print-execstack.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3725 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/rename-dynamic-symbols.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1261 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/repeated-updates.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1025 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/replace-add-needed.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      761 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/replace-needed.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      212 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-empty-rpath.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      921 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-interpreter-long.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      428 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-interpreter-short.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1995 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath-library.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1015 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath-rel-map.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      710 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/shared-rpath.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1977 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/shared-rpath.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)   170253 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/short-first-segment.gz
+-rwxr-xr-x   0 runner    (1001) docker     (122)      716 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/short-first-segment.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1422 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/shrink-rpath-with-allowed-prefixes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      701 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/shrink-rpath.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/simple.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1005 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/soname.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/too-many-strtab.c
+-rwxr-xr-x   0 runner    (1001) docker     (122)      581 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/too-many-strtab.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/too-many-strtab2.s
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/tests/void.c
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/src/patchelf-upstream/version
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.371194 patchelf-0.18.0.0/src/patchelf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3395 2023-04-23 14:40:33.000000 patchelf-0.18.0.0/src/patchelf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-23 14:40:33.000000 patchelf-0.18.0.0/src/patchelf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 14:40:33.000000 patchelf-0.18.0.0/src/patchelf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-23 14:40:33.000000 patchelf-0.18.0.0/src/patchelf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-23 14:40:33.000000 patchelf-0.18.0.0/src/patchelf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 14:40:33.371194 patchelf-0.18.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-23 14:40:23.000000 patchelf-0.18.0.0/tests/test_patchelf.py
```

### Comparing `patchelf-0.17.2.1/.github/workflows/build.yml` & `patchelf-0.18.0.0/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,30 @@
           submodules: 'recursive'
 
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v2.1.0
         if: matrix.arch != 'x86_64'
 
       - name: Set up Docker Buildx
-        uses: docker/setup-buildx-action@v2.4.1
+        uses: docker/setup-buildx-action@v2.5.0
 
       - name: Build patchelf_build_${{ matrix.arch }} image
         uses: docker/build-push-action@v4.0.0
         with:
           context: .
           load: true
           push: false
           tags: patchelf_build_${{ matrix.arch == 'armv7l' && 'aarch64' || matrix.arch }}:latest
           build-args: |
             ARCH=${{ matrix.docker_arch }}
           cache-from: type=gha
           cache-to: type=gha,mode=max
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.0
+        uses: pypa/cibuildwheel@v2.12.3
         env:
           CIBW_ARCHS: "${{ matrix.arch == 'armv7l' && 'aarch64' || matrix.arch }}"
 
       - name: Test wheel on ${{ matrix.test_image }}
         run: |
           cat <<EOF > check.sh
           set -e
@@ -168,11 +168,11 @@
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - name: Upload to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_RELEASE_PASSWORD }}
```

### Comparing `patchelf-0.17.2.1/.gitignore` & `patchelf-0.18.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/.pre-commit-config.yaml` & `patchelf-0.18.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/CMakeLists.txt` & `patchelf-0.18.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/COPYING` & `patchelf-0.18.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/LICENSE` & `patchelf-0.18.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/PKG-INFO` & `patchelf-0.18.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchelf
-Version: 0.17.2.1
+Version: 0.18.0.0
 Summary: A small utility to modify the dynamic linker and RPATH of ELF executables.
 Home-page: https://github.com/NixOS/patchelf
 Maintainer: Matthieu Darbois
 Maintainer-email: mayeut@users.noreply.github.com
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://github.com/mayeut/patchelf-pypi
 Project-URL: Bug Tracker, https://github.com/mayeut/patchelf-pypi/issues
@@ -67,14 +67,17 @@
   +---------------+--------------------------+
   | Linux i686    | | manylinux1+            |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux aarch64 | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
+  | Linux armv7l  | | manylinux2014+         |
+  |               | | musllinux_1_1+         |
+  +---------------+--------------------------+
   | Linux ppc64le | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux s390x   | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
```

### Comparing `patchelf-0.17.2.1/README.rst` & `patchelf-0.18.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
   +---------------+--------------------------+
   | Linux i686    | | manylinux1+            |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux aarch64 | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
+  | Linux armv7l  | | manylinux2014+         |
+  |               | | musllinux_1_1+         |
+  +---------------+--------------------------+
   | Linux ppc64le | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux s390x   | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
```

### Comparing `patchelf-0.17.2.1/noxfile.py` & `patchelf-0.18.0.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/pyproject.toml` & `patchelf-0.18.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/setup.py` & `patchelf-0.18.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/COPYING` & `patchelf-0.18.0.0/src/patchelf-upstream/COPYING`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/README.md` & `patchelf-0.18.0.0/src/patchelf-upstream/README.md`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/bors.toml` & `patchelf-0.18.0.0/src/patchelf-upstream/bors.toml`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/configure.ac` & `patchelf-0.18.0.0/src/patchelf-upstream/configure.ac`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/flake.lock` & `patchelf-0.18.0.0/src/patchelf-upstream/flake.lock`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/flake.nix` & `patchelf-0.18.0.0/src/patchelf-upstream/flake.nix`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/m4/ax_cxx_compile_stdcxx.m4` & `patchelf-0.18.0.0/src/patchelf-upstream/m4/ax_cxx_compile_stdcxx.m4`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/patchelf.1` & `patchelf-0.18.0.0/src/patchelf-upstream/patchelf.1`

 * *Files 12% similar despite different names*

```diff
@@ -110,14 +110,31 @@
 .IP "--add-debug-tag"
 Adds DT_DEBUG tag to the .dynamic section if not yet present in an ELF
 object. A shared library (-shared) by default does not receive DT_DEBUG tag.
 This means that when a shared library has an entry point (so that it
 can be run as an executable), the debugger does not connect to it correctly and
 symbols are not resolved.
 
+.IP "--print-execstack"
+Prints the state of the executable flag of the GNU_STACK program header, if present.
+
+.IP "--clear-execstack"
+Clears the executable flag of the GNU_STACK program header, or adds a new header.
+
+.IP "--set-execstack"
+Sets the executable flag of the GNU_STACK program header, or adds a new header.
+
+.IP "--rename-dynamic-symbols NAME_MAP_FILE"
+Renames dynamic symbols. The name map file should contain lines
+with the old and the new name separated by spaces like this:
+
+old_name new_name
+
+Symbol names do not contain version specifier that are also shown in the output of the nm -D command from binutils. So instead of the name write@GLIBC_2.2.5 it is just write.
+
 .IP "--output FILE"
 Set the output file name.  If not specified, the input will be modified in place.
 
 .IP --debug
 Prints details of the changes made to the input file.
 
 .IP --version
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/patchelf.nix` & `patchelf-0.18.0.0/src/patchelf-upstream/patchelf.nix`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/patchelf.spec.in` & `patchelf-0.18.0.0/src/patchelf-upstream/patchelf.spec.in`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/src/elf.h` & `patchelf-0.18.0.0/src/patchelf-upstream/src/elf.h`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/src/patchelf.cc` & `patchelf-0.18.0.0/src/patchelf-upstream/src/patchelf.cc`

 * *Files 13% similar despite different names*

```diff
@@ -13,24 +13,27 @@
  *  General Public License for more details.
  *
  *  You should have received a copy of the GNU General Public License
  *  along with this program. If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include <algorithm>
+#include <fstream>
 #include <limits>
 #include <map>
 #include <memory>
+#include <optional>
 #include <set>
 #include <sstream>
 #include <stdexcept>
 #include <string>
+#include <string_view>
 #include <unordered_map>
+#include <unordered_set>
 #include <vector>
-#include <optional>
 
 #include <cassert>
 #include <cerrno>
 #include <cstdarg>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
@@ -65,22 +68,26 @@
 static int forcedPageSize = -1;
 #endif
 
 #ifndef EM_LOONGARCH
 #define EM_LOONGARCH    258
 #endif
 
-
-static std::vector<std::string> splitColonDelimitedString(const char * s)
+[[nodiscard]] static std::vector<std::string> splitColonDelimitedString(std::string_view s)
 {
-    std::string item;
     std::vector<std::string> parts;
-    std::stringstream ss(s);
-    while (std::getline(ss, item, ':'))
-        parts.push_back(item);
+
+    size_t pos;
+    while ((pos = s.find(':')) != std::string_view::npos) {
+        parts.emplace_back(s.substr(0, pos));
+        s = s.substr(pos + 1);
+    }
+
+    if (!s.empty())
+        parts.emplace_back(s);
 
     return parts;
 }
 
 static bool hasAllowedPrefix(const std::string & s, const std::vector<std::string> & allowedPrefixes)
 {
     return std::any_of(allowedPrefixes.begin(), allowedPrefixes.end(), [&](const std::string & i) { return !s.compare(0, i.size(), i); });
@@ -100,15 +107,15 @@
     return s;
 }
 
 /* !!! G++ creates broken code if this function is inlined, don't know
    why... */
 template<ElfFileParams>
 template<class I>
-I ElfFile<ElfFileParamNames>::rdi(I i) const
+constexpr I ElfFile<ElfFileParamNames>::rdi(I i) const noexcept
 {
     I r = 0;
     if (littleEndian) {
         for (unsigned int n = 0; n < sizeof(I); ++n) {
             r |= ((I) *(((unsigned char *) &i) + n)) << (n * 8);
         }
     } else {
@@ -127,15 +134,15 @@
         va_start(ap, format);
         vfprintf(stderr, format, ap);
         va_end(ap);
     }
 }
 
 
-void fmt2(std::ostringstream & out)
+static void fmt2([[maybe_unused]] std::ostringstream & out)
 {
 }
 
 
 template<typename T, typename... Args>
 void fmt2(std::ostringstream & out, T x, Args... args)
 {
@@ -158,15 +165,15 @@
     int errNo;
     explicit SysError(const std::string & msg)
         : std::runtime_error(fmt(msg + ": " + strerror(errno)))
         , errNo(errno)
     { }
 };
 
-__attribute__((noreturn)) static void error(const std::string & msg)
+[[noreturn]] static void error(const std::string & msg)
 {
     if (errno)
         throw SysError(msg);
     throw std::runtime_error(msg);
 }
 
 static FileContents readFile(const std::string & fileName,
@@ -187,34 +194,34 @@
     if (fd == -1) throw SysError(fmt("opening '", fileName, "'"));
 
     size_t bytesRead = 0;
     ssize_t portion;
     while ((portion = read(fd, contents->data() + bytesRead, size - bytesRead)) > 0)
         bytesRead += portion;
 
+    close(fd);
+
     if (bytesRead != size)
         throw SysError(fmt("reading '", fileName, "'"));
 
-    close(fd);
-
     return contents;
 }
 
 
 struct ElfType
 {
     bool is32Bit;
     int machine; // one of EM_*
 };
 
 
-ElfType getElfType(const FileContents & fileContents)
+[[nodiscard]] static ElfType getElfType(const FileContents & fileContents)
 {
     /* Check the ELF header for basic validity. */
-    if (fileContents->size() < static_cast<off_t>(sizeof(Elf32_Ehdr)))
+    if (fileContents->size() < sizeof(Elf32_Ehdr))
         error("missing ELF header");
 
     auto contents = fileContents->data();
 
     if (memcmp(contents, ELFMAG, SELFMAG) != 0)
         error("not an ELF executable");
 
@@ -227,22 +234,40 @@
     bool is32Bit = contents[EI_CLASS] == ELFCLASS32;
 
     // FIXME: endianness
     return ElfType { is32Bit, is32Bit ? (reinterpret_cast<Elf32_Ehdr *>(contents))->e_machine : (reinterpret_cast<Elf64_Ehdr *>(contents))->e_machine };
 }
 
 
-static void checkPointer(const FileContents & contents, void * p, unsigned int size)
+static void checkPointer(const FileContents & contents, const void * p, size_t size)
 {
-    auto q = static_cast<unsigned char *>(p);
-    if (!(q >= contents->data() && q + size <= contents->data() + contents->size()))
+    if (p < contents->data() || size > contents->size() || p > contents->data() + contents->size() - size)
         error("data region extends past file end");
 }
 
 
+static void checkOffset(const FileContents & contents, size_t offset, size_t size)
+{
+    size_t end;
+
+    if (offset > contents->size()
+        || size > contents->size()
+        || __builtin_add_overflow(offset, size, &end)
+        || end > contents->size())
+        error("data offset extends past file end");
+}
+
+
+static std::string extractString(const FileContents & contents, size_t offset, size_t size)
+{
+    checkOffset(contents, offset, size);
+    return { reinterpret_cast<const char *>(contents->data()) + offset, size };
+}
+
+
 template<ElfFileParams>
 ElfFile<ElfFileParamNames>::ElfFile(FileContents fContents)
     : fileContents(fContents)
 {
     /* Check the ELF header for basic validity. */
     if (fileContents->size() < (off_t) sizeof(Elf_Ehdr)) error("missing ELF header");
 
@@ -251,22 +276,42 @@
         error("not an ELF executable");
 
     littleEndian = hdr()->e_ident[EI_DATA] == ELFDATA2LSB;
 
     if (rdi(hdr()->e_type) != ET_EXEC && rdi(hdr()->e_type) != ET_DYN)
         error("wrong ELF type");
 
-    if (rdi(hdr()->e_phoff) + rdi(hdr()->e_phnum) * rdi(hdr()->e_phentsize) > fileContents->size())
-        error("program header table out of bounds");
+    {
+        auto ph_offset = rdi(hdr()->e_phoff);
+        auto ph_num = rdi(hdr()->e_phnum);
+        auto ph_entsize = rdi(hdr()->e_phentsize);
+        size_t ph_size, ph_end;
+
+        if (__builtin_mul_overflow(ph_num, ph_entsize, &ph_size)
+            || __builtin_add_overflow(ph_offset, ph_size, &ph_end)
+            || ph_end > fileContents->size()) {
+            error("program header table out of bounds");
+        }
+    }
 
     if (rdi(hdr()->e_shnum) == 0)
         error("no section headers. The input file is probably a statically linked, self-decompressing binary");
 
-    if (rdi(hdr()->e_shoff) + rdi(hdr()->e_shnum) * rdi(hdr()->e_shentsize) > fileContents->size())
-        error("section header table out of bounds");
+    {
+        auto sh_offset = rdi(hdr()->e_shoff);
+        auto sh_num = rdi(hdr()->e_shnum);
+        auto sh_entsize = rdi(hdr()->e_shentsize);
+        size_t sh_size, sh_end;
+
+        if (__builtin_mul_overflow(sh_num, sh_entsize, &sh_size)
+            || __builtin_add_overflow(sh_offset, sh_size, &sh_end)
+            || sh_end > fileContents->size()) {
+            error("section header table out of bounds");
+        }
+    }
 
     if (rdi(hdr()->e_phentsize) != sizeof(Elf_Phdr))
         error("program headers have wrong size");
 
     /* Copy the program and section headers. */
     for (int i = 0; i < rdi(hdr()->e_phnum); ++i) {
         Elf_Phdr *phdr = (Elf_Phdr *) (fileContents->data() + rdi(hdr()->e_phoff)) + i;
@@ -282,20 +327,23 @@
         checkPointer(fileContents, shdr, sizeof(*shdr));
         shdrs.push_back(*shdr);
     }
 
     /* Get the section header string table section (".shstrtab").  Its
        index in the section header table is given by e_shstrndx field
        of the ELF header. */
-    unsigned int shstrtabIndex = rdi(hdr()->e_shstrndx);
+    auto shstrtabIndex = rdi(hdr()->e_shstrndx);
     if (shstrtabIndex >= shdrs.size())
         error("string table index out of bounds");
 
-    unsigned int shstrtabSize = rdi(shdrs[shstrtabIndex].sh_size);
-    char * shstrtab = (char * ) fileContents->data() + rdi(shdrs[shstrtabIndex].sh_offset);
+    auto shstrtabSize = rdi(shdrs[shstrtabIndex].sh_size);
+    size_t shstrtabptr;
+    if (__builtin_add_overflow(reinterpret_cast<size_t>(fileContents->data()), rdi(shdrs[shstrtabIndex].sh_offset), &shstrtabptr))
+        error("string table overflow");
+    const char *shstrtab = reinterpret_cast<const char *>(shstrtabptr);
     checkPointer(fileContents, shstrtab, shstrtabSize);
 
     if (shstrtabSize == 0)
         error("string table size is zero");
 
     if (shstrtab[shstrtabSize - 1] != 0)
         error("string table is not zero terminated");
@@ -305,15 +353,15 @@
     sectionsByOldIndex.resize(shdrs.size());
     for (size_t i = 1; i < shdrs.size(); ++i)
         sectionsByOldIndex.at(i) = getSectionName(shdrs.at(i));
 }
 
 
 template<ElfFileParams>
-unsigned int ElfFile<ElfFileParamNames>::getPageSize() const
+unsigned int ElfFile<ElfFileParamNames>::getPageSize() const noexcept
 {
     if (forcedPageSize > 0)
         return forcedPageSize;
 
     // Architectures (and ABIs) can have different minimum section alignment
     // requirements. There is no authoritative list of these values. The
     // current list is extracted from GNU gold's source code (abi_pagesize).
@@ -427,14 +475,16 @@
         return;
     error("close");
 }
 
 
 static uint64_t roundUp(uint64_t n, uint64_t m)
 {
+    if (n == 0)
+        return m;
     return ((n - 1) / m + 1) * m;
 }
 
 
 template<ElfFileParams>
 void ElfFile<ElfFileParamNames>::shiftFile(unsigned int extraPages, size_t startOffset, size_t extraBytes)
 {
@@ -527,39 +577,60 @@
         error("section name offset out of bounds");
 
     return std::string(sectionNames.c_str() + name_off);
 }
 
 
 template<ElfFileParams>
-Elf_Shdr & ElfFile<ElfFileParamNames>::findSectionHeader(const SectionName & sectionName)
+const Elf_Shdr & ElfFile<ElfFileParamNames>::findSectionHeader(const SectionName & sectionName) const
 {
     auto shdr = tryFindSectionHeader(sectionName);
     if (!shdr) {
         std::string extraMsg;
         if (sectionName == ".interp" || sectionName == ".dynamic" || sectionName == ".dynstr")
             extraMsg = ". The input file is most likely statically linked";
         error("cannot find section '" + sectionName + "'" + extraMsg);
     }
     return *shdr;
 }
 
 
 template<ElfFileParams>
-std::optional<std::reference_wrapper<Elf_Shdr>> ElfFile<ElfFileParamNames>::tryFindSectionHeader(const SectionName & sectionName)
+std::optional<std::reference_wrapper<const Elf_Shdr>> ElfFile<ElfFileParamNames>::tryFindSectionHeader(const SectionName & sectionName) const
 {
     auto i = getSectionIndex(sectionName);
     if (i)
         return shdrs.at(i);
     return {};
 }
 
+template<ElfFileParams>
+template<class T>
+span<T> ElfFile<ElfFileParamNames>::getSectionSpan(const Elf_Shdr & shdr) const
+{
+    return span((T*)(fileContents->data() + rdi(shdr.sh_offset)), rdi(shdr.sh_size)/sizeof(T));
+}
 
 template<ElfFileParams>
-unsigned int ElfFile<ElfFileParamNames>::getSectionIndex(const SectionName & sectionName)
+template<class T>
+span<T> ElfFile<ElfFileParamNames>::getSectionSpan(const SectionName & sectionName)
+{
+    return getSectionSpan<T>(findSectionHeader(sectionName));
+}
+
+template<ElfFileParams>
+template<class T>
+span<T> ElfFile<ElfFileParamNames>::tryGetSectionSpan(const SectionName & sectionName)
+{
+    auto shdrOpt = tryFindSectionHeader(sectionName);
+    return shdrOpt ? getSectionSpan<T>(*shdrOpt) : span<T>();
+}
+
+template<ElfFileParams>
+unsigned int ElfFile<ElfFileParamNames>::getSectionIndex(const SectionName & sectionName) const
 {
     for (unsigned int i = 1; i < rdi(hdr()->e_shnum); ++i)
         if (getSectionName(shdrs.at(i)) == sectionName) return i;
     return 0;
 }
 
 template<ElfFileParams>
@@ -575,36 +646,36 @@
     auto i = replacedSections.find(sectionName);
     std::string s;
 
     if (i != replacedSections.end()) {
         s = std::string(i->second);
     } else {
         auto shdr = findSectionHeader(sectionName);
-        s = std::string((char *) fileContents->data() + rdi(shdr.sh_offset), rdi(shdr.sh_size));
+        s = extractString(fileContents, rdi(shdr.sh_offset), rdi(shdr.sh_size));
     }
 
     s.resize(size);
     replacedSections[sectionName] = s;
 
     return replacedSections[sectionName];
 }
 
 
 template<ElfFileParams>
 void ElfFile<ElfFileParamNames>::writeReplacedSections(Elf_Off & curOff,
     Elf_Addr startAddr, Elf_Off startOffset)
 {
-    /* Overwrite the old section contents with 'X's.  Do this
+    /* Overwrite the old section contents with 'Z's.  Do this
        *before* writing the new section contents (below) to prevent
        clobbering previously written new section contents. */
     for (auto & i : replacedSections) {
         const std::string & sectionName = i.first;
-        Elf_Shdr & shdr = findSectionHeader(sectionName);
+        const Elf_Shdr & shdr = findSectionHeader(sectionName);
         if (rdi(shdr.sh_type) != SHT_NOBITS)
-            memset(fileContents->data() + rdi(shdr.sh_offset), 'X', rdi(shdr.sh_size));
+            memset(fileContents->data() + rdi(shdr.sh_offset), 'Z', rdi(shdr.sh_size));
     }
 
     std::set<unsigned int> noted_phdrs = {};
 
     /* We iterate over the sorted section headers here, so that the relative
        position between replaced sections stays the same.  */
     for (auto & shdr : shdrs) {
@@ -613,15 +684,15 @@
         if (i == replacedSections.end())
             continue;
 
         Elf_Shdr orig_shdr = shdr;
         debug("rewriting section '%s' from offset 0x%x (size %d) to offset 0x%x (size %d)\n",
             sectionName.c_str(), rdi(shdr.sh_offset), rdi(shdr.sh_size), curOff, i->second.size());
 
-        memcpy(fileContents->data() + curOff, (unsigned char *) i->second.c_str(),
+        memcpy(fileContents->data() + curOff, i->second.c_str(),
             i->second.size());
 
         /* Update the section header for this section. */
         wri(shdr.sh_offset, curOff);
         wri(shdr.sh_addr, startAddr + (curOff - startOffset));
         wri(shdr.sh_size, i->second.size());
         wri(shdr.sh_addralign, sectionAlignment);
@@ -725,20 +796,25 @@
 {
     /* For dynamic libraries, we just place the replacement sections
        at the end of the file.  They're mapped into memory by a
        PT_LOAD segment located directly after the last virtual address
        page of other segments. */
     Elf_Addr startPage = 0;
     Elf_Addr firstPage = 0;
+    unsigned alignStartPage = getPageSize();
     for (auto & phdr : phdrs) {
-        Elf_Addr thisPage = roundUp(rdi(phdr.p_vaddr) + rdi(phdr.p_memsz), getPageSize());
+        Elf_Addr thisPage = rdi(phdr.p_vaddr) + rdi(phdr.p_memsz);
         if (thisPage > startPage) startPage = thisPage;
         if (rdi(phdr.p_type) == PT_PHDR) firstPage = rdi(phdr.p_vaddr) - rdi(phdr.p_offset);
+        unsigned thisAlign = rdi(phdr.p_align);
+        alignStartPage = std::max(alignStartPage, thisAlign);
     }
 
+    startPage = roundUp(startPage, alignStartPage);
+
     debug("last page is 0x%llx\n", (unsigned long long) startPage);
     debug("first page is 0x%llx\n", (unsigned long long) firstPage);
 
     /* When normalizing note segments we will in the worst case be adding
        1 program header for each SHT_NOTE section. */
     unsigned int num_notes = std::count_if(shdrs.begin(), shdrs.end(),
         [this](Elf_Shdr shdr) { return rdi(shdr.sh_type) == SHT_NOTE; });
@@ -751,19 +827,24 @@
     unsigned int i = 1;
     Elf_Addr pht_size = sizeof(Elf_Ehdr) + (phdrs.size() + num_notes + 1)*sizeof(Elf_Phdr);
     while( i < rdi(hdr()->e_shnum) && rdi(shdrs.at(i).sh_offset) <= pht_size ) {
         if (not haveReplacedSection(getSectionName(shdrs.at(i))))
             replaceSection(getSectionName(shdrs.at(i)), rdi(shdrs.at(i).sh_size));
         i++;
     }
+    bool moveHeaderTableToTheEnd = rdi(hdr()->e_shoff) < pht_size;
 
     /* Compute the total space needed for the replaced sections */
     off_t neededSpace = 0;
     for (auto & s : replacedSections)
         neededSpace += roundUp(s.second.size(), sectionAlignment);
+
+    off_t headerTableSpace = roundUp(rdi(hdr()->e_shnum) * rdi(hdr()->e_shentsize), sectionAlignment);
+    if (moveHeaderTableToTheEnd)
+        neededSpace += headerTableSpace;
     debug("needed space is %d\n", neededSpace);
 
     Elf_Off startOffset = roundUp(fileContents->size(), getPageSize());
 
     // In older version of binutils (2.30), readelf would check if the dynamic
     // section segment is strictly smaller than the file (and not same size).
     // By making it one byte larger, we don't break readelf.
@@ -785,32 +866,56 @@
        rewriteSectionsExecutable() won't work because it doesn't have
        any virtual address space to grow downwards into. */
     if (isExecutable && startOffset > startPage) {
         debug("shifting new PT_LOAD segment by %d bytes to work around a Linux kernel bug\n", startOffset - startPage);
         startPage = startOffset;
     }
 
-    /* Add a segment that maps the replaced sections into memory. */
     wri(hdr()->e_phoff, sizeof(Elf_Ehdr));
-    phdrs.resize(rdi(hdr()->e_phnum) + 1);
-    wri(hdr()->e_phnum, rdi(hdr()->e_phnum) + 1);
-    Elf_Phdr & phdr = phdrs.at(rdi(hdr()->e_phnum) - 1);
-    wri(phdr.p_type, PT_LOAD);
-    wri(phdr.p_offset, startOffset);
-    wri(phdr.p_vaddr, wri(phdr.p_paddr, startPage));
-    wri(phdr.p_filesz, wri(phdr.p_memsz, neededSpace));
-    wri(phdr.p_flags, PF_R | PF_W);
-    wri(phdr.p_align, getPageSize());
 
+    bool needNewSegment = true;
+    auto& lastSeg = phdrs.back();
+    /* Try to extend the last segment to include replaced sections */
+    if (!phdrs.empty() &&
+        rdi(lastSeg.p_type) == PT_LOAD &&
+        rdi(lastSeg.p_flags) == (PF_R | PF_W) &&
+        rdi(lastSeg.p_align) == alignStartPage) {
+        auto segEnd = roundUp(rdi(lastSeg.p_offset) + rdi(lastSeg.p_memsz), getPageSize());
+        if (segEnd == startOffset) {
+            auto newSz = startOffset + neededSpace - rdi(lastSeg.p_offset);
+            wri(lastSeg.p_filesz, wri(lastSeg.p_memsz, newSz));
+            needNewSegment = false;
+        }
+    }
+
+    if (needNewSegment) {
+        /* Add a segment that maps the replaced sections into memory. */
+        phdrs.resize(rdi(hdr()->e_phnum) + 1);
+        wri(hdr()->e_phnum, rdi(hdr()->e_phnum) + 1);
+        Elf_Phdr & phdr = phdrs.at(rdi(hdr()->e_phnum) - 1);
+        wri(phdr.p_type, PT_LOAD);
+        wri(phdr.p_offset, startOffset);
+        wri(phdr.p_vaddr, wri(phdr.p_paddr, startPage));
+        wri(phdr.p_filesz, wri(phdr.p_memsz, neededSpace));
+        wri(phdr.p_flags, PF_R | PF_W);
+        wri(phdr.p_align, alignStartPage);
+    }
 
     normalizeNoteSegments();
 
 
     /* Write out the replaced sections. */
     Elf_Off curOff = startOffset;
+
+    if (moveHeaderTableToTheEnd) {
+        debug("Moving the shtable to offset %d\n", curOff);
+        wri(hdr()->e_shoff, curOff);
+        curOff += headerTableSpace;
+    }
+
     writeReplacedSections(curOff, startPage, startOffset);
     assert(curOff == startOffset + neededSpace);
 
     /* Write out the updated program and section headers */
     rewriteHeaders(firstPage + rdi(hdr()->e_phoff));
 }
 
@@ -910,23 +1015,37 @@
     if (neededSpace > startOffset) {
         /* We also need an additional program header, so adjust for that. */
         neededSpace += sizeof(Elf_Phdr);
         debug("needed space is %d\n", neededSpace);
 
         /* Calculate how many bytes are needed out of the additional pages. */
         size_t extraSpace = neededSpace - startOffset; 
-        unsigned int neededPages = roundUp(extraSpace, getPageSize()) / getPageSize();
+        // Always give one extra page to avoid colliding with segments that start at
+        // unaligned addresses and will be rounded down when loaded
+        unsigned int neededPages = 1 + roundUp(extraSpace, getPageSize()) / getPageSize();
         debug("needed pages is %d\n", neededPages);
         if (neededPages * getPageSize() > firstPage)
             error("virtual address space underrun!");
 
         shiftFile(neededPages, startOffset, extraSpace);
 
         firstPage -= neededPages * getPageSize();
         startOffset += neededPages * getPageSize();
+    } else {
+        Elf_Off rewrittenSectionsOffset = sizeof(Elf_Ehdr) + phdrs.size() * sizeof(Elf_Phdr);
+        for (auto& phdr : phdrs)
+            if (rdi(phdr.p_type) == PT_LOAD &&
+                rdi(phdr.p_offset) <= rewrittenSectionsOffset &&
+                rdi(phdr.p_offset) + rdi(phdr.p_filesz) > rewrittenSectionsOffset &&
+                rdi(phdr.p_filesz) < neededSpace)
+            {
+                wri(phdr.p_filesz, neededSpace);
+                wri(phdr.p_memsz, neededSpace);
+                break;
+            }
     }
 
 
     /* Clear out the free space. */
     Elf_Off curOff = sizeof(Elf_Ehdr) + phdrs.size() * sizeof(Elf_Phdr);
     debug("clearing first %d bytes\n", startOffset - curOff);
     memset(fileContents->data() + curOff, 0, startOffset - curOff);
@@ -1006,18 +1125,18 @@
     phdrs.insert(phdrs.end(), newPhdrs.begin(), newPhdrs.end());
 
     wri(hdr()->e_phnum, phdrs.size());
 }
 
 
 template<ElfFileParams>
-void ElfFile<ElfFileParamNames>::rewriteSections()
+void ElfFile<ElfFileParamNames>::rewriteSections(bool force)
 {
 
-    if (replacedSections.empty()) return;
+    if (!force && replacedSections.empty()) return;
 
     for (auto & i : replacedSections)
         debug("replacing section '%s' with size %d\n",
             i.first.c_str(), i.second.size());
 
     if (rdi(hdr()->e_type) == ET_DYN) {
         debug("this is a dynamic library\n");
@@ -1182,18 +1301,21 @@
 {
     assert(pos + t.size() <= s.size());
     copy(t.begin(), t.end(), s.begin() + pos);
 }
 
 
 template<ElfFileParams>
-std::string ElfFile<ElfFileParamNames>::getInterpreter()
+std::string ElfFile<ElfFileParamNames>::getInterpreter() const
 {
     auto shdr = findSectionHeader(".interp");
-    return std::string((char *) fileContents->data() + rdi(shdr.sh_offset), rdi(shdr.sh_size) - 1);
+    auto size = rdi(shdr.sh_size);
+    if (size > 0)
+        size--;
+    return extractString(fileContents, rdi(shdr.sh_offset), size);
 }
 
 template<ElfFileParams>
 void ElfFile<ElfFileParamNames>::modifyOsAbi(osAbiMode op, const std::string & newOsAbi)
 {
     unsigned char abi = hdr()->e_ident[EI_OSABI];
 
@@ -1308,15 +1430,15 @@
         dynSoname->d_un.d_val = shdrDynStr.sh_size;
     } else {
         /* There is no DT_SONAME entry in the .dynamic section, so we
            have to grow the .dynamic section. */
         std::string & newDynamic = replaceSection(".dynamic", rdi(shdrDynamic.sh_size) + sizeof(Elf_Dyn));
 
         unsigned int idx = 0;
-        for (; rdi(((Elf_Dyn *) newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++);
+        for (; rdi(reinterpret_cast<const Elf_Dyn *>(newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++);
         debug("DT_NULL index is %d\n", idx);
 
         /* Shift all entries down by one. */
         setSubstr(newDynamic, sizeof(Elf_Dyn), std::string(newDynamic, 0, sizeof(Elf_Dyn) * (idx + 1)));
 
         /* Add the DT_SONAME entry at the top. */
         Elf_Dyn newDyn;
@@ -1424,15 +1546,15 @@
     if (rdi(shdrDynamic.sh_type) == SHT_NOBITS) {
             debug("no dynamic section\n");
             return;
     }
 
     /* !!! We assume that the virtual address in the DT_STRTAB entry
        of the dynamic section corresponds to the .dynstr section. */
-    auto shdrDynStr = findSectionHeader(".dynstr");
+    auto& shdrDynStr = findSectionHeader(".dynstr");
     char * strTab = (char *) fileContents->data() + rdi(shdrDynStr.sh_offset);
 
 
     /* Walk through the dynamic section, look for the RPATH/RUNPATH
        entry.
 
        According to the ld.so docs, DT_RPATH is obsolete, we should
@@ -1464,28 +1586,28 @@
             neededLibs.push_back(std::string(strTab + rdi(dyn->d_un.d_val)));
     }
 
     switch (op) {
         case rpPrint: {
             printf("%s\n", rpath ? rpath : "");
             return;
-        };
+        }
         case rpRemove: {
             if (!rpath) {
                 debug("no RPATH to delete\n");
                 return;
             }
             removeRPath(shdrDynamic);
             return;
         }
         case rpShrink: {
             if (!rpath) {
                 debug("no RPATH to shrink\n");
                 return;
-            ;}
+            }
             newRPath = shrinkRPath(rpath, neededLibs, allowedRpathPrefixes);
             break;
         }
         case rpAdd: {
             auto temp = std::string(rpath ? rpath : "");
             appendRPath(temp, newRPath);
             newRPath = temp;
@@ -1507,32 +1629,47 @@
     }
 
     if (rpath && rpath == newRPath) {
         return;
     }
     changed = true;
 
-    /* Zero out the previous rpath to prevent retained dependencies in
-       Nix. */
+    bool rpathStrShared = false;
     size_t rpathSize = 0;
     if (rpath) {
-        rpathSize = strlen(rpath);
+        std::string_view rpathView {rpath};
+        rpathSize = rpathView.size();
+
+        size_t rpathStrReferences = 0;
+        forAllStringReferences(shdrDynStr, [&] (auto refIdx) {
+            if (rpathView.end() == std::string_view(strTab + rdi(refIdx)).end())
+                rpathStrReferences++;
+        });
+        assert(rpathStrReferences >= 1);
+        debug("Number of rpath references: %lu\n", rpathStrReferences);
+        rpathStrShared = rpathStrReferences > 1;
+    }
+
+    /* Zero out the previous rpath to prevent retained dependencies in
+       Nix. */
+    if (rpath && !rpathStrShared) {
+        debug("Tainting old rpath with Xs\n");
         memset(rpath, 'X', rpathSize);
     }
 
     debug("new rpath is '%s'\n", newRPath.c_str());
 
 
-    if (newRPath.size() <= rpathSize) {
+    if (!rpathStrShared && newRPath.size() <= rpathSize) {
         if (rpath) memcpy(rpath, newRPath.c_str(), newRPath.size() + 1);
         return;
     }
 
     /* Grow the .dynstr section to make room for the new RPATH. */
-    debug("rpath is too long, resizing...\n");
+    debug("rpath is too long or shared, resizing...\n");
 
     std::string & newDynStr = replaceSection(".dynstr",
         rdi(shdrDynStr.sh_size) + newRPath.size() + 1);
     setSubstr(newDynStr, rdi(shdrDynStr.sh_size), newRPath + '\0');
 
     /* Update the DT_RUNPATH and DT_RPATH entries. */
     if (dynRunPath || dynRPath) {
@@ -1543,15 +1680,15 @@
     else {
         /* There is no DT_RUNPATH entry in the .dynamic section, so we
            have to grow the .dynamic section. */
         std::string & newDynamic = replaceSection(".dynamic",
             rdi(shdrDynamic.sh_size) + sizeof(Elf_Dyn));
 
         unsigned int idx = 0;
-        for ( ; rdi(((Elf_Dyn *) newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
+        for ( ; rdi(reinterpret_cast<const Elf_Dyn *>(newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
         debug("DT_NULL index is %d\n", idx);
 
         /* Shift all entries down by one. */
         setSubstr(newDynamic, sizeof(Elf_Dyn),
             std::string(newDynamic, 0, sizeof(Elf_Dyn) * (idx + 1)));
 
         /* Add the DT_RUNPATH entry at the top. */
@@ -1745,15 +1882,15 @@
     }
 
     /* add all new needed entries to the dynamic section */
     std::string & newDynamic = replaceSection(".dynamic",
         rdi(shdrDynamic.sh_size) + sizeof(Elf_Dyn) * libs.size());
 
     unsigned int idx = 0;
-    for ( ; rdi(((Elf_Dyn *) newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
+    for ( ; rdi(reinterpret_cast<const Elf_Dyn *>(newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
     debug("DT_NULL index is %d\n", idx);
 
     /* Shift all entries down by the number of new entries. */
     setSubstr(newDynamic, sizeof(Elf_Dyn) * libs.size(),
         std::string(newDynamic, 0, sizeof(Elf_Dyn) * (idx + 1)));
 
     /* Add the DT_NEEDED entries at the top. */
@@ -1768,21 +1905,21 @@
 
     changed = true;
 
     this->rewriteSections();
 }
 
 template<ElfFileParams>
-void ElfFile<ElfFileParamNames>::printNeededLibs() // const
+void ElfFile<ElfFileParamNames>::printNeededLibs() const
 {
     const auto shdrDynamic = findSectionHeader(".dynamic");
     const auto shdrDynStr = findSectionHeader(".dynstr");
-    const char *strTab = (char *)fileContents->data() + rdi(shdrDynStr.sh_offset);
+    const char *strTab = (const char *)fileContents->data() + rdi(shdrDynStr.sh_offset);
 
-    const Elf_Dyn *dyn = (Elf_Dyn *) (fileContents->data() + rdi(shdrDynamic.sh_offset));
+    const Elf_Dyn *dyn = (const Elf_Dyn *) (fileContents->data() + rdi(shdrDynamic.sh_offset));
 
     for (; rdi(dyn->d_tag) != DT_NULL; dyn++) {
         if (rdi(dyn->d_tag) == DT_NEEDED) {
             const char *name = strTab + rdi(dyn->d_un.d_val);
             printf("%s\n", name);
         }
     }
@@ -1807,15 +1944,15 @@
             return;
         dynFlags1->d_un.d_val |= DF_1_NODEFLIB;
     } else {
         std::string & newDynamic = replaceSection(".dynamic",
                 rdi(shdrDynamic.sh_size) + sizeof(Elf_Dyn));
 
         unsigned int idx = 0;
-        for ( ; rdi(((Elf_Dyn *) newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
+        for ( ; rdi(reinterpret_cast<const Elf_Dyn *>(newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
         debug("DT_NULL index is %d\n", idx);
 
         /* Shift all entries down by one. */
         setSubstr(newDynamic, sizeof(Elf_Dyn),
                 std::string(newDynamic, 0, sizeof(Elf_Dyn) * (idx + 1)));
 
         /* Add the DT_FLAGS_1 entry at the top. */
@@ -1840,15 +1977,15 @@
             return;
         }
     }
     std::string & newDynamic = replaceSection(".dynamic",
             rdi(shdrDynamic.sh_size) + sizeof(Elf_Dyn));
 
     unsigned int idx = 0;
-    for ( ; rdi(((Elf_Dyn *) newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
+    for ( ; rdi(reinterpret_cast<const Elf_Dyn *>(newDynamic.c_str())[idx].d_tag) != DT_NULL; idx++) ;
     debug("DT_NULL index is %d\n", idx);
 
     /* Shift all entries down by one. */
     setSubstr(newDynamic, sizeof(Elf_Dyn),
             std::string(newDynamic, 0, sizeof(Elf_Dyn) * (idx + 1)));
 
     /* Add the DT_DEBUG entry at the top. */
@@ -1857,14 +1994,228 @@
     newDyn.d_un.d_val = 0;
     setSubstr(newDynamic, 0, std::string((char *) &newDyn, sizeof(Elf_Dyn)));
 
     this->rewriteSections();
     changed = true;
 }
 
+static uint32_t gnuHash(std::string_view name) {
+    uint32_t h = 5381;
+    for (uint8_t c : name)
+        h = ((h << 5) + h) + c;
+    return h;
+}
+
+template<ElfFileParams>
+auto ElfFile<ElfFileParamNames>::parseGnuHashTable(span<char> sectionData) -> GnuHashTable
+{
+    auto hdr = (typename GnuHashTable::Header*)sectionData.begin();
+    auto bloomFilters = span((typename GnuHashTable::BloomWord*)(hdr+1), rdi(hdr->maskwords));
+    auto buckets = span((uint32_t*)bloomFilters.end(), rdi(hdr->numBuckets));
+    auto table = span(buckets.end(), ((uint32_t*)sectionData.end()) - buckets.end());
+    return GnuHashTable{*hdr, bloomFilters, buckets, table};
+}
+
+template<ElfFileParams>
+void ElfFile<ElfFileParamNames>::rebuildGnuHashTable(span<char> strTab, span<Elf_Sym> dynsyms)
+{
+    auto sectionData = tryGetSectionSpan<char>(".gnu.hash");
+    if (!sectionData)
+        return;
+
+    auto ght = parseGnuHashTable(sectionData);
+
+    // We can't trust the value of symndx when the hash table is empty
+    if (ght.m_table.size() == 0)
+        return;
+
+    // The hash table includes only a subset of dynsyms
+    auto firstSymIdx = rdi(ght.m_hdr.symndx);
+    dynsyms = span(&dynsyms[firstSymIdx], dynsyms.end());
+
+    // Only use the range of symbol versions that will be changed
+    auto versyms = tryGetSectionSpan<Elf_Versym>(".gnu.version");
+    if (versyms)
+        versyms = span(&versyms[firstSymIdx], versyms.end());
+
+    struct Entry
+    {
+        uint32_t hash, bucketIdx, originalPos;
+    };
+
+    std::vector<Entry> entries;
+    entries.reserve(dynsyms.size());
+
+    uint32_t pos = 0; // Track the original position of the symbol in the table
+    for (auto& sym : dynsyms)
+    {
+        Entry e;
+        e.hash = gnuHash(&strTab[rdi(sym.st_name)]);
+        e.bucketIdx = e.hash % ght.m_buckets.size();
+        e.originalPos = pos++;
+        entries.push_back(e);
+    }
+
+    // Sort the entries based on the buckets. This is a requirement for gnu hash table to work
+    std::sort(entries.begin(), entries.end(), [&] (auto& l, auto& r) {
+        return l.bucketIdx < r.bucketIdx;
+    });
+
+    // Create a map of old positions to new positions after sorting
+    std::vector<uint32_t> old2new(entries.size());
+    for (size_t i = 0; i < entries.size(); ++i)
+        old2new[entries[i].originalPos] = i;
+
+    // Update the symbol table with the new order and
+    // all tables that refer to symbols through indexes in the symbol table
+    auto reorderSpan = [] (auto dst, auto& old2new)
+    {
+        std::vector tmp(dst.begin(), dst.end());
+        for (size_t i = 0; i < tmp.size(); ++i)
+            dst[old2new[i]] = tmp[i];
+    };
+
+    reorderSpan(dynsyms, old2new);
+    if (versyms)
+        reorderSpan(versyms, old2new);
+
+    auto remapSymbolId = [&old2new, firstSymIdx] (auto& oldSymIdx)
+    {
+        return oldSymIdx >= firstSymIdx ? old2new[oldSymIdx - firstSymIdx] + firstSymIdx
+                                        : oldSymIdx;
+    };
+
+    for (unsigned int i = 1; i < rdi(hdr()->e_shnum); ++i)
+    {
+        auto& shdr = shdrs.at(i);
+        auto shtype = rdi(shdr.sh_type);
+        if (shtype == SHT_REL)
+            changeRelocTableSymIds<Elf_Rel>(shdr, remapSymbolId);
+        else if (shtype == SHT_RELA)
+            changeRelocTableSymIds<Elf_Rela>(shdr, remapSymbolId);
+    }
+
+    // Update bloom filters
+    std::fill(ght.m_bloomFilters.begin(), ght.m_bloomFilters.end(), 0); 
+    for (size_t i = 0; i < entries.size(); ++i)
+    {
+        auto h = entries[i].hash;
+        size_t idx = (h / ElfClass) % ght.m_bloomFilters.size();
+        auto val = rdi(ght.m_bloomFilters[idx]);
+        val |= uint64_t(1) << (h % ElfClass);
+        val |= uint64_t(1) << ((h >> rdi(ght.m_hdr.shift2)) % ElfClass);
+        wri(ght.m_bloomFilters[idx], val);
+    }
+
+    // Fill buckets
+    std::fill(ght.m_buckets.begin(), ght.m_buckets.end(), 0); 
+    for (size_t i = 0; i < entries.size(); ++i)
+    {
+        auto symBucketIdx = entries[i].bucketIdx;
+        if (!ght.m_buckets[symBucketIdx])
+            wri(ght.m_buckets[symBucketIdx], i + firstSymIdx);
+    }
+
+    // Fill hash table
+    for (size_t i = 0; i < entries.size(); ++i)
+    {
+        auto& n = entries[i];
+        bool isLast = (i == entries.size() - 1) || (n.bucketIdx != entries[i+1].bucketIdx);
+        // Add hash with first bit indicating end of chain
+        wri(ght.m_table[i], isLast ? (n.hash | 1) : (n.hash & ~1));
+    }
+}
+
+static uint32_t sysvHash(std::string_view name) {
+    uint32_t h = 0;
+    for (uint8_t c : name)
+    {
+        h = (h << 4) + c;
+        uint32_t g = h & 0xf0000000;
+        if (g != 0)
+            h ^= g >> 24;
+        h &= ~g;
+    }
+    return h;
+}
+
+template<ElfFileParams>
+auto ElfFile<ElfFileParamNames>::parseHashTable(span<char> sectionData) -> HashTable
+{
+    auto hdr = (typename HashTable::Header*)sectionData.begin();
+    auto buckets = span((uint32_t*)(hdr+1), rdi(hdr->numBuckets));
+    auto table = span(buckets.end(), ((uint32_t*)sectionData.end()) - buckets.end());
+    return HashTable{*hdr, buckets, table};
+}
+
+template<ElfFileParams>
+void ElfFile<ElfFileParamNames>::rebuildHashTable(span<char> strTab, span<Elf_Sym> dynsyms)
+{
+    auto sectionData = tryGetSectionSpan<char>(".hash");
+    if (!sectionData)
+        return;
+
+    auto ht = parseHashTable(sectionData);
+
+    std::fill(ht.m_buckets.begin(), ht.m_buckets.end(), 0);
+    std::fill(ht.m_chain.begin(), ht.m_chain.end(), 0);
+
+    // The hash table includes only a subset of dynsyms
+    auto firstSymIdx = dynsyms.size() - ht.m_chain.size();
+    dynsyms = span(&dynsyms[firstSymIdx], dynsyms.end());
+
+    for (auto& sym : dynsyms)
+    {
+        auto name = &strTab[rdi(sym.st_name)];
+        uint32_t i = &sym - dynsyms.begin();
+        uint32_t hash = sysvHash(name) % ht.m_buckets.size();
+        wri(ht.m_chain[i], rdi(ht.m_buckets[hash]));
+        wri(ht.m_buckets[hash], i);
+    }
+}
+
+template<ElfFileParams>
+void ElfFile<ElfFileParamNames>::renameDynamicSymbols(const std::unordered_map<std::string_view, std::string>& remap)
+{
+    auto dynsyms = getSectionSpan<Elf_Sym>(".dynsym");
+    auto strTab = getSectionSpan<char>(".dynstr");
+
+    std::vector<char> extraStrings;
+    extraStrings.reserve(remap.size() * 30); // Just an estimate
+    for (auto& dynsym : dynsyms)
+    {
+        std::string_view name = &strTab[rdi(dynsym.st_name)];
+        auto it = remap.find(name);
+        if (it != remap.end())
+        {
+            wri(dynsym.st_name, strTab.size() + extraStrings.size());
+            auto& newName = it->second;
+            debug("renaming dynamic symbol %s to %s\n", name.data(), it->second.c_str());
+            extraStrings.insert(extraStrings.end(), newName.begin(), newName.end() + 1);
+            changed = true;
+        } else {
+            debug("skip renaming dynamic symbol %sn", name.data());
+        }
+    }
+
+    if (!extraStrings.empty())
+    {
+        auto newStrTabSize = strTab.size() + extraStrings.size();
+        auto& newSec = replaceSection(".dynstr", newStrTabSize);
+        auto newStrTabSpan = span(newSec.data(), newStrTabSize);
+
+        std::copy(extraStrings.begin(), extraStrings.end(), &newStrTabSpan[strTab.size()]);
+
+        rebuildGnuHashTable(newStrTabSpan, dynsyms);
+        rebuildHashTable(newStrTabSpan, dynsyms);
+    }
+
+    this->rewriteSections();
+}
+
 template<ElfFileParams>
 void ElfFile<ElfFileParamNames>::clearSymbolVersions(const std::set<std::string> & syms)
 {
     if (syms.empty()) return;
 
     auto shdrDynStr = findSectionHeader(".dynstr");
     auto shdrDynsym = findSectionHeader(".dynsym");
@@ -1886,36 +2237,157 @@
             wri(versyms[i], 1);
         }
     }
     changed = true;
     this->rewriteSections();
 }
 
+template<ElfFileParams>
+void ElfFile<ElfFileParamNames>::modifyExecstack(ExecstackMode op)
+{
+    if (op == ExecstackMode::clear || op == ExecstackMode::set) {
+        size_t nullhdr = (size_t)-1;
+
+        for (size_t i = 0; i < phdrs.size(); i++) {
+            auto & header = phdrs[i];
+            const auto type = rdi(header.p_type);
+            if (type != PT_GNU_STACK) {
+                if (!nullhdr && type == PT_NULL)
+                    nullhdr = i;
+                continue;
+            }
+
+            if (op == ExecstackMode::clear && (rdi(header.p_flags) & PF_X) == PF_X) {
+                debug("simple execstack clear of header %zu\n", i);
+
+                wri(header.p_flags, rdi(header.p_flags) & ~PF_X);
+                * ((Elf_Phdr *) (fileContents->data() + rdi(hdr()->e_phoff)) + i) = header;
+                changed = true;
+            } else if (op == ExecstackMode::set && (rdi(header.p_flags) & PF_X) != PF_X) {
+                debug("simple execstack set of header %zu\n", i);
+
+                wri(header.p_flags, rdi(header.p_flags) | PF_X);
+                * ((Elf_Phdr *) (fileContents->data() + rdi(hdr()->e_phoff)) + i) = header;
+                changed = true;
+            } else {
+                debug("execstack already in requested state\n");
+            }
+
+            return;
+        }
+
+        if (nullhdr != (size_t)-1) {
+            debug("replacement execstack of header %zu\n", nullhdr);
+
+            auto & header = phdrs[nullhdr];
+            header = {};
+            wri(header.p_type,  PT_GNU_STACK);
+            wri(header.p_flags, PF_R | PF_W | (op == ExecstackMode::set ? PF_X : 0));
+            wri(header.p_align, 0x1);
+
+            * ((Elf_Phdr *) (fileContents->data() + rdi(hdr()->e_phoff)) + nullhdr) = header;
+            changed = true;
+            return;
+        }
+
+        debug("header addition for execstack\n");
+
+        Elf_Phdr new_phdr = {};
+        wri(new_phdr.p_type,  PT_GNU_STACK);
+        wri(new_phdr.p_flags, PF_R | PF_W | (op == ExecstackMode::set ? PF_X : 0));
+        wri(new_phdr.p_align, 0x1);
+        phdrs.push_back(new_phdr);
+
+        wri(hdr()->e_phnum, rdi(hdr()->e_phnum) + 1);
+
+        changed = true;
+        rewriteSections(true);
+        return;
+    }
+
+    char result = '?';
+
+    for (const auto & header : phdrs) {
+        if (rdi(header.p_type) != PT_GNU_STACK)
+            continue;
+
+        if ((rdi(header.p_flags) & PF_X) == PF_X)
+            result = 'X';
+        else
+            result = '-';
+        break;
+    }
+
+    printf("execstack: %c\n", result);
+}
+
+template<ElfFileParams>
+template<class StrIdxCallback>
+void ElfFile<ElfFileParamNames>::forAllStringReferences(const Elf_Shdr& strTabHdr, StrIdxCallback&& fn)
+{
+    for (auto& sym : tryGetSectionSpan<Elf_Sym>(".dynsym"))
+        fn(sym.st_name);
+
+    for (auto& dyn : tryGetSectionSpan<Elf_Dyn>(".dynamic"))
+        switch (rdi(dyn.d_tag))
+        {
+            case DT_NEEDED:
+            case DT_SONAME:
+            case DT_RPATH:
+            case DT_RUNPATH: fn(dyn.d_un.d_val);
+            default:;
+        }
+
+    if (auto verdHdr = tryFindSectionHeader(".gnu.version_d"))
+    {
+        if (&shdrs.at(rdi(verdHdr->get().sh_link)) == &strTabHdr)
+            forAll_ElfVer(getSectionSpan<Elf_Verdef>(*verdHdr),
+                [] (auto& /*vd*/) {},
+                [&] (auto& vda) { fn(vda.vda_name); }
+            );
+    }
+
+    if (auto vernHdr = tryFindSectionHeader(".gnu.version_r"))
+    {
+        if (&shdrs.at(rdi(vernHdr->get().sh_link)) == &strTabHdr)
+            forAll_ElfVer(getSectionSpan<Elf_Verneed>(*vernHdr),
+                [&] (auto& vn) { fn(vn.vn_file); },
+                [&] (auto& vna) { fn(vna.vna_name); }
+            );
+    }
+}
+
 static bool printInterpreter = false;
 static bool printOsAbi = false;
 static bool setOsAbi = false;
 static std::string newOsAbi;
 static bool printSoname = false;
 static bool setSoname = false;
 static std::string newSoname;
 static std::string newInterpreter;
 static bool shrinkRPath = false;
 static std::vector<std::string> allowedRpathPrefixes;
 static bool removeRPath = false;
 static bool setRPath = false;
 static bool addRPath = false;
 static bool addDebugTag = false;
+static bool renameDynamicSymbols = false;
 static bool printRPath = false;
 static std::string newRPath;
 static std::set<std::string> neededLibsToRemove;
 static std::map<std::string, std::string> neededLibsToReplace;
 static std::set<std::string> neededLibsToAdd;
 static std::set<std::string> symbolsToClearVersion;
+static std::unordered_map<std::string_view, std::string> symbolsToRename;
+static std::unordered_set<std::string> symbolsToRenameKeys;
 static bool printNeeded = false;
 static bool noDefaultLib = false;
+static bool printExecstack = false;
+static bool clearExecstack = false;
+static bool setExecstack = false;
 
 template<class ElfFile>
 static void patchElf2(ElfFile && elfFile, const FileContents & fileContents, const std::string & fileName)
 {
     if (printInterpreter)
         printf("%s\n", elfFile.getInterpreter().c_str());
 
@@ -1933,14 +2405,21 @@
 
     if (!newInterpreter.empty())
         elfFile.setInterpreter(newInterpreter);
 
     if (printRPath)
         elfFile.modifyRPath(elfFile.rpPrint, {}, "");
 
+    if (printExecstack)
+        elfFile.modifyExecstack(ElfFile::ExecstackMode::print);
+    else if (clearExecstack)
+        elfFile.modifyExecstack(ElfFile::ExecstackMode::clear);
+    else if (setExecstack)
+        elfFile.modifyExecstack(ElfFile::ExecstackMode::set);
+
     if (shrinkRPath)
         elfFile.modifyRPath(elfFile.rpShrink, allowedRpathPrefixes, "");
     else if (removeRPath)
         elfFile.modifyRPath(elfFile.rpRemove, {}, "");
     else if (setRPath)
         elfFile.modifyRPath(elfFile.rpSet, {}, newRPath);
     else if (addRPath)
@@ -1955,14 +2434,17 @@
 
     if (noDefaultLib)
         elfFile.noDefaultLib();
 
     if (addDebugTag)
         elfFile.addDebugTag();
 
+    if (renameDynamicSymbols)
+        elfFile.renameDynamicSymbols(symbolsToRename);
+
     if (elfFile.isChanged()){
         writeFile(fileName, elfFile.fileContents);
     } else if (alwaysWrite) {
         debug("not modified, but alwaysWrite=true\n");
         writeFile(fileName, fileContents);
     }
 }
@@ -1974,31 +2456,31 @@
         if (!printInterpreter && !printRPath && !printSoname && !printNeeded)
             debug("patching ELF file '%s'\n", fileName.c_str());
 
         auto fileContents = readFile(fileName);
         const std::string & outputFileName2 = outputFileName.empty() ? fileName : outputFileName;
 
         if (getElfType(fileContents).is32Bit)
-            patchElf2(ElfFile<Elf32_Ehdr, Elf32_Phdr, Elf32_Shdr, Elf32_Addr, Elf32_Off, Elf32_Dyn, Elf32_Sym, Elf32_Verneed, Elf32_Versym>(fileContents), fileContents, outputFileName2);
+            patchElf2(ElfFile<Elf32_Ehdr, Elf32_Phdr, Elf32_Shdr, Elf32_Addr, Elf32_Off, Elf32_Dyn, Elf32_Sym, Elf32_Versym, Elf32_Verdef, Elf32_Verdaux, Elf32_Verneed, Elf32_Vernaux, Elf32_Rel, Elf32_Rela, 32>(fileContents), fileContents, outputFileName2);
         else
-            patchElf2(ElfFile<Elf64_Ehdr, Elf64_Phdr, Elf64_Shdr, Elf64_Addr, Elf64_Off, Elf64_Dyn, Elf64_Sym, Elf64_Verneed, Elf64_Versym>(fileContents), fileContents, outputFileName2);
+            patchElf2(ElfFile<Elf64_Ehdr, Elf64_Phdr, Elf64_Shdr, Elf64_Addr, Elf64_Off, Elf64_Dyn, Elf64_Sym, Elf64_Versym, Elf64_Verdef, Elf64_Verdaux, Elf64_Verneed, Elf64_Vernaux, Elf64_Rel, Elf64_Rela, 64>(fileContents), fileContents, outputFileName2);
     }
 }
 
-std::string resolveArgument(const char *arg) {
+[[nodiscard]] static std::string resolveArgument(const char *arg) {
   if (strlen(arg) > 0 && arg[0] == '@') {
     FileContents cnts = readFile(arg + 1);
     return std::string((char *)cnts->data(), cnts->size());
   }
 
   return std::string(arg);
 }
 
 
-void showHelp(const std::string & progName)
+static void showHelp(const std::string & progName)
 {
         fprintf(stderr, "syntax: %s\n\
   [--set-interpreter FILENAME]\n\
   [--page-size SIZE]\n\
   [--print-interpreter]\n\
   [--print-os-abi]\t\tPrints 'EI_OSABI' field of ELF header\n\
   [--set-os-abi ABI]\t\tSets 'EI_OSABI' field of ELF header to ABI.\n\
@@ -2015,22 +2497,26 @@
   [--remove-needed LIBRARY]\n\
   [--replace-needed LIBRARY NEW_LIBRARY]\n\
   [--print-needed]\n\
   [--no-default-lib]\n\
   [--no-sort]\t\tDo not sort program+section headers; useful for debugging patchelf.\n\
   [--clear-symbol-version SYMBOL]\n\
   [--add-debug-tag]\n\
+  [--print-execstack]\t\tPrints whether the object requests an executable stack\n\
+  [--clear-execstack]\n\
+  [--set-execstack]\n\
+  [--rename-dynamic-symbols NAME_MAP_FILE]\tRenames dynamic symbols. The map file should contain two symbols (old_name new_name) per line\n\
   [--output FILE]\n\
   [--debug]\n\
   [--version]\n\
   FILENAME...\n", progName.c_str());
 }
 
 
-int mainWrapped(int argc, char * * argv)
+static int mainWrapped(int argc, char * * argv)
 {
     if (argc <= 1) {
         showHelp(argv[0]);
         return 1;
     }
 
     if (getenv("PATCHELF_DEBUG") != nullptr)
@@ -2123,28 +2609,62 @@
             neededLibsToReplace[ argv[i+1] ] = argv[i+2];
             i += 2;
         }
         else if (arg == "--clear-symbol-version") {
             if (++i == argc) error("missing argument");
             symbolsToClearVersion.insert(resolveArgument(argv[i]));
         }
+        else if (arg == "--print-execstack") {
+            printExecstack = true;
+        }
+        else if (arg == "--clear-execstack") {
+            clearExecstack = true;
+        }
+        else if (arg == "--set-execstack") {
+            setExecstack = true;
+        }
         else if (arg == "--output") {
             if (++i == argc) error("missing argument");
             outputFileName = resolveArgument(argv[i]);
             alwaysWrite = true;
         }
         else if (arg == "--debug") {
             debugMode = true;
         }
         else if (arg == "--no-default-lib") {
             noDefaultLib = true;
         }
         else if (arg == "--add-debug-tag") {
             addDebugTag = true;
         }
+        else if (arg == "--rename-dynamic-symbols") {
+            renameDynamicSymbols = true;
+            if (++i == argc) error("missing argument");
+
+            const char* fname = argv[i];
+            std::ifstream infile(fname);
+            if (!infile) error(fmt("Cannot open map file ", fname));
+
+            std::string line, from, to;
+            size_t lineCount = 1;
+            while (std::getline(infile, line))
+            {
+                std::istringstream iss(line);
+                if (!(iss >> from))
+                    break;
+                if (!(iss >> to))
+                    error(fmt(fname, ":", lineCount, ": Map file line is missing the second element"));
+                if (symbolsToRenameKeys.count(from))
+                    error(fmt(fname, ":", lineCount, ": Name '", from, "' appears twice in the map file"));
+                if (from.find('@') != std::string_view::npos || to.find('@') != std::string_view::npos)
+                    error(fmt(fname, ":", lineCount, ": Name pair contains version tag: ", from, " ", to));
+                lineCount++;
+                symbolsToRename[*symbolsToRenameKeys.insert(from).first] = to;
+            }
+        }
         else if (arg == "--help" || arg == "-h" ) {
             showHelp(argv[0]);
             return 0;
         }
         else if (arg == "--version") {
             printf(PACKAGE_STRING "\n");
             return 0;
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/Makefile.am` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/Makefile.am`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LIBS =
 
-check_PROGRAMS = simple-pie simple main too-many-strtab main-scoped big-dynstr no-rpath contiguous-note-sections
+check_PROGRAMS = simple-pie simple simple-execstack main too-many-strtab main-scoped big-dynstr no-rpath contiguous-note-sections
 
 no_rpath_arch_TESTS = \
   no-rpath-amd64.sh \
   no-rpath-armel.sh \
   no-rpath-armhf.sh \
   no-rpath-hurd-i386.sh \
   no-rpath-i386.sh \
@@ -39,22 +39,31 @@
   args-from-file.sh \
   basic-flags.sh \
   set-empty-rpath.sh \
   phdr-corruption.sh \
   replace-needed.sh \
   replace-add-needed.sh \
   add-debug-tag.sh \
+  repeated-updates.sh \
+  empty-note.sh \
+  print-execstack.sh \
+  modify-execstack.sh \
+  rename-dynamic-symbols.sh \
+  overlapping-segments-after-rounding.sh \
+  shared-rpath.sh \
+  short-first-segment.sh \
   empty-note.sh
 
 build_TESTS = \
   $(no_rpath_arch_TESTS)
 
 TESTS = $(src_TESTS) $(build_TESTS)
 
-EXTRA_DIST = no-rpath-prebuild $(src_TESTS) no-rpath-prebuild.sh invalid-elf endianness empty-note
+EXTRA_DIST = no-rpath-prebuild $(src_TESTS) no-rpath-prebuild.sh invalid-elf endianness empty-note \
+			 overlapping-segments-after-rounding short-first-segment.gz
 
 TESTS_ENVIRONMENT = PATCHELF_DEBUG=1 STRIP=$(STRIP) OBJDUMP=$(OBJDUMP) READELF=$(READELF) OBJCOPY=$(OBJCOPY)
 
 $(no_rpath_arch_TESTS): no-rpath-prebuild.sh
 	@ln -s $< $@
 
 CLEANFILES = big-dynstr.c
@@ -67,18 +76,23 @@
 LDFLAGS_sharedlib = -Wl,--disable-new-dtags -shared -L. $(AM_LDFLAGS)
 export NIX_DONT_SET_RPATH=1
 export NIX_LDFLAGS=
 
 simple_SOURCES = simple.c
 # no -fpic for simple.o
 simple_CFLAGS =
+simple_LDFLAGS = -Wl,-z,noexecstack
 
 simple_pie_SOURCES = simple.c
 simple_pie_CFLAGS = -fPIC -pie
 
+simple_execstack_SOURCES = simple.c
+simple_execstack_CFLAGS =
+simple_execstack_LDFLAGS = -Wl,-z,execstack
+
 main_SOURCES = main.c
 main_LDADD = -lfoo $(AM_LDADD)
 main_DEPENDENCIES = libfoo.so
 main_LDFLAGS = $(LDFLAGS_local)
 
 main_scoped_SOURCES = main.c
 main_scoped_LDADD = -lfoo-scoped $(AM_LDADD)
@@ -104,16 +118,16 @@
 check_DATA = libbig-dynstr.debug
 
 
 # declare local shared libraries as programs as:
 # - without libtool, only archives (static libraries) can be built by automake
 # - with libtool, it is difficult to control options
 # - with libtool, it is not possible to compile convenience *dynamic* libraries :-(
-check_PROGRAMS += libfoo.so libfoo-scoped.so libbar.so libbar-scoped.so libsimple.so libbuildid.so libtoomanystrtab.so \
-                  phdr-corruption.so
+check_PROGRAMS += libfoo.so libfoo-scoped.so libbar.so libbar-scoped.so libsimple.so libsimple-execstack.so libbuildid.so libtoomanystrtab.so \
+                  phdr-corruption.so many-syms-main libmany-syms.so liboveralign.so libshared-rpath.so
 
 libbuildid_so_SOURCES = simple.c
 libbuildid_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,--build-id
 
 libfoo_so_SOURCES = foo.c
 libfoo_so_LDADD = -lbar $(AM_LDADD)
 libfoo_so_DEPENDENCIES = libbar.so
@@ -127,24 +141,50 @@
 libbar_so_SOURCES = bar.c
 libbar_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,-rpath,`pwd`/no-such-path
 
 libbar_scoped_so_SOURCES = bar.c
 libbar_scoped_so_LDFLAGS = $(LDFLAGS_sharedlib)
 
 libsimple_so_SOURCES = simple.c
-libsimple_so_LDFLAGS = $(LDFLAGS_sharedlib)
+libsimple_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,-z,noexecstack
+
+liboveralign_so_SOURCES = simple.c
+liboveralign_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,-z,max-page-size=0x10000
+
+libshared_rpath_so_SOURCES = shared-rpath.c
+libshared_rpath_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,-rpath=a_symbol_name
+
+libsimple_execstack_so_SOURCES = simple.c
+libsimple_execstack_so_LDFLAGS = $(LDFLAGS_sharedlib) -Wl,-z,execstack
 
 too_many_strtab_SOURCES = too-many-strtab.c too-many-strtab2.s
 libtoomanystrtab_so_SOURCES = too-many-strtab.c too-many-strtab2.s
 libtoomanystrtab_so_LDFLAGS = $(LDFLAGS_sharedlib)
 
+many_syms_main_SOURCES = many-syms-main.c 
+many_syms_main_LDFLAGS = $(LDFLAGS_local) 
+many_syms_main_LDADD = -lmany-syms $(AM_LDADD)
+many_syms_main_DEPENDENCIES = libmany-syms.so
+many_syms_main_CFLAGS = -pie
+libmany_syms_so_SOURCES = many-syms.c
+libmany_syms_so_LDFLAGS = $(LDFLAGS_sharedlib)
+
 no_rpath_SOURCES = no-rpath.c
 # no -fpic for no-rpath.o
 no_rpath_CFLAGS =
 
 contiguous_note_sections_SOURCES = contiguous-note-sections.s contiguous-note-sections.ld
 contiguous_note_sections_LDFLAGS = -nostdlib -T $(srcdir)/contiguous-note-sections.ld
 contiguous_note_sections_CFLAGS = -pie
 
 phdr_corruption_so_SOURCES = void.c phdr-corruption.ld
 phdr_corruption_so_LDFLAGS = -nostdlib -shared -Wl,-T$(srcdir)/phdr-corruption.ld
 phdr_corruption_so_CFLAGS =
+
+many-syms.c:
+	i=1; while [ $$i -le 2000 ]; do echo "void f$$i() {};"; i=$$(($$i + 1)); done > $@
+
+many-syms-main.c:
+	echo "int main() {" > $@
+	i=1; while [ $$i -le 2000 ]; do echo "void f$$i(); f$$i();"; i=$$(($$i + 1)); done >> $@
+	echo "}" >> $@
+
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/add-debug-tag.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/add-debug-tag.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 READELF=${READELF:-readelf}
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp libsimple.so ${SCRATCH}/
+cp libsimple.so "${SCRATCH}"/
 
 # check there is no DT_DEBUG tag
-debugTag=$($READELF -d ${SCRATCH}/libsimple.so)
+debugTag=$($READELF -d "${SCRATCH}/libsimple.so")
 echo ".dynamic before: $debugTag"
 if echo "$debugTag" | grep -q DEBUG; then
     echo "failed --add-debug-tag test. Expected no line with (DEBUG), got: $debugTag"
     exit 1
 fi
 
 # set DT_DEBUG
-../src/patchelf --add-debug-tag ${SCRATCH}/libsimple.so
+../src/patchelf --add-debug-tag "${SCRATCH}/libsimple.so"
 
 # check there is DT_DEBUG tag
-debugTag=$($READELF -d ${SCRATCH}/libsimple.so)
+debugTag=$($READELF -d "${SCRATCH}/libsimple.so")
 echo ".dynamic before: $debugTag"
 if ! echo "$debugTag" | grep -q DEBUG; then
     echo "failed --add-debug-tag test. Expected line with (DEBUG), got: $debugTag"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/add-rpath.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-mkdir -p ${SCRATCH}/libsA
-mkdir -p ${SCRATCH}/libsB
-
-cp main ${SCRATCH}/
-cp libfoo.so ${SCRATCH}/libsA/
-cp libbar.so ${SCRATCH}/libsB/
-
-../src/patchelf --force-rpath --add-rpath $(pwd)/${SCRATCH}/libsA ${SCRATCH}/main
-../src/patchelf --force-rpath --add-rpath $(pwd)/${SCRATCH}/libsB ${SCRATCH}/main
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+mkdir -p "${SCRATCH}"/libsA
+mkdir -p "${SCRATCH}"/libsB
+
+cp main "${SCRATCH}"/
+cp libfoo.so "${SCRATCH}/libsA/"
+cp libbar.so "${SCRATCH}/libsB/"
+
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/main")
+if test -z "$oldRPath"; then oldRPath="/oops"; fi
+../src/patchelf --force-rpath --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/main"
 
 if test "$(uname)" = FreeBSD; then
-    export LD_LIBRARY_PATH=$(pwd)/${SCRATCH}/libsB
+    LD_LIBRARY_PATH="$(pwd)/${SCRATCH}/libsB"
+    export LD_LIBRARY_PATH
 fi
 
 exitCode=0
-(cd ${SCRATCH} && ./main) || exitCode=$?
+(cd "${SCRATCH}" && ./main) || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/big-dynstr.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath-rel-map.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-mkdir -p ${SCRATCH}/libsA
-mkdir -p ${SCRATCH}/libsB
-
-cp big-dynstr ${SCRATCH}/
-cp libfoo.so ${SCRATCH}/libsA/
-cp libbar.so ${SCRATCH}/libsB/
+SCRATCH=scratch/$(basename "$0" .sh)
+OBJDUMP=${OBJDUMP:-objdump}
+OBJCOPY=${OBJCOPY:-objcopy}
+
+if ! $OBJDUMP -p main | grep -q MIPS_RLD_MAP_REL; then
+    echo "No MIPS_RLD_MAP_REL dynamic section entry, skipping"
+    exit 77
+fi
+
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+mkdir -p "${SCRATCH}/libsA"
+mkdir -p "${SCRATCH}/libsB"
+
+cp main "${SCRATCH}/"
+cp libfoo.so "${SCRATCH}/libsA/"
+cp libbar.so "${SCRATCH}/libsB/"
 
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/big-dynstr)
+# break the main executable by removing .rld_map section
+${OBJCOPY} --remove-section .rld_map "${SCRATCH}/main"
+
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/main")
 if test -z "$oldRPath"; then oldRPath="/oops"; fi
-../src/patchelf --force-rpath --set-rpath $oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB ${SCRATCH}/big-dynstr
+../src/patchelf --force-rpath --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/main"
 
 if test "$(uname)" = FreeBSD; then
-    export LD_LIBRARY_PATH=$(pwd)/${SCRATCH}/libsB
+    LD_LIBRARY_PATH=$(pwd)/"${SCRATCH}"/libsB
+    export LD_LIBRARY_PATH
 fi
 
 exitCode=0
-cd ${SCRATCH} && ./big-dynstr || exitCode=$?
+
+(cd "${SCRATCH}" && ./main) || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/build-id.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/build-id.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 READELF=${READELF:-readelf}
 
 rm -rf "${SCRATCH}"
 mkdir -p "${SCRATCH}"
 
 cp libbuildid.so "${SCRATCH}/"
 
 long_rpath="AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"
 
 ../src/patchelf \
   --set-rpath "$long_rpath" "${SCRATCH}/libbuildid.so"
 
 # older readelf versions do not recognize build id, but we can grep by constant
+LANG=en_US
 ${READELF} -n "${SCRATCH}/libbuildid.so" |  grep -q -F -e 'Build ID' -e 'Unknown note type: (0x00000003)'
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/contiguous-note-sections.s` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/contiguous-note-sections.s`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/empty-note` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/empty-note`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64/libtest.so` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64/libtest.so`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64/main` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64/main`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64le/libtest.so` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64le/libtest.so`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/endianness/ppc64le/main` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/endianness/ppc64le/main`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/force-rpath.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/force-rpath.sh`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 OBJDUMP=${OBJDUMP:-objdump}
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
 SCRATCHFILE=${SCRATCH}/libfoo.so
-cp libfoo.so $SCRATCHFILE
+cp libfoo.so "$SCRATCHFILE"
 
 doit() {
-    echo patchelf $*
-    ../src/patchelf $* $SCRATCHFILE
+    set +x
+    ../src/patchelf "$@" "$SCRATCHFILE"
+    set -x
 }
 
 expect() {
-    out=$(echo $($OBJDUMP -x $SCRATCHFILE | grep PATH))
+    out=$("$OBJDUMP" -x "$SCRATCHFILE" | grep PATH || true)
 
-    if [ "$out" != "$*" ]; then
-        echo "Expected '$*' but got '$out'"
-        exit 1
-    fi
+    for i in $out; do
+        if [ "$i" != "$1" ]; then
+            echo "Expected '$*' but got '$out'"
+            exit 1
+        fi
+        shift
+    done
 }
 
 doit --remove-rpath
-expect
+expect ""
 doit --set-rpath foo
 expect RUNPATH foo
 doit --force-rpath --set-rpath foo
 expect RPATH foo
 doit --force-rpath --set-rpath bar
 expect RPATH bar
 doit --remove-rpath
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shdr-name` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shdr-name`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-nonterm` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-nonterm`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-zero` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf/invalid-shrstrtab-zero`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/invalid-elf.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/invalid-elf.sh`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # Usage: killed_by_signal $?
 #
 # Returns true if the exit code indicates that the program was killed
 # by a signal. This works because the exit code of processes that were
 # killed by a signal is 128 plus the signal number.
 killed_by_signal() {
-    [ $1 -ge 128 ]
+    [ "$1" -ge 128 ]
 }
 
 
 # The directory containing all our input files.
-TEST_DIR=$(dirname $(readlink -f $0))/invalid-elf
+TEST_DIR=$(dirname "$(readlink -f "$0")")/invalid-elf
 
 # Each test case is listed here. The names should roughly indicate
 # what makes the given ELF file invalid.
 TEST_CASES="invalid-shrstrtab-idx invalid-shrstrtab-size invalid-shrstrtab-zero
             invalid-shrstrtab-nonterm invalid-shdr-name invalid-phdr-offset"
 
 FAILED_TESTS=""
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-pie-powerpc.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-pie-powerpc.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #! /bin/sh -e
 set -x
 SCRATCH=scratch/no-rpath-pie-powerpc
 READELF=${READELF:-readelf}
 
-no_rpath_bin="${srcdir}/no-rpath-prebuild/no-rpath-pie-powerpc"
+no_rpath_bin="${srcdir:?}/no-rpath-prebuild/no-rpath-pie-powerpc"
 
-if [ ! -f $no_rpath_bin ]; then
-  echo "no 'no-rpath' binary for '$ARCH' in '${srcdir}/no-rpath-prebuild'"
+if [ ! -f "$no_rpath_bin" ]; then
+  echo "no 'no-rpath' binary for '$ARCH' in '${srcdir:?}/no-rpath-prebuild'"
   exit 1
 fi
 
 rm -rf ${SCRATCH}
 mkdir -p ${SCRATCH}
 
-cp $no_rpath_bin ${SCRATCH}/no-rpath
+cp "$no_rpath_bin" ${SCRATCH}/no-rpath
 
 oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/no-rpath)
 if test -n "$oldRPath"; then exit 1; fi
 ../src/patchelf \
   --set-interpreter "$(../src/patchelf --print-interpreter ../src/patchelf)" \
   --set-rpath /foo:/bar:/xxxxxxxxxxxxxxx ${SCRATCH}/no-rpath
 
@@ -26,15 +26,15 @@
     echo "incomplete RPATH"
     exit 1
 fi
 
 # Tests for powerpc PIE endianness regressions
 readelfData=$(${READELF} -l ${SCRATCH}/no-rpath 2>&1)
 
-if [ $(echo "$readelfData" | grep --count "PHDR") != 1 ]; then
+if [ "$(echo "$readelfData" | grep -c "PHDR")" != 1 ]; then
   # Triggered if PHDR errors appear on stderr
   echo "Unexpected number of occurences of PHDR in readelf results"
   exit 1
 fi
 
 virtAddr=$(echo "$readelfData" | grep "PHDR" | awk '{print $3}')
 if [ "$virtAddr" != "0x00000034" ]; then
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-amd64` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-amd64`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armel` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armel`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armhf` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-armhf`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-hurd-i386` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-hurd-i386`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-i386` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-i386`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-ia64` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-ia64`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-amd64` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-amd64`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-i386` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-kfreebsd-i386`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mips` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mips`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mipsel` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-mipsel`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-pie-powerpc` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-pie-powerpc`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-powerpc` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-powerpc`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-s390` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-s390`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sh4` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sh4`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sparc` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild/no-rpath-sparc`

 * *Files identical despite different names*

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath-prebuild.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath-prebuild.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #! /bin/sh -e
 set -x
 ARCH="$1"
 PAGESIZE=4096
 
 if [ -z "$ARCH" ]; then
-  ARCH=$(basename $0 .sh | sed -e 's/^no-rpath-//')
+  ARCH=$(basename "$0" .sh | sed -e 's/^no-rpath-//')
 fi
 
 SCRATCH=scratch/no-rpath-$ARCH
 
-if [ -z "$ARCH" ] || [ $ARCH = prebuild ] ; then
+if [ -z "$ARCH" ] || [ "$ARCH" = prebuild ] ; then
   echo "Architecture required"
   exit 1
 fi
 
-no_rpath_bin="${srcdir}/no-rpath-prebuild/no-rpath-$ARCH"
+no_rpath_bin="${srcdir:?}/no-rpath-prebuild/no-rpath-$ARCH"
 
-if [ ! -f $no_rpath_bin ]; then
-  echo "no 'no-rpath' binary for '$ARCH' in '${srcdir}/no-rpath-prebuild'"
+if [ ! -f "$no_rpath_bin" ]; then
+  echo "no 'no-rpath' binary for '$ARCH' in '${srcdir:?}/no-rpath-prebuild'"
   exit 1
 fi
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp $no_rpath_bin ${SCRATCH}/no-rpath
+cp "$no_rpath_bin" "${SCRATCH}"/no-rpath
 
-oldRPath=$(../src/patchelf --page-size ${PAGESIZE} --print-rpath ${SCRATCH}/no-rpath)
+oldRPath=$(../src/patchelf --page-size "${PAGESIZE}" --print-rpath "${SCRATCH}/no-rpath")
 if test -n "$oldRPath"; then exit 1; fi
-../src/patchelf --page-size ${PAGESIZE} \
-  --set-interpreter "$(../src/patchelf --page-size ${PAGESIZE} --print-interpreter ../src/patchelf)" \
-  --set-rpath /foo:/bar:/xxxxxxxxxxxxxxx ${SCRATCH}/no-rpath
+../src/patchelf --page-size "${PAGESIZE}" \
+  --set-interpreter "$(../src/patchelf --page-size "${PAGESIZE}" --print-interpreter ../src/patchelf)" \
+  --set-rpath /foo:/bar:/xxxxxxxxxxxxxxx "${SCRATCH}"/no-rpath
 
-newRPath=$(../src/patchelf --page-size ${PAGESIZE} --print-rpath ${SCRATCH}/no-rpath)
+newRPath=$(../src/patchelf --page-size "${PAGESIZE}" --print-rpath "${SCRATCH}/no-rpath")
 if ! echo "$newRPath" | grep -q '/foo:/bar'; then
     echo "incomplete RPATH"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/no-rpath.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/no-rpath.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp no-rpath ${SCRATCH}/
+cp no-rpath "${SCRATCH}/"
 
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/no-rpath)
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/no-rpath")
 if test -n "$oldRPath"; then exit 1; fi
 ../src/patchelf \
   --set-interpreter "$(../src/patchelf --print-interpreter ../src/patchelf)" \
-  --set-rpath /foo:/bar:/xxxxxxxxxxxxxxx ${SCRATCH}/no-rpath
+  --set-rpath /foo:/bar:/xxxxxxxxxxxxxxx "${SCRATCH}/no-rpath"
 
-newRPath=$(../src/patchelf --print-rpath ${SCRATCH}/no-rpath)
+newRPath=$(../src/patchelf --print-rpath "${SCRATCH}/no-rpath")
 if ! echo "$newRPath" | grep -q '/foo:/bar'; then
     echo "incomplete RPATH"
     exit 1
 fi
 
-cd ${SCRATCH} && ./no-rpath
+cd "${SCRATCH}" && ./no-rpath
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/phdr-corruption.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/phdr-corruption.sh`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /bin/sh -e
 
 PATCHELF="../src/patchelf"
 SONAME="phdr-corruption.so"
-SCRATCH="scratch/$(basename $0 .sh)"
+SCRATCH="scratch/$(basename "$0" .sh)"
 SCRATCH_SO="${SCRATCH}/${SONAME}"
 READELF=${READELF:-readelf}
 
 rm -rf "${SCRATCH}"
 mkdir -p "${SCRATCH}"
 cp "${SONAME}" "${SCRATCH}"
 
 "${PATCHELF}" --set-rpath "$(pwd)" "${SCRATCH_SO}"
 
 # Check for PT_PHDR entry VirtAddr corruption
 readelfData=$(${READELF} -l "${SCRATCH_SO}" 2>&1)
 
-if [ $(echo "$readelfData" | grep --count "PHDR") != 1 ]; then
+if [ "$(echo "$readelfData" | grep -c "PHDR")" != 1 ]; then
   # Triggered if PHDR errors appear on stderr
   echo "ERROR: Unexpected number of occurences of PHDR in readelf results!"
   exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/plain-needed.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/plain-needed.sh`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #! /bin/sh
 set -e
 
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 MAIN_ELF="${SCRATCH}/main"
 
 PATCHELF="../src/patchelf"
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-cp main ${SCRATCH}/
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+cp main "${SCRATCH}"/
 
 echo "Confirming main requires libfoo"
 ${PATCHELF} --print-needed "${MAIN_ELF}" | grep -q libfoo.so
 
 echo "Testing --add-needed functionality"
 ${PATCHELF} --add-needed bar.so "${MAIN_ELF}"
 ${PATCHELF} --print-needed "${MAIN_ELF}" | grep -q bar.so
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/replace-add-needed.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/replace-add-needed.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 PATCHELF=$(readlink -f "../src/patchelf")
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp simple ${SCRATCH}/
-cp libfoo.so ${SCRATCH}/
-cp libbar.so ${SCRATCH}/
+cp simple "${SCRATCH}"/
+cp libfoo.so "${SCRATCH}"/
+cp libbar.so "${SCRATCH}"/
 
-cd ${SCRATCH}
+cd "${SCRATCH}"
 
 libcldd=$(ldd ./simple | awk '/ => / { print $3 }' | grep -E "(libc(-[0-9.]*)*.so|ld-musl)")
 
 # We have to set the soname on these libraries
 ${PATCHELF} --set-soname libbar.so ./libbar.so
 
 # Add a libbar.so so we can rewrite it later
 ${PATCHELF} --add-needed libbar.so ./simple
 
 # Make the NEEDED in libfoo the same as simple
 # This is a current "bug" in musl
 # https://www.openwall.com/lists/musl/2021/12/21/1
-${PATCHELF} --replace-needed libbar.so $(readlink -f ./libbar.so) ./libfoo.so
+${PATCHELF} --replace-needed libbar.so "$(readlink -f ./libbar.so)" ./libfoo.so
 
-${PATCHELF} --replace-needed libc.so.6 ${libcldd} \
-            --replace-needed libbar.so $(readlink -f ./libbar.so) \
-            --add-needed $(readlink -f ./libfoo.so) \
+${PATCHELF} --replace-needed libc.so.6 "${libcldd}" \
+            --replace-needed libbar.so "$(readlink -f ./libbar.so)" \
+            --add-needed "$(readlink -f ./libfoo.so)" \
             ./simple
 
 exitCode=0
 ./simple || exitCode=$?
 
 if test "$exitCode" != 0; then
     ldd ./simple
     exit 1
-fi
+fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/replace-needed.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/replace-needed.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-oldNeeded=$(../src/patchelf --print-needed big-dynstr)
 oldLibc=$(../src/patchelf --print-needed big-dynstr | grep -v 'foo\.so')
-../src/patchelf --output ${SCRATCH}/big-needed --replace-needed ${oldLibc} long_long_very_long_libc.so.6 --replace-needed libfoo.so lf.so big-dynstr
+../src/patchelf --output "${SCRATCH}/big-needed" --replace-needed "${oldLibc}" long_long_very_long_libc.so.6 --replace-needed libfoo.so lf.so big-dynstr
 
-if [ -z "$(../src/patchelf --print-needed ${SCRATCH}/big-needed | grep -Fx "long_long_very_long_libc.so.6")" ]; then
+if ! ../src/patchelf --print-needed "${SCRATCH}/big-needed" | grep -Fxq "long_long_very_long_libc.so.6"; then
 	echo "library long_long_very_long_libc.so.6 not found as NEEDED"
-	../src/patchelf --print-needed ${SCRATCH}/big-needed
+	../src/patchelf --print-needed "${SCRATCH}/big-needed"
 	exit 1
 fi
 
-if [ -z "$(../src/patchelf --print-needed ${SCRATCH}/big-needed | grep -Fx "lf.so")" ]; then
+if ! ../src/patchelf --print-needed "${SCRATCH}/big-needed" | grep -Fxq "lf.so"; then
 	echo "library lf.so not found as NEEDED"
-	../src/patchelf --print-needed ${SCRATCH}/big-needed
+	../src/patchelf --print-needed "${SCRATCH}/big-needed"
 	exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/set-interpreter-long.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/set-interpreter-long.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
 ./simple
 
 oldInterpreter=$(../src/patchelf --print-interpreter ./simple)
 echo "current interpreter is $oldInterpreter"
 
 if test "$(uname)" = Linux; then
     echo "running with explicit interpreter..."
     "$oldInterpreter" ./simple
 fi
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-newInterpreter=$(pwd)/${SCRATCH}/iiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiii
-cp simple ${SCRATCH}/
-../src/patchelf --set-interpreter "$newInterpreter" ${SCRATCH}/simple
+newInterpreter="$(pwd)/${SCRATCH}/iiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiii"
+cp simple "${SCRATCH}/"
+../src/patchelf --set-interpreter "$newInterpreter" "${SCRATCH}/simple"
 
 echo "running with missing interpreter..."
-if ${SCRATCH}/simple; then
+if "${SCRATCH}"/simple; then
     echo "simple works, but it shouldn't"
     exit 1
 fi
 
 echo "running with new interpreter..."
 ln -s "$oldInterpreter" "$newInterpreter"
-${SCRATCH}/simple
+"${SCRATCH}"/simple
 
 if test "$(uname)" = Linux; then
     echo "running with explicit interpreter..."
-    "$oldInterpreter" ${SCRATCH}/simple
+    "$oldInterpreter" "${SCRATCH}/simple"
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/set-rpath-library.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/set-rpath-library.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
 if test "$(uname)" = FreeBSD; then
     echo "skipping on FreeBSD"
-    exit 0
+    exit 77
 fi
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-mkdir -p ${SCRATCH}/libsA
-mkdir -p ${SCRATCH}/libsB
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+mkdir -p "${SCRATCH}/libsA"
+mkdir -p "${SCRATCH}/libsB"
+
+cp main-scoped "${SCRATCH}/"
+cp libfoo-scoped.so "${SCRATCH}/libsA/"
+cp libbar-scoped.so "${SCRATCH}/libsB/"
+cp liboveralign.so "${SCRATCH}/"
 
-cp main-scoped ${SCRATCH}/
-cp libfoo-scoped.so ${SCRATCH}/libsA/
-cp libbar-scoped.so ${SCRATCH}/libsB/
-
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/main-scoped)
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}"/main-scoped)
 if test -z "$oldRPath"; then oldRPath="/oops"; fi
-../src/patchelf --set-rpath $oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB ${SCRATCH}/main-scoped
+../src/patchelf --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/main-scoped"
 
 # "main" contains libbar in its RUNPATH, but that's ignored when
 # resolving libfoo.  So libfoo won't find libbar and this will fail.
 exitCode=0
-(cd ${SCRATCH} && ./main-scoped) || exitCode=$?
+(cd "${SCRATCH}" && ./main-scoped) || exitCode=$?
 
 if test "$exitCode" = 46; then
     echo "expected failure"
 fi
 
 # So set an RUNPATH on libfoo as well.
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/libsA/libfoo-scoped.so)
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/libsA/libfoo-scoped.so")
 if test -z "$oldRPath"; then oldRPath="/oops"; fi
-../src/patchelf --set-rpath $oldRPath:$(pwd)/${SCRATCH}/libsB ${SCRATCH}/libsA/libfoo-scoped.so
+../src/patchelf --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/libsA/libfoo-scoped.so"
 
 exitCode=0
-(cd ${SCRATCH} && ./main-scoped) || exitCode=$?
+(cd "${SCRATCH}" && ./main-scoped) || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
 
 # Remove the libbar PATH from main using --shrink-rpath.
-../src/patchelf --shrink-rpath ${SCRATCH}/main-scoped
-if ../src/patchelf --print-rpath ${SCRATCH}/main-scoped | grep /libsB; then
+../src/patchelf --shrink-rpath "${SCRATCH}/main-scoped"
+if ../src/patchelf --print-rpath "${SCRATCH}/main-scoped" | grep /libsB; then
     echo "shrink failed"
     exit 1
 fi
 
 # And it should still run.
 exitCode=0
-(cd ${SCRATCH} && ./main-scoped) || exitCode=$?
+(cd "${SCRATCH}" && ./main-scoped) || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
+
+# ALL loads should have the same alignment
+lib="${SCRATCH}/liboveralign.so"
+../src/patchelf --set-rpath "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx" "$lib"
+num_alignments=$(${READELF} -W -l "${lib}"  | awk '/LOAD/ { print $NF }' | sort -u | wc -l)
+echo "$num_alignments"
+if test "${num_alignments}" -ne "1"; then
+    exit 1
+fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/set-rpath.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/output-flag.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-mkdir -p ${SCRATCH}/libsA
-mkdir -p ${SCRATCH}/libsB
-
-cp main ${SCRATCH}/
-cp libfoo.so ${SCRATCH}/libsA/
-cp libbar.so ${SCRATCH}/libsB/
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+mkdir -p "${SCRATCH}/libsA"
+mkdir -p "${SCRATCH}/libsB"
+
+cp main "${SCRATCH}"/
+cp libfoo.so "${SCRATCH}/libsA/"
+cp libbar.so "${SCRATCH}/libsB/"
 
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/main)
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/main")
 if test -z "$oldRPath"; then oldRPath="/oops"; fi
-../src/patchelf --force-rpath --set-rpath $oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB ${SCRATCH}/main
+
+../src/patchelf --force-rpath --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/main" --output "${SCRATCH}/main2"
+# make sure it copies even when there is nothing to do (because rpath is already set)
+../src/patchelf --force-rpath --set-rpath "$oldRPath:$(pwd)/${SCRATCH}/libsA:$(pwd)/${SCRATCH}/libsB" "${SCRATCH}/main2" --output "${SCRATCH}/main3"
 
 if test "$(uname)" = FreeBSD; then
-    export LD_LIBRARY_PATH=$(pwd)/${SCRATCH}/libsB
+    LD_LIBRARY_PATH="$(pwd)/${SCRATCH}/libsB"
+    export LD_LIBRARY_PATH
+fi
+
+exitCode=0
+(cd "${SCRATCH}" && ./main2) || exitCode=$?
+
+if test "$exitCode" != 46; then
+    echo "bad exit code!"
+    exit 1
 fi
 
 exitCode=0
-(cd ${SCRATCH} && ./main) || exitCode=$?
+(cd "${SCRATCH}" && ./main3) || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/shrink-rpath-with-allowed-prefixes.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/shrink-rpath-with-allowed-prefixes.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-mkdir -p ${SCRATCH}/libsA
-mkdir -p ${SCRATCH}/libsB
-
-cp main ${SCRATCH}/
-cp libfoo.so libbar.so ${SCRATCH}/libsA/
-cp libfoo.so libbar.so ${SCRATCH}/libsB/
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+mkdir -p "${SCRATCH}/libsA"
+mkdir -p "${SCRATCH}/libsB"
+
+cp main "${SCRATCH}"/
+cp libfoo.so libbar.so "${SCRATCH}/libsA/"
+cp libfoo.so libbar.so "${SCRATCH}/libsB/"
 
-oldRPath=$(../src/patchelf --print-rpath ${SCRATCH}/main)
+oldRPath=$(../src/patchelf --print-rpath "${SCRATCH}/main")
 if test -z "$oldRPath"; then oldRPath="/oops"; fi
 pathA="$(pwd)/${SCRATCH}/libsA"
 pathB="$(pwd)/${SCRATCH}/libsB"
-../src/patchelf --force-rpath --set-rpath $oldRPath:$pathA:$pathB ${SCRATCH}/main
+../src/patchelf --force-rpath --set-rpath "$oldRPath:$pathA:$pathB" "${SCRATCH}/main"
 
-cp ${SCRATCH}/main ${SCRATCH}/mainA
-cp ${SCRATCH}/main ${SCRATCH}/mainB
+cp "${SCRATCH}"/main "${SCRATCH}/mainA"
+cp "${SCRATCH}"/main "${SCRATCH}/mainB"
 
-../src/patchelf --shrink-rpath ${SCRATCH}/main
-../src/patchelf --shrink-rpath --allowed-rpath-prefixes $oldRPath:$pathA ${SCRATCH}/mainA
-../src/patchelf --shrink-rpath --allowed-rpath-prefixes $oldRPath:$pathB ${SCRATCH}/mainB
+../src/patchelf --shrink-rpath "${SCRATCH}/main"
+../src/patchelf --shrink-rpath --allowed-rpath-prefixes "$oldRPath:$pathA" "${SCRATCH}/mainA"
+../src/patchelf --shrink-rpath --allowed-rpath-prefixes "$oldRPath:$pathB" "${SCRATCH}/mainB"
 
 check() {
     exe=$1
     mustContain=$2
     mustNotContain=$3
 
-    rpath=$(../src/patchelf --print-rpath $exe)
+    rpath=$(../src/patchelf --print-rpath "$exe")
     echo "RPATH of $exe after: $rpath"
 
-    if ! echo "$rpath" | grep -q $mustContain; then
+    if ! echo "$rpath" | grep -q "$mustContain"; then
         echo "RPATH didn't contain '$mustContain' when it should have"
         exit 1
     fi
 
-    if echo "$rpath" | grep -q $mustNotContain; then
+    if echo "$rpath" | grep -q "$mustNotContain"; then
         echo "RPATH contained '$mustNotContain' when it shouldn't have"
         exit 1
     fi
 }
 
-check ${SCRATCH}/main  $pathA $pathB
-check ${SCRATCH}/mainA $pathA $pathB
-check ${SCRATCH}/mainB $pathB $pathA
+check "${SCRATCH}/main"  "$pathA" "$pathB"
+check "${SCRATCH}/mainA" "$pathA" "$pathB"
+check "${SCRATCH}/mainB" "$pathB" "$pathA"
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/shrink-rpath.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/shrink-rpath.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
 rpath=$(../src/patchelf --print-rpath ./libbar.so)
 echo "RPATH before: $rpath"
 if ! echo "$rpath" | grep -q /no-such-path; then
     echo "incomplete RPATH"
     exit 1
 fi
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
-cp libbar.so ${SCRATCH}/
-../src/patchelf --shrink-rpath ${SCRATCH}/libbar.so
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
+cp libbar.so "${SCRATCH}"/
+../src/patchelf --shrink-rpath "${SCRATCH}/libbar.so"
 
-rpath=$(../src/patchelf --print-rpath ${SCRATCH}/libbar.so)
+rpath=$(../src/patchelf --print-rpath "${SCRATCH}/libbar.so")
 echo "RPATH after: $rpath"
 if echo "$rpath" | grep -q /no-such-path; then
     echo "RPATH not shrunk"
     exit 1
 fi
 
-cp libfoo.so ${SCRATCH}/
+cp libfoo.so "${SCRATCH}/"
 
 exitCode=0
-cd ${SCRATCH} && LD_LIBRARY_PATH=. ../../main || exitCode=$?
+cd "${SCRATCH}" && LD_LIBRARY_PATH=. ../../main || exitCode=$?
 
 if test "$exitCode" != 46; then
     echo "bad exit code!"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/soname.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/soname.sh`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp libsimple.so ${SCRATCH}/
+cp libsimple.so "${SCRATCH}/"
 
 # set an initial DT_SONAME entry
-../src/patchelf --set-soname libsimple.so.1.0 ${SCRATCH}/libsimple.so
-newSoname=$(../src/patchelf --print-soname ${SCRATCH}/libsimple.so)
+../src/patchelf --set-soname libsimple.so.1.0 "${SCRATCH}/libsimple.so"
+newSoname=$(../src/patchelf --print-soname "${SCRATCH}/libsimple.so")
 if test "$newSoname" != libsimple.so.1.0; then
     echo "failed --set-soname test. Expected newSoname: libsimple.so.1.0, got: $newSoname"
     exit 1
 fi
 
 # print DT_SONAME
-soname=$(../src/patchelf --print-soname ${SCRATCH}/libsimple.so)
+soname=$(../src/patchelf --print-soname "${SCRATCH}/libsimple.so")
 if test "$soname" != libsimple.so.1.0; then
     echo "failed --print-soname test. Expected soname: libsimple.so.1.0, got: $soname"
     exit 1
 fi
 
 # replace DT_SONAME entry
-../src/patchelf --set-soname libsimple.so.1.1 ${SCRATCH}/libsimple.so
-newSoname=$(../src/patchelf --print-soname ${SCRATCH}/libsimple.so)
+../src/patchelf --set-soname libsimple.so.1.1 "${SCRATCH}/libsimple.so"
+newSoname=$(../src/patchelf --print-soname "${SCRATCH}/libsimple.so")
 if test "$newSoname" != libsimple.so.1.1; then
     echo "failed --set-soname test. Expected newSoname: libsimple.so.1.1, got: $newSoname"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf-upstream/tests/too-many-strtab.sh` & `patchelf-0.18.0.0/src/patchelf-upstream/tests/too-many-strtab.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #! /bin/sh -e
-SCRATCH=scratch/$(basename $0 .sh)
+SCRATCH=scratch/$(basename "$0" .sh)
 
-rm -rf ${SCRATCH}
-mkdir -p ${SCRATCH}
+rm -rf "${SCRATCH}"
+mkdir -p "${SCRATCH}"
 
-cp libtoomanystrtab.so ${SCRATCH}/
+cp libtoomanystrtab.so "${SCRATCH}"/
 
 # Set a RUNPATH on the library
-../src/patchelf --set-rpath '$ORIGIN' ${SCRATCH}/libtoomanystrtab.so
+../src/patchelf --set-rpath "\$ORIGIN" "${SCRATCH}/libtoomanystrtab.so"
 
 # Check that patchelf is able to patch it again without crashing. Previously,
 # it will wrongly identify the lib as a static object because there was no
 # .dynamic section
 exitCode=0
-(../src/patchelf --set-rpath '$ORIGIN' ${SCRATCH}/libtoomanystrtab.so) || exitCode=$?
+(../src/patchelf --set-rpath "\$ORIGIN" "${SCRATCH}/libtoomanystrtab.so") || exitCode=$?
 if test "$exitCode" != 0; then
     echo "bad exit code!"
     exit 1
 fi
```

### Comparing `patchelf-0.17.2.1/src/patchelf.egg-info/PKG-INFO` & `patchelf-0.18.0.0/src/patchelf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchelf
-Version: 0.17.2.1
+Version: 0.18.0.0
 Summary: A small utility to modify the dynamic linker and RPATH of ELF executables.
 Home-page: https://github.com/NixOS/patchelf
 Maintainer: Matthieu Darbois
 Maintainer-email: mayeut@users.noreply.github.com
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://github.com/mayeut/patchelf-pypi
 Project-URL: Bug Tracker, https://github.com/mayeut/patchelf-pypi/issues
@@ -67,14 +67,17 @@
   +---------------+--------------------------+
   | Linux i686    | | manylinux1+            |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux aarch64 | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
+  | Linux armv7l  | | manylinux2014+         |
+  |               | | musllinux_1_1+         |
+  +---------------+--------------------------+
   | Linux ppc64le | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
   | Linux s390x   | | manylinux2014+         |
   |               | | musllinux_1_1+         |
   +---------------+--------------------------+
```

### Comparing `patchelf-0.17.2.1/src/patchelf.egg-info/SOURCES.txt` & `patchelf-0.18.0.0/src/patchelf.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/patchelf-upstream/default.nix
 src/patchelf-upstream/flake.lock
 src/patchelf-upstream/flake.nix
 src/patchelf-upstream/patchelf.1
 src/patchelf-upstream/patchelf.nix
 src/patchelf-upstream/patchelf.spec.in
 src/patchelf-upstream/version
+src/patchelf-upstream/completions/zsh/_patchelf
 src/patchelf-upstream/m4/ax_cxx_compile_stdcxx.m4
 src/patchelf-upstream/src/Makefile.am
 src/patchelf-upstream/src/elf.h
 src/patchelf-upstream/src/patchelf.cc
 src/patchelf-upstream/src/patchelf.h
 src/patchelf-upstream/tests/Makefile.am
 src/patchelf-upstream/tests/add-debug-tag.sh
@@ -48,34 +49,44 @@
 src/patchelf-upstream/tests/empty-note.sh
 src/patchelf-upstream/tests/endianness.sh
 src/patchelf-upstream/tests/foo.c
 src/patchelf-upstream/tests/force-rpath.sh
 src/patchelf-upstream/tests/grow-file.sh
 src/patchelf-upstream/tests/invalid-elf.sh
 src/patchelf-upstream/tests/main.c
+src/patchelf-upstream/tests/modify-execstack.sh
 src/patchelf-upstream/tests/no-dynamic-section.sh
 src/patchelf-upstream/tests/no-gnu-hash.sh
 src/patchelf-upstream/tests/no-rpath-pie-powerpc.sh
 src/patchelf-upstream/tests/no-rpath-prebuild.sh
 src/patchelf-upstream/tests/no-rpath.c
 src/patchelf-upstream/tests/no-rpath.sh
 src/patchelf-upstream/tests/output-flag.sh
+src/patchelf-upstream/tests/overlapping-segments-after-rounding
+src/patchelf-upstream/tests/overlapping-segments-after-rounding.sh
 src/patchelf-upstream/tests/phdr-corruption.ld
 src/patchelf-upstream/tests/phdr-corruption.sh
 src/patchelf-upstream/tests/plain-fail.sh
 src/patchelf-upstream/tests/plain-needed.sh
 src/patchelf-upstream/tests/plain-run.sh
+src/patchelf-upstream/tests/print-execstack.sh
+src/patchelf-upstream/tests/rename-dynamic-symbols.sh
+src/patchelf-upstream/tests/repeated-updates.sh
 src/patchelf-upstream/tests/replace-add-needed.sh
 src/patchelf-upstream/tests/replace-needed.sh
 src/patchelf-upstream/tests/set-empty-rpath.sh
 src/patchelf-upstream/tests/set-interpreter-long.sh
 src/patchelf-upstream/tests/set-interpreter-short.sh
 src/patchelf-upstream/tests/set-rpath-library.sh
 src/patchelf-upstream/tests/set-rpath-rel-map.sh
 src/patchelf-upstream/tests/set-rpath.sh
+src/patchelf-upstream/tests/shared-rpath.c
+src/patchelf-upstream/tests/shared-rpath.sh
+src/patchelf-upstream/tests/short-first-segment.gz
+src/patchelf-upstream/tests/short-first-segment.sh
 src/patchelf-upstream/tests/shrink-rpath-with-allowed-prefixes.sh
 src/patchelf-upstream/tests/shrink-rpath.sh
 src/patchelf-upstream/tests/simple.c
 src/patchelf-upstream/tests/soname.sh
 src/patchelf-upstream/tests/too-many-strtab.c
 src/patchelf-upstream/tests/too-many-strtab.sh
 src/patchelf-upstream/tests/too-many-strtab2.s
```

### Comparing `patchelf-0.17.2.1/tests/test_patchelf.py` & `patchelf-0.18.0.0/tests/test_patchelf.py`

 * *Files identical despite different names*

