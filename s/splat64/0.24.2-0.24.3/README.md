# Comparing `tmp/splat64-0.24.2.tar.gz` & `tmp/splat64-0.24.3.tar.gz`

## Comparing `splat64-0.24.2.tar` & `splat64-0.24.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0    50260 2020-02-02 00:00:00.000000 splat64-0.24.2/CHANGELOG.md
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 splat64-0.24.2/create_config.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 splat64-0.24.2/mypy.ini
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 splat64-0.24.2/requirements.txt
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 splat64-0.24.2/split.py
--rwxr-xr-x   0        0        0    16295 2020-02-02 00:00:00.000000 splat64-0.24.2/test.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/black.yml
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/publish_docs_to_wiki.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/test_lib.yml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 splat64-0.24.2/.github/workflows/unit_tests.yml
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Adding-Symbols.md
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Advanced.md
--rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Configuration.md
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Examples.md
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/General-Workflow.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Home.md
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Quickstart.md
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/Segments.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 splat64-0.24.2/docs/VramClasses.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/py.typed
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/disassembler.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/disassembler_instance.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/disassembler_section.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/null_disassembler.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/disassembler/spimdisasm_disassembler.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/platforms/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/platforms/n64.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/platforms/ps2.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/platforms/psp.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/platforms/psx.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/scripts/__init__.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/scripts/capy.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/scripts/create_config.py
--rw-r--r--   0        0        0    20351 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/scripts/split.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/__init__.py
--rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/linker_entry.py
--rw-r--r--   0        0        0    25214 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/segment.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/__init__.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/asm.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/bin.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/bss.py
--rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/c.py
--rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/code.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/codesubsegment.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/cpp.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/data.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/databin.py
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/group.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/hasm.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/header.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/lib.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/pad.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/rdata.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/rodata.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/rodatabin.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/sbss.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/sdata.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/segment.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/common/textbin.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/asm.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ci.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ci4.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ci8.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/decompressor.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/gfx.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/hasm.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/header.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/i1.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/i4.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/i8.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ia16.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ia4.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ia8.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/img.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/ipl3.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/linker_offset.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/mio0.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/palette.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/rgba16.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/rgba32.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/rsp.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/segment.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/vtx.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/n64/yay0.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/asm.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/ctor.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/lit4.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/lit8.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/ps2/vtables.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psp/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psp/segment.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psx/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psx/asm.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psx/header.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/segtypes/psx/segment.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/__init__.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/cache_handler.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/color.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/compiler.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/log.py
--rw-r--r--   0        0        0    25718 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/options.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/palettes.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/progress_bar.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/relocs.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/statistics.py
--rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/symbols.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/vram_classes.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/n64/__init__.py
--rwxr-xr-x   0        0        0     1414 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/n64/find_code_length.py
--rwxr-xr-x   0        0        0     9046 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/n64/rominfo.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/psx/__init__.py
--rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 splat64-0.24.2/src/splat/util/psx/psxexeinfo.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 splat64-0.24.2/test/Dockerfile
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 splat64-0.24.2/test/README.md
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 splat64-0.24.2/test/test_gen_expected.sh
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/.gitignore
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/Makefile
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/dummy_ipl3.s
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/handwritten.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/header.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/main.c
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/.splache
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/undefined_funcs_auto.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/undefined_syms_auto.txt
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/handwritten.s
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/header.s
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/data/main.bss.s
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/data/main.data.s
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/nonmatchings/main/D_80000510.s
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/assets/dummy_ipl3.bin
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 splat64-0.24.2/test/basic_app/expected/src/main.c
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 splat64-0.24.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 splat64-0.24.2/LICENSE
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 splat64-0.24.2/README.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 splat64-0.24.2/pyproject.toml
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 splat64-0.24.2/PKG-INFO
+-rw-r--r--   0        0        0    50636 2020-02-02 00:00:00.000000 splat64-0.24.3/CHANGELOG.md
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 splat64-0.24.3/create_config.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 splat64-0.24.3/mypy.ini
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 splat64-0.24.3/requirements.txt
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 splat64-0.24.3/split.py
+-rwxr-xr-x   0        0        0    16295 2020-02-02 00:00:00.000000 splat64-0.24.3/test.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/publish_docs_to_wiki.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/test_lib.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 splat64-0.24.3/.github/workflows/unit_tests.yml
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Adding-Symbols.md
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Advanced.md
+-rw-r--r--   0        0        0    14136 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Configuration.md
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Examples.md
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/General-Workflow.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Home.md
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Quickstart.md
+-rw-r--r--   0        0        0    10615 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/Segments.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 splat64-0.24.3/docs/VramClasses.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/py.typed
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/disassembler.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/disassembler_instance.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/disassembler_section.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/null_disassembler.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/disassembler/spimdisasm_disassembler.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/platforms/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/platforms/n64.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/platforms/ps2.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/platforms/psp.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/platforms/psx.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/scripts/__init__.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/scripts/capy.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/scripts/create_config.py
+-rw-r--r--   0        0        0    20351 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/scripts/split.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/__init__.py
+-rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/linker_entry.py
+-rw-r--r--   0        0        0    25602 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/segment.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/__init__.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/asm.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/bin.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/bss.py
+-rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/c.py
+-rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/code.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/codesubsegment.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/cpp.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/data.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/databin.py
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/group.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/hasm.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/header.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/lib.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/pad.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/rdata.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/rodata.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/rodatabin.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/sbss.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/sdata.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/segment.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/common/textbin.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/asm.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ci.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ci4.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ci8.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/decompressor.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/gfx.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/hasm.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/header.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/i1.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/i4.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/i8.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ia16.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ia4.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ia8.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/img.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/ipl3.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/linker_offset.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/mio0.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/palette.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/rgba16.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/rgba32.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/rsp.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/segment.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/vtx.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/n64/yay0.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/asm.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/ctor.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/lit4.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/lit8.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/ps2/vtables.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psp/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psp/segment.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psx/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psx/asm.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psx/header.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/segtypes/psx/segment.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/cache_handler.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/color.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/compiler.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/log.py
+-rw-r--r--   0        0        0    25942 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/options.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/palettes.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/progress_bar.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/relocs.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/statistics.py
+-rw-r--r--   0        0        0    26846 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/symbols.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/vram_classes.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/n64/__init__.py
+-rwxr-xr-x   0        0        0     1414 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/n64/find_code_length.py
+-rwxr-xr-x   0        0        0     9046 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/n64/rominfo.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/psx/__init__.py
+-rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 splat64-0.24.3/src/splat/util/psx/psxexeinfo.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 splat64-0.24.3/test/Dockerfile
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 splat64-0.24.3/test/README.md
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 splat64-0.24.3/test/test_gen_expected.sh
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/.gitignore
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/Makefile
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/dummy_ipl3.s
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/handwritten.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/header.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/main.c
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/.splache
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/undefined_funcs_auto.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/undefined_syms_auto.txt
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/handwritten.s
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/header.s
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/data/main.bss.s
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/data/main.data.s
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/nonmatchings/main/D_80000510.s
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/assets/dummy_ipl3.bin
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 splat64-0.24.3/test/basic_app/expected/src/main.c
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 splat64-0.24.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 splat64-0.24.3/LICENSE
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 splat64-0.24.3/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 splat64-0.24.3/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 splat64-0.24.3/PKG-INFO
```

### Comparing `splat64-0.24.2/CHANGELOG.md` & `splat64-0.24.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # splat Release Notes
 
