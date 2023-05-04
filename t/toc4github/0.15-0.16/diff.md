# Comparing `tmp/toc4github-0.15.tar.gz` & `tmp/toc4github-0.16.tar.gz`

## Comparing `toc4github-0.15.tar` & `toc4github-0.16.tar`

### file list

```diff
@@ -1,8 +1,137 @@
--rw-r--r--   0        0        0    29526 2020-02-02 00:00:00.000000 toc4github-0.15/screenshot.png
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 toc4github-0.15/toc4github.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 toc4github-0.15/tox.ini
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 toc4github-0.15/utest.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 toc4github-0.15/LICENSE
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 toc4github-0.15/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 toc4github-0.15/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 toc4github-0.15/PKG-INFO
+-rw-r--r--   0        0        0    29526 2020-02-02 00:00:00.000000 toc4github-0.16/showcase.png
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 toc4github-0.16/toc4github.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 toc4github-0.16/tox.ini
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 toc4github-0.16/utest.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   184668 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    54018 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    25212 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    21815 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0   157895 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0        0        0    62680 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1076982 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   125940 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   111328 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    64094 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0   136025 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    90763 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    92281 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48616 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    80867 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   151140 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15077 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    29704 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53062 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    25999 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   168154 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   142709 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    69238 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    46030 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0     7022 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/toc4github.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/toc4github.meta.json
+-rw-r--r--   0        0        0   264769 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   428246 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    56483 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/utest.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/utest.meta.json
+-rw-r--r--   0        0        0    23539 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    89735 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   380630 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   138825 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     8339 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24975 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    59282 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    32617 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    76266 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69583 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    94434 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   151244 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0   366593 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    25735 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   220792 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12377 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    21766 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 toc4github-0.16/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 toc4github-0.16/LICENSE
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 toc4github-0.16/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 toc4github-0.16/pyproject.toml
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 toc4github-0.16/PKG-INFO
```

### Comparing `toc4github-0.15/screenshot.png` & `toc4github-0.16/showcase.png`

 * *Files identical despite different names*

### Comparing `toc4github-0.15/toc4github.py` & `toc4github-0.16/toc4github.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 #!/usr/bin/env python3
+"""
+Author:   xinlin-z
+Github:   https://github.com/xinlin-z/toc4github
+Blog:     https://cs.pynote.net
+License:  MIT
+"""
 import sys
 import re
 import argparse
 from functools import singledispatch
 from typing import Iterable, Union
 
 
@@ -22,68 +28,71 @@
             skip = abs(skip-1)
         if skip:
             continue
         # try to find placeholder {toc} and skip
         if line.strip().lower() == '{toc}':
             pos = i
             continue
-        # search and join
+        # line search and make toc
         if strs:=re.match(r'\s*(#+)\s(.*)',line):
             h = strs.group(1)
             if (hn:=len(h)) > 6:  # max head level is 6
                 continue
             rest = strs.group(2).strip()
-            # git rid of markdown syntax elements ~*_
+            # remove markdown syntax elements ~*_
             while a:=re.search(r'([~*_]{1,2})(.*)\1',rest):
                 rest = rest[:a.start()] + a.group(2) + rest[a.end():]
             rest = re.sub(r'\s', '-', rest)  # space --> -
             rest = re.sub(r'[^-\w]', '', rest)  # squeeze other chars
             toc += ''.join((' '*(hn-1)*4, '* ',
                            '[',strs.group(2).strip(),'](#', rest,')'))+'\n'
     else:
         if skip:
             raise ValueError('``` block is open.')
 
-    return pos, toc.rstrip('\n')
+    return pos, toc
 
 
 @singledispatch
 def make_toc(lines: Union[list[str],str]) -> str:
     """Return the TOC contents."""
     return _make_toc(lines)[1]
 
 
 @make_toc.register
 def _(strlines: str) -> str:
     return _make_toc(strlines.split('\n'))[1]
 
 
