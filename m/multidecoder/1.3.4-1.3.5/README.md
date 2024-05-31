# Comparing `tmp/multidecoder-1.3.4.tar.gz` & `tmp/multidecoder-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidecoder-1.3.4.tar", last modified: Fri May 17 00:08:15 2024, max compression
+gzip compressed data, was "multidecoder-1.3.5.tar", last modified: Fri May 31 18:36:09 2024, max compression
```

## Comparing `multidecoder-1.3.4.tar` & `multidecoder-1.3.5.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.349407 multidecoder-1.3.4/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.git-blame-ignore-revs
--rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.293406 multidecoder-1.3.4/.vscode/
--rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.vscode/settings.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-05-17 00:07:40.000000 multidecoder-1.3.4/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-05-17 00:07:40.000000 multidecoder-1.3.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-17 00:08:15.349407 multidecoder-1.3.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-05-17 00:07:40.000000 multidecoder-1.3.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.297406 multidecoder-1.3.4/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pipelines/azure-tests.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-05-17 00:08:15.349407 multidecoder-1.3.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-17 00:07:40.000000 multidecoder-1.3.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.293406 multidecoder-1.3.4/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.297406 multidecoder-1.3.4/src/multidecoder/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.301406 multidecoder-1.3.4/src/multidecoder/decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4389 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)      999 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13035 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/reverse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6227 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/domains.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/hit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/json_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keyword.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.309406 multidecoder-1.3.4/src/multidecoder/keywords/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/src/multidecoder/keywords/api/
--rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.advapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.apphelp
--rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl
--rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl80
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl90
--rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.au3zip
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.avicap32
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cabinet
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.clbcatq
--rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cmdial32
--rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.comctl32
--rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.credui
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cryptbase
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cryptdll
--rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cscapi
--rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dbghelp
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.devmgr
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dnsapi
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.drprov
--rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dsound
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dsuiext
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.esent
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.fveapi
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.fwpuclnt
--rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.gdi32
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.gina
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.icmp
--rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.imagehlp
--rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.iphlpapi
--rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernel32
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernelbase
--rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.libeay32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.lsasrv
--rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mapi32
--rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mfc42
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mpr
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mprapi
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msacm32
--rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msasn1
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mscoree
--rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msi
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msimg32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mspdb80
--rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mssign32
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msutb
--rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvbvm60
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvcrt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvfw32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mswsock
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mydocs
--rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.nddeapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.netapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.netplwiz
--rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdll
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdsapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntoskrnl
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntshrui
--rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbc32
--rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbccp32
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbctrac
--rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ole32
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.oleaut32
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.oledlg
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.onex
--rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.packet
--rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.pdh
--rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.powrprof
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.psapi
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.pstorec
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.query
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rasapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rastapi
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.riched20
--rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rpcrt4
--rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.scarddlg
--rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.scecli
--rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.se
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.secur32
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.sensapi
--rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.setupapi
--rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.sfc
--rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shell32
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shimgvw
--rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shlwapi
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shsvcs
--rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ssleay32
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.unknown
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.urlmon
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.user32
--rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.userenv
--rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.usp10
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.version
--rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winhttp
--rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wininet
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winmm
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winscard
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winshfhc
--rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsock
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winspool
--rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsta
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wintrust
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wlanapi
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wldap32
--rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wship6
--rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wsnmp32
--rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wtsapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/archive
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/av.name
--rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/cryptography
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/debugger.device.name
--rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/enable_content
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/environment.windows
--rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/event
--rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/guid
--rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/key
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/network.protocol
--rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/network.string
--rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/oid
--rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/os_name
--rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/powershell.cmdlet
--rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/privilege
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/ransomware.string
--rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/sandbox.id
--rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/security_identifier
--rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/user_agent
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/vba.name
--rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/windows.registry
--rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords_to_review.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     2998 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/node.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/query.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/string_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/xor_helper.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.349407 multidecoder-1.3.4/src/multidecoder.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7373 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 00:07:53.000000 multidecoder-1.3.4/src/multidecoder.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-17 00:07:40.000000 multidecoder-1.3.4/stubs/pefile.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.345407 multidecoder-1.3.4/tests/test_decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)     2953 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_encoding.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11797 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_path.py
--rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)      394 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_reverse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10165 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_xor_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.559481 multidecoder-1.3.5/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-31 18:35:34.000000 multidecoder-1.3.5/.git-blame-ignore-revs
+-rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-05-31 18:35:34.000000 multidecoder-1.3.5/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.515480 multidecoder-1.3.5/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-05-31 18:35:34.000000 multidecoder-1.3.5/.vscode/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-05-31 18:35:34.000000 multidecoder-1.3.5/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-05-31 18:35:34.000000 multidecoder-1.3.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-31 18:36:09.559481 multidecoder-1.3.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-05-31 18:35:34.000000 multidecoder-1.3.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.519480 multidecoder-1.3.5/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-31 18:35:34.000000 multidecoder-1.3.5/pipelines/azure-tests.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-05-31 18:35:34.000000 multidecoder-1.3.5/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-05-31 18:35:34.000000 multidecoder-1.3.5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-05-31 18:36:09.559481 multidecoder-1.3.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-31 18:35:34.000000 multidecoder-1.3.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.511480 multidecoder-1.3.5/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.523481 multidecoder-1.3.5/src/multidecoder/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.527480 multidecoder-1.3.5/src/multidecoder/decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4428 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      999 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13230 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/reverse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6227 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/decoders/xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/domains.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/hit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/json_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keyword.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.535481 multidecoder-1.3.5/src/multidecoder/keywords/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.555481 multidecoder-1.3.5/src/multidecoder/keywords/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.advapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.apphelp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.atl
+-rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.atl80
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.atl90
+-rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.au3zip
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.avicap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.cabinet
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.clbcatq
+-rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.cmdial32
+-rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.comctl32
+-rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.credui
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.cryptbase
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.cryptdll
+-rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.cscapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.dbghelp
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.devmgr
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.dnsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.drprov
+-rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.dsound
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.dsuiext
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.esent
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.fveapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.fwpuclnt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.gdi32
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.gina
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.icmp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.imagehlp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.iphlpapi
+-rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.kernel32
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.kernelbase
+-rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.libeay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.lsasrv
+-rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mfc42
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mpr
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mprapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msacm32
+-rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msasn1
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mscoree
+-rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msi
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msimg32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mspdb80
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mssign32
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msutb
+-rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msvbvm60
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msvcrt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.msvfw32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mswsock
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.mydocs
+-rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.nddeapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.netapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.netplwiz
+-rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntdll
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntdsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntoskrnl
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntshrui
+-rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.odbc32
+-rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.odbccp32
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.odbctrac
+-rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ole32
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.oleaut32
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.oledlg
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.onex
+-rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.packet
+-rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.pdh
+-rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.powrprof
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.psapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.pstorec
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.query
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.rasapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.rastapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.riched20
+-rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.rpcrt4
+-rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.scarddlg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.scecli
+-rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.se
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.secur32
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.sensapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.setupapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.sfc
+-rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.shell32
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.shimgvw
+-rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.shlwapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.shsvcs
+-rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.ssleay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.unknown
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.urlmon
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.user32
+-rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.userenv
+-rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.usp10
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.version
+-rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winhttp
+-rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wininet
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winmm
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winscard
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winshfhc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winsock
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winspool
+-rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.winsta
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wintrust
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wlanapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wldap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wship6
+-rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wsnmp32
+-rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/api/api.wtsapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/archive
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/av.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/cryptography
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/debugger.device.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/enable_content
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/environment.windows
+-rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/event
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/guid
+-rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/key
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/network.protocol
+-rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/network.string
+-rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/oid
+-rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/os_name
+-rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/powershell.cmdlet
+-rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/privilege
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/ransomware.string
+-rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/sandbox.id
+-rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/security_identifier
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/user_agent
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/vba.name
+-rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords/windows.registry
+-rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/keywords_to_review.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     2998 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/query.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/string_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-05-31 18:35:34.000000 multidecoder-1.3.5/src/multidecoder/xor_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.555481 multidecoder-1.3.5/src/multidecoder.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7373 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 18:35:47.000000 multidecoder-1.3.5/src/multidecoder.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-31 18:36:09.000000 multidecoder-1.3.5/src/multidecoder.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.555481 multidecoder-1.3.5/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-31 18:35:34.000000 multidecoder-1.3.5/stubs/pefile.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.555481 multidecoder-1.3.5/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 18:36:09.555481 multidecoder-1.3.5/tests/test_decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3906 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12110 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      394 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_reverse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10165 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_decoders/test_xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tests/test_xor_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-31 18:35:34.000000 multidecoder-1.3.5/tox.ini
```

### Comparing `multidecoder-1.3.4/.gitignore` & `multidecoder-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/.vscode/settings.json` & `multidecoder-1.3.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/LICENSE.md` & `multidecoder-1.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/PKG-INFO` & `multidecoder-1.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.3.4
+Version: 1.3.5
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.3.4 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.3.5 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.3.4/README.md` & `multidecoder-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/pipelines/azure-tests.yaml` & `multidecoder-1.3.5/pipelines/azure-tests.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/pipelines/publish.yaml` & `multidecoder-1.3.5/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/pyproject.toml` & `multidecoder-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/setup.cfg` & `multidecoder-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/__main__.py` & `multidecoder-1.3.5/src/multidecoder/__main__.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/base64.py` & `multidecoder-1.3.5/src/multidecoder/decoders/base64.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 
 from __future__ import annotations
 
 import binascii
 
 import regex as re