+### 0.24.3
+
+* New yaml option: `ld_align_segment_start`
+  * Allows specifying an alignment for the start of all the segments.
+  * The alignment can be overriden or disabled per segment too.
+* Add `visibility` attribute to symbols.
+  * Allows to specify if a symbol should be declared as `local`, `weak`, etc in the disassembly.
+* `spimdisasm` 1.26.0 or above is now required
+
 ### 0.24.2
 
 * Fixed create_config to replace "/" in detected binary names with "_"
 
 ### 0.24.1
 
 * Tweak the disassembler's configuration for PSP platform to improve assembly analysis.
```

### Comparing `splat64-0.24.2/test.py` & `splat64-0.24.3/test.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/.github/workflows/mypy.yml` & `splat64-0.24.3/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/.github/workflows/publish_docs_to_wiki.yml` & `splat64-0.24.3/.github/workflows/publish_docs_to_wiki.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/.github/workflows/pypi.yml` & `splat64-0.24.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/.github/workflows/unit_tests.yml` & `splat64-0.24.3/.github/workflows/unit_tests.yml`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/Adding-Symbols.md` & `splat64-0.24.3/docs/Adding-Symbols.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/Configuration.md` & `splat64-0.24.3/docs/Configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -423,24 +423,34 @@
 
 It must be either an integer, which will be used as the parameter for the `FILL` statement, or `null`, which tells splat to not emit `FILL` statements.
 
 This behavior can be customized per segment too. See [ld_fill_value](Segments.md#ld_fill_value) on the Segments section.
 
 Defaults to 0.
 
-
 ### ld_bss_is_noload
 
 Allows to control if `bss` sections (and derivatived sections) will be put on a `NOLOAD` segment on the generated linker script or not.
 
 Applies to all `bss` (`sbss`, `common`, `scommon`, etc) sections.
 
 Defaults to `True`, meaning `bss` sections will be put on `NOLOAD` segments.
 
 
+### ld_align_segment_start
+
+Specify that segments should be aligned before starting them.
+
+This option specifies the desired alignment value, or `null` if no aligment should be imposed on the segment start.
+
+This behavior can be customized per segment too. See [ld_align_segment_start](Segments.md#ld_align_segment_start) on the Segments section.
+
+Defaults to `null`.
+
+
 ### ld_align_segment_vram_end
 
 Allows to toggle aligning the `*_VRAM_END` linker symbol of each segment.
 
 Setting this to `True` will make the `*_VRAM_END` to be aligned to the configured alignment of the segment.
 
 Defaults to `True`.
```

