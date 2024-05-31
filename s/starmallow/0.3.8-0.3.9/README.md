# Comparing `tmp/starmallow-0.3.8.tar.gz` & `tmp/starmallow-0.3.9.tar.gz`

## Comparing `starmallow-0.3.8.tar` & `starmallow-0.3.9.tar`

### file list

```diff
@@ -1,1230 +1,1230 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 starmallow-0.3.8/.editorconfig
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 starmallow-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/missing_stubs
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   196607 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    47071 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    63544 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19761 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   187674 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   124955 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0    89659 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    27152 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    25958 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    55199 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    68518 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    22330 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    66362 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0    17864 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/base64.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/base64.meta.json
--rw-r--r--   0        0        0    12622 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/binascii.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/binascii.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1223723 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   134946 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   119157 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    41316 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    12976 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    63393 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   154734 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    68679 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    76205 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0    98670 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   139269 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    24385 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    34863 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0   351931 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    93244 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   150002 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ipaddress.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ipaddress.meta.json
--rw-r--r--   0        0        0   292334 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0    57518 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/mimetypes.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/mimetypes.meta.json
--rw-r--r--   0        0        0    25529 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    53932 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    93805 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    48536 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    82093 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0    33277 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0   183320 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    55862 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0    82871 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    30752 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    54025 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   206015 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    30288 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   183933 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   173202 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   127577 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    70524 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    41353 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    62107 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0   260892 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   461606 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    56451 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    46000 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0    36687 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    25973 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   156299 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    96961 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/__init__.data.json
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/__init__.meta.json
--rw-r--r--   0        0        0    74630 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/from_thread.data.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/from_thread.meta.json
--rw-r--r--   0        0        0    33526 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/lowlevel.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/lowlevel.meta.json
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/to_thread.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/to_thread.meta.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/__init__.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/__init__.meta.json
--rw-r--r--   0        0        0    52701 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_compat.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_compat.meta.json
--rw-r--r--   0        0        0    14221 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_eventloop.data.json
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_exceptions.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json
--rw-r--r--   0        0        0   131665 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_fileio.data.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_fileio.meta.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_resources.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_resources.meta.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_signals.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_signals.meta.json
--rw-r--r--   0        0        0    36737 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_sockets.data.json
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_sockets.meta.json
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_streams.data.json
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_streams.meta.json
--rw-r--r--   0        0        0     8619 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json
--rw-r--r--   0        0        0    85851 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_synchronization.data.json
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json
--rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_tasks.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_tasks.meta.json
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_testing.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_testing.meta.json
--rw-r--r--   0        0        0    17868 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_typedattr.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/__init__.data.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/__init__.meta.json
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_resources.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_resources.meta.json
--rw-r--r--   0        0        0    33875 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_sockets.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_sockets.meta.json
--rw-r--r--   0        0        0    42234 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_streams.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_streams.meta.json
--rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json
--rw-r--r--   0        0        0    19889 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_tasks.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_tasks.meta.json
--rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_testing.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_testing.meta.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/__init__.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/__init__.meta.json
--rw-r--r--   0        0        0    66349 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/memory.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/memory.meta.json
--rw-r--r--   0        0        0    42462 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/stapled.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/stapled.meta.json
--rw-r--r--   0        0        0    41738 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/tls.data.json
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/tls.meta.json
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   113313 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/constants.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/constants.meta.json
--rw-r--r--   0        0        0    24738 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   218488 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0    10647 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    22666 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/proactor_events.data.json
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/proactor_events.meta.json
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    25185 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36293 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   111214 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    29759 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    36902 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_events.data.json
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_events.meta.json
--rw-r--r--   0        0        0    21829 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_utils.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_utils.meta.json
--rw-r--r--   0        0        0   446252 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    65889 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    65947 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    23805 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   149492 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    13275 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26988 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    86480 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    24377 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/utils.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/email/utils.meta.json
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0    25265 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/__init__.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/__init__.meta.json
--rw-r--r--   0        0        0    71988 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/client.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/client.meta.json
--rw-r--r--   0        0        0    43680 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/cookies.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/http/cookies.meta.json
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/__init__.meta.json
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/core.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/core.meta.json
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/idnadata.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/idnadata.meta.json
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/intranges.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/intranges.meta.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/package_data.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/package_data.meta.json
--rw-r--r--   0        0        0   103203 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/uts46data.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/idna/uts46data.meta.json
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75966 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    69929 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    98817 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   157576 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/__init__.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/__init__.meta.json
--rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/base.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/base.meta.json
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/class_registry.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/class_registry.meta.json
--rw-r--r--   0        0        0    19019 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/decorators.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/decorators.meta.json
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/error_store.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/error_store.meta.json
--rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/exceptions.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/exceptions.meta.json
--rw-r--r--   0        0        0   193168 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/fields.data.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/fields.meta.json
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/orderedset.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/orderedset.meta.json
--rw-r--r--   0        0        0    66078 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/schema.data.json
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/schema.meta.json
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/types.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/types.meta.json
--rw-r--r--   0        0        0    30041 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/utils.data.json
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/utils.meta.json
--rw-r--r--   0        0        0    77488 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/validate.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/validate.meta.json
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/warnings.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow/warnings.meta.json
--rw-r--r--   0        0        0    41806 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/__init__.data.json
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/__init__.meta.json
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/collection_field.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/collection_field.meta.json
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.meta.json
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/union_field.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/union_field.meta.json
--rw-r--r--   0        0        0    33086 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    92565 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   160937 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    56122 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    19203 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    21449 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    31806 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    73266 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    27889 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    25639 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   258642 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    15115 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    71254 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/__init__.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/__init__.meta.json
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/_impl.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/_impl.meta.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/_version.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/sniffio/_version.meta.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/__init__.meta.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/_compat.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/_compat.meta.json
--rw-r--r--   0        0        0    19689 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/_utils.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/_utils.meta.json
--rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/applications.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/applications.meta.json
--rw-r--r--   0        0        0    15001 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/background.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/background.meta.json
--rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/concurrency.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/concurrency.meta.json
--rw-r--r--   0        0        0    20566 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/convertors.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/convertors.meta.json
--rw-r--r--   0        0        0   133761 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/datastructures.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/datastructures.meta.json
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/exceptions.data.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/exceptions.meta.json
--rw-r--r--   0        0        0    31022 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/formparsers.data.json
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/formparsers.meta.json
--rw-r--r--   0        0        0    49872 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/requests.data.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/requests.meta.json
--rw-r--r--   0        0        0    38218 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/responses.data.json
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/responses.meta.json
--rw-r--r--   0        0        0   104345 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/routing.data.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/routing.meta.json
--rw-r--r--   0        0        0    40113 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/schemas.data.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/schemas.meta.json
--rw-r--r--   0        0        0    26999 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/status.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/status.meta.json
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/types.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/types.meta.json
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/websockets.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/websockets.meta.json
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/__init__.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/__init__.meta.json
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/base.data.json
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/base.meta.json
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/errors.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/errors.meta.json
--rw-r--r--   0        0        0    15378 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/exceptions.data.json
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/constants.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/constants.meta.json
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/datastructures.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/datastructures.meta.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/ext/__init__.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/ext/__init__.meta.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/__init__.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/__init__.meta.json
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/utils.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/utils.meta.json
--rw-r--r--   0        0        0     6698 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26142 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   230086 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    15877 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    22405 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   166266 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.8/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/10065f98add6ff0b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/109652e6f487f139
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1106bf394c2545f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/12b0bfced4f057e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/12d1bc2c3e3b4a83
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/139c88403d1436da
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/14baa50d760b85f4
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1516734ebe4cdf9e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/151fd4ca81800c29
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/15a4a56b6d885d72
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/169835d4ef6b2c76
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/174fbe9cb15ee3f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/176c4bc33d477f1d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/17ca9af0f4e890c7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/17e6233e2c8b4c57
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/18d115039f810722
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/195be7e3cc61159d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/199a679ef9eca4bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/19c4c1ec56600a9d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1b018c700a29eb6f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1b13d07e79be7008
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1b26045f7dbe2c85
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1bf76ae827ae0969
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1c4c20698345622a
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1c6b52f43e1f9ecf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1c8174d3fb6cfd4e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1d52da0fa1b46226
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1d5d931f005b2fdc
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1dd1a63493403b23
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1def590345254ce2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1e30b5622736e8a3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1e4c43773e562a1a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1e65a4edae7315f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1fbcf4cbb9a072d6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/1fc01fc4d329dab6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/20337f428fbbb1d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/20fc180033536e0d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2127f1f3b00218f9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/21b97c5c1040e4c9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/21c8f3eeb3c07e96
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2262d3af001fa52
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2289427a3df44cb9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/22a479e6212e06c7
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/22e59ff54546802
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/233075a4f3a6966a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2485840abb576749
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2487af63be8b8306
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/249c82b6a73b5cfd
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/252b6dc2a81aef95
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2614de03a6ac0abe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/262c1eb7a9069152
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/264bbc6647c0e341
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/268544df23daab8c
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/269e03795b762f8d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/26be189398dfa434
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2858eb97bacc4ed0
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/287ddde3a6ca88a3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/29000d4e36a3bb35
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2937fde94e0481bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2a8f2c618d9b68da
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2aa41b7defb4c2b4
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2b70e11145143c04
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2b84f3b60c3f4ce2
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2c5a467b39e90cbd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2ca403bf0fe46336
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2d5501076d63249d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2d66c86ed1832aa9
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2e0bd27ab75541a2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2e104a4d6d6c1cac
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2e1e9d73bdf26155
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2e531a3e4055c4a7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2eb7766d60702afc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/2f65fa8ebd69bb9f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3005f0cf358bc7e8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3034338d29bd0d2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/304637d7993de5f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/31fe912797f2f86
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3266c15c9bcda55d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/327e96f4d73223da
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/329ab05acd5391c4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/331cdf7bb4ec0b95
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/33351ddf7f6a55e0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3374f90390198332
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/338231b83975bd39
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/33e652e64f3581e8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/341e5cd078caef2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/345c1edda7fd4966
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/34c80c09b62c5a09
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/35b006b879963385
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/35b8d049779b1e8e
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/37500715047f4095
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/378f7e4eb0f96b0a
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/37a0895ad5a24844
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/37df1b78462054b9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/38a96cb0df513a62
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3928ea296d5bd126
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/39773375b92b92ea
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/39e422c0476f77f6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/39faf17634d3b691
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3a484f9c6d7a700a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3af5e30cd1f4b8ee
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3b0a0f9693e5b8ac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3bf82f696da70502
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3c66c25a2d6d8e46
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3ca218411159387e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3d5a8a89935df6a7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3e3190adfdc6ed6d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3f333473e057c20f
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3f65fba17c2c828e
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3fb764ea8e4e29de
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3fcd02df48e526dc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/3fcfafad557c3da2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4006f4513e986df3
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/402ef363ed6bacb6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/40376271cea804e8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/40da5e124435fc66
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4172f27f3e5a44e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/41cdafe0ae37147
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/41e02c9c9fb737f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/434c97ad6ded852
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/43ad104541e0a88f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/43c4702dd09cf8f3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4443e21f99867067
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/447bdec362667066
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/44f0cc448324a416
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/45ce791d83e308e7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/460e8d9f60c9276b
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/46348294dcb5d2bd
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/46712eb880e5f2b2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/469a939cf6b8a62a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/46a7b9f2027e8f5f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/46bc616ae842a2fc
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/471a20b055a348ff
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/47c59c416ffc8ff6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/47f54a4e5f45b64e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/48d17bfe8ddb7a05
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4930d7c7bdcefdce
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4992d5421ef46439
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4ab811e0c66581a5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4adf7386e7952612
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4b14f4fab7bf7160
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4bae766eed40caea
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4cd9e6da2528969d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4d2d34a3b143e879
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4da55f94b6f612e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4db6335677cb3233
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4de60391dbe6e95b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4ead4839ff6c502f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4f08defd53d9e12f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4f4e6262d3319c76
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/4ffde77c1cebc6f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/504e081b6b86c34f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/50e9aa222b98e60b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/50eca8ea6523d687
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5108df00cee7c52a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/510f76af0881ae19
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5197297370819168
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5256d43574700b90
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/52740cf306398353
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5301160ed35ee24f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/53aee33a1e27a7d3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/53ecbb987fdf03cd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/53ef8d5b3de7027a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/542aa314ffb3e245
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/54ac7245c6762958
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/554655233635d77c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/56123b5402b9818f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/56165200cc754ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/563735a7b8350845
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/57fc3c1eb8eab2d1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/581448974c8c2e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/58273efa49032530
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/58914b1b2500fe96
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/58c885267ee0a5d1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/58f15b3440acd2bc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5943368bf2b067db
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/594a35ca98ca2998
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/598a265df09ca33f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5993d0b8f1292b73
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5a085e9801eea808
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5a5a5ab11a912f82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5aaae113b6cc86f0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5ad09421f26d7e2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5aeb4d3c8194e4a0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5aec1e6c8cc2b524
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5d1fd97beca72c14
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5d3efad83bfd6258
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5d8fac59f0cec78c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5dbd91aa98e60d9a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5e40840c96aad063
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5ee600790e634e81
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5f404a0988062267
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5f62bc5e9923e06a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5f65edf15ca8de3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/5fe5a3ef3aff3394
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6008d98efeb1bd95
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/60b8d88975789254
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/60bd03468ffc65b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/60e3c198b607405a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6281d4777a34d609
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/62df83f800c42655
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6308ee5ec56b0229
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/634b930fb8219af7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/638ceb769f55bf50
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/639a3370ebbbf012
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/640098bfc7d282a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/64305ba858c272e5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/644126c2f14d4289
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6465889e66e3e70b
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/653086b13938658e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/65bf28f3ea69d129
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/66110399687da8c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6645edcf399c84f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/666d5411b3b1d958
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6739e9fb96a67266
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/67624662c5cfa7db
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/67bf5b1741c383f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/67f2a61223f52707
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/680cc717f698c4d0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6862ff8a8c81969
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/689c68a64edda297
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/691c8f2a6609f701
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/697923c62c1a93c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/698b2b3de7f937b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/699f9bdce9c365cc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6a0e28959df807be
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6a8c6e2446a0e0f0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6ac9e8243f47c737
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6c8757e1fc9166d1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6d2b5b260f0c1cd1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6d4960a679856fde
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6dab5bbbf339e76a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6e75b37380d4a78d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6e769e3cc3adb24b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/6ed0f8f22ff2ea8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7055ae29f4533438
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/70a0005b296bc40a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7122a1fbe43b8a92
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7232884e4491b031
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/726fb633f05d7396
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/728a6af40ef75f0b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/72a1e90161c1b3ad
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/72d35530b5713d8e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7343834aa4d9be43
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7352e8ece9e48014
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/737a5c2f20f0e563
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/737d8542b26d541c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/73be20a88210e1b0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/73d9a104cc256927
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/74d2f905ef324529
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7546ff395f02fce0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/755d4ac7664b4b84
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/75721927b265b00d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/757d1e107c70faa5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/75b06e7da441998c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/76e35a2d2488cd44
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7763d1c74d3f3d79
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/77708d5cb78dd07
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/77a6f45ccd9c5189
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/781434f33a0ce47d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7822a569cc3514a9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/78465423b1393216
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/78dc0d9fb75505f6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/78e988cea0798964
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/78ebdb9690b23a48
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7994f6e4f513da81
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/79f9864468bb7c46
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7a1fa1b3a4cd21ec
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7aa94e8ec617f1ed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7affc65075fff593
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7b196aff3b0d34e2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7b5d93007eefea0a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7bad7fcac6f8b588
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7c1898781cb9a71e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7c5d7683aa891ee0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7d025b8cbfc7ca82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7d55b4761aca1221
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7d78a4ee1621e773
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7de8bf8e1dbae4ce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7e19739959663129
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7e1b459c54f96094
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7e36d76e73aaa50e
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7e54814a652afa6c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/7efc398adabd83d1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/819ba4aac88ad4c5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/821abfbe8996dfee
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/82af181b99ed362f
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/82c96a979ec45ed8
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/84c1c0b9ef5a0bd1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/859699dc827e64bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/85d2aa90f441ac84
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/85f38c1e1a98b4ce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/85fc672825474a7e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/861ae70c60f4b515
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/863e0505e99b4912
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/868204f1007fa159
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/877a8374d55041a6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/87829d9f8a7970c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8873ff56d0e35f6e
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/88b8af873f0d9b6a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/88c961d879ca8414
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/88db9b5f1f41d922
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/88df5cd35ee3b18b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/891cc4279db032f5
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/89c58146af7dd774
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/89dcd4c51a32910d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8a10752ada77f3da
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8a22cc9ac5a2ca05
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8b09af6a575d0128
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8b72587297729c97
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8c361c3048c9e03c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8c43c7a2cd04e833
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8c7b1a64e885ea22
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8cc4f00b5d755361
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8ccb15e75038ea9a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8d0e8223e6b4ccb8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8dcea8de9ad315a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8dee251c5e37502e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8f1565c9f27de57
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8f33fd6f86bd12b6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8f56bbb2a5a9d676
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/8f7ebfd14401571a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/906379e2c501a56f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/90cfd16b86df9d53
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/90dbc1fd08ac21c8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/90f78c6105477537
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9109516011be0efe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/912ed319e99754d3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/91918d3958deff8a
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/92ccca9574be50d0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9303923bacc3dddb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9408c1595b56b385
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9442816411d7a40
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/94c4d3be2fbdce31
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/94f1fae028452aa4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/95851fc6ca36a564
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/95fa211029579181
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/963d7293fdfe61b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/965a17d45a914dcc
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/968749843c9c57e7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/980207d3fc07e68e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/981e38eb01988cf0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/98651da6fa50673a
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/986beeceff7436e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/98b1e360b558e80d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/98cad6932a3c67c3
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/992d4921e74a9030
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9959ffb4a33fa8eb
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/99dc8d8d36634b12
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9a0b35403acb1393
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9adb15a6742d6c5b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9ae8692e209e9c27
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9afeadccb73fbb4e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9b1cc72aefa30a9e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9b513dbbc3df1d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9b687e58fc1eb59f
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9b86335591fffcf1
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9b9a5ac90d2fab8d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9c477e944343f783
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9c50e4535eef3c1c
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9c720a051a865466
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9c809b5e7ea60ddf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9dd9baf20243b58b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9e574d7a8e334e38
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9edfaee2be42e198
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9f92d286a2c9f437
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/9fd95161096f3293
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a029c6d1c66ed345
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a02ffb962a1775ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a048a3a84c65fc5a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a0666de0a0a6144e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a0d2b9d3f2819f04
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a0ea9ba2a1f3ac46
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a15a78db12299f05
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a1e3b889b6944ebc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a237a0e7f1942bf6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a25a50613ceceb15
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a25bc77eede1bc2b
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a278ff735bba2bd7
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a33190b6d5891f6f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a4ae48ae62f93e63
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a4c31e01eda226cf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a4ca9aac0340823a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a4ecfd8d7b2a05b1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a6389703eb1073dd
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a658af58aec4af00
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a6de514a8b333187
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a732b9acda145222
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a74c6e6de0087343
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a76aa6fa628e6e01
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a7c84faee2aef013
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a8064825516e7ed1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a93524573859e47
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a97d4e2e87bf7f0a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a98e56ec663ce742
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/a9ee35e28e552173
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/aab62ef2f0b61424
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/aae9fa55d6e694a1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ab0add8b5cb8772e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ab68f152b19cdbaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ab7c16f4f92a5323
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/abcf1e5f80686ee5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ac2c2af7bed3210f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ac3540001bafc8d5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ac47082cb735457a
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/acb93c139a04adce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/acde528f5682578e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ad2ddab1a4a9ffa5
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/add1e3cb649188ee
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/aebe09bc5b7c0a0f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/aef437e818024f4e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/aefb1d1657f360bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/af29f1e208841600
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/afb0cca1477e5dae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/afcae95aa44aaff4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b062ec76b33ad03e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b0a59f1097595518
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b10fb291ead98cc4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b15a64bf0b9296c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b1dc6da3e82aeaeb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b1dceb4a4b40e486
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b2318a06449286b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b2cf3cdb44c18edf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b2fa10faf80c3d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b3321c7dcb8681ea
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b3c3129957608740
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b437574d4bcee451
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b4bb01c4fc1406cf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b4cc050e59a22fd9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b60a9e948956196d
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b62f346ab1b9696f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b66d8d45fb1d3d36
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b6845876145bd198
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b6e38f34eea822d6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b6e8254c0f21e056
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b757d0f14dfc70b9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b795a29f637ec0bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b7d1660c447af83d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b7e5485382e3da45
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b949882417ecfe1f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b9c3fb657e2899b5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/b9ed0232339ac16a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ba18502f0545eb06
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ba2f86bf75fec67d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bb56ec9e41027b47
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bb57e4d3c2509675
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bb759db627f4325
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bba3f7509c666e08
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bbb680356e35537b
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bbfade420b1078ed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bc22f55ed8d52a4b
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bc2ec99feb4e9954
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bc757653ca011057
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bc7b268c6b194652
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bc85cb56fba2f6b9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bccc99e22d071034
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bcfea61c791fc274
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bd24213539411981
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bd4defc3d7670b36
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bd539245d4cac9ba
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bd7c61026703a0af
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bd7ee16910a7e4a6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bdc22adea1cb15d8
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/be90521730430f10
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bea6cce6e0520aff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bec86529de61c55e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bee8547360003ad7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bf28b0d53d6344a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bf74275c64c846e4
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bf767767343056e7
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/bf9a486d3cb01172
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c058a23b30a7c0a8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c083a6ea029de8d7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c0d10c81df8cce05
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c18c9aaf67596c6e
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c19418c2294bc7a0
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c21bef522b1327db
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c2a99a6e393c799a
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c312dc5879acf73b
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c32806f29722c480
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c441c960648d4cda
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c47681fb80798d61
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c4c1d17c7684dc2a
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c4e5ca2325c7548f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c563c8c53efb149d
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c5dbe9a612eb2b7a
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c6a45dcc88a5ae3d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c71f830573d0476f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c73e5aec75b4e0d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c8354555d62ff86d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c8417fe0df58ee00
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c92cc8d023659eb
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c95731c0dcf23963
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c99e152a2241e5cc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c9d959d5764014e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c9db389e76b219bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/c9f745e1bae9f680
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ca20ee2afd333a10
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ca2e8924391b3f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cb54ded01fe6b4f6
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cbe65e1002f5fd6c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cc0be9f748bf9dd3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cc211a030fc003ae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ccebe3aae61e815d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cda5d652dd84d33e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cdbcf0e3d6af049
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ce12d8babbe0d5ed
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ce138eabc32ec47f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ce1bcb3c169d4d20
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ce31b144ca7de221
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cf2f8dc495152580
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/cf66bd1bb356fe33
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d0ed7606b979b6e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d10aabc932825e87
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d12283686bfafc1f
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d146ca24731df374
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d1e32904c5bdf84e
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d25a26fe1532fd03
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d2d9f5e60e291d83
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d34c979023267577
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d3df357e4ea4d715
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d3e13080f600608c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d4288bef0af4952b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d44d37b619ba6a6a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d4ebb9fedf208d02
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d527e9fbd4726df3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d58b4fb1b6e3fd7b
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d59558e277116736
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d68397ebd6398436
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d718e00764494b4d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d7bd113c19a70211
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d7e0e9b17173ffd4
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d87f15f99094c746
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d87fdb74181f2e2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d8cd637a74619889
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d9cad3b63fe41b52
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/d9fdc2b07697d273
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/da2b5b9536a29c68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/da652243bae84b9d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/da65889c16cb8f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/da95d58fd3380bda
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/da9e424af2a8568
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/db027fc934ad12f6
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/db319579930a6a93
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/db4c428ef6ef1edf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dbd768fa9f3941a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dbf7552319fdb2d3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dd1591c04ecabcd0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dd4e590ee10e42f0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dd56859c585a5393
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dd9482bf653962a9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ddd2dfa607c5a6bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dea82128b761959d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/df7a75baa9ec7267
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dfe35422871599b0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/dffd8488a2a6e55f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e05cc8e6955ee8f3
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e0a24a2f3d827eef
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e10005f877bb08c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e28f5b3ecf401b26
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e2dfcd44cdf50fd0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e35a5c82adbd7090
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e461910d3b5eac5c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e51fa57177e2ad76
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e5c6c3ec048de5f6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e6173d92e674e696
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e625af9efbdc5133
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e647bd0233886d8e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e66d6ed0df401d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e70ec4a4bb3a1969
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e7e59226bd435d91
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e843234b953a6a03
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e8e9a219bc223c8f
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e9573648e991150a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e974c6ed31e1d65e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/e9f8b6156d53bd2e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ea8b9fb99ac0af95
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/eaa0a03793f5d0e3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/eb0702f597720a18
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ebaf5f48125a341b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ebb81fbf28bfa1d1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ebe9c26b6904a9e5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ec13b0a74444a213
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ed1cfe51cabb9cb9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ed76f976fc2a1c6d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ed84669a7e1d404c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ede2ca89afe21d2c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ee48083f2472b478
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/eec5292955e2d066
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ef5f47a8927b7b2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/efacccd107c2c85d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f00b6cc692537065
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f013348e63cda51b
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f099f9eb1c1147dd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f0e73f0ffe4f8a54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f16cbf3f44838247
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f1dcd1d126eb496d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f260db2f43976947
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f30748b819632f47
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f33c31ff32648a9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f348ab358d9b7de
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f354ce77777a3fde
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f3cf2997b679d495
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f3d96d8308757109
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f40ea8bf36de723c
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f5279ed90efcf646
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f66a9fa79f4d7308
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f7ea55172ca94eb3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f7f9370b073af185
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8201f2ca19e4869
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8555aa61dbc2fce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f85570f88b516821
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f879391990362a70
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8a837df92925af5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8ade57ef4283255
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8d44c5e02d0eb79
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f8f0f3f907b5850d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f968f9dab2c2b3e5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f98c67dfc848c0db
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f9a04332e8111e68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/f9f85066ae805a2f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fbaf5254f3311546
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fbc91714867d451c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fbcd1c17003d9a1e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fc24ade5ce6e49f0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fd7e535bf6c11893
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fe36ee4cd1811680
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ff1f1a537133e073
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/ff3aa8bd3801d02
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 starmallow-0.3.8/.ruff_cache/content/fff88bec3f6cb70d
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 starmallow-0.3.8/docs/design_ideas.md
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 starmallow-0.3.8/examples/flask_server.py
--rw-r--r--   0        0        0    11887 2020-02-02 00:00:00.000000 starmallow-0.3.8/examples/goals.ipynb
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 starmallow-0.3.8/examples/recommended_server.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 starmallow-0.3.8/examples/sample_server.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/__init__.py
--rw-r--r--   0        0        0    29708 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/applications.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/concurrency.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/constants.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/dataclasses.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/datastructures.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/decorators.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/delimited_field.py
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/docs.py
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/endpoint.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/endpoints.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/exception_handlers.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/exceptions.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/fields.py
--rw-r--r--   0        0        0     8661 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/params.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/request_resolver.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/responses.py
--rw-r--r--   0        0        0    39203 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/routing.py
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/schema_generator.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/serializers.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/types.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/utils.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/ext/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/ext/marshmallow/__init__.py
--rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/ext/marshmallow/openapi.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/middleware/__init__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/middleware/asyncexitstack.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/__init__.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/api_key.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/base.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/http.py
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/oauth2.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 starmallow-0.3.8/starmallow/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/basic_api.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_properties.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_annotated.py
--rw-r--r--   0        0        0    85058 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_basic_api.py
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_dataclass_fields.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_delimited_params.py
--rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_http_endpoints.py
--rw-r--r--   0        0        0    35744 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_input.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_resolved_param_contextmanagers.py
--rw-r--r--   0        0        0     9902 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_resolved_params.py
--rw-r--r--   0        0        0    19565 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_responses.py
--rw-r--r--   0        0        0    20361 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_responses_orjson.py
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_responses_ujson.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/test_ws_router.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/__init__.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_cookie.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_cookie_description.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_header.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_header_description.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_header_optional.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_query.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_query_description.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/api_key/test_api_key_query_optional.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/__init__.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_base.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_base_description.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_base_optional.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_basic.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_basic_realm.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_basic_realm_description.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_bearer.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_bearer_description.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_bearer_optional.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_digest.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_digest_description.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/http/test_http_digest_optional.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/__init__.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_optional.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_optional_description.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/oauth2/test_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/openid_connect/__init__.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/openid_connect/test_openid_connect.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/openid_connect/test_openid_connect_description.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 starmallow-0.3.8/tests/security/openid_connect/test_openid_connect_optional.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 starmallow-0.3.8/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 starmallow-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 starmallow-0.3.8/README.md
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starmallow-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 starmallow-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 starmallow-0.3.9/.editorconfig
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 starmallow-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/missing_stubs
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   196607 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    47071 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    63544 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19761 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   187674 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   124955 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0    89659 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    27152 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    25958 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    55199 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    68518 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    22330 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    66362 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0    17864 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/base64.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/base64.meta.json
+-rw-r--r--   0        0        0    12622 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/binascii.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/binascii.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1223723 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   134946 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   119157 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    41316 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    12976 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    63393 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   154734 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    68679 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    76205 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0    98670 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   139269 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    24385 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    34863 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0   351931 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    93244 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   150002 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ipaddress.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ipaddress.meta.json
+-rw-r--r--   0        0        0   292334 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0    57518 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/mimetypes.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/mimetypes.meta.json
+-rw-r--r--   0        0        0    25529 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    53932 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    93805 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    48536 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    82093 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0    33277 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0   183320 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    55862 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0    82871 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    30752 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    54025 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   206015 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    30288 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   183933 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   173202 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   127577 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    70524 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    41353 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    62107 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0   260892 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   461606 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    56451 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    46000 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0    36687 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    25973 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   156299 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    96961 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/__init__.data.json
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/__init__.meta.json
+-rw-r--r--   0        0        0    74630 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/from_thread.data.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/from_thread.meta.json
+-rw-r--r--   0        0        0    33526 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/lowlevel.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/lowlevel.meta.json
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/to_thread.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/to_thread.meta.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/__init__.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/__init__.meta.json
+-rw-r--r--   0        0        0    52701 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_compat.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_compat.meta.json
+-rw-r--r--   0        0        0    14221 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_eventloop.data.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_exceptions.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json
+-rw-r--r--   0        0        0   131665 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_fileio.data.json
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_fileio.meta.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_resources.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_resources.meta.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_signals.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_signals.meta.json
+-rw-r--r--   0        0        0    36737 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_sockets.data.json
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_sockets.meta.json
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_streams.data.json
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_streams.meta.json
+-rw-r--r--   0        0        0     8619 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json
+-rw-r--r--   0        0        0    85851 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_synchronization.data.json
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json
+-rw-r--r--   0        0        0    23840 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_tasks.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_tasks.meta.json
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_testing.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_testing.meta.json
+-rw-r--r--   0        0        0    17868 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_typedattr.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/__init__.data.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/__init__.meta.json
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_resources.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_resources.meta.json
+-rw-r--r--   0        0        0    33875 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_sockets.data.json
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_sockets.meta.json
+-rw-r--r--   0        0        0    42234 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_streams.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_streams.meta.json
+-rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json
+-rw-r--r--   0        0        0    19889 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_tasks.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_tasks.meta.json
+-rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_testing.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_testing.meta.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/__init__.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/__init__.meta.json
+-rw-r--r--   0        0        0    66349 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/memory.data.json
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/memory.meta.json
+-rw-r--r--   0        0        0    42462 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/stapled.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/stapled.meta.json
+-rw-r--r--   0        0        0    41738 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/tls.data.json
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/tls.meta.json
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   113313 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/constants.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/constants.meta.json
+-rw-r--r--   0        0        0    24738 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   218488 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0    10647 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    41804 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    22666 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/proactor_events.data.json
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/proactor_events.meta.json
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    25185 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36293 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    26301 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   111214 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    29759 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    36902 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_events.data.json
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_events.meta.json
+-rw-r--r--   0        0        0    21829 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_utils.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_utils.meta.json
+-rw-r--r--   0        0        0   446252 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    65889 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    65947 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    23805 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   149492 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    13275 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26988 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    86480 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    24377 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/utils.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/email/utils.meta.json
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0    25265 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/__init__.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/__init__.meta.json
+-rw-r--r--   0        0        0    71988 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/client.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/client.meta.json
+-rw-r--r--   0        0        0    43680 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/cookies.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/http/cookies.meta.json
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/__init__.meta.json
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/core.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/core.meta.json
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/idnadata.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/idnadata.meta.json
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/intranges.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/intranges.meta.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/package_data.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/package_data.meta.json
+-rw-r--r--   0        0        0   103203 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/uts46data.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/idna/uts46data.meta.json
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75966 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69929 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    98817 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   157576 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/__init__.data.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/__init__.meta.json
+-rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/base.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/base.meta.json
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/class_registry.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/class_registry.meta.json
+-rw-r--r--   0        0        0    19019 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/decorators.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/decorators.meta.json
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/error_store.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/error_store.meta.json
+-rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/exceptions.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/exceptions.meta.json
+-rw-r--r--   0        0        0   193168 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/fields.data.json
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/fields.meta.json
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/orderedset.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/orderedset.meta.json
+-rw-r--r--   0        0        0    66078 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/schema.data.json
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/schema.meta.json
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/types.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/types.meta.json
+-rw-r--r--   0        0        0    30041 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/utils.data.json
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/utils.meta.json
+-rw-r--r--   0        0        0    77488 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/validate.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/validate.meta.json
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/warnings.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow/warnings.meta.json
+-rw-r--r--   0        0        0    41806 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/__init__.data.json
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/__init__.meta.json
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/collection_field.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/collection_field.meta.json
+-rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.meta.json
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/union_field.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/union_field.meta.json
+-rw-r--r--   0        0        0    33086 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    92565 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   160937 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    56122 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    19203 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    21449 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    31806 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    73266 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    27889 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    25639 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   258642 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    15115 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    71254 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/__init__.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/__init__.meta.json
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/_impl.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/_impl.meta.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/_version.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/sniffio/_version.meta.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/__init__.meta.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/_compat.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/_compat.meta.json
+-rw-r--r--   0        0        0    19689 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/_utils.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/_utils.meta.json
+-rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/applications.data.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/applications.meta.json
+-rw-r--r--   0        0        0    15001 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/background.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/background.meta.json
+-rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/concurrency.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/concurrency.meta.json
+-rw-r--r--   0        0        0    20566 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/convertors.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/convertors.meta.json
+-rw-r--r--   0        0        0   133761 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/datastructures.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/datastructures.meta.json
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/exceptions.data.json
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/exceptions.meta.json
+-rw-r--r--   0        0        0    31022 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/formparsers.data.json
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/formparsers.meta.json
+-rw-r--r--   0        0        0    49872 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/requests.data.json
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/requests.meta.json
+-rw-r--r--   0        0        0    38218 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/responses.data.json
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/responses.meta.json
+-rw-r--r--   0        0        0   104345 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/routing.data.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/routing.meta.json
+-rw-r--r--   0        0        0    40113 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/schemas.data.json
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/schemas.meta.json
+-rw-r--r--   0        0        0    26999 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/status.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/status.meta.json
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/types.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/types.meta.json
+-rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/websockets.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/websockets.meta.json
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/__init__.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/__init__.meta.json
+-rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/base.data.json
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/base.meta.json
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/errors.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/errors.meta.json
+-rw-r--r--   0        0        0    15378 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/exceptions.data.json
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/constants.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/constants.meta.json
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/datastructures.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/datastructures.meta.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/ext/__init__.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/ext/__init__.meta.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/__init__.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/__init__.meta.json
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/utils.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/utils.meta.json
+-rw-r--r--   0        0        0     6698 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26142 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   230086 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    15877 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12750 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    22405 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   166266 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 starmallow-0.3.9/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/10065f98add6ff0b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/109652e6f487f139
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1106bf394c2545f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/12b0bfced4f057e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/12d1bc2c3e3b4a83
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/139c88403d1436da
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/14baa50d760b85f4
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1516734ebe4cdf9e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/151fd4ca81800c29
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/15a4a56b6d885d72
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/169835d4ef6b2c76
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/174fbe9cb15ee3f5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/176c4bc33d477f1d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/17ca9af0f4e890c7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/17e6233e2c8b4c57
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/18d115039f810722
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/195be7e3cc61159d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/199a679ef9eca4bd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/19c4c1ec56600a9d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1b018c700a29eb6f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1b13d07e79be7008
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1b26045f7dbe2c85
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1bf76ae827ae0969
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1c4c20698345622a
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1c6b52f43e1f9ecf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1c8174d3fb6cfd4e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1d52da0fa1b46226
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1d5d931f005b2fdc
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1dd1a63493403b23
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1def590345254ce2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1e30b5622736e8a3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1e4c43773e562a1a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1e65a4edae7315f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1fbcf4cbb9a072d6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/1fc01fc4d329dab6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/20337f428fbbb1d8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/20fc180033536e0d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2127f1f3b00218f9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/21b97c5c1040e4c9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/21c8f3eeb3c07e96
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2262d3af001fa52
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2289427a3df44cb9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/22a479e6212e06c7
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/22e59ff54546802
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/233075a4f3a6966a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2485840abb576749
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2487af63be8b8306
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/249c82b6a73b5cfd
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/252b6dc2a81aef95
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2614de03a6ac0abe
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/262c1eb7a9069152
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/264bbc6647c0e341
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/268544df23daab8c
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/269e03795b762f8d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/26be189398dfa434
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2858eb97bacc4ed0
+-rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/287ddde3a6ca88a3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/29000d4e36a3bb35
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2937fde94e0481bd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2a8f2c618d9b68da
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2aa41b7defb4c2b4
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2b70e11145143c04
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2b84f3b60c3f4ce2
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2c5a467b39e90cbd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2ca403bf0fe46336
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2d5501076d63249d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2d66c86ed1832aa9
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2e0bd27ab75541a2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2e104a4d6d6c1cac
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2e1e9d73bdf26155
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2e531a3e4055c4a7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2eb7766d60702afc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/2f65fa8ebd69bb9f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3005f0cf358bc7e8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3034338d29bd0d2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/304637d7993de5f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/31fe912797f2f86
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3266c15c9bcda55d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/327e96f4d73223da
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/329ab05acd5391c4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/331cdf7bb4ec0b95
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/33351ddf7f6a55e0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3374f90390198332
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/338231b83975bd39
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/33e652e64f3581e8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/341e5cd078caef2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/345c1edda7fd4966
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/34c80c09b62c5a09
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/35b006b879963385
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/35b8d049779b1e8e
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/37500715047f4095
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/378f7e4eb0f96b0a
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/37a0895ad5a24844
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/37df1b78462054b9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/38a96cb0df513a62
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3928ea296d5bd126
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/39773375b92b92ea
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/39e422c0476f77f6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/39faf17634d3b691
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3a484f9c6d7a700a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3af5e30cd1f4b8ee
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3b0a0f9693e5b8ac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3bf82f696da70502
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3c66c25a2d6d8e46
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3ca218411159387e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3d5a8a89935df6a7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3e3190adfdc6ed6d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3f333473e057c20f
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3f65fba17c2c828e
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3fb764ea8e4e29de
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3fcd02df48e526dc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/3fcfafad557c3da2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4006f4513e986df3
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/402ef363ed6bacb6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/40376271cea804e8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/40da5e124435fc66
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4172f27f3e5a44e1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/41cdafe0ae37147
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/41e02c9c9fb737f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/434c97ad6ded852
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/43ad104541e0a88f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/43c4702dd09cf8f3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4443e21f99867067
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/447bdec362667066
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/44f0cc448324a416
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/45ce791d83e308e7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/460e8d9f60c9276b
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/46348294dcb5d2bd
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/46712eb880e5f2b2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/469a939cf6b8a62a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/46a7b9f2027e8f5f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/46bc616ae842a2fc
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/471a20b055a348ff
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/47c59c416ffc8ff6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/47f54a4e5f45b64e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/48d17bfe8ddb7a05
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4930d7c7bdcefdce
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4992d5421ef46439
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4ab811e0c66581a5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4adf7386e7952612
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4b14f4fab7bf7160
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4bae766eed40caea
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4cd9e6da2528969d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4d2d34a3b143e879
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4da55f94b6f612e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4db6335677cb3233
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4de60391dbe6e95b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4ead4839ff6c502f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4f08defd53d9e12f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4f4e6262d3319c76
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/4ffde77c1cebc6f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/504e081b6b86c34f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/50e9aa222b98e60b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/50eca8ea6523d687
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5108df00cee7c52a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/510f76af0881ae19
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5197297370819168
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5256d43574700b90
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/52740cf306398353
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5301160ed35ee24f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/53aee33a1e27a7d3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/53ecbb987fdf03cd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/53ef8d5b3de7027a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/542aa314ffb3e245
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/54ac7245c6762958
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/554655233635d77c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/56123b5402b9818f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/56165200cc754ff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/563735a7b8350845
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/57fc3c1eb8eab2d1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/581448974c8c2e1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/58273efa49032530
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/58914b1b2500fe96
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/58c885267ee0a5d1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/58f15b3440acd2bc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5943368bf2b067db
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/594a35ca98ca2998
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/598a265df09ca33f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5993d0b8f1292b73
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5a085e9801eea808
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5a5a5ab11a912f82
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5aaae113b6cc86f0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5ad09421f26d7e2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5aeb4d3c8194e4a0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5aec1e6c8cc2b524
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5d1fd97beca72c14
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5d3efad83bfd6258
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5d8fac59f0cec78c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5dbd91aa98e60d9a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5e40840c96aad063
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5ee600790e634e81
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5f404a0988062267
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5f62bc5e9923e06a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5f65edf15ca8de3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/5fe5a3ef3aff3394
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6008d98efeb1bd95
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/60b8d88975789254
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/60bd03468ffc65b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/60e3c198b607405a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6281d4777a34d609
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/62df83f800c42655
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6308ee5ec56b0229
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/634b930fb8219af7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/638ceb769f55bf50
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/639a3370ebbbf012
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/640098bfc7d282a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/64305ba858c272e5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/644126c2f14d4289
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6465889e66e3e70b
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/653086b13938658e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/65bf28f3ea69d129
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/66110399687da8c3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6645edcf399c84f5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/666d5411b3b1d958
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6739e9fb96a67266
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/67624662c5cfa7db
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/67bf5b1741c383f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/67f2a61223f52707
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/680cc717f698c4d0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6862ff8a8c81969
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/689c68a64edda297
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/691c8f2a6609f701
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/697923c62c1a93c1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/698b2b3de7f937b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/699f9bdce9c365cc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6a0e28959df807be
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6a8c6e2446a0e0f0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6ac9e8243f47c737
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6c8757e1fc9166d1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6d2b5b260f0c1cd1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6d4960a679856fde
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6dab5bbbf339e76a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6e75b37380d4a78d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6e769e3cc3adb24b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/6ed0f8f22ff2ea8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7055ae29f4533438
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/70a0005b296bc40a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7122a1fbe43b8a92
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7232884e4491b031
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/726fb633f05d7396
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/728a6af40ef75f0b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/72a1e90161c1b3ad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/72d35530b5713d8e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7343834aa4d9be43
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7352e8ece9e48014
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/737a5c2f20f0e563
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/737d8542b26d541c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/73be20a88210e1b0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/73d9a104cc256927
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/74d2f905ef324529
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7546ff395f02fce0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/755d4ac7664b4b84
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/75721927b265b00d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/757d1e107c70faa5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/75b06e7da441998c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/76e35a2d2488cd44
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7763d1c74d3f3d79
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/77708d5cb78dd07
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/77a6f45ccd9c5189
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/781434f33a0ce47d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7822a569cc3514a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/78465423b1393216
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/78dc0d9fb75505f6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/78e988cea0798964
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/78ebdb9690b23a48
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7994f6e4f513da81
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/79f9864468bb7c46
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7a1fa1b3a4cd21ec
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7aa94e8ec617f1ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7affc65075fff593
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7b196aff3b0d34e2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7b5d93007eefea0a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7bad7fcac6f8b588
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7c1898781cb9a71e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7c5d7683aa891ee0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7d025b8cbfc7ca82
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7d55b4761aca1221
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7d78a4ee1621e773
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7de8bf8e1dbae4ce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7e19739959663129
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7e1b459c54f96094
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7e36d76e73aaa50e
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7e54814a652afa6c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/7efc398adabd83d1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/819ba4aac88ad4c5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/821abfbe8996dfee
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/82af181b99ed362f
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/82c96a979ec45ed8
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/84c1c0b9ef5a0bd1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/859699dc827e64bd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/85d2aa90f441ac84
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/85f38c1e1a98b4ce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/85fc672825474a7e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/861ae70c60f4b515
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/863e0505e99b4912
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/868204f1007fa159
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/877a8374d55041a6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/87829d9f8a7970c3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8873ff56d0e35f6e
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/88b8af873f0d9b6a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/88c961d879ca8414
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/88db9b5f1f41d922
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/88df5cd35ee3b18b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/891cc4279db032f5
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/89c58146af7dd774
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/89dcd4c51a32910d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8a10752ada77f3da
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8a22cc9ac5a2ca05
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8b09af6a575d0128
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8b72587297729c97
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8c361c3048c9e03c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8c43c7a2cd04e833
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8c7b1a64e885ea22
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8cc4f00b5d755361
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8ccb15e75038ea9a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8d0e8223e6b4ccb8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8dcea8de9ad315a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8dee251c5e37502e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8f1565c9f27de57
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8f33fd6f86bd12b6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8f56bbb2a5a9d676
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/8f7ebfd14401571a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/906379e2c501a56f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/90cfd16b86df9d53
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/90dbc1fd08ac21c8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/90f78c6105477537
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9109516011be0efe
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/912ed319e99754d3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/91918d3958deff8a
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/92ccca9574be50d0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9303923bacc3dddb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9408c1595b56b385
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9442816411d7a40
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/94c4d3be2fbdce31
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/94f1fae028452aa4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/95851fc6ca36a564
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/95fa211029579181
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/963d7293fdfe61b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/965a17d45a914dcc
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/968749843c9c57e7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/980207d3fc07e68e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/981e38eb01988cf0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/98651da6fa50673a
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/986beeceff7436e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/98b1e360b558e80d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/98cad6932a3c67c3
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/992d4921e74a9030
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9959ffb4a33fa8eb
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/99dc8d8d36634b12
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9a0b35403acb1393
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9adb15a6742d6c5b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9ae8692e209e9c27
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9afeadccb73fbb4e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9b1cc72aefa30a9e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9b513dbbc3df1d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9b687e58fc1eb59f
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9b86335591fffcf1
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9b9a5ac90d2fab8d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9c477e944343f783
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9c50e4535eef3c1c
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9c720a051a865466
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9c809b5e7ea60ddf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9dd9baf20243b58b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9e574d7a8e334e38
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9edfaee2be42e198
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9f92d286a2c9f437
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/9fd95161096f3293
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a029c6d1c66ed345
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a02ffb962a1775ff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a048a3a84c65fc5a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a0666de0a0a6144e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a0d2b9d3f2819f04
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a0ea9ba2a1f3ac46
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a15a78db12299f05
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a1e3b889b6944ebc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a237a0e7f1942bf6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a25a50613ceceb15
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a25bc77eede1bc2b
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a278ff735bba2bd7
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a33190b6d5891f6f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a4ae48ae62f93e63
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a4c31e01eda226cf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a4ca9aac0340823a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a4ecfd8d7b2a05b1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a6389703eb1073dd
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a658af58aec4af00
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a6de514a8b333187
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a732b9acda145222
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a74c6e6de0087343
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a76aa6fa628e6e01
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a7c84faee2aef013
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a8064825516e7ed1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a93524573859e47
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a97d4e2e87bf7f0a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a98e56ec663ce742
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/a9ee35e28e552173
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/aab62ef2f0b61424
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/aae9fa55d6e694a1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ab0add8b5cb8772e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ab68f152b19cdbaa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ab7c16f4f92a5323
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/abcf1e5f80686ee5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ac2c2af7bed3210f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ac3540001bafc8d5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ac47082cb735457a
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/acb93c139a04adce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/acde528f5682578e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ad2ddab1a4a9ffa5
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/add1e3cb649188ee
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/aebe09bc5b7c0a0f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/aef437e818024f4e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/aefb1d1657f360bf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/af29f1e208841600
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/afb0cca1477e5dae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/afcae95aa44aaff4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b062ec76b33ad03e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b0a59f1097595518
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b10fb291ead98cc4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b15a64bf0b9296c1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b1dc6da3e82aeaeb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b1dceb4a4b40e486
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b2318a06449286b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b2cf3cdb44c18edf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b2fa10faf80c3d9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b3321c7dcb8681ea
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b3c3129957608740
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b437574d4bcee451
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b4bb01c4fc1406cf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b4cc050e59a22fd9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b60a9e948956196d
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b62f346ab1b9696f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b66d8d45fb1d3d36
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b6845876145bd198
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b6e38f34eea822d6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b6e8254c0f21e056
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b757d0f14dfc70b9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b795a29f637ec0bf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b7d1660c447af83d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b7e5485382e3da45
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b949882417ecfe1f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b9c3fb657e2899b5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/b9ed0232339ac16a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ba18502f0545eb06
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ba2f86bf75fec67d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bb56ec9e41027b47
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bb57e4d3c2509675
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bb759db627f4325
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bba3f7509c666e08
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bbb680356e35537b
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bbfade420b1078ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bc22f55ed8d52a4b
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bc2ec99feb4e9954
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bc757653ca011057
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bc7b268c6b194652
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bc85cb56fba2f6b9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bccc99e22d071034
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bcfea61c791fc274
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bd24213539411981
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bd4defc3d7670b36
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bd539245d4cac9ba
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bd7c61026703a0af
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bd7ee16910a7e4a6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bdc22adea1cb15d8
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/be90521730430f10
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bea6cce6e0520aff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bec86529de61c55e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bee8547360003ad7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bf28b0d53d6344a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bf74275c64c846e4
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bf767767343056e7
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/bf9a486d3cb01172
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c058a23b30a7c0a8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c083a6ea029de8d7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c0d10c81df8cce05
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c18c9aaf67596c6e
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c19418c2294bc7a0
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c21bef522b1327db
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c2a99a6e393c799a
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c312dc5879acf73b
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c32806f29722c480
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c441c960648d4cda
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c47681fb80798d61
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c4c1d17c7684dc2a
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c4e5ca2325c7548f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c563c8c53efb149d
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c5dbe9a612eb2b7a
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c6a45dcc88a5ae3d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c71f830573d0476f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c73e5aec75b4e0d9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c8354555d62ff86d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c8417fe0df58ee00
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c92cc8d023659eb
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c95731c0dcf23963
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c99e152a2241e5cc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c9d959d5764014e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c9db389e76b219bf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/c9f745e1bae9f680
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ca20ee2afd333a10
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ca2e8924391b3f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cb54ded01fe6b4f6
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cbe65e1002f5fd6c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cc0be9f748bf9dd3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cc211a030fc003ae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ccebe3aae61e815d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cda5d652dd84d33e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cdbcf0e3d6af049
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ce12d8babbe0d5ed
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ce138eabc32ec47f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ce1bcb3c169d4d20
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ce31b144ca7de221
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cf2f8dc495152580
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/cf66bd1bb356fe33
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d0ed7606b979b6e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d10aabc932825e87
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d12283686bfafc1f
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d146ca24731df374
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d1e32904c5bdf84e
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d25a26fe1532fd03
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d2d9f5e60e291d83
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d34c979023267577
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d3df357e4ea4d715
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d3e13080f600608c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d4288bef0af4952b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d44d37b619ba6a6a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d4ebb9fedf208d02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d527e9fbd4726df3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d58b4fb1b6e3fd7b
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d59558e277116736
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d68397ebd6398436
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d718e00764494b4d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d7bd113c19a70211
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d7e0e9b17173ffd4
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d87f15f99094c746
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d87fdb74181f2e2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d8cd637a74619889
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d9cad3b63fe41b52
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/d9fdc2b07697d273
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/da2b5b9536a29c68
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/da652243bae84b9d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/da65889c16cb8f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/da95d58fd3380bda
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/da9e424af2a8568
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/db027fc934ad12f6
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/db319579930a6a93
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/db4c428ef6ef1edf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dbd768fa9f3941a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dbf7552319fdb2d3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dd1591c04ecabcd0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dd4e590ee10e42f0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dd56859c585a5393
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dd9482bf653962a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ddd2dfa607c5a6bf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dea82128b761959d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/df7a75baa9ec7267
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dfe35422871599b0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/dffd8488a2a6e55f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e05cc8e6955ee8f3
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e0a24a2f3d827eef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e10005f877bb08c3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e28f5b3ecf401b26
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e2dfcd44cdf50fd0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e35a5c82adbd7090
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e461910d3b5eac5c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e51fa57177e2ad76
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e5c6c3ec048de5f6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e6173d92e674e696
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e625af9efbdc5133
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e647bd0233886d8e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e66d6ed0df401d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e70ec4a4bb3a1969
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e7e59226bd435d91
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e843234b953a6a03
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e8e9a219bc223c8f
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e9573648e991150a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e974c6ed31e1d65e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/e9f8b6156d53bd2e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ea8b9fb99ac0af95
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/eaa0a03793f5d0e3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/eb0702f597720a18
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ebaf5f48125a341b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ebb81fbf28bfa1d1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ebe9c26b6904a9e5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ec13b0a74444a213
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ed1cfe51cabb9cb9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ed76f976fc2a1c6d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ed84669a7e1d404c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ede2ca89afe21d2c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ee48083f2472b478
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/eec5292955e2d066
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ef5f47a8927b7b2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/efacccd107c2c85d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f00b6cc692537065
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f013348e63cda51b
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f099f9eb1c1147dd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f0e73f0ffe4f8a54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f16cbf3f44838247
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f1dcd1d126eb496d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f260db2f43976947
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f30748b819632f47
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f33c31ff32648a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f348ab358d9b7de
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f354ce77777a3fde
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f3cf2997b679d495
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f3d96d8308757109
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f40ea8bf36de723c
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f5279ed90efcf646
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f66a9fa79f4d7308
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f7ea55172ca94eb3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f7f9370b073af185
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8201f2ca19e4869
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8555aa61dbc2fce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f85570f88b516821
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f879391990362a70
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8a837df92925af5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8ade57ef4283255
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8d44c5e02d0eb79
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f8f0f3f907b5850d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f968f9dab2c2b3e5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f98c67dfc848c0db
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f9a04332e8111e68
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/f9f85066ae805a2f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fbaf5254f3311546
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fbc91714867d451c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fbcd1c17003d9a1e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fc24ade5ce6e49f0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fd7e535bf6c11893
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fe36ee4cd1811680
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ff1f1a537133e073
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/ff3aa8bd3801d02
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 starmallow-0.3.9/.ruff_cache/content/fff88bec3f6cb70d
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 starmallow-0.3.9/docs/design_ideas.md
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 starmallow-0.3.9/examples/flask_server.py
+-rw-r--r--   0        0        0    11887 2020-02-02 00:00:00.000000 starmallow-0.3.9/examples/goals.ipynb
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 starmallow-0.3.9/examples/recommended_server.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 starmallow-0.3.9/examples/sample_server.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/__init__.py
+-rw-r--r--   0        0        0    29708 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/applications.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/concurrency.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/constants.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/dataclasses.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/datastructures.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/decorators.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/delimited_field.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/docs.py
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/endpoint.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/endpoints.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/exception_handlers.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/exceptions.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/fields.py
+-rw-r--r--   0        0        0     8661 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/params.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/request_resolver.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/responses.py
+-rw-r--r--   0        0        0    39203 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/routing.py
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/schema_generator.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/serializers.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/types.py
+-rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/utils.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/ext/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/ext/marshmallow/__init__.py
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/ext/marshmallow/openapi.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/middleware/__init__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/__init__.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/api_key.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/base.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/http.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/oauth2.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 starmallow-0.3.9/starmallow/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/basic_api.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_annotated.py
+-rw-r--r--   0        0        0    85058 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_basic_api.py
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_dataclass_fields.py
+-rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_delimited_params.py
+-rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_http_endpoints.py
+-rw-r--r--   0        0        0    35744 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_input.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_resolved_param_contextmanagers.py
+-rw-r--r--   0        0        0     9902 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_resolved_params.py
+-rw-r--r--   0        0        0    19565 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_responses.py
+-rw-r--r--   0        0        0    20361 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_responses_orjson.py
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_responses_ujson.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/test_ws_router.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_cookie.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_header.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_header_description.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_header_optional.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_query.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_query_description.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/api_key/test_api_key_query_optional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/__init__.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_base.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_base_description.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_base_optional.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_basic.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_basic_realm.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_bearer.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_bearer_description.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_bearer_optional.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_digest.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_digest_description.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/http/test_http_digest_optional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_optional.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/oauth2/test_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/openid_connect/test_openid_connect.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/openid_connect/test_openid_connect_description.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 starmallow-0.3.9/tests/security/openid_connect/test_openid_connect_optional.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 starmallow-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 starmallow-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 starmallow-0.3.9/README.md
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starmallow-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 starmallow-0.3.9/PKG-INFO
```

