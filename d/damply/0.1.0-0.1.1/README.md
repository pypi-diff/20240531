# Comparing `tmp/damply-0.1.0.tar.gz` & `tmp/damply-0.1.1.tar.gz`

## Comparing `damply-0.1.0.tar` & `damply-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0   403256 2020-02-02 00:00:00.000000 damply-0.1.0/pixi.lock
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.1.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 damply-0.1.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 damply-0.1.0/config/coverage.toml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 damply-0.1.0/config/hatch.toml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.1.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.1.0/config/releaserc.toml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 damply-0.1.0/config/ruff.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.1.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.1.0/docs/about.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.1.0/src/damply/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 damply-0.1.0/src/damply/cli.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.1.0/tests/test_general.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 damply-0.1.0/.gitignore
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 damply-0.1.0/README.md
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 damply-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 damply-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.1.1/pixi.lock
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.1.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 damply-0.1.1/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 damply-0.1.1/config/coverage.toml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 damply-0.1.1/config/hatch.toml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.1.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.1.1/config/releaserc.toml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 damply-0.1.1/config/ruff.toml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 damply-0.1.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.1.1/docs/about.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.1.1/src/damply/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 damply-0.1.1/src/damply/cli.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.1.1/tests/test_general.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 damply-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 damply-0.1.1/README.md
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 damply-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 damply-0.1.1/PKG-INFO
```

### Comparing `damply-0.1.0/pixi.lock` & `damply-0.1.1/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -2029,15 +2029,14 @@
   version: '0.1'
   build: conda_forge
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
   sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
   md5: d7c89558ba9fa0495403155b64376d81
   license: None
-  purls: []
   size: 2562
   timestamp: 1578324546067
 - kind: conda
   name: _openmp_mutex
   version: '4.5'
   build: 2_gnu
   build_number: 16
@@ -2048,15 +2047,14 @@
   depends:
   - _libgcc_mutex 0.1 conda_forge
   - libgomp >=7.5.0
   constrains:
   - openmp_impl 9999
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 23621
   timestamp: 1650670423406
 - kind: pypi
   name: annotated-types
   version: 0.7.0
   url: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
   sha256: 1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53
@@ -2150,15 +2148,14 @@
   url: https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda
   sha256: 711602276ae39276cb0faaca6fd0ac851fff0ca17151917569174841ef830bbd
   md5: 54ca2e08b3220c148a1d8329c2678e02
   depends:
   - python >=2.7
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 5950
   timestamp: 1669158729416
 - kind: conda
   name: backports.tarfile
   version: 1.0.0
   build: pyhd8ed1ab_1
   build_number: 1
@@ -2271,29 +2268,27 @@
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
   sha256: 61fb2b488928a54d9472113e1280b468a309561caa54f33825a3593da390b242
   md5: 6097a6ca9ada32699b5fc4312dd6ef18
   license: bzip2-1.0.6
   license_family: BSD
-  purls: []
   size: 127885
   timestamp: 1699280178474
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: h93a5062_5
   build_number: 5
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
   sha256: bfa84296a638bea78a8bb29abc493ee95f2a0218775642474a840411b950fe5f
   md5: 1bbc659ca658bfd49a481b5ef7a0f40f
   license: bzip2-1.0.6
   license_family: BSD
-  purls: []
   size: 122325
   timestamp: 1699280294368
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: hcfcfb64_5
   build_number: 5
@@ -2303,15 +2298,14 @@
   md5: 26eb8ca6ea332b675e11704cce84a3be
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: bzip2-1.0.6
   license_family: BSD
-  purls: []
   size: 124580
   timestamp: 1699280668742
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: hd590300_5
   build_number: 5
@@ -2319,63 +2313,58 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
   sha256: 242c0c324507ee172c0e0dd2045814e746bb303d1eb78870d182ceb0abc726a8
   md5: 69b8b6202a07720f448be700e300ccf4
   depends:
   - libgcc-ng >=12
   license: bzip2-1.0.6
   license_family: BSD
-  purls: []
   size: 254228
   timestamp: 1699279927352
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: h56e8100_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
   sha256: 4d587088ecccd393fec3420b64f1af4ee1a0e6897a45cfd5ef38055322cea5d0
   md5: 63da060240ab8087b60d1357051ea7d6
   license: ISC
-  purls: []
   size: 155886
   timestamp: 1706843918052
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: h8857fd0_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
   sha256: 54a794aedbb4796afeabdf54287b06b1d27f7b13b3814520925f4c2c80f58ca9
   md5: f2eacee8c33c43692f1ccfd33d0f50b1
   license: ISC
-  purls: []
   size: 155665
   timestamp: 1706843838227
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: hbcca054_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
   sha256: 91d81bfecdbb142c15066df70cc952590ae8991670198f92c66b62019b251aeb
   md5: 2f4327a1cbe7f022401b236e915a5fef
   license: ISC
-  purls: []
   size: 155432
   timestamp: 1706843687645
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: hf0a4a13_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
   sha256: 49bc3439816ac72d0c0e0f144b8cc870fdcc4adec2e861407ec818d8116b2204
   md5: fb416a1795f18dcc5a038bc2dc54edf9
   license: ISC
-  purls: []
   size: 155725
   timestamp: 1706844034242
 - kind: conda
   name: certifi
   version: 2024.2.2
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -2864,31 +2853,17 @@
   license_family: BSD
   purls:
   - pkg:pypi/cryptography?source=conda-forge-mapping
   size: 1978679
   timestamp: 1715044173081
 - kind: pypi
   name: damply
-  version: 0.1.0
+  version: 0.1.1
   path: .
-  sha256: 3400363e7023f013c4a610d7b82281f5bfcf6f706fb5181e060d1e84252210d4
-  requires_dist:
-  - rich
-  - rich-click
-  - pydantic
-  - textual
-  - trogon
-  - dataclasses-json
-  requires_python: '>=3.10'
-  editable: true
-- kind: pypi
-  name: damply
-  version: 0.1.0
-  path: .
-  sha256: 10e42ca166f9bc5a0bae64ff33d5cebbfcc70b8292c687208dc70aa8d61584f9
+  sha256: fbe3e7786c541551a0549533a070128b6a1c8d8604bac8f7fa32127c8a74d975
   requires_dist:
   - rich
   - rich-click
   - pydantic
   - textual
   - trogon
   - dataclasses-json