+
 from multidecoder.node import Node
 from multidecoder.registry import decoder
 from multidecoder.xor_helper import apply_xor_key, get_xorkey
 
 HTML_ESCAPE_RE = rb"&#(?:x[a-fA-F0-9]{1,4}|\d{1,4});"
 BASE64_RE = rb"(?:[A-Za-z0-9+/]{4,}(?:<\x00  \x00)?(?:&#13;|&#xD;)?(?:&#10;|&#xA)?\r?\n?){5,}[A-Za-z0-9+/]{2,}=?=?"
-BASE64DECODE_RE = rb'(?i)Base64Decode\("([a-z0-9/+]+=?=?)"\)'
-FROMB64STRING_RE = rb"(?i)(\[System.Convert\]::)?FromBase64String\('([a-z0-9+/]+=?=?)'\)"
+BASE64DECODE_RE = rb"(?i)Base64Decode\(['\"]([a-z0-9/+]+=?=?)['\"]\)"
+FROMB64STRING_RE = rb"(?i)(\[System.Convert\]::)?FromBase64String\(['\"]([a-z0-9+/]+=?=?)['\"]\)"
+ATOB_RE = rb"atob\(['\"]([A-Za-z0-9+/]+=?=?)['\"]\)"
 
 CAMEL_RE = rb"(?i)[a-z]+"
 HEX_RE = rb"(?i)[a-f0-9]+"
 MIN_B64_CHARS = 6
 
 
 def pad_base64(b64: bytes) -> bytes:
@@ -36,15 +38,15 @@
     return b64 + b"=" * padding
 
 
 @decoder
 def find_atob(data: bytes) -> list[Node]:
     """Find the javascript base64 decoding function atob and decode its argument."""
     out: list[Node] = []
-    for match in re.finditer(rb"atob\(\'([A-Za-z0-9+/]+={0,2})\'\)", data):
+    for match in re.finditer(ATOB_RE, data):
         try:
             b64 = binascii.a2b_base64(match.group(1))
             out.append(Node("javascript.string", b64, "encoding.base64", *match.span()))
         except binascii.Error:
             continue
     return out
```

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/chr.py` & `multidecoder-1.3.5/src/multidecoder/decoders/chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/codec.py` & `multidecoder-1.3.5/src/multidecoder/decoders/codec.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/concat.py` & `multidecoder-1.3.5/src/multidecoder/decoders/concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/filename.py` & `multidecoder-1.3.5/src/multidecoder/decoders/filename.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/hex.py` & `multidecoder-1.3.5/src/multidecoder/decoders/hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/network.py` & `multidecoder-1.3.5/src/multidecoder/decoders/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     out = []
     for match in re.finditer(URL_RE, data):
         group = match.group()
         start, end = match.span()
         prev = data[start - 1]
         if start == 0:
             pass  # No context
-        elif group[prev : prev + 1] == b"0":
+        elif group[prev : prev + 1] == b"0" and not _is_printable(data[start - 10 : start]):
             # Pascal string in PE file
             end = start + prev
             group = group[:prev]
         elif prev in contexts:
             close = group.find(contexts[prev])
             if close > -1:
                 end = start + close
@@ -414,7 +414,14 @@
                 dotless.pop()
         else:
             dotless.append(segment)
     if dotless == [b""]:
         # Maintain starting / if the entire path is dot segments
         return b"/", "url.dotpath"
     return b"/".join(dotless), "url.dotpath" if len(dotless) < len(segments) else ""
+
+
+def _is_printable(b: bytes) -> bool:
+    try:
+        return b.decode("ascii").isprintable()
+    except UnicodeDecodeError:
+        return False
```

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/path.py` & `multidecoder-1.3.5/src/multidecoder/decoders/path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/pe_file.py` & `multidecoder-1.3.5/src/multidecoder/decoders/pe_file.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/replace.py` & `multidecoder-1.3.5/src/multidecoder/decoders/replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/shell.py` & `multidecoder-1.3.5/src/multidecoder/decoders/shell.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/vba.py` & `multidecoder-1.3.5/src/multidecoder/decoders/vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/decoders/xml.py` & `multidecoder-1.3.5/src/multidecoder/decoders/xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/domains.py` & `multidecoder-1.3.5/src/multidecoder/domains.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/hit.py` & `multidecoder-1.3.5/src/multidecoder/hit.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/json_conversion.py` & `multidecoder-1.3.5/src/multidecoder/json_conversion.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keyword.py` & `multidecoder-1.3.5/src/multidecoder/keyword.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.advapi32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.advapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.atl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.dbghelp` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.dbghelp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.gdi32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.gdi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.imagehlp` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.imagehlp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.iphlpapi` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.iphlpapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernel32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.kernel32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.libeay32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.libeay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.mfc42` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.mfc42`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msi` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.msi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.mssign32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.mssign32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvbvm60` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.msvbvm60`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvcrt` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.msvcrt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.nddeapi` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.nddeapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.netapi32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.netapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdll` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntdll`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntoskrnl` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.ntoskrnl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbc32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.odbc32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbccp32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.odbccp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ole32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.ole32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.oleaut32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.oleaut32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.packet` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.packet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.powrprof` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.powrprof`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.rpcrt4` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.rpcrt4`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.scecli` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.scecli`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.se` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.se`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.shell32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.shell32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.shlwapi` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.shlwapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ssleay32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.ssleay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.urlmon` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.urlmon`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.user32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.user32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.wininet` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.wininet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsock` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.winsock`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsta` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.winsta`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/api/api.wsnmp32` & `multidecoder-1.3.5/src/multidecoder/keywords/api/api.wsnmp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/event` & `multidecoder-1.3.5/src/multidecoder/keywords/event`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/guid` & `multidecoder-1.3.5/src/multidecoder/keywords/guid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/key` & `multidecoder-1.3.5/src/multidecoder/keywords/key`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/network.string` & `multidecoder-1.3.5/src/multidecoder/keywords/network.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/oid` & `multidecoder-1.3.5/src/multidecoder/keywords/oid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/os_name` & `multidecoder-1.3.5/src/multidecoder/keywords/os_name`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/powershell.cmdlet` & `multidecoder-1.3.5/src/multidecoder/keywords/powershell.cmdlet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/privilege` & `multidecoder-1.3.5/src/multidecoder/keywords/privilege`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/ransomware.string` & `multidecoder-1.3.5/src/multidecoder/keywords/ransomware.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/security_identifier` & `multidecoder-1.3.5/src/multidecoder/keywords/security_identifier`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords/windows.registry` & `multidecoder-1.3.5/src/multidecoder/keywords/windows.registry`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/keywords_to_review.txt` & `multidecoder-1.3.5/src/multidecoder/keywords_to_review.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/multidecoder.py` & `multidecoder-1.3.5/src/multidecoder/multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/node.py` & `multidecoder-1.3.5/src/multidecoder/node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/query.py` & `multidecoder-1.3.5/src/multidecoder/query.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/registry.py` & `multidecoder-1.3.5/src/multidecoder/registry.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder/xor_helper.py` & `multidecoder-1.3.5/src/multidecoder/xor_helper.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/src/multidecoder.egg-info/PKG-INFO` & `multidecoder-1.3.5/src/multidecoder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.3.4
+Version: 1.3.5
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.3.4 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.3.5 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.3.4/src/multidecoder.egg-info/SOURCES.txt` & `multidecoder-1.3.5/src/multidecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_chr.py` & `multidecoder-1.3.5/tests/test_decoders/test_chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_concat.py` & `multidecoder-1.3.5/tests/test_decoders/test_concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_encoding.py` & `multidecoder-1.3.5/tests/test_decoders/test_encoding.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_hex.py` & `multidecoder-1.3.5/tests/test_decoders/test_hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_network.py` & `multidecoder-1.3.5/tests/test_decoders/test_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,14 +271,18 @@
         (
             b"part of a phrase with a url https://example.com/, still works",
             b"https://example.com/",
         ),
         (b"barefunction(https://example.com) works", b"https://example.com"),
         (b'in a string content "https://example.com"works.', b"https://example.com"),
         (b"'https://example.com/'; ", b"https://example.com/"),