+_VER = 'toc4github V0.16 by xinlin-z with love'\
+       ' (https://github.com/xinlin-z/toc4github)'
+
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument('-V', action='version',
-                        version='toc4github V0.15 by xinlin-z with love')
+    parser.add_argument('-V', '--version', action='version', version=_VER)
     parser.add_argument('-d','--dryrun', action='store_true',
-                        help='do not really do write, only print out')
+                        help='do not touch file, only show the TOC')
     parser.add_argument('-t','--title', action='store_true',
-                        help='add title: Table of Contents')
-    parser.add_argument('mdfile',
+                        help='add a fixed title: Table of Contents')
+    parser.add_argument('markdown_file',
                         help='the input markdown file, like README.md')
     args = parser.parse_args()
 
     try:
-        with open(args.mdfile) as f:
+        with open(args.markdown_file) as f:
             lines = f.readlines()
         pos, toc = _make_toc(lines)
-        if pos == -1:
-            raise ValueError('No {toc} placeholder found!')
         toc = ('','# Table of Contents\n\n')[args.title] + toc
         if args.dryrun:
-            print(toc)
-        else:
-            lines[pos] = toc + '\n'
-            with open(args.mdfile,'w') as f:
-                f.write(''.join(lines))
+            print(toc, end='')
+            sys.exit(0)
+        if pos == -1:
+            raise ValueError('No {toc} placeholder found!')
+        lines[pos] = toc
+        with open(args.markdown_file,'w') as f:
+            f.write(''.join(lines))
     except Exception as e:
         print('Err:', str(e))
         sys.exit(1)
```

### Comparing `toc4github-0.15/tox.ini` & `toc4github-0.16/tox.ini`

 * *Files identical despite different names*

### Comparing `toc4github-0.15/utest.py` & `toc4github-0.16/utest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import unittest
 from toc4github import make_toc
 import os
 import subprocess
 
 
-def shcmd(cmd, shell=False):
+def cmd(cmd, shell=False):
     """execute a cmd without shell, return exitcode"""
     proc = subprocess.run(cmd if shell else cmd.split(),
                           shell=shell,
                           stdout=subprocess.PIPE,
                           stderr=subprocess.PIPE)
     return proc.returncode
 
 
-raw = """
+raw = """\
 {toc}
 
 # Test
 ## header
 ### head 3
 #### head 4
 ##### head 5