### Comparing `splat64-0.24.2/docs/Examples.md` & `splat64-0.24.3/docs/Examples.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/General-Workflow.md` & `splat64-0.24.3/docs/General-Workflow.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/Home.md` & `splat64-0.24.3/docs/Home.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/Quickstart.md` & `splat64-0.24.3/docs/Quickstart.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/docs/Segments.md` & `splat64-0.24.3/docs/Segments.md`

 * *Files 9% similar despite different names*

```diff
@@ -351,14 +351,22 @@
 
 It must be either an integer, which will be used as the parameter for the `FILL` statement, or `null`, which tells splat to not emit a `FILL` statement for this segment.
 
 If not set, then the global configuration is used. See [ld_fill_value](Configuration.md#ld_fill_value) on the Configuration section.
 
 Defaults to the value of the global option.
 
+### `ld_align_segment_start`
+
+Specify the current segment should be aligned before starting it.
+
+This option specifies the desired alignment value, or `null` if no aligment should be imposed on the segment start.
+
+If not set, then the global configuration is used. See [ld_align_segment_start](Configuration.md#ld_align_segment_start) on the Configuration section.
+
 ### `subalign`
 
 Sub-alignment (in bytes) of sections.
 
 Only works on top-level segments
 
 `subalign` can be `null` to not force any specific alignment and use the built section's declared alignment instead.
```

### Comparing `splat64-0.24.2/docs/VramClasses.md` & `splat64-0.24.3/docs/VramClasses.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/__main__.py` & `splat64-0.24.3/src/splat/__main__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/disassembler/disassembler_instance.py` & `splat64-0.24.3/src/splat/disassembler/disassembler_instance.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/disassembler/disassembler_section.py` & `splat64-0.24.3/src/splat/disassembler/disassembler_section.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/disassembler/spimdisasm_disassembler.py` & `splat64-0.24.3/src/splat/disassembler/spimdisasm_disassembler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import rabbitizer
 from ..util import log, compiler, options
 from typing import Set
 
 
 class SpimdisasmDisassembler(disassembler.Disassembler):
     # This value should be kept in sync with the version listed on requirements.txt and pyproject.toml
-    SPIMDISASM_MIN = (1, 25, 0)
+    SPIMDISASM_MIN = (1, 26, 0)
 
     def configure(self):
         # Configure spimdisasm
         spimdisasm.common.GlobalConfig.PRODUCE_SYMBOLS_PLUS_OFFSET = True
         spimdisasm.common.GlobalConfig.TRUST_USER_FUNCTIONS = True
         spimdisasm.common.GlobalConfig.TRUST_JAL_FUNCTIONS = True
         spimdisasm.common.GlobalConfig.GLABEL_ASM_COUNT = False
```

### Comparing `splat64-0.24.2/src/splat/scripts/capy.py` & `splat64-0.24.3/src/splat/scripts/capy.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/scripts/create_config.py` & `splat64-0.24.3/src/splat/scripts/create_config.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/scripts/split.py` & `splat64-0.24.3/src/splat/scripts/split.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/linker_entry.py` & `splat64-0.24.3/src/splat/segtypes/linker_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,20 @@
                         f"\nError on linker script generation: section '{prev_entry}' not found.\n  Make sure the section '{prev_entry}' is listed on 'section_order' of the yaml options."
                     )
                 section_entries[prev_entry].append(entry)
             any_load = any_load or not entry.noload
             any_noload = any_noload or entry.noload
             prev_entry = entry.section_order_type
 