### Comparing `starmallow-0.3.8/.pre-commit-config.yaml` & `starmallow-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/__future__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/__future__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_ast.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_ast.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_bisect.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_bisect.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_codecs.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_codecs.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_collections_abc.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_collections_abc.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_ctypes.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_ctypes.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_decimal.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_decimal.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_operator.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_operator.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_socket.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_socket.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_stat.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_stat.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_thread.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_thread.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_warnings.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_warnings.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_weakref.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_weakref.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_weakrefset.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_weakrefset.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_winapi.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_winapi.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/abc.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/abc.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/array.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/array.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/base64.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/base64.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/base64.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/base64.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/binascii.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/binascii.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/binascii.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/binascii.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/bisect.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/bisect.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/builtins.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/builtins.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/codecs.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/codecs.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/contextlib.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/contextlib.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/contextvars.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/contextvars.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/copy.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/copy.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/copyreg.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/copyreg.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/dataclasses.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/dataclasses.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/datetime.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/datetime.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/decimal.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/decimal.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/dis.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/dis.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/doctest.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/doctest.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/enum.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/enum.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/functools.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/functools.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/genericpath.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/genericpath.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/hashlib.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/hashlib.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/inspect.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/inspect.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/io.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/io.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ipaddress.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/ipaddress.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ipaddress.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/ipaddress.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/itertools.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/itertools.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/math.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/math.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/mimetypes.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/mimetypes.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/mimetypes.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/mimetypes.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/mmap.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/mmap.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ntpath.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ntpath.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/numbers.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/numbers.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/opcode.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/opcode.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/operator.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/operator.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pathlib.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pathlib.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pickle.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pickle.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/posixpath.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/posixpath.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pprint.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/pprint.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/queue.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/queue.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/re.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/re.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/selectors.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/selectors.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/shlex.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/shlex.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/signal.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/signal.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/socket.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/socket.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_compile.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_compile.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_constants.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_constants.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_parse.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sre_parse.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ssl.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ssl.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/stat.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/stat.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/string.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/string.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/subprocess.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/subprocess.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sys.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sys.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/tempfile.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/tempfile.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/threading.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/threading.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/time.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/time.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/traceback.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/traceback.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/types.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/types.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/typing.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/typing.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/typing_extensions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/typing_extensions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unicodedata.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unicodedata.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/uuid.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/uuid.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/warnings.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/warnings.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/weakref.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/weakref.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_typeshed/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/from_thread.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/from_thread.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/from_thread.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/from_thread.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/lowlevel.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/lowlevel.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/lowlevel.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/lowlevel.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/to_thread.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/to_thread.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/to_thread.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/to_thread.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_compat.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_compat.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_compat.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_eventloop.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_eventloop.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_eventloop.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_exceptions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_fileio.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_fileio.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_fileio.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_fileio.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_resources.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_resources.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_resources.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_resources.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_signals.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_signals.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_signals.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_signals.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_sockets.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_sockets.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_sockets.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_sockets.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_streams.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_streams.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_streams.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_streams.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_subprocesses.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_subprocesses.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_synchronization.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_synchronization.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_synchronization.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_tasks.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_tasks.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_tasks.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_tasks.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_testing.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_testing.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_testing.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_testing.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_typedattr.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_typedattr.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/_core/_typedattr.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_resources.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_resources.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_resources.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_resources.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_sockets.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_sockets.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_sockets.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_sockets.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_streams.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_streams.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_streams.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_streams.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_subprocesses.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_subprocesses.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_tasks.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_tasks.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_tasks.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_tasks.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_testing.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_testing.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/abc/_testing.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/abc/_testing.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/memory.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/memory.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/memory.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/memory.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/stapled.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/stapled.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/stapled.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/stapled.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/tls.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/tls.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/anyio/streams/tls.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/anyio/streams/tls.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/base_events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/base_events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/constants.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/constants.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/constants.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/constants.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/coroutines.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/exceptions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/futures.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/futures.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/locks.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/locks.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/mixins.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/mixins.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/proactor_events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/proactor_events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/proactor_events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/proactor_events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/protocols.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/protocols.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/queues.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/queues.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/runners.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/runners.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/selector_events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/streams.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/streams.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/subprocess.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/tasks.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/tasks.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/threads.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/threads.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/timeouts.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/transports.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/transports.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/unix_events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_events.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_events.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_events.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_events.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_utils.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_utils.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/asyncio/windows_utils.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/asyncio/windows_utils.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/collections/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/collections/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/collections/abc.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/collections/abc.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/process.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ctypes/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/ctypes/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/charset.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/charset.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/contentmanager.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/contentmanager.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/errors.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/errors.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/header.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/header.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/message.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/message.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/policy.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/policy.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/utils.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/utils.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/email/utils.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/email/utils.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/html/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/html/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/client.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/client.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/client.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/client.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/cookies.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/cookies.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/http/cookies.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/http/cookies.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/core.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/core.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/core.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/core.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/idnadata.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/idnadata.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/idnadata.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/idnadata.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/intranges.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/intranges.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/intranges.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/intranges.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/package_data.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/package_data.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/package_data.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/package_data.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/uts46data.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/uts46data.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/idna/uts46data.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/idna/uts46data.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/abc.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/abc.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/machinery.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/machinery.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/decoder.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/decoder.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/encoder.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/json/encoder.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/logging/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/logging/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/base.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/base.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/base.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/base.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/class_registry.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/class_registry.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/class_registry.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/class_registry.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/decorators.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/decorators.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/decorators.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/error_store.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/error_store.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/error_store.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/error_store.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/exceptions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/exceptions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/fields.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/fields.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/fields.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/fields.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/orderedset.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/orderedset.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/orderedset.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/orderedset.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/schema.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/schema.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/schema.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/schema.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/types.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/types.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/types.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/types.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/utils.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/utils.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/utils.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/utils.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/validate.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/validate.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/validate.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/validate.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/warnings.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/warnings.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow/warnings.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/collection_field.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/collection_field.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/collection_field.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/collection_field.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/lazy_class_attribute.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/union_field.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/union_field.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/marshmallow_dataclass/union_field.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/marshmallow_dataclass/union_field.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/connection.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/context.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/context.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/managers.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/pool.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/process.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/process.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/queues.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/util.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/multiprocessing/util.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/os/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/os/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/os/path.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/os/path.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/_structures.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/_structures.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/version.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/packaging/version.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/_impl.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/_impl.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/_impl.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/_impl.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/_version.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/_version.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/sniffio/_version.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/sniffio/_version.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/_compat.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/_compat.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/_compat.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/_utils.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/_utils.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/_utils.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/applications.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/applications.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/applications.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/applications.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/background.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/background.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/background.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/background.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/concurrency.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/concurrency.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/convertors.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/convertors.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/convertors.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/convertors.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/datastructures.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/datastructures.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/datastructures.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/datastructures.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/exceptions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/exceptions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/formparsers.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/formparsers.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/formparsers.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/formparsers.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/requests.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/requests.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/requests.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/requests.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/responses.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/responses.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/responses.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/responses.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/routing.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/routing.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/routing.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/routing.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/schemas.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/schemas.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/schemas.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/schemas.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/status.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/status.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/status.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/status.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/types.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/types.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/types.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/types.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/websockets.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/websockets.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/websockets.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/websockets.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/base.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/base.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/base.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/base.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/errors.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/errors.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/errors.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/errors.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/exceptions.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starlette/middleware/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/constants.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/constants.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/constants.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/constants.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/datastructures.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/datastructures.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/datastructures.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/datastructures.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/ext/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/ext/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/ext/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/ext/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/utils.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/utils.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/starmallow/security/utils.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/starmallow/security/utils.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/_log.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/_log.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/async_case.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/async_case.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/case.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/case.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/loader.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/loader.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/main.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/main.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/result.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/result.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/runner.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/runner.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/signals.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/signals.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/suite.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/unittest/suite.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/urllib/__init__.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/urllib/__init__.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/urllib/parse.data.json` & `starmallow-0.3.9/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.mypy_cache/3.11/urllib/parse.meta.json` & `starmallow-0.3.9/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/249c82b6a73b5cfd` & `starmallow-0.3.9/.ruff_cache/content/249c82b6a73b5cfd`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/252b6dc2a81aef95` & `starmallow-0.3.9/.ruff_cache/content/252b6dc2a81aef95`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/287ddde3a6ca88a3` & `starmallow-0.3.9/.ruff_cache/content/287ddde3a6ca88a3`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/2c5a467b39e90cbd` & `starmallow-0.3.9/.ruff_cache/content/2c5a467b39e90cbd`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/35b006b879963385` & `starmallow-0.3.9/.ruff_cache/content/35b006b879963385`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/3f65fba17c2c828e` & `starmallow-0.3.9/.ruff_cache/content/3f65fba17c2c828e`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/3fb764ea8e4e29de` & `starmallow-0.3.9/.ruff_cache/content/3fb764ea8e4e29de`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/46712eb880e5f2b2` & `starmallow-0.3.9/.ruff_cache/content/46712eb880e5f2b2`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/47c59c416ffc8ff6` & `starmallow-0.3.9/.ruff_cache/content/47c59c416ffc8ff6`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/57fc3c1eb8eab2d1` & `starmallow-0.3.9/.ruff_cache/content/57fc3c1eb8eab2d1`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/82c96a979ec45ed8` & `starmallow-0.3.9/.ruff_cache/content/82c96a979ec45ed8`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/89c58146af7dd774` & `starmallow-0.3.9/.ruff_cache/content/89c58146af7dd774`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/968749843c9c57e7` & `starmallow-0.3.9/.ruff_cache/content/968749843c9c57e7`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/9b86335591fffcf1` & `starmallow-0.3.9/.ruff_cache/content/9b86335591fffcf1`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/9b9a5ac90d2fab8d` & `starmallow-0.3.9/.ruff_cache/content/9b9a5ac90d2fab8d`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/a1e3b889b6944ebc` & `starmallow-0.3.9/.ruff_cache/content/a1e3b889b6944ebc`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/a278ff735bba2bd7` & `starmallow-0.3.9/.ruff_cache/content/a278ff735bba2bd7`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/a33190b6d5891f6f` & `starmallow-0.3.9/.ruff_cache/content/a33190b6d5891f6f`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/b4bb01c4fc1406cf` & `starmallow-0.3.9/.ruff_cache/content/b4bb01c4fc1406cf`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/b62f346ab1b9696f` & `starmallow-0.3.9/.ruff_cache/content/b62f346ab1b9696f`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/bbfade420b1078ed` & `starmallow-0.3.9/.ruff_cache/content/bbfade420b1078ed`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/c18c9aaf67596c6e` & `starmallow-0.3.9/.ruff_cache/content/c18c9aaf67596c6e`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/c21bef522b1327db` & `starmallow-0.3.9/.ruff_cache/content/c21bef522b1327db`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/c312dc5879acf73b` & `starmallow-0.3.9/.ruff_cache/content/c312dc5879acf73b`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/c32806f29722c480` & `starmallow-0.3.9/.ruff_cache/content/c32806f29722c480`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/c47681fb80798d61` & `starmallow-0.3.9/.ruff_cache/content/c47681fb80798d61`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/ce12d8babbe0d5ed` & `starmallow-0.3.9/.ruff_cache/content/ce12d8babbe0d5ed`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/ce138eabc32ec47f` & `starmallow-0.3.9/.ruff_cache/content/ce138eabc32ec47f`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/d25a26fe1532fd03` & `starmallow-0.3.9/.ruff_cache/content/d25a26fe1532fd03`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/db319579930a6a93` & `starmallow-0.3.9/.ruff_cache/content/db319579930a6a93`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/e625af9efbdc5133` & `starmallow-0.3.9/.ruff_cache/content/e625af9efbdc5133`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/e9573648e991150a` & `starmallow-0.3.9/.ruff_cache/content/e9573648e991150a`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/ebaf5f48125a341b` & `starmallow-0.3.9/.ruff_cache/content/ebaf5f48125a341b`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/f013348e63cda51b` & `starmallow-0.3.9/.ruff_cache/content/f013348e63cda51b`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/f3d96d8308757109` & `starmallow-0.3.9/.ruff_cache/content/f3d96d8308757109`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/f7ea55172ca94eb3` & `starmallow-0.3.9/.ruff_cache/content/f7ea55172ca94eb3`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/f8201f2ca19e4869` & `starmallow-0.3.9/.ruff_cache/content/f8201f2ca19e4869`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/f8d44c5e02d0eb79` & `starmallow-0.3.9/.ruff_cache/content/f8d44c5e02d0eb79`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/ff3aa8bd3801d02` & `starmallow-0.3.9/.ruff_cache/content/ff3aa8bd3801d02`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.ruff_cache/content/fff88bec3f6cb70d` & `starmallow-0.3.9/.ruff_cache/content/fff88bec3f6cb70d`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/docs/design_ideas.md` & `starmallow-0.3.9/docs/design_ideas.md`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/examples/flask_server.py` & `starmallow-0.3.9/examples/flask_server.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/examples/goals.ipynb` & `starmallow-0.3.9/examples/goals.ipynb`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/examples/recommended_server.py` & `starmallow-0.3.9/examples/recommended_server.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/examples/sample_server.py` & `starmallow-0.3.9/examples/sample_server.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/applications.py` & `starmallow-0.3.9/starmallow/applications.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/concurrency.py` & `starmallow-0.3.9/starmallow/concurrency.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/dataclasses.py` & `starmallow-0.3.9/starmallow/dataclasses.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/datastructures.py` & `starmallow-0.3.9/starmallow/datastructures.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/decorators.py` & `starmallow-0.3.9/starmallow/decorators.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/delimited_field.py` & `starmallow-0.3.9/starmallow/delimited_field.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/docs.py` & `starmallow-0.3.9/starmallow/docs.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/endpoint.py` & `starmallow-0.3.9/starmallow/endpoint.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/endpoints.py` & `starmallow-0.3.9/starmallow/endpoints.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/exception_handlers.py` & `starmallow-0.3.9/starmallow/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/exceptions.py` & `starmallow-0.3.9/starmallow/exceptions.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/fields.py` & `starmallow-0.3.9/starmallow/fields.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/params.py` & `starmallow-0.3.9/starmallow/params.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/request_resolver.py` & `starmallow-0.3.9/starmallow/request_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,33 +265,33 @@
         request,
         response,
         background_tasks,
         params.get(ParamType.security),
         dependency_cache=dependency_cache,
     )
     if errors:
-        return None, errors, background_tasks
+        return None, errors, background_tasks, response
 
     arg_values, errors = await resolve_basic_args(
         request,
         response,
         background_tasks,
         params,
     )
     if errors:
-        return None, errors, background_tasks
+        return None, errors, background_tasks, response
 
     resolved_values, errors = await resolve_subparams(
         request,
         response,
         background_tasks,
         params.get(ParamType.resolved),
         dependency_cache=dependency_cache,
     )
     if errors:
-        return None, errors, background_tasks
+        return None, errors, background_tasks, response
 
     return {
         **security_values,
         **arg_values,
         **resolved_values,
     }, {}, background_tasks, response
```

### Comparing `starmallow-0.3.8/starmallow/responses.py` & `starmallow-0.3.9/starmallow/responses.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/routing.py` & `starmallow-0.3.9/starmallow/routing.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/schema_generator.py` & `starmallow-0.3.9/starmallow/schema_generator.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/serializers.py` & `starmallow-0.3.9/starmallow/serializers.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/types.py` & `starmallow-0.3.9/starmallow/types.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/utils.py` & `starmallow-0.3.9/starmallow/utils.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/websockets.py` & `starmallow-0.3.9/starmallow/websockets.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/ext/marshmallow/openapi.py` & `starmallow-0.3.9/starmallow/ext/marshmallow/openapi.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/middleware/asyncexitstack.py` & `starmallow-0.3.9/starmallow/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/security/api_key.py` & `starmallow-0.3.9/starmallow/security/api_key.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/security/base.py` & `starmallow-0.3.9/starmallow/security/base.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/security/http.py` & `starmallow-0.3.9/starmallow/security/http.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/security/oauth2.py` & `starmallow-0.3.9/starmallow/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/starmallow/security/open_id_connect_url.py` & `starmallow-0.3.9/starmallow/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/basic_api.py` & `starmallow-0.3.9/tests/basic_api.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_properties.py` & `starmallow-0.3.9/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_response_extra.py` & `starmallow-0.3.9/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_bad.py` & `starmallow-0.3.9/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_custom_model_in_callback.py` & `starmallow-0.3.9/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_custom_validationerror.py` & `starmallow-0.3.9/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_default_validationerror.py` & `starmallow-0.3.9/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_response_class.py` & `starmallow-0.3.9/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_additional_responses_router.py` & `starmallow-0.3.9/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_annotated.py` & `starmallow-0.3.9/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_basic_api.py` & `starmallow-0.3.9/tests/test_basic_api.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_dataclass_fields.py` & `starmallow-0.3.9/tests/test_dataclass_fields.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_delimited_params.py` & `starmallow-0.3.9/tests/test_delimited_params.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_http_endpoints.py` & `starmallow-0.3.9/tests/test_http_endpoints.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_input.py` & `starmallow-0.3.9/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_resolved_param_contextmanagers.py` & `starmallow-0.3.9/tests/test_resolved_param_contextmanagers.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_resolved_params.py` & `starmallow-0.3.9/tests/test_resolved_params.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_responses.py` & `starmallow-0.3.9/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_responses_orjson.py` & `starmallow-0.3.9/tests/test_responses_orjson.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_responses_ujson.py` & `starmallow-0.3.9/tests/test_responses_ujson.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/test_ws_router.py` & `starmallow-0.3.9/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/utils.py` & `starmallow-0.3.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_cookie.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_cookie_description.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_cookie_optional.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_header.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_header.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_header_description.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_header_optional.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_query.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_query.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_query_description.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/api_key/test_api_key_query_optional.py` & `starmallow-0.3.9/tests/security/api_key/test_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_base.py` & `starmallow-0.3.9/tests/security/http/test_http_base.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_base_description.py` & `starmallow-0.3.9/tests/security/http/test_http_base_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_base_optional.py` & `starmallow-0.3.9/tests/security/http/test_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_basic.py` & `starmallow-0.3.9/tests/security/http/test_http_basic.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_basic_realm.py` & `starmallow-0.3.9/tests/security/http/test_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_basic_realm_description.py` & `starmallow-0.3.9/tests/security/http/test_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_bearer.py` & `starmallow-0.3.9/tests/security/http/test_http_bearer.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_bearer_description.py` & `starmallow-0.3.9/tests/security/http/test_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_bearer_optional.py` & `starmallow-0.3.9/tests/security/http/test_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_digest.py` & `starmallow-0.3.9/tests/security/http/test_http_digest.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_digest_description.py` & `starmallow-0.3.9/tests/security/http/test_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/http/test_http_digest_optional.py` & `starmallow-0.3.9/tests/security/http/test_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_authorization_code_bearer.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_authorization_code_bearer_description.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_optional.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_optional_description.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_password_bearer_optional.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/oauth2/test_oauth2_password_bearer_optional_description.py` & `starmallow-0.3.9/tests/security/oauth2/test_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/openid_connect/test_openid_connect.py` & `starmallow-0.3.9/tests/security/openid_connect/test_openid_connect.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/openid_connect/test_openid_connect_description.py` & `starmallow-0.3.9/tests/security/openid_connect/test_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/tests/security/openid_connect/test_openid_connect_optional.py` & `starmallow-0.3.9/tests/security/openid_connect/test_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/.gitignore` & `starmallow-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/LICENSE.md` & `starmallow-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/README.md` & `starmallow-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/pyproject.toml` & `starmallow-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starmallow-0.3.8/PKG-INFO` & `starmallow-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmallow
-Version: 0.3.8
+Version: 0.3.9
 Summary: StarMallow framework
 Project-URL: Homepage, https://github.com/mvanderlee/starmallow
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