@@ -36,87 +36,88 @@
 # _italic2 12345_
 # __bold2 12345__
 # ~cross out~
 # ~~cross out 2~~
 # **~bold cross out~**
 # __~~blod cross out 2~~__
 """
-cooked = ('* [Test](#Test)\n    '
-          '* [header](#header)\n        '
-          '* [head 3](#head-3)\n            '
-          '* [head 4](#head-4)\n                '
-          '* [head 5](#head-5)\n                    '
-          '* [head 6](#head-6)\n'
+cooked = ('* [Test](#Test)\n'
+          '    * [header](#header)\n'
+          '        * [head 3](#head-3)\n'
+          '            * [head 4](#head-4)\n'
+          '                * [head 5](#head-5)\n'
+          '                    * [head 6](#head-6)\n'
           '* [_abc](#_abc)\n'
           '* [a & b & c](#a--b--c)\n'
           '* [a       c](#a-------c)\n'
           '* [a ( c )](#a--c-)\n'
           '* [a(c)](#ac)\n'
           '* [a.,.,!@#$%^&*().,.7](#a7)\n'
           '* [*italic 12345*](#italic-12345)\n'
           '* [**bold 12345**](#bold-12345)\n'
           '* [_italic2 12345_](#italic2-12345)\n'
           '* [__bold2 12345__](#bold2-12345)\n'
           '* [~cross out~](#cross-out)\n'
           '* [~~cross out 2~~](#cross-out-2)\n'
           '* [**~bold cross out~**](#bold-cross-out)\n'
-          '* [__~~blod cross out 2~~__](#blod-cross-out-2)')
+          '* [__~~blod cross out 2~~__](#blod-cross-out-2)\n')
 
 
 class test_make_toc(unittest.TestCase):
 
     def test_make_toc_1(self):
         toc = make_toc(raw)
         self.assertEqual(toc, cooked)
         toc = make_toc(raw.split('\n'))
         self.assertEqual(toc, cooked)
 
     def test_make_toc_2(self):
-        fn = '__tocy_test.txt'
+        fn = '__toc4github_test2.txt'
         with open(fn,'w') as f:
             f.write(raw)
-        shcmd('python3 toc4github.py %s' % fn)
+        cmd('python3 toc4github.py %s' % fn)
         with open(fn) as f:
             cont = f.read()
-        self.assertEqual(cont, '\n'+cooked+raw[6:])
+        self.assertEqual(cont, cooked+raw[6:])
         os.remove(fn)
 
     def test_make_toc_21(self):
-        fn = '__tocy_test.txt'
+        fn = '__toc4github_test21.txt'
         with open(fn,'w') as f:
             f.write(raw)
-        shcmd('python3 toc4github.py --title %s' % fn)
+        cmd('python3 toc4github.py --title %s' % fn)
         with open(fn) as f:
             cont = f.read()
-        self.assertEqual(cont, '\n'+'# Table of Contents\n\n'+cooked+raw[6:])
+        self.assertEqual(cont, '# Table of Contents\n\n'+cooked+raw[6:])
         os.remove(fn)
 
     def test_make_toc_3(self):
         raw = """
         ```
         123456
         """
         self.assertRaises(ValueError, make_toc, raw)
 
     def test_make_toc_4(self):
         s = "# 中文效果"
-        self.assertEqual('* ['+s[2:]+'](#'+s[2:]+')', make_toc(s))
+        self.assertEqual('* ['+s[2:]+'](#'+s[2:]+')\n', make_toc(s))
         s = "## 中文效果"
-        self.assertEqual('    * ['+s[3:]+'](#'+s[3:]+')', make_toc(s))
+        self.assertEqual('    * ['+s[3:]+'](#'+s[3:]+')\n', make_toc(s))
         s = "# 中EN混Mix"
-        self.assertEqual('* ['+s[2:]+'](#'+s[2:]+')', make_toc(s))
+        self.assertEqual('* ['+s[2:]+'](#'+s[2:]+')\n', make_toc(s))
         s = "## 中EN混Mix"
-        self.assertEqual('    * ['+s[3:]+'](#'+s[3:]+')', make_toc(s))
+        self.assertEqual('    * ['+s[3:]+'](#'+s[3:]+')\n', make_toc(s))
 
     def test_make_toc_5(self):
         s = '#abcde'
         self.assertEqual(make_toc(s), '')
         s = '#  abcde'
-        self.assertEqual(make_toc(s), '* [abcde](#abcde)')
+        self.assertEqual(make_toc(s), '* [abcde](#abcde)\n')
         s = ' #abcde'
         self.assertEqual(make_toc(s), '')
         s = '  #  abcde'
-        self.assertEqual(make_toc(s), '* [abcde](#abcde)')
+        self.assertEqual(make_toc(s), '* [abcde](#abcde)\n')
 
 
 if __name__ == '__main__':
     unittest.main()
+
```

### Comparing `toc4github-0.15/LICENSE` & `toc4github-0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `toc4github-0.15/README.md` & `toc4github-0.16/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 # Table of Contents
 