+        if segment.ld_align_segment_start:
+            self._write_symbol(
+                "__romPos", f"ALIGN(__romPos, 0x{segment.ld_align_segment_start:X})"
+            )
+            self._write_symbol(".", f"ALIGN(., 0x{segment.ld_align_segment_start:X})")
+
         seg_rom_start = get_segment_rom_start(seg_name)
         self._write_symbol(seg_rom_start, "__romPos")
 
         is_first = True
         if any_load:
             # Only emit normal segment if there's at least one normal entry
             self._write_segment_sections(
@@ -301,14 +307,20 @@
         for entry in reversed(entries):
             if (
                 entry.section_order_type in options.opts.section_order
                 and entry.section_order_type not in last_seen_sections.values()
             ):
                 last_seen_sections[entry] = entry.section_order_type
 
+        if segment.ld_align_segment_start:
+            self._write_symbol(
+                "__romPos", f"ALIGN(__romPos, 0x{segment.ld_align_segment_start:X})"
+            )
+            self._write_symbol(".", f"ALIGN(., 0x{segment.ld_align_segment_start:X})")
+
         seg_rom_start = get_segment_rom_start(seg_name)
         self._write_symbol(seg_rom_start, "__romPos")
 
         self._begin_segment(segment, seg_name, noload=False, is_first=True)
 
         i = 0
         for entry in entries:
@@ -355,14 +367,20 @@
         assert segments_path is not None
 
         seg_name = segment.get_cname()
 
         for sym, segs in max_vram_syms:
             self.write_max_vram_end_sym(sym, segs)
 
+        if segment.ld_align_segment_start:
+            self._write_symbol(
+                "__romPos", f"ALIGN(__romPos, 0x{segment.ld_align_segment_start:X})"
+            )
+            self._write_symbol(".", f"ALIGN(., 0x{segment.ld_align_segment_start:X})")
+
         seg_rom_start = get_segment_rom_start(seg_name)
         self._write_symbol(seg_rom_start, "__romPos")
 
         any_load = any(not e.noload for e in entries)
         is_first = True
         if any_load:
             # Only emit normal segment if there's at least one normal entry
```

### Comparing `splat64-0.24.2/src/splat/segtypes/segment.py` & `splat64-0.24.3/src/splat/segtypes/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,20 @@
     def parse_ld_fill_value(
         yaml: Union[dict, list], default: Optional[int]
     ) -> Optional[int]:
         if isinstance(yaml, dict) and "ld_fill_value" in yaml:
             return yaml["ld_fill_value"]
         return default
 
+    @staticmethod
+    def parse_ld_align_segment_start(yaml: Union[dict, list]) -> Optional[int]:
+        if isinstance(yaml, dict) and "ld_align_segment_start" in yaml:
+            return yaml["ld_align_segment_start"]
+        return options.opts.ld_align_segment_start
+
     def __init__(
         self,
         rom_start: Optional[int],
         rom_end: Optional[int],
         type: str,
         name: str,
         vram_start: Optional[int],
@@ -284,14 +290,18 @@
         self.linker_section: Optional[str] = self.parse_linker_section(yaml)
 
         # If not defined on the segment then default to the global option
         self.ld_fill_value: Optional[int] = self.parse_ld_fill_value(
             yaml, options.opts.ld_fill_value
         )
 
+        self.ld_align_segment_start: Optional[int] = self.parse_ld_align_segment_start(
+            yaml
+        )
+
         # True if this segment was generated based on auto_all_sections
         self.is_auto_all: bool = False
 
         if self.rom_start is not None and self.rom_end is not None:
             if self.rom_start > self.rom_end:
                 log.error(
                     f"Error: segments out of order - ({self.name} starts at 0x{self.rom_start:X}, but next segment starts at 0x{self.rom_end:X})"
```

### Comparing `splat64-0.24.2/src/splat/segtypes/common/__init__.py` & `splat64-0.24.3/src/splat/segtypes/common/__init__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/asm.py` & `splat64-0.24.3/src/splat/segtypes/common/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/bin.py` & `splat64-0.24.3/src/splat/segtypes/common/bin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/bss.py` & `splat64-0.24.3/src/splat/segtypes/common/bss.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/c.py` & `splat64-0.24.3/src/splat/segtypes/common/c.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/code.py` & `splat64-0.24.3/src/splat/segtypes/common/code.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/codesubsegment.py` & `splat64-0.24.3/src/splat/segtypes/common/codesubsegment.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/data.py` & `splat64-0.24.3/src/splat/segtypes/common/data.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/databin.py` & `splat64-0.24.3/src/splat/segtypes/common/databin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/group.py` & `splat64-0.24.3/src/splat/segtypes/common/group.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/hasm.py` & `splat64-0.24.3/src/splat/segtypes/common/hasm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/header.py` & `splat64-0.24.3/src/splat/segtypes/common/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/lib.py` & `splat64-0.24.3/src/splat/segtypes/common/lib.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/pad.py` & `splat64-0.24.3/src/splat/segtypes/common/pad.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/rodata.py` & `splat64-0.24.3/src/splat/segtypes/common/rodata.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/rodatabin.py` & `splat64-0.24.3/src/splat/segtypes/common/rodatabin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/common/textbin.py` & `splat64-0.24.3/src/splat/segtypes/common/textbin.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/__init__.py` & `splat64-0.24.3/src/splat/segtypes/n64/__init__.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/asm.py` & `splat64-0.24.3/src/splat/segtypes/n64/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/ci.py` & `splat64-0.24.3/src/splat/segtypes/n64/ci.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/decompressor.py` & `splat64-0.24.3/src/splat/segtypes/n64/decompressor.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/gfx.py` & `splat64-0.24.3/src/splat/segtypes/n64/gfx.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/hasm.py` & `splat64-0.24.3/src/splat/segtypes/n64/hasm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/header.py` & `splat64-0.24.3/src/splat/segtypes/n64/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/img.py` & `splat64-0.24.3/src/splat/segtypes/n64/img.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/linker_offset.py` & `splat64-0.24.3/src/splat/segtypes/n64/linker_offset.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/palette.py` & `splat64-0.24.3/src/splat/segtypes/n64/palette.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/n64/vtx.py` & `splat64-0.24.3/src/splat/segtypes/n64/vtx.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/ps2/asm.py` & `splat64-0.24.3/src/splat/segtypes/ps2/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/ps2/ctor.py` & `splat64-0.24.3/src/splat/segtypes/ps2/ctor.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/ps2/lit4.py` & `splat64-0.24.3/src/splat/segtypes/ps2/lit4.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/ps2/lit8.py` & `splat64-0.24.3/src/splat/segtypes/ps2/lit8.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/ps2/vtables.py` & `splat64-0.24.3/src/splat/segtypes/ps2/vtables.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/psx/asm.py` & `splat64-0.24.3/src/splat/segtypes/psx/asm.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/segtypes/psx/header.py` & `splat64-0.24.3/src/splat/segtypes/psx/header.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/cache_handler.py` & `splat64-0.24.3/src/splat/util/cache_handler.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/compiler.py` & `splat64-0.24.3/src/splat/util/compiler.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/log.py` & `splat64-0.24.3/src/splat/util/log.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/options.py` & `splat64-0.24.3/src/splat/util/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,16 @@
     segment_symbols_style: str
     # Specifies the starting offset for rom address symbols in the linker script.
     ld_rom_start: int
     # The value passed to the FILL statement on each segment. `None` disables using FILL statements on the linker script. Defaults to a fill value of 0.
     ld_fill_value: Optional[int]
     # Allows to control if `bss` sections (and derivatived sections) will be put on a `NOLOAD` segment on the generated linker script or not.
     ld_bss_is_noload: bool
+    # Aligns the start of the segment to the given value
+    ld_align_segment_start: Optional[int]
     # Allows to toggle aligning the `*_VRAM_END` linker symbol for each segment.
     ld_align_segment_vram_end: bool
     # Allows to toggle aligning the `*_END` linker symbol for each section of each section.
     ld_align_section_vram_end: bool
     # If enabled, the generated linker script will have a linker symbol for each data file
     ld_generate_symbol_per_data_segment: bool
     # Sets the default option for the `bss_contains_common` attribute of all segments.
@@ -444,14 +446,17 @@
             "segment_symbols_style", str, ["splat", "makerom"], "splat"
         ),
         ld_rom_start=p.parse_opt("ld_rom_start", int, 0),
         ld_fill_value=p.parse_optional_opt_with_default("ld_fill_value", int, 0),
         ld_bss_is_noload=p.parse_opt(
             "ld_bss_is_noload", bool, default_ld_bss_is_noload
         ),
+        ld_align_segment_start=p.parse_optional_opt_with_default(
+            "ld_align_segment_start", int, None
+        ),
         ld_align_segment_vram_end=p.parse_opt("ld_align_segment_vram_end", bool, True),
         ld_align_section_vram_end=p.parse_opt("ld_align_section_vram_end", bool, True),
         ld_generate_symbol_per_data_segment=p.parse_opt(
             "ld_generate_symbol_per_data_segment", bool, True
         ),
         ld_bss_contains_common=p.parse_opt("ld_bss_contains_common", bool, False),
         create_c_files=p.parse_opt("create_c_files", bool, True),
```

### Comparing `splat64-0.24.2/src/splat/util/palettes.py` & `splat64-0.24.3/src/splat/util/palettes.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/relocs.py` & `splat64-0.24.3/src/splat/util/relocs.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/statistics.py` & `splat64-0.24.3/src/splat/util/statistics.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/symbols.py` & `splat64-0.24.3/src/splat/util/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,17 @@
                                 continue
                             if attr_name == "name_end":
                                 sym.given_name_end = attr_val
                                 continue
                             if attr_name == "filename":
                                 sym.given_filename = attr_val
                                 continue
+                            if attr_name == "visibility":
+                                sym.given_visibility = attr_val
+                                continue
                         except:
                             log.parsing_error_preamble(path, line_num, line)
                             log.write(
                                 f"value of attribute '{attr_name}' could not be read:"
                             )
                             log.write("")
                             raise
@@ -457,14 +460,16 @@
     if sym.allow_addend:
         context_sym.allowedToReferenceAddends = True
     if sym.dont_allow_addend:
         context_sym.notAllowedToReferenceAddends = True
     context_sym.setNameGetCallbackIfUnset(lambda _: sym.name)
     if sym.given_name_end:
         context_sym.nameEnd = sym.given_name_end
+    if sym.given_visibility:
+        context_sym.visibility = sym.given_visibility
 
     return context_sym
 
 
 def add_symbol_to_spim_section(
     section: spimdisasm.mips.sections.SectionBase, sym: "Symbol"
 ) -> spimdisasm.common.ContextSymbol:
@@ -502,14 +507,16 @@
     if sym.force_migration:
         context_sym.forceMigration = True
     if sym.force_not_migration:
         context_sym.forceNotMigration = True
     context_sym.setNameGetCallbackIfUnset(lambda _: sym.name)
     if sym.given_name_end:
         context_sym.nameEnd = sym.given_name_end
+    if sym.given_visibility:
+        context_sym.visibility = sym.given_visibility
 
     return context_sym
 
 
 def create_symbol_from_spim_symbol(
     segment: "Segment", context_sym: spimdisasm.common.ContextSymbol
 ) -> "Symbol":
@@ -595,14 +602,15 @@
     dont_allow_addend: bool = False
 
     linker_section: Optional[str] = None
 
     allow_duplicated: bool = False
 
     given_filename: Optional[str] = None
+    given_visibility: Optional[str] = None
 
     _generated_default_name: Optional[str] = None
     _last_type: Optional[str] = None
 
     def __str__(self):
         return self.name
```

### Comparing `splat64-0.24.2/src/splat/util/vram_classes.py` & `splat64-0.24.3/src/splat/util/vram_classes.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/n64/find_code_length.py` & `splat64-0.24.3/src/splat/util/n64/find_code_length.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/n64/rominfo.py` & `splat64-0.24.3/src/splat/util/n64/rominfo.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/src/splat/util/psx/psxexeinfo.py` & `splat64-0.24.3/src/splat/util/psx/psxexeinfo.py`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/README.md` & `splat64-0.24.3/test/README.md`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/Makefile` & `splat64-0.24.3/test/basic_app/Makefile`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/header.s` & `splat64-0.24.3/test/basic_app/header.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/main.c` & `splat64-0.24.3/test/basic_app/main.c`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/expected/.splache` & `splat64-0.24.3/test/basic_app/expected/.splache`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/expected/asm/handwritten.s` & `splat64-0.24.3/test/basic_app/expected/asm/handwritten.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/expected/asm/header.s` & `splat64-0.24.3/test/basic_app/expected/asm/header.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s` & `splat64-0.24.3/test/basic_app/expected/asm/nonmatchings/main/func_80000400.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s` & `splat64-0.24.3/test/basic_app/expected/asm/nonmatchings/main/func_800004A0.s`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/LICENSE` & `splat64-0.24.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splat64-0.24.2/README.md` & `splat64-0.24.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 The brackets corresponds to the optional dependencies to install while installing splat. Refer to [Optional dependencies](#optional-dependencies) to see the list of available groups.
 
 If you use a `requirements.txt` file in your repository, then you can add this library with the following line:
 
 ```txt
-splat64[mips]>=0.24.2,<1.0.0
+splat64[mips]>=0.24.3,<1.0.0
 ```
 
 ### Optional dependencies
 
 - `mips`: Required when using the N64, PSX, PS2 or PSp platforms.
 - `dev`: Installs all the available dependencies groups and other packages for development.
```

### Comparing `splat64-0.24.2/pyproject.toml` & `splat64-0.24.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "splat64"
 # Should be synced with src/splat/__init__.py
-version = "0.24.2"
+version = "0.24.3"
 description = "A binary splitting tool to assist with decompilation and modding projects"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -16,15 +16,15 @@
     "tqdm",
     "intervaltree",
     "colorama",
 ]
 
 [project.optional-dependencies]
 mips = [
-    "spimdisasm>=1.25.0,<2.0.0", # This value should be keep in sync with the version listed on disassembler/spimdisasm_disassembler.py
+    "spimdisasm>=1.26.0,<2.0.0", # This value should be keep in sync with the version listed on disassembler/spimdisasm_disassembler.py
     "rabbitizer>=1.10.0,<2.0.0",
     "pygfxd",
     "n64img>=0.1.4",
     "crunch64>=0.2.0,<1.0.0",
 ]
 dev = [
     "splat64[mips]",
```

### Comparing `splat64-0.24.2/PKG-INFO` & `splat64-0.24.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: splat64
-Version: 0.24.2
+Version: 0.24.3
 Summary: A binary splitting tool to assist with decompilation and modding projects
 Project-URL: Repository, https://github.com/ethteck/splat
 Project-URL: Issues, https://github.com/ethteck/splat/issues
 Project-URL: Changelog, https://github.com/ethteck/splat/blob/master/CHANGELOG.md
 License: MIT License
         
         Copyright (c) 2021 Ethan Roseman
@@ -38,23 +38,23 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: crunch64<1.0.0,>=0.2.0; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: n64img>=0.1.4; extra == 'dev'
 Requires-Dist: pygfxd; extra == 'dev'
 Requires-Dist: rabbitizer<2.0.0,>=1.10.0; extra == 'dev'
-Requires-Dist: spimdisasm<2.0.0,>=1.25.0; extra == 'dev'
+Requires-Dist: spimdisasm<2.0.0,>=1.26.0; extra == 'dev'
 Requires-Dist: types-colorama; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Provides-Extra: mips
 Requires-Dist: crunch64<1.0.0,>=0.2.0; extra == 'mips'
 Requires-Dist: n64img>=0.1.4; extra == 'mips'
 Requires-Dist: pygfxd; extra == 'mips'
 Requires-Dist: rabbitizer<2.0.0,>=1.10.0; extra == 'mips'
-Requires-Dist: spimdisasm<2.0.0,>=1.25.0; extra == 'mips'
+Requires-Dist: spimdisasm<2.0.0,>=1.26.0; extra == 'mips'
 Description-Content-Type: text/markdown
 
 # splat
 
 [![PyPI](https://img.shields.io/pypi/v/splat64)](https://pypi.org/project/splat64/)
 
 A binary splitting tool to assist with decompilation and modding projects
@@ -72,15 +72,15 @@
 ```
 
 The brackets corresponds to the optional dependencies to install while installing splat. Refer to [Optional dependencies](#optional-dependencies) to see the list of available groups.
 
 If you use a `requirements.txt` file in your repository, then you can add this library with the following line:
 
 ```txt
-splat64[mips]>=0.24.2,<1.0.0
+splat64[mips]>=0.24.3,<1.0.0
 ```
 
 ### Optional dependencies
 
 - `mips`: Required when using the N64, PSX, PS2 or PSp platforms.
 - `dev`: Installs all the available dependencies groups and other packages for development.
```