@@ -2914,15 +2889,14 @@
   md5: ecfff944ba3960ecb334b9a2663d708d
   depends:
   - expat >=2.4.2,<3.0a0
   - libgcc-ng >=9.4.0
   - libglib >=2.70.2,<3.0a0
   license: GPL-2.0-or-later
   license_family: GPL
-  purls: []
   size: 618596
   timestamp: 1640112124844
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py310h00ffb61_0
   subdir: win-64
@@ -3277,15 +3251,14 @@
   sha256: 89916c536ae5b85bb8bf0cfa27d751e274ea0911f04e4a928744735c14ef5155
   md5: 53fb86322bdb89496d7579fe3f02fd61
   depends:
   - libexpat 2.6.2 h59595ed_0
   - libgcc-ng >=12
   license: MIT
   license_family: MIT
-  purls: []
   size: 137627
   timestamp: 1710362144873
 - kind: conda
   name: filelock
   version: 3.14.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -4294,15 +4267,14 @@
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
   sha256: 150c05a6e538610ca7c43beb3a40d65c90537497a4f6a5f4d15ec0451b6f5ebb
   md5: 30186d27e2c9fa62b45fb1476b7200e3
   depends:
   - libgcc-ng >=10.3.0
   license: LGPL-2.1-or-later
-  purls: []
   size: 117831
   timestamp: 1646151697040
 - kind: conda
   name: krb5
   version: 1.21.2
   build: h659d440_0
   subdir: linux-64
@@ -4314,15 +4286,14 @@
   - libedit >=3.1.20191231,<3.2.0a0
   - libedit >=3.1.20191231,<4.0a0
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - openssl >=3.1.2,<4.0a0
   license: MIT
   license_family: MIT
-  purls: []
   size: 1371181
   timestamp: 1692097755782
 - kind: conda
   name: krb5
   version: 1.21.2
   build: h92f50d5_0
   subdir: osx-arm64
@@ -4332,15 +4303,14 @@
   depends:
   - libcxx >=15.0.7
   - libedit >=3.1.20191231,<3.2.0a0
   - libedit >=3.1.20191231,<4.0a0
   - openssl >=3.1.2,<4.0a0
   license: MIT
   license_family: MIT
-  purls: []
   size: 1195575
   timestamp: 1692098070699
 - kind: conda
   name: krb5
   version: 1.21.2
   build: hb884880_0
   subdir: osx-64
@@ -4350,15 +4320,14 @@
   depends:
   - libcxx >=15.0.7
   - libedit >=3.1.20191231,<3.2.0a0
   - libedit >=3.1.20191231,<4.0a0
   - openssl >=3.1.2,<4.0a0
   license: MIT
   license_family: MIT
-  purls: []
   size: 1183568
   timestamp: 1692098004387
 - kind: conda
   name: krb5
   version: 1.21.2
   build: heb0366b_0
   subdir: win-64
@@ -4368,15 +4337,14 @@
   depends:
   - openssl >=3.1.2,<4.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
-  purls: []
   size: 710894
   timestamp: 1692098129546
 - kind: conda
   name: ld_impl_linux-64
   version: '2.40'
   build: hf3520f5_1
   build_number: 1
@@ -4384,45 +4352,42 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-hf3520f5_1.conda
   sha256: cb54a873c1c84c47f7174093889686b626946b8143905ec0f76a56785b26a304
   md5: 33b7851c39c25da14f6a233a8ccbeeca
   constrains:
   - binutils_impl_linux-64 2.40
   license: GPL-3.0-only
   license_family: GPL
-  purls: []
   size: 707934
   timestamp: 1716583433869
 - kind: conda
   name: libcxx
   version: 17.0.6
   build: h5f092b4_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-17.0.6-h5f092b4_0.conda
   sha256: 119d3d9306f537d4c89dc99ed99b94c396d262f0b06f7833243646f68884f2c2
   md5: a96fd5dda8ce56c86a971e0fa02751d0
   depends:
   - __osx >=11.0
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
-  purls: []
   size: 1248885
   timestamp: 1715020154867
 - kind: conda
   name: libcxx
   version: 17.0.6
   build: h88467a6_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-17.0.6-h88467a6_0.conda
   sha256: e7b57062c1edfcbd13d2129467c94cbff7f0a988ee75782bf48b1dc0e6300b8b
   md5: 0fe355aecb8d24b8bc07c763209adbd9
   depends:
   - __osx >=10.13
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
-  purls: []
   size: 1249309
   timestamp: 1715020018902
 - kind: conda
   name: libedit
   version: 3.1.20191231
   build: h0678c8f_2
   build_number: 2
@@ -4430,15 +4395,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
   sha256: dbd3c3f2eca1d21c52e4c03b21930bbce414c4592f8ce805801575b9e9256095
   md5: 6016a8a1d0e63cac3de2c352cd40208b
   depends:
   - ncurses >=6.2,<7.0.0a0
   license: BSD-2-Clause
   license_family: BSD
-  purls: []
   size: 105382
   timestamp: 1597616576726
 - kind: conda
   name: libedit
   version: 3.1.20191231
   build: hc8eb9b7_2
   build_number: 2
@@ -4446,15 +4410,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libedit-3.1.20191231-hc8eb9b7_2.tar.bz2
   sha256: 3912636197933ecfe4692634119e8644904b41a58f30cad9d1fc02f6ba4d9fca
   md5: 30e4362988a2623e9eb34337b83e01f9
   depends:
   - ncurses >=6.2,<7.0.0a0
   license: BSD-2-Clause
   license_family: BSD
-  purls: []
   size: 96607
   timestamp: 1597616630749
 - kind: conda
   name: libedit
   version: 3.1.20191231
   build: he28a2e2_2
   build_number: 2
@@ -4463,15 +4426,14 @@
   sha256: a57d37c236d8f7c886e01656f4949d9dcca131d2a0728609c6f7fa338b65f1cf
   md5: 4d331e44109e3f0e19b4cb8f9b82f3e1
   depends:
   - libgcc-ng >=7.5.0
   - ncurses >=6.2,<7.0.0a0
   license: BSD-2-Clause
   license_family: BSD
-  purls: []
   size: 123878
   timestamp: 1597616541093
 - kind: conda
   name: libexpat
   version: 2.6.2
   build: h59595ed_0
   subdir: linux-64