-* [toc4github Intro](#toc4github-Intro)
+* [Intro](#Intro)
 * [Install](#Install)
-* [Command Line](#Command-Line)
-* [Interface](#Interface)
-* [Screenshot](#Screenshot)
-
-# toc4github Intro
-
-A tiny tool to automatically generate Table of Contents (TOC) for
-markdown file, like README.md of Github.com. It might also be used
-for other markdown rendering system, but I never tested!:)
+* [Command Line Usage](#Command-Line-Usage)
+* [API](#API)
+* [Showcase](#Showcase)
+
+# Intro
+
+Toc4github is a tiny tool to automatically generate Table of
+Contents (TOC) for Markdown file, like README.md in Github.com.
+It might also be used for other markdown rendering system, but
+I never tested! :)
 
 # Install
 
 ``` shell
 $ pip3 install toc4github
 ```
 
-# Command Line
+# Command Line Usage
 
-Insert a placeholder `{toc}` in a proper line of README.md. The
-placeholder itself should be single line, and it most likely be
+You should insert a line of placeholder with content `{toc}` in README.md.
+
+The placeholder itself must be single line, and it most likely be
 at the beginning of markdown file. This is the start position
-of TOC section, then run:
+of TOC section.
+
+When the placeholder line is ready:
 
 ``` shell
 $ python3 -m toc4github [--dryrun|-d] [--title|-t] <path/to/README.md>
 ```
 
-Now, the placeholder line is replaced and expanded by TOC,
+Now, the placeholder line is replaced and expanded by TOC generated,
 your markdown file is updated.
 
 You can use `--dryrun(-d)` to check the generated TOC first, this option
 would only print out TOC, file is intact and nothing is changed.
 
 `--title(-t)` option is used if you need a title for TOC section.
-The title is always `Table of Contents`, just like this README.md file.
+The title is fixed with `Table of Contents`, just like this README.md file.
+
+Different languages can be mixed, but I only tested English and Chinese.
 
 Here is an example:
 
 ``` shell
 $ python3 -m toc4github -dt text.txt
 # Table of Contents
 
@@ -51,23 +57,25 @@
         * [Item-2](#Item-2)
         * [Item-3](#Item-3)
         * [Item-4](#Item-4)
     * [Future 未来](#Future-未来)
     * [中英文can mix哦](#中英文can-mix哦)
 ```
 
-# Interface
+# API
 
 Or, you can call `make_toc` interface in your python code like:
 
 ``` python
+>>> from toc4github import make_toc
+>>>
 >>> with open('text.txt') as f:
 ...     lines = f.read()
 ...
->>> print(lines)
+>>> print(lines)  # show original content
 {toc}
 
 # Hello
 
 Hi, here is a test.
 
 ## Past 过去
@@ -90,32 +98,31 @@
 
 ## Future 未来
 
 Future is created by your imagination.
 
 ## 中英文can mix哦
 
->>> from toc4github import make_toc
->>> print(make_toc(lines))
+>>> print(make_toc(lines))  # show TOC
 * [Hello](#Hello)
     * [Past 过去](#Past-过去)
     * [Present 现在](#Present-现在)
         * [Item-1](#Item-1)
         * [Item-2](#Item-2)
         * [Item-3](#Item-3)
         * [Item-4](#Item-4)
     * [Future 未来](#Future-未来)
     * [中英文can mix哦](#中英文can-mix哦)
 >>>
 ```
 
-Interface `make_toc` only return the generated TOC, and you should
+Interface `make_toc` only return the generated TOC, you should
 insert it to your file anywhere you like by yourself. And this
-is the only interface toc4github provides, and no other parameters.
+is the only interface toc4github provides.
 
-# Screenshot
+# Showcase
 
-![toc4github](/screenshot.png)
+![toc4github](/showcase.png)
 
 In addition, All my repos' TOC are generated by toc4github.
 Have fun ... ^___^
```

### Comparing `toc4github-0.15/pyproject.toml` & `toc4github-0.16/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = 'toc4github'
-version = '0.15'
+version = '0.16'
+requires-python = '>=3.8'
+description = 'Generate Table of Contents (TOC) for Markdown file (like README.md) automatically'
+readme = 'README.md'
+license = { file='LICENSE' }
+keywords = ['TOC', 'markdown', 'github', 'README.md']
 authors = [
   { name='xinlin-z', email='xinlin.zhang@hotmail.com' },
 ]
-description = 'Generate Table of Contents (TOC) for markdown file (like README.md) automatically'
-readme = 'README.md'
-requires-python = '>=3.8'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
 ]
 
 
 [project.urls]
 homepage = 'https://github.com/xinlin-z/toc4github'
-'Bug Tracker' = 'https://github.com/xinlin-z/toc4github/issues'
+
```