+        (
+            b"webhook_url = 'https://discord.com/api/webhooks/1244340229192548423/hRSjv25n8leII_p1pKEJSFSIUr_dLBX0-EY8ZMW3rakLh682QX0zByEpotnryCtRfK_Z'",
+            b"https://discord.com/api/webhooks/1244340229192548423/hRSjv25n8leII_p1pKEJSFSIUr_dLBX0-EY8ZMW3rakLh682QX0zByEpotnryCtRfK_Z",
+        ),
     ],
 )
 def test_URL_RE_context(data, url):
     """Test that URL_RE correctly matches URLs in context"""
     assert re.search(URL_RE, data).group() == url
```

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_path.py` & `multidecoder-1.3.5/tests/test_decoders/test_path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_replace.py` & `multidecoder-1.3.5/tests/test_decoders/test_replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_shell.py` & `multidecoder-1.3.5/tests/test_decoders/test_shell.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_vba.py` & `multidecoder-1.3.5/tests/test_decoders/test_vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_decoders/test_xml.py` & `multidecoder-1.3.5/tests/test_decoders/test_xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_multidecoder.py` & `multidecoder-1.3.5/tests/test_multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_node.py` & `multidecoder-1.3.5/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.4/tests/test_xor_helper.py` & `multidecoder-1.3.5/tests/test_xor_helper.py`

 * *Files identical despite different names*