@@ -4480,88 +4442,82 @@
   md5: e7ba12deb7020dd080c6c70e7b6f6a3d
   depends:
   - libgcc-ng >=12
   constrains:
   - expat 2.6.2.*
   license: MIT
   license_family: MIT
-  purls: []
   size: 73730
   timestamp: 1710362120304
 - kind: conda
   name: libexpat
   version: 2.6.2
   build: h63175ca_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
   sha256: 79f612f75108f3e16bbdc127d4885bb74729cf66a8702fca0373dad89d40c4b7
   md5: bc592d03f62779511d392c175dcece64
   constrains:
   - expat 2.6.2.*
   license: MIT
   license_family: MIT
-  purls: []
   size: 139224
   timestamp: 1710362609641
 - kind: conda
   name: libexpat
   version: 2.6.2
   build: h73e2aa4_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
   sha256: a188a77b275d61159a32ab547f7d17892226e7dac4518d2c6ac3ac8fc8dfde92
   md5: 3d1d51c8f716d97c864d12f7af329526
   constrains:
   - expat 2.6.2.*
   license: MIT
   license_family: MIT
-  purls: []
   size: 69246
   timestamp: 1710362566073
 - kind: conda
   name: libexpat
   version: 2.6.2
   build: hebf3989_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
   sha256: ba7173ac30064ea901a4c9fb5a51846dcc25512ceb565759be7d18cbf3e5415e
   md5: e3cde7cfa87f82f7cb13d482d5e0ad09
   constrains:
   - expat 2.6.2.*
   license: MIT
   license_family: MIT
-  purls: []
   size: 63655
   timestamp: 1710362424980
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h0d85af4_5
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
   sha256: 7a2d27a936ceee6942ea4d397f9c7d136f12549d86f7617e8b6bad51e01a941f
   md5: ccb34fb14960ad8b125962d3d79b31a9
   license: MIT
   license_family: MIT
-  purls: []
   size: 51348
   timestamp: 1636488394370
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h3422bc3_5
   build_number: 5
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
   sha256: 41b3d13efb775e340e4dba549ab5c029611ea6918703096b2eaa9c015c0750ca
   md5: 086914b672be056eb70fd4285b6783b6
   license: MIT
   license_family: MIT
-  purls: []
   size: 39020
   timestamp: 1636488587153
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h7f98852_5
   build_number: 5
@@ -4569,15 +4525,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
   sha256: ab6e9856c21709b7b517e940ae7028ae0737546122f83c2aa5d692860c3b149e
   md5: d645c6d2ac96843a2bfaccd2d62b3ac3
   depends:
   - libgcc-ng >=9.4.0
   license: MIT
   license_family: MIT
-  purls: []
   size: 58292
   timestamp: 1636488182923
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h8ffe710_5
   build_number: 5
@@ -4586,15 +4541,14 @@
   sha256: 1951ab740f80660e9bc07d2ed3aefb874d78c107264fd810f24a1a6211d4b1a5
   md5: 2c96d1b6915b408893f9472569dee135
   depends:
   - vc >=14.1,<15.0a0
   - vs2015_runtime >=14.16.27012
   license: MIT
   license_family: MIT
-  purls: []
   size: 42063
   timestamp: 1636489106777
 - kind: conda
   name: libgcc-ng
   version: 13.2.0
   build: h77fa898_7
   build_number: 7
@@ -4605,15 +4559,14 @@
   depends:
   - _libgcc_mutex 0.1 conda_forge
   - _openmp_mutex >=4.5
   constrains:
   - libgomp 13.2.0 h77fa898_7
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  purls: []
   size: 775806
   timestamp: 1715016057793
 - kind: conda
   name: libglib
   version: 2.80.2
   build: hf974151_0
   subdir: linux-64
@@ -4625,15 +4578,14 @@
   - libgcc-ng >=12
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<2.0.0a0
   - pcre2 >=10.43,<10.44.0a0
   constrains:
   - glib 2.80.2 *_0
   license: LGPL-2.1-or-later
-  purls: []
   size: 3912673
   timestamp: 1715252654366
 - kind: conda
   name: libgomp
   version: 13.2.0
   build: h77fa898_7
   build_number: 7
@@ -4641,73 +4593,68 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
   sha256: 781444fa069d3b50e8ed667b750571cacda785761c7fc2a89ece1ac49693d4ad
   md5: abf3fec87c2563697defa759dec3d639
   depends:
   - _libgcc_mutex 0.1 conda_forge
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  purls: []
   size: 422336
   timestamp: 1715015995979
 - kind: conda
   name: libiconv
   version: '1.17'
   build: hd590300_2
   build_number: 2
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
   sha256: 8ac2f6a9f186e76539439e50505d98581472fedb347a20e7d1f36429849f05c9
   md5: d66573916ffcf376178462f1b61c941e
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1-only
-  purls: []
   size: 705775
   timestamp: 1702682170569
 - kind: conda
   name: libnsl
   version: 2.0.1
   build: hd590300_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
   sha256: 26d77a3bb4dceeedc2a41bd688564fe71bf2d149fdcf117049970bc02ff1add6
   md5: 30fd6e37fe21f86f4bd26d6ee73eeec7
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1-only
   license_family: GPL
-  purls: []
   size: 33408
   timestamp: 1697359010159
 - kind: conda
   name: libsodium
   version: 1.0.18
   build: h27ca646_1
   build_number: 1
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
   sha256: 1d95fe5e5e6a0700669aab454b2a32f97289c9ed8d1f7667c2ba98327a6f05bc
   md5: 90859688dbca4735b74c02af14c4c793
   license: ISC
-  purls: []
   size: 324912
   timestamp: 1605135878892
 - kind: conda
   name: libsodium
   version: 1.0.18
   build: h36c2ea0_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
   sha256: 53da0c8b79659df7b53eebdb80783503ce72fb4b10ed6e9e05cc0e9e4207a130
   md5: c3788462a6fbddafdb413a9f9053e58d
   depends:
   - libgcc-ng >=7.5.0
   license: ISC
-  purls: []
   size: 374999
   timestamp: 1605135674116
 - kind: conda
   name: libsodium
   version: 1.0.18
   build: h8d14728_1
   build_number: 1
@@ -4715,71 +4662,66 @@
   url: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
   sha256: ecc463f0ab6eaf6bc5bd6ff9c17f65595de6c7a38db812222ab8ffde0d3f4bc2
   md5: 5c1fb45b5e2912c19098750ae8a32604
   depends:
   - vc >=14.1,<15.0a0
   - vs2015_runtime >=14.16.27012
   license: ISC
-  purls: []
   size: 713431
   timestamp: 1605135918736
 - kind: conda
   name: libsodium
   version: 1.0.18
   build: hbcb3906_1
   build_number: 1
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
   sha256: 2da45f14e3d383b4b9e3a8bacc95cd2832aac2dbf9fbc70d255d384a310c5660
   md5: 24632c09ed931af617fe6d5292919cab
   license: ISC
-  purls: []
   size: 528765
   timestamp: 1605135849110
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h091b4b1_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
   sha256: 4337f466eb55bbdc74e168b52ec8c38f598e3664244ec7a2536009036e2066cc
   md5: c8c1186c7f3351f6ffddb97b1f54fc58
   depends:
   - libzlib >=1.2.13,<2.0.0a0
   license: Unlicense
-  purls: []
   size: 824794
   timestamp: 1713367748819
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h2797004_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
   sha256: e2273d6860eadcf714a759ffb6dc24a69cfd01f2a0ea9d6c20f86049b9334e0c
   md5: b3316cbe90249da4f8e84cd66e1cc55b
   depends:
   - libgcc-ng >=12
   - libzlib >=1.2.13,<2.0.0a0
   license: Unlicense
-  purls: []
   size: 859858
   timestamp: 1713367435849
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h92b6c6a_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
   sha256: 4d44b68fb29dcbc2216a8cae0b274b02ef9b4ae05d1d0f785362ed30b91c9b52
   md5: 68e462226209f35182ef66eda0f794ff
   depends:
   - libzlib >=1.2.13,<2.0.0a0
   license: Unlicense
-  purls: []
   size: 902546
   timestamp: 1713367776445
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: hcfcfb64_0
   subdir: win-64
@@ -4787,59 +4729,55 @@
   sha256: 06ec75faa51d7ec6d5db98889e869b579a9df19d7d3d9baff8359627da4a3b7e
   md5: 73f5dc8e2d55d9a1e14b11f49c3b4a28
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Unlicense
-  purls: []
   size: 870518
   timestamp: 1713367888406
 - kind: conda
   name: libstdcxx-ng
   version: 13.2.0
   build: hc0a3c3a_7
   build_number: 7
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-hc0a3c3a_7.conda
   sha256: 35f1e08be0a84810c9075f5bd008495ac94e6c5fe306dfe4b34546f11fed850f
   md5: 53ebd4c833fa01cb2c6353e99f905406
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
-  purls: []
   size: 3837704
   timestamp: 1715016117360
 - kind: conda
   name: libuuid
   version: 2.38.1
   build: h0b41bf4_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
   sha256: 787eb542f055a2b3de553614b25f09eefb0a0931b0c87dbcce6efdfd92f04f18
   md5: 40b61aab5c7ba9ff276c41cfffe6b80b
   depends:
   - libgcc-ng >=12
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 33601
   timestamp: 1680112270483
 - kind: conda
   name: libxcrypt
   version: 4.4.36
   build: hd590300_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
   sha256: 6ae68e0b86423ef188196fff6207ed0c8195dd84273cb5623b85aa08033a410c
   md5: 5aa797f8787fe7a17d1b0821485b5adc
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1-or-later
-  purls: []
   size: 100393
   timestamp: 1702724383534
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: h4ab18f5_6
   build_number: 6
@@ -4849,15 +4787,14 @@
   md5: 27329162c0dc732bcf67a4e0cd488125
   depends:
   - libgcc-ng >=12
   constrains:
   - zlib 1.2.13 *_6
   license: Zlib
   license_family: Other
-  purls: []
   size: 61571
   timestamp: 1716874066944
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: h87427d6_6
   build_number: 6
@@ -4867,15 +4804,14 @@
   md5: c0ef3c38a80c02ae1d86588c055184fc
   depends:
   - __osx >=10.13
   constrains:
   - zlib 1.2.13 *_6
   license: Zlib
   license_family: Other
-  purls: []
   size: 57373
   timestamp: 1716874185419
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: hfb2fe0b_6
   build_number: 6
@@ -4885,15 +4821,14 @@
   md5: 9c4e121cd926cab631bd1c4a61d18b17
   depends:
   - __osx >=11.0
   constrains:
   - zlib 1.2.13 *_6
   license: Zlib
   license_family: Other
-  purls: []
   size: 46768
   timestamp: 1716874151980
 - kind: conda
   name: libzlib
   version: 1.3.1
   build: h2466b09_1
   build_number: 1
@@ -4905,15 +4840,14 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   constrains:
   - zlib 1.3.1 *_1
   license: Zlib
   license_family: Other
-  purls: []
   size: 56186
   timestamp: 1716874730539
 - kind: pypi
   name: linkify-it-py
   version: 2.0.3
   url: https://files.pythonhosted.org/packages/04/1e/b832de447dee8b582cac175871d2f6c3d5077cc56d5575cadba1fd1cccfa/linkify_it_py-2.0.3-py3-none-any.whl
   sha256: 6bcbc417b0ac14323382aef5c5192c0075bf8a9d6b41820a2b66371eac6b6d79
@@ -5256,41 +5190,38 @@
   version: '6.5'
   build: h5846eda_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
   sha256: 6ecc73db0e49143092c0934355ac41583a5d5a48c6914c5f6ca48e562d3a4b79
   md5: 02a888433d165c99bf09784a7b14d900
   license: X11 AND BSD-3-Clause
-  purls: []
   size: 823601
   timestamp: 1715195267791
 - kind: conda
   name: ncurses
   version: '6.5'
   build: h59595ed_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
   sha256: 4fc3b384f4072b68853a0013ea83bdfd3d66b0126e2238e1d6e1560747aa7586
   md5: fcea371545eda051b6deafb24889fc69
   depends:
   - libgcc-ng >=12
   license: X11 AND BSD-3-Clause
-  purls: []
   size: 887465
   timestamp: 1715194722503
 - kind: conda
   name: ncurses
   version: '6.5'
   build: hb89a1cb_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
   sha256: 87d7cf716d9d930dab682cb57b3b8d3a61940b47d6703f3529a155c938a6990a
   md5: b13ad5724ac9ae98b6b4fd87e4500ba4
   license: X11 AND BSD-3-Clause
-  purls: []
   size: 795131
   timestamp: 1715194898402
 - kind: conda
   name: nest-asyncio
   version: 1.6.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -5338,15 +5269,14 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  purls: []
   size: 8368468
   timestamp: 1716471282135
 - kind: conda
   name: openssl
   version: 3.3.0
   build: h4ab18f5_3
   build_number: 3
@@ -5357,15 +5287,14 @@
   depends:
   - ca-certificates
   - libgcc-ng >=12
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  purls: []
   size: 2891147
   timestamp: 1716468354865
 - kind: conda
   name: openssl
   version: 3.3.0
   build: h87427d6_3
   build_number: 3
@@ -5376,15 +5305,14 @@
   depends:
   - __osx >=10.13
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  purls: []
   size: 2542959
   timestamp: 1716468436467
 - kind: conda
   name: openssl
   version: 3.3.0
   build: hfb2fe0b_3
   build_number: 3
@@ -5395,15 +5323,14 @@
   depends:
   - __osx >=11.0
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  purls: []
   size: 2893954
   timestamp: 1716468329572
 - kind: pypi
   name: packaging
   version: '24.0'
   url: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
   sha256: 2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5
@@ -5469,15 +5396,14 @@
   md5: 8292dea9e022d9610a11fce5e0896ed8
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - libgcc-ng >=12
   - libzlib >=1.2.13,<2.0.0a0
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 950847
   timestamp: 1708118050286
 - kind: conda
   name: pexpect
   version: 4.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -5894,88 +5820,88 @@
   sha256: 24b214b7ee3bd3b865e963dbed0f8bc5375f49449d70e8d407b567af3222aae4
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
-  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
+  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
+  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
+  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
+  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
+  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
+  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/e2/67/85ee8a54220139159b14088dd40f4d43e60822f8d64bb2a5b9b04d673bd2/pydantic_core-2.18.3-cp310-none-win_amd64.whl
-  sha256: 45e4ffbae34f7ae30d0047697e724e534a7ec0a82ef9994b7913a412c21462a0
+  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
-  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
+  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
+  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
-  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
+  url: https://files.pythonhosted.org/packages/e2/67/85ee8a54220139159b14088dd40f4d43e60822f8d64bb2a5b9b04d673bd2/pydantic_core-2.18.3-cp310-none-win_amd64.whl
+  sha256: 45e4ffbae34f7ae30d0047697e724e534a7ec0a82ef9994b7913a412c21462a0
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/4a/cf/2847167bab3e7676ba6f0b49963ba04112b1e4281d8c70e302c2fd29e08c/pydantic_core-2.18.3-cp311-cp311-macosx_10_12_x86_64.whl
   sha256: b9ebe8231726c49518b16b237b9fe0d7d361dd221302af511a83d4ada01183ab
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
-  sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
+  url: https://files.pythonhosted.org/packages/08/6b/391098a7f0863b5e54c60244c069acfca969af56af4eb7cf52e08b009560/pydantic_core-2.18.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: bd7df92f28d351bb9f12470f4c533cf03d1b52ec5a6e5c58c65b183055a60106
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/08/6b/391098a7f0863b5e54c60244c069acfca969af56af4eb7cf52e08b009560/pydantic_core-2.18.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: bd7df92f28d351bb9f12470f4c533cf03d1b52ec5a6e5c58c65b183055a60106
+  url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
+  sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
@@ -6232,15 +6158,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.10.* *_cp310
   license: Python-2.0
-  purls: []
   size: 11890228
   timestamp: 1710940046031
 - kind: conda
   name: python
   version: 3.10.14
   build: h2469fbe_0_cpython
   subdir: osx-arm64
@@ -6257,15 +6182,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.10.* *_cp310
   license: Python-2.0
-  purls: []
   size: 12336005
   timestamp: 1710939659384
 - kind: conda
   name: python
   version: 3.10.14
   build: h4de0772_0_cpython
   subdir: win-64
@@ -6282,15 +6206,14 @@
   - tzdata
   - vc >=14.1,<15
   - vc14_runtime >=14.16.27033
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.10.* *_cp310
   license: Python-2.0
-  purls: []
   size: 15864027
   timestamp: 1710938888352
 - kind: conda
   name: python
   version: 3.10.14
   build: hd12c33a_0_cpython
   subdir: linux-64
@@ -6312,15 +6235,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.10.* *_cp310
   license: Python-2.0
-  purls: []
   size: 25517742
   timestamp: 1710939725109
 - kind: conda
   name: python
   version: 3.11.9
   build: h631f459_0_cpython
   subdir: win-64
@@ -6339,15 +6261,14 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
-  purls: []
   size: 18232422
   timestamp: 1713551717924
 - kind: conda
   name: python
   version: 3.11.9
   build: h657bba9_0_cpython
   subdir: osx-64
@@ -6366,15 +6287,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
-  purls: []
   size: 15503226
   timestamp: 1713553747073
 - kind: conda
   name: python
   version: 3.11.9
   build: h932a869_0_cpython
   subdir: osx-arm64
@@ -6393,15 +6313,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
-  purls: []
   size: 14644189
   timestamp: 1713552154779
 - kind: conda
   name: python
   version: 3.11.9
   build: hb806964_0_cpython
   subdir: linux-64
@@ -6424,15 +6343,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
-  purls: []
   size: 30884494
   timestamp: 1713553104915
 - kind: conda
   name: python
   version: 3.12.3
   build: h1411813_0_cpython
   subdir: osx-64
@@ -6451,15 +6369,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  purls: []
   size: 14557341
   timestamp: 1713208068012
 - kind: conda
   name: python
   version: 3.12.3
   build: h2628c8c_0_cpython
   subdir: win-64
@@ -6478,15 +6395,14 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  purls: []
   size: 16179248
   timestamp: 1713205644673
 - kind: conda
   name: python
   version: 3.12.3
   build: h4a7b5fc_0_cpython
   subdir: osx-arm64
@@ -6505,15 +6421,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  purls: []
   size: 13207557
   timestamp: 1713206576646
 - kind: conda
   name: python
   version: 3.12.3
   build: hab00c5b_0_cpython
   subdir: linux-64
@@ -6536,15 +6451,14 @@
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  purls: []
   size: 31991381
   timestamp: 1713208036041
 - kind: conda
   name: python-dateutil
   version: 2.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -6618,15 +6532,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-4_cp310.conda
   sha256: 456bec815bfc2b364763084d08b412fdc4c17eb9ccc66a36cb775fa7ac3cbaec
   md5: 26322ec5d7712c3ded99dd656142b8ce
   constrains:
   - python 3.10.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6398
   timestamp: 1695147363189
 - kind: conda
   name: python_abi
   version: '3.10'
   build: 4_cp310
   build_number: 4
@@ -6634,15 +6547,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-4_cp310.conda
   sha256: abc26b3b5a62f9c8112a2303d24b0c590d5f7fc9470521f5a520472d59c2223e
   md5: b15c816c5a86abcc4d1458dd63aa4c65
   constrains:
   - python 3.10.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6484
   timestamp: 1695147705581
 - kind: conda
   name: python_abi
   version: '3.10'
   build: 4_cp310
   build_number: 4
@@ -6650,15 +6562,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.10-4_cp310.conda
   sha256: f69bac2f28082a275ef67313968b2c366d8236c3a6869b9cdf5cdb97a5821812
   md5: 1a3d9c6bb5f0b1b22d9e9296c127e8c7
   constrains:
   - python 3.10.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6490
   timestamp: 1695147522999
 - kind: conda
   name: python_abi
   version: '3.10'
   build: 4_cp310
   build_number: 4
@@ -6666,15 +6577,14 @@
   url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-4_cp310.conda
   sha256: 19066c462fd0e32c64503c688f77cb603beb4019b812caf855d03f2a5447960b
   md5: b41195997c14fb7473d26637ea4c3946
   constrains:
   - python 3.10.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6773
   timestamp: 1695147715814
 - kind: conda
   name: python_abi
   version: '3.11'
   build: 4_cp311
   build_number: 4
@@ -6682,15 +6592,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-4_cp311.conda
   sha256: 0be3ac1bf852d64f553220c7e6457e9c047dfb7412da9d22fbaa67e60858b3cf
   md5: d786502c97404c94d7d58d258a445a65
   constrains:
   - python 3.11.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6385
   timestamp: 1695147338551
 - kind: conda
   name: python_abi
   version: '3.11'
   build: 4_cp311
   build_number: 4
@@ -6698,15 +6607,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-4_cp311.conda
   sha256: f56dfe2a57b3b27bad3f9527f943548e8b2526e949d9d6fc0a383020d9359afe
   md5: fef7a52f0eca6bae9e8e2e255bc86394
   constrains:
   - python 3.11.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6478
   timestamp: 1695147518012
 - kind: conda
   name: python_abi
   version: '3.11'
   build: 4_cp311
   build_number: 4
@@ -6714,15 +6622,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.11-4_cp311.conda
   sha256: 4837089c477b9b84fa38a17f453e6634e68237267211b27a8a2f5ccd847f4e55
   md5: 8d3751bc73d3bbb66f216fa2331d5649
   constrains:
   - python 3.11.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6492
   timestamp: 1695147509940
 - kind: conda
   name: python_abi
   version: '3.11'
   build: 4_cp311
   build_number: 4
@@ -6730,15 +6637,14 @@
   url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-4_cp311.conda
   sha256: 67c2aade3e2160642eec0742384e766b20c766055e3d99335681e3e05d88ed7b
   md5: 70513332c71b56eace4ee6441e66c012
   constrains:
   - python 3.11.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6755
   timestamp: 1695147711935
 - kind: conda
   name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
@@ -6746,15 +6652,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
   sha256: 182a329de10a4165f6e8a3804caf751f918f6ea6176dd4e5abcdae1ed3095bf6
   md5: dccc2d142812964fcc6abdc97b672dff
   constrains:
   - python 3.12.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6385
   timestamp: 1695147396604
 - kind: conda
   name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
@@ -6762,15 +6667,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
   sha256: 82c154d95c1637604671a02a89e72f1382e89a4269265a03506496bd928f6f14
   md5: 87201ac4314b911b74197e588cca3639
   constrains:
   - python 3.12.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6496
   timestamp: 1695147498447
 - kind: conda
   name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
@@ -6778,15 +6682,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
   sha256: db25428e4f24f8693ffa39f3ff6dfbb8fd53bc298764b775b57edab1c697560f
   md5: bbb3a02c78b2d8219d7213f76d644a2a
   constrains:
   - python 3.12.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6508
   timestamp: 1695147497048
 - kind: conda
   name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
@@ -6794,15 +6697,14 @@
   url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
   sha256: 488f8519d04b48f59bd6fde21ebe2d7a527718ff28aac86a8b53aa63658bdef6
   md5: 17f4ccf6be9ded08bd0a376f489ac1a6
   constrains:
   - python 3.12.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 6785
   timestamp: 1695147430513
 - kind: conda
   name: pywin32
   version: '306'
   build: py310h00ffb61_2
   build_number: 2
@@ -7249,15 +7151,14 @@
   sha256: 5435cf39d039387fbdc977b0a762357ea909a7694d9528ab40f005e9208744d7
   md5: 47d31b792659ce70f470b5c82fdfb7a4
   depends:
   - libgcc-ng >=12
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
-  purls: []
   size: 281456
   timestamp: 1679532220005
 - kind: conda
   name: readline
   version: '8.2'
   build: h92ec313_1
   build_number: 1
@@ -7265,15 +7166,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
   sha256: a1dfa679ac3f6007362386576a704ad2d0d7a02e98f5d0b115f207a2da63e884
   md5: 8cbb776a2f641b943d413b3e19df71f4
   depends:
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
-  purls: []
   size: 250351
   timestamp: 1679532511311
 - kind: conda
   name: readline
   version: '8.2'
   build: h9e318b2_1
   build_number: 1
@@ -7281,15 +7181,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
   sha256: 41e7d30a097d9b060037f0c6a2b1d4c4ae7e942c06c943d23f9d481548478568
   md5: f17f77f2acf4d344734bda76829ce14e
   depends:
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
-  purls: []
   size: 255870
   timestamp: 1679532707590
 - kind: conda
   name: requests
   version: 2.32.3
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -7616,15 +7515,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
   sha256: 30412b2e9de4ff82d8c2a7e5d06a15f4f4fef1809a72138b6ccb53a33b26faf5
   md5: bf830ba5afc507c6232d4ef0fb1a882d
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
-  purls: []
   size: 3270220
   timestamp: 1699202389792
 - kind: conda
   name: tk
   version: 8.6.13
   build: h5083fa2_1
   build_number: 1
@@ -7632,15 +7530,14 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
   sha256: 72457ad031b4c048e5891f3f6cb27a53cb479db68a52d965f796910e71a403a8
   md5: b50a57ba89c32b62428b71a875291c9b
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
-  purls: []
   size: 3145523
   timestamp: 1699202432999
 - kind: conda
   name: tk
   version: 8.6.13
   build: h5226925_1
   build_number: 1
@@ -7650,15 +7547,14 @@
   md5: fc048363eb8f03cd1737600a5d08aafe
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: TCL
   license_family: BSD
-  purls: []
   size: 3503410
   timestamp: 1699202577803
 - kind: conda
   name: tk
   version: 8.6.13
   build: noxft_h4845f30_101
   build_number: 101
@@ -7667,15 +7563,14 @@
   sha256: e0569c9caa68bf476bead1bed3d79650bb080b532c64a4af7d8ca286c08dea4e
   md5: d453b98d9c83e71da0741bb0ff4d76bc
   depends:
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
-  purls: []
   size: 3318875
   timestamp: 1699202167581
 - kind: conda
   name: toml
   version: 0.10.2
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -8019,15 +7914,14 @@
   url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
   sha256: aecbd9c601ba5a6c128da8975276fd817b968a9edc969b7ae97aee76e80a14a6
   md5: 471e3988f8ca5e9eb3ce6be7eac3bcee
   depends:
   - typing_extensions 4.11.0 pyha770c72_0
   license: PSF-2.0
   license_family: PSF
-  purls: []
   size: 10093
   timestamp: 1712330094282
 - kind: pypi
   name: typing-inspect
   version: 0.9.0
   url: https://files.pythonhosted.org/packages/65/f3/107a22063bf27bdccf2024833d3445f4eea42b2e598abfbd46f6a63b6cb0/typing_inspect-0.9.0-py3-none-any.whl
   sha256: 9ee6fc59062311ef8547596ab6b955e1b8aa46242d854bfc78f4f6b0eff35f9f
@@ -8058,15 +7952,14 @@
   build: h0c530f3_0
   subdir: noarch
   noarch: generic
   url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
   sha256: 7b2b69c54ec62a243eb6fba2391b5e443421608c3ae5dbff938ad33ca8db5122
   md5: 161081fc7cec0bfda0d86d7cb595f8d8
   license: LicenseRef-Public-Domain
-  purls: []
   size: 119815
   timestamp: 1706886945727
 - kind: pypi
   name: uc-micro-py
   version: 1.0.3
   url: https://files.pythonhosted.org/packages/37/87/1f677586e8ac487e29672e4b17455758fce261de06a0d086167bb760361a/uc_micro_py-1.0.3-py3-none-any.whl
   sha256: db1dffff340817673d7b466ec86114a9dc0e9d4d9b5ba229d9d60e5c12600cd5
@@ -8083,15 +7976,14 @@
   url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
   sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
   md5: 72608f6cd3e5898229c3ea16deb1ac43
   constrains:
   - vs2015_runtime >=14.29.30037
   license: LicenseRef-Proprietary
   license_family: PROPRIETARY
-  purls: []
   size: 1283972
   timestamp: 1666630199266
 - kind: conda
   name: ukkonen
   version: 1.0.1
   build: py312h0d7def4_4
   build_number: 4
@@ -8219,15 +8111,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/uv-0.2.5-h0ea3d13_0.conda
   sha256: 46dc6efb4fd9595f74e09f44bf91d66ebbf6c6318e86acb9e4988a75eade0973
   md5: 4e4270a72feafce93c4376d4099c8b43
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   license: Apache-2.0 OR MIT
-  purls: []
   size: 12429492
   timestamp: 1716957759143
 - kind: conda
   name: uv
   version: 0.2.5
   build: h4e38c46_0
   subdir: osx-64
@@ -8236,15 +8127,14 @@
   md5: 4953ba35c34975d67840015493e2065b
   depends:
   - __osx >=10.13
   - libcxx >=16
   constrains:
   - __osx >=10.12
   license: Apache-2.0 OR MIT
-  purls: []
   size: 8917483
   timestamp: 1716958061272
 - kind: conda
   name: uv
   version: 0.2.5
   build: hc069d6b_0
   subdir: osx-arm64
@@ -8253,15 +8143,14 @@
   md5: 17a64e1cf819f21f06afc893c77c5c44
   depends:
   - __osx >=11.0
   - libcxx >=16
   constrains:
   - __osx >=11.0
   license: Apache-2.0 OR MIT
-  purls: []
   size: 9237688
   timestamp: 1716958441105
 - kind: conda
   name: vc
   version: '14.3'
   build: ha32ba9b_20
   build_number: 20
@@ -8271,15 +8160,14 @@
   md5: 2abfb5cb1b9d41a50f765d60f0be563d
   depends:
   - vc14_runtime >=14.38.33135
   track_features:
   - vc14
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 17122
   timestamp: 1716231244564
 - kind: conda
   name: vc14_runtime
   version: 14.38.33135
   build: h835141b_20
   build_number: 20
@@ -8289,15 +8177,14 @@
   md5: e971b35a5765862fabc4ba6e5ddf9470
   depends:
   - ucrt >=10.0.20348.0
   constrains:
   - vs2015_runtime 14.38.33135.* *_20
   license: LicenseRef-ProprietaryMicrosoft
   license_family: Proprietary
-  purls: []
   size: 744189
   timestamp: 1716231234745
 - kind: conda
   name: virtualenv
   version: 20.26.2
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -8325,15 +8212,14 @@
   url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
   sha256: 2cebabc39766ea051e577762d813ad4151e9d0ff96f3ff3374d575a272951416
   md5: bb4f5ab332e46e1b022d8842e72905b1
   depends:
   - vc14_runtime >=14.38.33135
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 17124
   timestamp: 1716231247457
 - kind: conda
   name: watchdog
   version: 4.0.1
   build: py312h2e8e312_0
   subdir: win-64
@@ -8449,82 +8335,76 @@
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
   sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
   md5: 2161070d867d1b1204ea749c8eec4ef0
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1 and GPL-2.0
-  purls: []
   size: 418368
   timestamp: 1660346797927
 - kind: conda
   name: xz
   version: 5.2.6
   build: h57fd34a_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
   sha256: 59d78af0c3e071021cfe82dc40134c19dab8cdf804324b62940f5c8cd71803ec
   md5: 39c6b54e94014701dd157f4f576ed211
   license: LGPL-2.1 and GPL-2.0
-  purls: []
   size: 235693
   timestamp: 1660346961024
 - kind: conda
   name: xz
   version: 5.2.6
   build: h775f41a_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
   sha256: eb09823f34cc2dd663c0ec4ab13f246f45dcd52e5b8c47b9864361de5204a1c8
   md5: a72f9d4ea13d55d745ff1ed594747f10
   license: LGPL-2.1 and GPL-2.0
-  purls: []
   size: 238119
   timestamp: 1660346964847
 - kind: conda
   name: xz
   version: 5.2.6
   build: h8d14728_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
   sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
   md5: 515d77642eaa3639413c6b1bc3f94219
   depends:
   - vc >=14.1,<15
   - vs2015_runtime >=14.16.27033
   license: LGPL-2.1 and GPL-2.0
-  purls: []
   size: 217804
   timestamp: 1660346976440
 - kind: conda
   name: yaml
   version: 0.2.5
   build: h0d85af4_2
   build_number: 2
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
   sha256: 5301417e2c8dea45b401ffee8df3957d2447d4ce80c83c5ff151fc6bfe1c4148
   md5: d7e08fcf8259d742156188e8762b4d20
   license: MIT
   license_family: MIT
-  purls: []
   size: 84237
   timestamp: 1641347062780
 - kind: conda
   name: yaml
   version: 0.2.5
   build: h3422bc3_2
   build_number: 2
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
   sha256: 93181a04ba8cfecfdfb162fc958436d868cc37db504c58078eab4c1a3e57fbb7
   md5: 4bb3f014845110883a3c5ee811fd84b4
   license: MIT
   license_family: MIT
-  purls: []
   size: 88016
   timestamp: 1641347076660
 - kind: conda
   name: yaml
   version: 0.2.5
   build: h7f98852_2
   build_number: 2
@@ -8532,15 +8412,14 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
   sha256: a4e34c710eeb26945bdbdaba82d3d74f60a78f54a874ec10d373811a5d217535
   md5: 4cb3ad778ec2d5a7acbdf254eb1c42ae
   depends:
   - libgcc-ng >=9.4.0
   license: MIT
   license_family: MIT
-  purls: []
   size: 89141
   timestamp: 1641346969816
 - kind: conda
   name: yaml
   version: 0.2.5
   build: h8ffe710_2
   build_number: 2
@@ -8549,15 +8428,14 @@
   sha256: 4e2246383003acbad9682c7c63178e2e715ad0eb84f03a8df1fbfba455dfedc5
   md5: adbfb9f45d1004a26763652246a33764
   depends:
   - vc >=14.1,<15.0a0
   - vs2015_runtime >=14.16.27012
   license: MIT
   license_family: MIT
-  purls: []
   size: 63274
   timestamp: 1641347623319
 - kind: conda
   name: zeromq
   version: 4.3.5
   build: h75354e8_4
   build_number: 4
@@ -8568,15 +8446,14 @@
   depends:
   - krb5 >=1.21.2,<1.22.0a0
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   license: MPL-2.0
   license_family: MOZILLA
-  purls: []
   size: 353229
   timestamp: 1715607188837
 - kind: conda
   name: zeromq
   version: 4.3.5
   build: hcc0f68c_4
   build_number: 4
@@ -8587,15 +8464,14 @@
   depends:
   - __osx >=11.0
   - krb5 >=1.21.2,<1.22.0a0
   - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   license: MPL-2.0
   license_family: MOZILLA
-  purls: []
   size: 298555
   timestamp: 1715607628741
 - kind: conda
   name: zeromq
   version: 4.3.5
   build: hde137ed_4
   build_number: 4
@@ -8606,15 +8482,14 @@
   depends:
   - __osx >=10.13
   - krb5 >=1.21.2,<1.22.0a0
   - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   license: MPL-2.0
   license_family: MOZILLA
-  purls: []
   size: 304498
   timestamp: 1715607961981
 - kind: conda
   name: zeromq
   version: 4.3.5
   build: he1f189c_4
   build_number: 4
@@ -8626,15 +8501,14 @@
   - krb5 >=1.21.2,<1.22.0a0
   - libsodium >=1.0.18,<1.0.19.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MPL-2.0
   license_family: MOZILLA
-  purls: []
   size: 2707065
   timestamp: 1715607874610
 - kind: conda
   name: zipp
   version: 3.17.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -8720,30 +8594,28 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
   sha256: 7e1fe6057628bbb56849a6741455bbb88705bae6d6646257e57904ac5ee5a481
   md5: 5b212cfb7f9d71d603ad891879dc7933
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 400508
   timestamp: 1693151393180
 - kind: conda
   name: zstd
   version: 1.5.5
   build: h829000d_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
   sha256: d54e31d3d8de5e254c0804abd984807b8ae5cd3708d758a8bf1adff1f5df166c
   md5: 80abc41d0c48b82fe0f04e7f42f5cb7e
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 499383
   timestamp: 1693151312586
 - kind: conda
   name: zstd
   version: 1.5.5
   build: hfc55251_0
   subdir: linux-64
@@ -8752,10 +8624,9 @@
   md5: 04b88013080254850d6c01ed54810589
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   license: BSD-3-Clause
   license_family: BSD
-  purls: []
   size: 545199
   timestamp: 1693151163452
```

### Comparing `damply-0.1.0/.github/workflows/main.yaml` & `damply-0.1.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/config/mkdocs.yaml` & `damply-0.1.1/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/config/releaserc.toml` & `damply-0.1.1/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/config/ruff.toml` & `damply-0.1.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/docs/about.md` & `damply-0.1.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/.gitignore` & `damply-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/README.md` & `damply-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `damply-0.1.0/pyproject.toml` & `damply-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "damply"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["damply", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `damply-0.1.0/PKG-INFO` & `damply-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: damply
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/damply
 Project-URL: repository, https://github.com/jjjermiah/damply
 Project-URL: documentation, https://jjjermiah.github.io/damply/
 Project-URL: changelog, https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/damply/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

