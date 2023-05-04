# Comparing `tmp/mail_deduplicate-7.2.0.tar.gz` & `tmp/mail_deduplicate-7.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail_deduplicate-7.2.0.tar", max compression
+gzip compressed data, was "mail_deduplicate-7.2.3.tar", max compression
```

## Comparing `mail_deduplicate-7.2.0.tar` & `mail_deduplicate-7.2.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     6694 2023-02-15 16:16:46.995195 mail_deduplicate-7.2.0/mail_deduplicate/__init__.py
--rw-r--r--   0        0        0     2035 2023-02-15 16:16:46.995195 mail_deduplicate-7.2.0/mail_deduplicate/__main__.py
--rw-r--r--   0        0        0     5226 2023-02-15 16:16:46.995195 mail_deduplicate-7.2.0/mail_deduplicate/action.py
--rw-r--r--   0        0        0    13940 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/cli.py
--rw-r--r--   0        0        0    20076 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/deduplicate.py
--rw-r--r--   0        0        0    13530 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/mail.py
--rw-r--r--   0        0        0     7375 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/mailbox.py
--rw-r--r--   0        0        0        0 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/py.typed
--rw-r--r--   0        0        0     8220 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/strategy.py
--rw-r--r--   0        0        0      770 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/__init__.py
--rw-r--r--   0        0        0     5653 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/conftest.py
--rw-r--r--   0        0        0     1191 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/test_action.py
--rw-r--r--   0        0        0     1673 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/test_cli.py
--rw-r--r--   0        0        0     3053 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/test_mail.py
--rw-r--r--   0        0        0     1334 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/test_mailbox.py
--rw-r--r--   0        0        0    11089 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/mail_deduplicate/tests/test_strategy.py
--rw-r--r--   0        0        0     3531 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/pyproject.toml
--rw-r--r--   0        0        0     4140 2023-02-15 16:16:46.999195 mail_deduplicate-7.2.0/readme.md
--rw-r--r--   0        0        0     5296 1970-01-01 00:00:00.000000 mail_deduplicate-7.2.0/setup.py
--rw-r--r--   0        0        0     6095 1970-01-01 00:00:00.000000 mail_deduplicate-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6685 2023-05-04 11:32:18.882184 mail_deduplicate-7.2.3/mail_deduplicate/__init__.py
+-rw-r--r--   0        0        0     2034 2023-05-04 11:32:18.882184 mail_deduplicate-7.2.3/mail_deduplicate/__main__.py
+-rw-r--r--   0        0        0     5226 2023-05-04 11:32:18.882184 mail_deduplicate-7.2.3/mail_deduplicate/action.py
+-rw-r--r--   0        0        0    13968 2023-05-04 11:32:18.882184 mail_deduplicate-7.2.3/mail_deduplicate/cli.py
+-rw-r--r--   0        0        0    20087 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/deduplicate.py
+-rw-r--r--   0        0        0    13528 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/mail.py
+-rw-r--r--   0        0        0     7374 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/mailbox.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/py.typed
+-rw-r--r--   0        0        0     8219 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/strategy.py
+-rw-r--r--   0        0        0      770 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/__init__.py
+-rw-r--r--   0        0        0     5652 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/conftest.py
+-rw-r--r--   0        0        0     1191 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/test_action.py
+-rw-r--r--   0        0        0     1673 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/test_cli.py
+-rw-r--r--   0        0        0     3053 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/test_mail.py
+-rw-r--r--   0        0        0     1334 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/test_mailbox.py
+-rw-r--r--   0        0        0    11089 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/mail_deduplicate/tests/test_strategy.py
+-rw-r--r--   0        0        0     4027 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4132 2023-05-04 11:32:18.886184 mail_deduplicate-7.2.3/readme.md
+-rw-r--r--   0        0        0     6012 1970-01-01 00:00:00.000000 mail_deduplicate-7.2.3/PKG-INFO
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/__init__.py` & `mail_deduplicate-7.2.3/mail_deduplicate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-
 """Expose package-wide elements."""
 from __future__ import annotations
 
 from pathlib import Path
 
 from boltons.iterutils import unique
 
-__version__ = "7.2.0"
+__version__ = "7.2.3"
 
 from click_extra.logging import logger  # noqa: F401
 
 HASH_HEADERS = (
     "Date",
     "From",
     "To",
@@ -36,16 +35,15 @@
     "MIME-Version",
     "Content-Type",
     "Content-Disposition",
     "User-Agent",
     "X-Priority",
     "Message-ID",
 )
-"""
-Default ordered list of headers to use to compute the unique hash of a mail.
+"""Default ordered list of headers to use to compute the unique hash of a mail.
 
 By default we choose to exclude:
 
 ``Cc``
   Since ``mailman`` apparently `sometimes trims list members
   <https://mail.python.org/pipermail/mailman-developers/2002-September/013233.html>`_
   from the ``Cc`` header to avoid sending duplicates. Which means that copies of mail
@@ -63,16 +61,15 @@
 
 
 MINIMAL_HEADERS_COUNT = 4
 """Below this value, we consider not having enough headers to compute a solid hash."""
 
 
 DEFAULT_SIZE_THRESHOLD = 512
-"""
-Default size threshold in bytes.
+"""Default size threshold in bytes.
 
 Since we're ignoring the ``Content-Length`` header by default `because of mailing-list
 effects <https://kdeldycke.github.io/mail-deduplicate/design.html#mailing-lists>`_, we
 introduced a limit on the allowed difference between the sizes of the message payloads.
 
 If this is exceeded, a warning is issued and the messages are not considered duplicates,
 because this could point to message corruption somewhere, or a false positive.
@@ -88,60 +85,55 @@
     mechanism or mailing list server.
 
     This threshold has to be large enough to allow for footers added by mailing list
     servers.
 """
 
 DEFAULT_CONTENT_THRESHOLD = 768
-"""
-Default content threshold in bytes.
+"""Default content threshold in bytes.
 
-As above, we similarly generates unified diffs of duplicates and ensure that the diff
-is not greater than a certain size to limit false-positives.
+As above, we similarly generates unified diffs of duplicates and ensure that the diff is
+not greater than a certain size to limit false-positives.
 """
 
 DATE_HEADER = "date-header"
 CTIME = "ctime"
 TIME_SOURCES = frozenset([DATE_HEADER, CTIME])
-""" Methods used to extract a mail's canonical timestamp:
+"""Methods used to extract a mail's canonical timestamp:
 
 - ``date-header``: sourced from the message's ``Date`` header.
 - ``ctime``: sourced from the email's file from the filesystem. Only available for
   ``maildir`` sources.
 
 Also see:
 https://kdeldycke.github.io/mail-deduplicate/mail_deduplicate.html#mail_deduplicate.mail.DedupMail.timestamp
 """
 
 
 class TooFewHeaders(Exception):
-
     """Not enough headers were found to produce a solid hash."""
 
 
 class SizeDiffAboveThreshold(Exception):
-
     """Difference in mail size is greater than `threshold.
 
     <https://kdeldycke.github.io/mail-
     deduplicate/mail_deduplicate.html#mail_deduplicate.DEFAULT_SIZE_THRESHOLD>`_.
     """
 
 
 class ContentDiffAboveThreshold(Exception):
-
     """Difference in mail content is greater than `threshold.
 
     <https://kdeldycke.github.io/mail-
     deduplicate/mail_deduplicate.html#mail_deduplicate.DEFAULT_CONTENT_THRESHOLD>`_.
     """
 
 
 class Config:
-
     """Holds global configuration."""
 
     # Keep these defaults in sync with CLI option definitions.
     default_conf = {
         "dry_run": False,
         "input_format": False,
         "force_unlock": False,
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/__main__.py` & `mail_deduplicate-7.2.3/mail_deduplicate/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-
 """Allow the module to be run as a CLI. I.e.:
 
 .. code-block:: shell-session
 
     $ python -m mail_deduplicate
 
 Removes empty string and current working directory from the first entry of
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/action.py` & `mail_deduplicate-7.2.3/mail_deduplicate/action.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/cli.py` & `mail_deduplicate-7.2.3/mail_deduplicate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     Choice,
     argument,
     echo,
     extra_command,
     option,
     option_group,
     pass_context,
+    path,
     progressbar,
 )
-from click_extra import Path as ClickPath
 from click_extra.colorize import default_theme as theme
 from click_extra.commands import ExtraCommand
 
 from . import (
     DATE_HEADER,
     DEFAULT_CONTENT_THRESHOLD,
     DEFAULT_SIZE_THRESHOLD,
@@ -101,14 +101,15 @@
 @extra_command(
     cls=MdedupCommand,
     version=__version__,
     short_help="Deduplicate mail boxes.",
     # Force linear layout for definition lists. See:
     # https://cloup.readthedocs.io/en/stable/pages/formatting.html#the-linear-layout-for-definition-lists
     formatter_settings={"col2_min_width": 9999999999},
+    # Removes the -h short option as we reserve it for --hash-header.
     context_settings={"help_option_names": ("--help",)},
 )
 @option_group(
     "Mail sources (step #1)",
     option(
         "-i",
         "--input-format",
@@ -241,15 +242,15 @@
         "it is the safest: it only reads the mail sources and create a brand new mail "
         "box with the selection results.",
     ),
     option(
         "-E",
         "--export",
         metavar="MAIL_BOX_PATH",
-        type=ClickPath(resolve_path=True),
+        type=path(resolve_path=True),
         help="Location of the destination mail box to where to copy or move "
         f"deduplicated mails. Required in {COPY_SELECTED}, {COPY_DISCARDED}, "
         f"{MOVE_SELECTED} and {MOVE_DISCARDED} actions.",
     ),
     option(
         "-e",
         "--export-format",
@@ -277,15 +278,15 @@
         "would have been performed otherwise.",
     ),
 )
 @argument(
     "mail_sources",
     nargs=-1,
     metavar="MAIL_SOURCE_1 MAIL_SOURCE_2 ...",
-    type=ClickPath(exists=True, resolve_path=True),
+    type=path(exists=True, resolve_path=True),
     help="Mail sources to deduplicate. Can be a single mail box or a list of mails.",
 )
 @pass_context
 def mdedup(
     ctx,
     input_format,
     force_unlock,
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/deduplicate.py` & `mail_deduplicate-7.2.3/mail_deduplicate/deduplicate.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from pathlib import Path
 
 if sys.version_info >= (3, 8):
     from functools import cached_property
 else:
     from boltons.cacheutils import cachedproperty as cached_property
 
-import click
 from boltons.dictutils import FrozenDict
+from click_extra import progressbar
 from click_extra.colorize import default_theme as theme
 from tabulate import tabulate
 
 from . import ContentDiffAboveThreshold, SizeDiffAboveThreshold, TooFewHeaders, logger
 from .mailbox import open_box
 from .strategy import apply_strategy
 
@@ -122,15 +122,14 @@
         BODY_HASHER_NORMALIZED: lambda m: m.hash_normalized_body,
     }
 )
 """Method used to hash the body of mails."""
 
 
 class DuplicateSet:
-
     """A set of mails sharing the same hash.
 
     Implements all the safety checks required before we can apply any selection
     strategy.
     """
 
     def __init__(self, hash_key, mail_set, conf):
@@ -203,15 +202,14 @@
         if self.conf.content_threshold < 0:
             logger.info("Skip checking for content differences.")
         if self.conf.size_threshold < 0 and self.conf.content_threshold < 0:
             return
 
         # Compute differences of mail against one another.
         for mail_a, mail_b in combinations(self.pool, 2):
-
             # Compare mails on size.
             if self.conf.size_threshold > -1:
                 size_difference = abs(mail_a.size - mail_b.size)
                 logger.debug(
                     f"{mail_a!r} and {mail_b!r} differs by {size_difference} bytes "
                     "in size."
                 )
@@ -329,15 +327,14 @@
         self.stats["mail_discarded"] += self.size - candidate_count
         self.stats["set_deduplicated"] += 1
         self.selection = selected
         self.discard = self.pool.difference(selected)
 
 
 class Deduplicate:
-
     """Load-up messages, search for duplicates, apply selection strategy and perform the
     action.
 
     Similar messages sharing the same hash are grouped together in a ``DuplicateSet``.
     """
 
     def __init__(self, conf):
@@ -396,23 +393,21 @@
 
         body_hasher = BODY_HASHERS.get(self.conf.hash_body)
         if not body_hasher:
             raise NotImplementedError(
                 f"{self.conf.hash_body} body hasher not implemented yet."
             )
 
-        with click.progressbar(
+        with progressbar(
             length=self.stats["mail_found"],
             label="Hashed mails",
             show_pos=True,
         ) as progress:
-
             for box in self.sources.values():
                 for mail_id, mail in box.iteritems():
-
                     mail.add_box_metadata(box, mail_id)
 
                     mail.conf = self.conf
 
                     try:
                         mail_hash = mail.hash_key + body_hasher(mail)
                     except TooFewHeaders as expt:
@@ -440,15 +435,14 @@
             )
         else:
             logger.warning("No strategy configured, skip selection.")
 
         self.stats["set_total"] = len(self.mails)
 
         for hash_key, mail_set in self.mails.items():
-
             # Alter log level depending on set length.
             mail_count = len(mail_set)
             log_level = logger.debug if mail_count == 1 else logger.info
             log_level(theme.subheading(f"◼ {mail_count} mails sharing hash {hash_key}"))
 
             # Apply the selection strategy to discriminate mails within the set.
             duplicates = DuplicateSet(hash_key, mail_set, self.conf)
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/mail.py` & `mail_deduplicate-7.2.3/mail_deduplicate/mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 import arrow
 from tabulate import tabulate
 
 from . import CTIME, MINIMAL_HEADERS_COUNT, TooFewHeaders, logger
 
 
 class DedupMail:
-
     """Message with deduplication-specific properties and utilities.
 
     Extends `standard library's mailbox.Message
     <https://github.com/python/cpython/blob/45ffab40e86777ecd49786a2c18c0c044ef0cb5b/Lib/mailbox.py#L1489-L1523>`_,
     and shouln't be used directly, but composed with ``mailbox.Message`` sub-classes.
     """
 
@@ -225,15 +224,14 @@
     @cached_property
     def canonical_headers(self):
         """Returns the full list of all canonical headers names and values in
         preparation for hashing."""
         canonical_headers = []
 
         for header_id in self.conf.hash_headers:
-
             # Skip absent header.
             if header_id not in self:
                 continue
 
             # Fetch all occurrences of the header.
             canonical_values = []
             for header_value in self.get_all(header_id):
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/mailbox.py` & `mail_deduplicate-7.2.3/mail_deduplicate/mailbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-
 """Patch and tweak `Python's standard library mail box constructors.
 
 <https://docs.python.org/3.11/library/mailbox.html>`_ to set sane defaults.
 
 Also forces out our own message factories to add deduplication tools and utilities.
 """
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/strategy.py` & `mail_deduplicate-7.2.3/mail_deduplicate/strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-
 """Strategy definitions."""
 from __future__ import annotations
 
 import random
 import re
 
 from boltons.dictutils import FrozenDict
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/__init__.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/conftest.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 @pytest.fixture
 def invoke(invoke_extra):  # noqa: F811
     return partial(invoke_extra, mdedup)
 
 
 class MailFactory:
-
     """Create fake mail messages to serve as unittest fixtures.
 
     Help production of either random, customized or deterministic mail message.
     """
 
     def __init__(self, **custom_fields):
         """Init the mail with custom fields.
```

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/test_action.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/test_cli.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/test_mail.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/test_mailbox.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/mail_deduplicate/tests/test_strategy.py` & `mail_deduplicate-7.2.3/mail_deduplicate/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `mail_deduplicate-7.2.0/pyproject.toml` & `mail_deduplicate-7.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "mail-deduplicate"
-version = "7.2.0"
+version = "7.2.3"
 description = "📧 CLI to deduplicate mails from mail boxes."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/mail-deduplicate'
 repository = 'https://github.com/kdeldycke/mail-deduplicate'
 documentation = 'https://kdeldycke.github.io/mail-deduplicate'
@@ -45,37 +45,36 @@
 "Changelog" = "https://kdeldycke.github.io/mail-deduplicate/changelog.html"
 
 [tool.poetry.dependencies]
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
 python = "^3.7"
 arrow = "^1.2.3"
-boltons = "^21.0.0"
+boltons = "^23.0.0"
 click = "^8.1.2"
-click-extra = "^3.4.0"
+click-extra = "^3.10.0"
 tabulate = { extras = ["widechars"], version = "^0.9.0" }
-typing-extensions = { version = "^4.3.0", python = "< 3.10" }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
-coverage = { extras = ["toml"], version = "^7.1" }
-furo = "^2022.9.29"
+coverage = { extras = ["toml"], version = "^7.2" }
+furo = "^2023.03.27"
 mypy = "^1.0"
-myst-parser = "^0.18.0"
+myst-parser = "^1.0.0"
 pytest = "^7.2.1"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cov = "^4.0.0"
 pytest-randomly = "^3.12.0"
-pytest-xdist = { extras = ["psutil"], version = "^3.2.0" }
 sphinx = "^5.3.0"
 sphinx-autodoc-typehints = "^1.22"
 sphinx-click = "^4.4.0"
 sphinx-copybutton = "^0.5.1"
-sphinx-design = "^0.3.0"
+sphinx-design = "^0.4.1"
 sphinx-issues = "^3.0.1"
+sphinxcontrib-mermaid = "^0.8"
 sphinxext-opengraph = "^0.7.5"
 types-tabulate = "^0.9.0"
 tomli = { version = "^2.0.1", python = "< 3.11" }
 
 [tool.poetry.scripts]
 mdedup = 'mail_deduplicate.__main__:main'
 
@@ -89,28 +88,31 @@
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = ["boltons.*"]
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/latest/customize.html#pyproject-toml
-# --full-trace: have a full traceback printed on KeyboardInterrupt
-# XXX --numprocesses 1: concurrent tests don't work well for now.
-addopts = "--numprocesses 1 --durations=10 --cov-report term --cov=mail_deduplicate"
+# XXX The ``testpaths`` parameter has no effect since pytest is only looking for a ``conftest.py`` right next to this
+# ``pyproject.toml`` file. This issue is tracked upstream at: https://github.com/pytest-dev/pytest/issues/10665
+# In the meantime, we have to rely on the ``addopts`` parameter to hard-code the test path and have our custom options
+# recognized.
+testpaths = ["mail_deduplicate/tests/"]
+# --cov-config=pyproject.toml : is specified at CLI level instead of letting coverage find it because of this bug:
+#   https://github.com/nedbat/coveragepy/issues/512#issuecomment-399707938
+#   https://github.com/pytest-dev/pytest-cov/issues/168#issuecomment-327533847
+#   https://github.com/pytest-dev/pytest-cov/issues/243
+addopts = "--durations=10 --cov-report=term --cov-report=xml --cov-config=pyproject.toml --cov=."
+# Make sure tests that are expected to fail do not resurect and start working all of a sudden.
 xfail_strict = true
 
-[tool.coverage.paths]
 # https://coverage.readthedocs.io/en/latest/config.html
-source = ["mail_deduplicate"]
 [tool.coverage.run]
-source = ["mail_deduplicate"]
 branch = true
-omit = ["*/tests/*"]
 [tool.coverage.report]
-omit = ["*/tests/*"]
 precision = 2
 
 [tool.check-wheel-contents]
 ignore = [
     # W002: Wheel contains duplicate files:
     #   mail_deduplicate/managers/__init__.py
     #   mail_deduplicate/tests/__init__.py
```

### Comparing `mail_deduplicate-7.2.0/readme.md` & `mail_deduplicate-7.2.3/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <p align="center">
   <a href="https://github.com/kdeldycke/mail-deduplicate/">
-    <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/mail-deduplicate-logo-header.png" alt="Mail Deduplicate">
+    <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/mail-deduplicate-logo-header.png" alt="Mail Deduplicate">
   </a>
 </p>
 
 [![Last release](https://img.shields.io/pypi/v/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)
 [![Python versions](https://img.shields.io/pypi/pyversions/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)
 [![Unittests status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml?query=branch%3Amain)
 [![Documentation status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml?query=branch%3Amain)
-[![Coverage status](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main)
+[![Coverage status](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://app.codecov.io/gh/kdeldycke/mail-deduplicate)
 [![DOI](https://zenodo.org/badge/9016537.svg)](https://zenodo.org/badge/latestdoi/9016537)
 
 **What is Mail Deduplicate?**
 
 Provides the `mdedup` CLI, an utility to deduplicate mails from a set of boxes.
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/cli-coloured-header.png" alt="Mail Deduplicate">
+  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/cli-coloured-header.png" alt="Mail Deduplicate">
 </p>
 
 ## Features
 
 - Duplicate detection based on cherry-picked and normalized mail
   headers.
 - Fetch mails from multiple sources.
@@ -42,15 +42,15 @@
 > If this is good enough for a volume of a couple of gigabytes, the more emails `mdedup` try to parse, the closer you'll reach the memory limits of your machine. In which case [`mdedup` will exit abrubtly](https://github.com/kdeldycke/mail-deduplicate/issues/362#issuecomment-1266743045), zapped by the [OOM killer](https://en.wikipedia.org/wiki/Out_of_memory) of your OS. Of course your mileage may vary depending on your hardware.
 >
 > You can influence implementation of this feature with pull requests, or [purchase of business support 🤝 and sponsorship 🫶](https://github.com/sponsors/kdeldycke).
 
 ## Example
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/cli-coloured-run.png">
+  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/cli-coloured-run.png">
 </p>
 
 ## Installation
 
 ### From sources
 
 Easiest way is to install `mdedup` from sources with [`pipx`](https://pypa.github.io/pipx/):
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 pypi/mail-deduplicate) [![Unittests status](https://github.com/kdeldycke/mail-
 deduplicate/actions/workflows/tests.yaml/badge.svg?branch=main)](https://
 github.com/kdeldycke/mail-deduplicate/actions/workflows/
 tests.yaml?query=branch%3Amain) [![Documentation status](https://github.com/
 kdeldycke/mail-deduplicate/actions/workflows/docs.yaml/badge.svg?branch=main)]
 (https://github.com/kdeldycke/mail-deduplicate/actions/workflows/
 docs.yaml?query=branch%3Amain) [![Coverage status](https://codecov.io/gh/
-kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://codecov.io/gh/
-kdeldycke/mail-deduplicate/branch/main) [![DOI](https://zenodo.org/badge/
+kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://
+app.codecov.io/gh/kdeldycke/mail-deduplicate) [![DOI](https://zenodo.org/badge/
 9016537.svg)](https://zenodo.org/badge/latestdoi/9016537) **What is Mail
 Deduplicate?** Provides the `mdedup` CLI, an utility to deduplicate mails from
 a set of boxes.
                               [Mail Deduplicate]
 ## Features - Duplicate detection based on cherry-picked and normalized mail
 headers. - Fetch mails from multiple sources. - Reads and writes to `mbox`,
 `maildir`, `babyl`, `mh` and `mmdf` formats. - Deduplication strategies based
@@ -29,15 +29,15 @@
 closer you'll reach the memory limits of your machine. In which case [`mdedup`
 will exit abrubtly](https://github.com/kdeldycke/mail-deduplicate/issues/
 362#issuecomment-1266743045), zapped by the [OOM killer](https://
 en.wikipedia.org/wiki/Out_of_memory) of your OS. Of course your mileage may
 vary depending on your hardware. > > You can influence implementation of this
 feature with pull requests, or [purchase of business support ð¤ and
 sponsorship ð«¶](https://github.com/sponsors/kdeldycke). ## Example
-[https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/
+[https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/
                              cli-coloured-run.png]
 ## Installation ### From sources Easiest way is to install `mdedup` from
 sources with [`pipx`](https://pypa.github.io/pipx/): ```shell-session $ pipx
 install mail-deduplicate ``` Other [alternatives installation methods](https://
 kdeldycke.github.io/mail-deduplicate/install.html) are available in the
 documentation. ### Executables Standalone executables of `mdedup`'s latest
 version are available for several platforms and architectures: | Platform |
```

### Comparing `mail_deduplicate-7.2.0/setup.py` & `mail_deduplicate-7.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mail-deduplicate
+Version: 7.2.3
+Summary: 📧 CLI to deduplicate mails from mail boxes.
+Home-page: https://github.com/kdeldycke/mail-deduplicate
+License: GPL-2.0-or-later
+Keywords: CLI,mail,email,maildir,mbox,deduplication,dedupe,cleanup,mailbox,Babyl,MH,mbox,MMDF
+Author: Kevin Deldycke
+Author-email: kevin@deldycke.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Communications :: Email
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: boltons (>=23.0.0,<24.0.0)
+Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: click-extra (>=3.10.0,<4.0.0)
+Requires-Dist: tabulate[widechars] (>=0.9.0,<0.10.0)
+Project-URL: Changelog, https://kdeldycke.github.io/mail-deduplicate/changelog.html
+Project-URL: Documentation, https://kdeldycke.github.io/mail-deduplicate
+Project-URL: Funding, https://github.com/sponsors/kdeldycke
+Project-URL: Issues, https://github.com/kdeldycke/mail-deduplicate/issues
+Project-URL: Repository, https://github.com/kdeldycke/mail-deduplicate
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <a href="https://github.com/kdeldycke/mail-deduplicate/">
+    <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/mail-deduplicate-logo-header.png" alt="Mail Deduplicate">
+  </a>
+</p>
+
+[![Last release](https://img.shields.io/pypi/v/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)
+[![Python versions](https://img.shields.io/pypi/pyversions/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)
+[![Unittests status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml?query=branch%3Amain)
+[![Documentation status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml?query=branch%3Amain)
+[![Coverage status](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://app.codecov.io/gh/kdeldycke/mail-deduplicate)
+[![DOI](https://zenodo.org/badge/9016537.svg)](https://zenodo.org/badge/latestdoi/9016537)
+
+**What is Mail Deduplicate?**
+
+Provides the `mdedup` CLI, an utility to deduplicate mails from a set of boxes.
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/cli-coloured-header.png" alt="Mail Deduplicate">
+</p>
+
+## Features
+
+- Duplicate detection based on cherry-picked and normalized mail
+  headers.
+- Fetch mails from multiple sources.
+- Reads and writes to `mbox`, `maildir`, `babyl`, `mh` and `mmdf`
+  formats.
+- Deduplication strategies based on size, content, timestamp, file path
+  or random choice.
+- Copy, move or delete the resulting set of duplicates.
+- Dry-run mode.
+- Protection against false-positives with safety checks on size and content differences.
+- Supports macOS, Linux and Windows.
+- [Standalone executables](#executables) for Linux, macOS and Windows.
+- Shell auto-completion for Bash, Zsh and Fish.
+
+> ⚠️ **Warning**: Performances
+>
+> `mdedup` implementation is quite naive at the moment and everything resides in memory.
+>
+> If this is good enough for a volume of a couple of gigabytes, the more emails `mdedup` try to parse, the closer you'll reach the memory limits of your machine. In which case [`mdedup` will exit abrubtly](https://github.com/kdeldycke/mail-deduplicate/issues/362#issuecomment-1266743045), zapped by the [OOM killer](https://en.wikipedia.org/wiki/Out_of_memory) of your OS. Of course your mileage may vary depending on your hardware.
+>
+> You can influence implementation of this feature with pull requests, or [purchase of business support 🤝 and sponsorship 🫶](https://github.com/sponsors/kdeldycke).
+
+## Example
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/cli-coloured-run.png">
+</p>
+
+## Installation
+
+### From sources
+
+Easiest way is to install `mdedup` from sources with [`pipx`](https://pypa.github.io/pipx/):
+
+```shell-session
+$ pipx install mail-deduplicate
+```
+
+Other
+[alternatives installation methods](https://kdeldycke.github.io/mail-deduplicate/install.html)
+are available in the documentation.
+
+### Executables
+
+Standalone executables of `mdedup`'s latest version are available for several platforms and architectures:
+
+| Platform    | `x86_64`                                                                                                                           |
+| ----------- | ---------------------------------------------------------------------------------------------------------------------------------- |
+| **Linux**   | [Download `mdedup-linux-x64.bin`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-linux-x64.bin)     |
+| **macOS**   | [Download `mdedup-macos-x64.bin`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-macos-x64.bin)     |
+| **Windows** | [Download `mdedup-windows-x64.exe`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-windows-x64.exe) |
 
-packages = \
-['mail_deduplicate', 'mail_deduplicate.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['arrow>=1.2.3,<2.0.0',
- 'boltons>=21.0.0,<22.0.0',
- 'click-extra>=3.4.0,<4.0.0',
- 'click>=8.1.2,<9.0.0',
- 'tabulate[widechars]>=0.9.0,<0.10.0']
-
-extras_require = \
-{':python_version < "3.10"': ['typing-extensions>=4.3.0,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['mdedup = mail_deduplicate.__main__:main']}
-
-setup_kwargs = {
-    'name': 'mail-deduplicate',
-    'version': '7.2.0',
-    'description': '📧 CLI to deduplicate mails from mail boxes.',
-    'long_description': '<p align="center">\n  <a href="https://github.com/kdeldycke/mail-deduplicate/">\n    <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/mail-deduplicate-logo-header.png" alt="Mail Deduplicate">\n  </a>\n</p>\n\n[![Last release](https://img.shields.io/pypi/v/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)\n[![Python versions](https://img.shields.io/pypi/pyversions/mail-deduplicate.svg)](https://pypi.python.org/pypi/mail-deduplicate)\n[![Unittests status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/tests.yaml?query=branch%3Amain)\n[![Documentation status](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/mail-deduplicate/actions/workflows/docs.yaml?query=branch%3Amain)\n[![Coverage status](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/mail-deduplicate/branch/main)\n[![DOI](https://zenodo.org/badge/9016537.svg)](https://zenodo.org/badge/latestdoi/9016537)\n\n**What is Mail Deduplicate?**\n\nProvides the `mdedup` CLI, an utility to deduplicate mails from a set of boxes.\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/cli-coloured-header.png" alt="Mail Deduplicate">\n</p>\n\n## Features\n\n- Duplicate detection based on cherry-picked and normalized mail\n  headers.\n- Fetch mails from multiple sources.\n- Reads and writes to `mbox`, `maildir`, `babyl`, `mh` and `mmdf`\n  formats.\n- Deduplication strategies based on size, content, timestamp, file path\n  or random choice.\n- Copy, move or delete the resulting set of duplicates.\n- Dry-run mode.\n- Protection against false-positives with safety checks on size and content differences.\n- Supports macOS, Linux and Windows.\n- [Standalone executables](#executables) for Linux, macOS and Windows.\n- Shell auto-completion for Bash, Zsh and Fish.\n\n> ⚠️ **Warning**: Performances\n>\n> `mdedup` implementation is quite naive at the moment and everything resides in memory.\n>\n> If this is good enough for a volume of a couple of gigabytes, the more emails `mdedup` try to parse, the closer you\'ll reach the memory limits of your machine. In which case [`mdedup` will exit abrubtly](https://github.com/kdeldycke/mail-deduplicate/issues/362#issuecomment-1266743045), zapped by the [OOM killer](https://en.wikipedia.org/wiki/Out_of_memory) of your OS. Of course your mileage may vary depending on your hardware.\n>\n> You can influence implementation of this feature with pull requests, or [purchase of business support 🤝 and sponsorship 🫶](https://github.com/sponsors/kdeldycke).\n\n## Example\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/images/cli-coloured-run.png">\n</p>\n\n## Installation\n\n### From sources\n\nEasiest way is to install `mdedup` from sources with [`pipx`](https://pypa.github.io/pipx/):\n\n```shell-session\n$ pipx install mail-deduplicate\n```\n\nOther\n[alternatives installation methods](https://kdeldycke.github.io/mail-deduplicate/install.html)\nare available in the documentation.\n\n### Executables\n\nStandalone executables of `mdedup`\'s latest version are available for several platforms and architectures:\n\n| Platform    | `x86_64`                                                                                                                           |\n| ----------- | ---------------------------------------------------------------------------------------------------------------------------------- |\n| **Linux**   | [Download `mdedup-linux-x64.bin`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-linux-x64.bin)     |\n| **macOS**   | [Download `mdedup-macos-x64.bin`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-macos-x64.bin)     |\n| **Windows** | [Download `mdedup-windows-x64.exe`](https://github.com/kdeldycke/mail-deduplicate/releases/latest/download/mdedup-windows-x64.exe) |\n',
-    'author': 'Kevin Deldycke',
-    'author_email': 'kevin@deldycke.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kdeldycke/mail-deduplicate',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,68 +1,76 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['mail_deduplicate', 'mail_deduplicate.tests'] package_data = \ {'': ['*']}
-install_requires = \ ['arrow>=1.2.3,<2.0.0', 'boltons>=21.0.0,<22.0.0', 'click-
-extra>=3.4.0,<4.0.0', 'click>=8.1.2,<9.0.0', 'tabulate
-[widechars]>=0.9.0,<0.10.0'] extras_require = \ {':python_version < "3.10"':
-['typing-extensions>=4.3.0,<5.0.0']} entry_points = \ {'console_scripts':
-['mdedup = mail_deduplicate.__main__:main']} setup_kwargs = { 'name': 'mail-
-deduplicate', 'version': '7.2.0', 'description': 'ð§ CLI to deduplicate mails
-from mail boxes.', 'long_description': '
-                         \n \n_[Mail_Deduplicate]\n\n
-\n\n[![Last release](https://img.shields.io/pypi/v/mail-deduplicate.svg)]
-(https://pypi.python.org/pypi/mail-deduplicate)\n[![Python versions](https://
+Metadata-Version: 2.1 Name: mail-deduplicate Version: 7.2.3 Summary: ð§ CLI
+to deduplicate mails from mail boxes. Home-page: https://github.com/kdeldycke/
+mail-deduplicate License: GPL-2.0-or-later Keywords:
+CLI,mail,email,maildir,mbox,deduplication,dedupe,cleanup,mailbox,Babyl,MH,mbox,MMDF
+Author: Kevin Deldycke Author-email: kevin@deldycke.com Requires-Python:
+>=3.7,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
+Environment :: Console Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Information Technology Classifier: License :: OSI Approved
+:: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
+:: MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: Communications :: Email
+Classifier: Topic :: Utilities Classifier: Typing :: Typed Requires-Dist: arrow
+(>=1.2.3,<2.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
+(>=8.1.2,<9.0.0) Requires-Dist: click-extra (>=3.10.0,<4.0.0) Requires-Dist:
+tabulate[widechars] (>=0.9.0,<0.10.0) Project-URL: Changelog, https://
+kdeldycke.github.io/mail-deduplicate/changelog.html Project-URL: Documentation,
+https://kdeldycke.github.io/mail-deduplicate Project-URL: Funding, https://
+github.com/sponsors/kdeldycke Project-URL: Issues, https://github.com/
+kdeldycke/mail-deduplicate/issues Project-URL: Repository, https://github.com/
+kdeldycke/mail-deduplicate Description-Content-Type: text/markdown
+                              [Mail_Deduplicate]
+[![Last release](https://img.shields.io/pypi/v/mail-deduplicate.svg)](https://
+pypi.python.org/pypi/mail-deduplicate) [![Python versions](https://
 img.shields.io/pypi/pyversions/mail-deduplicate.svg)](https://pypi.python.org/
-pypi/mail-deduplicate)\n[![Unittests status](https://github.com/kdeldycke/mail-
+pypi/mail-deduplicate) [![Unittests status](https://github.com/kdeldycke/mail-
 deduplicate/actions/workflows/tests.yaml/badge.svg?branch=main)](https://
 github.com/kdeldycke/mail-deduplicate/actions/workflows/
-tests.yaml?query=branch%3Amain)\n[![Documentation status](https://github.com/
+tests.yaml?query=branch%3Amain) [![Documentation status](https://github.com/
 kdeldycke/mail-deduplicate/actions/workflows/docs.yaml/badge.svg?branch=main)]
 (https://github.com/kdeldycke/mail-deduplicate/actions/workflows/
-docs.yaml?query=branch%3Amain)\n[![Coverage status](https://codecov.io/gh/
-kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://codecov.io/gh/
-kdeldycke/mail-deduplicate/branch/main)\n[![DOI](https://zenodo.org/badge/
-9016537.svg)](https://zenodo.org/badge/latestdoi/9016537)\n\n**What is Mail
-Deduplicate?**\n\nProvides the `mdedup` CLI, an utility to deduplicate mails
-from a set of boxes.\n\n
-                            \n [Mail Deduplicate]\n
-\n\n## Features\n\n- Duplicate detection based on cherry-picked and normalized
-mail\n headers.\n- Fetch mails from multiple sources.\n- Reads and writes to
-`mbox`, `maildir`, `babyl`, `mh` and `mmdf`\n formats.\n- Deduplication
-strategies based on size, content, timestamp, file path\n or random choice.\n-
-Copy, move or delete the resulting set of duplicates.\n- Dry-run mode.\n-
-Protection against false-positives with safety checks on size and content
-differences.\n- Supports macOS, Linux and Windows.\n- [Standalone executables]
-(#executables) for Linux, macOS and Windows.\n- Shell auto-completion for Bash,
-Zsh and Fish.\n\n> â ï¸ **Warning**: Performances\n>\n> `mdedup`
-implementation is quite naive at the moment and everything resides in
-memory.\n>\n> If this is good enough for a volume of a couple of gigabytes, the
-more emails `mdedup` try to parse, the closer you\'ll reach the memory limits
-of your machine. In which case [`mdedup` will exit abrubtly](https://
-github.com/kdeldycke/mail-deduplicate/issues/362#issuecomment-1266743045),
-zapped by the [OOM killer](https://en.wikipedia.org/wiki/Out_of_memory) of your
-OS. Of course your mileage may vary depending on your hardware.\n>\n> You can
-influence implementation of this feature with pull requests, or [purchase of
-business support ð¤ and sponsorship ð«¶](https://github.com/sponsors/
-kdeldycke).\n\n## Example\n\n
-  \n [https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/
-                        images/cli-coloured-run.png]\n
-\n\n## Installation\n\n### From sources\n\nEasiest way is to install `mdedup`
-from sources with [`pipx`](https://pypa.github.io/pipx/):\n\n```shell-
-session\n$ pipx install mail-deduplicate\n```\n\nOther\n[alternatives
-installation methods](https://kdeldycke.github.io/mail-deduplicate/
-install.html)\nare available in the documentation.\n\n###
-Executables\n\nStandalone executables of `mdedup`\'s latest version are
-available for several platforms and architectures:\n\n| Platform | `x86_64`
-|\n| ----------- | ------------------------------------------------------------
----------------------------------------------------------------------- |\n|
-**Linux** | [Download `mdedup-linux-x64.bin`](https://github.com/kdeldycke/
-mail-deduplicate/releases/latest/download/mdedup-linux-x64.bin) |\n| **macOS**
-| [Download `mdedup-macos-x64.bin`](https://github.com/kdeldycke/mail-
-deduplicate/releases/latest/download/mdedup-macos-x64.bin) |\n| **Windows** |
-[Download `mdedup-windows-x64.exe`](https://github.com/kdeldycke/mail-
-deduplicate/releases/latest/download/mdedup-windows-x64.exe) |\n', 'author':
-'Kevin Deldycke', 'author_email': 'kevin@deldycke.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/kdeldycke/mail-
-deduplicate', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+docs.yaml?query=branch%3Amain) [![Coverage status](https://codecov.io/gh/
+kdeldycke/mail-deduplicate/branch/main/graph/badge.svg)](https://
+app.codecov.io/gh/kdeldycke/mail-deduplicate) [![DOI](https://zenodo.org/badge/
+9016537.svg)](https://zenodo.org/badge/latestdoi/9016537) **What is Mail
+Deduplicate?** Provides the `mdedup` CLI, an utility to deduplicate mails from
+a set of boxes.
+                              [Mail Deduplicate]
+## Features - Duplicate detection based on cherry-picked and normalized mail
+headers. - Fetch mails from multiple sources. - Reads and writes to `mbox`,
+`maildir`, `babyl`, `mh` and `mmdf` formats. - Deduplication strategies based
+on size, content, timestamp, file path or random choice. - Copy, move or delete
+the resulting set of duplicates. - Dry-run mode. - Protection against false-
+positives with safety checks on size and content differences. - Supports macOS,
+Linux and Windows. - [Standalone executables](#executables) for Linux, macOS
+and Windows. - Shell auto-completion for Bash, Zsh and Fish. > â ï¸
+**Warning**: Performances > > `mdedup` implementation is quite naive at the
+moment and everything resides in memory. > > If this is good enough for a
+volume of a couple of gigabytes, the more emails `mdedup` try to parse, the
+closer you'll reach the memory limits of your machine. In which case [`mdedup`
+will exit abrubtly](https://github.com/kdeldycke/mail-deduplicate/issues/
+362#issuecomment-1266743045), zapped by the [OOM killer](https://
+en.wikipedia.org/wiki/Out_of_memory) of your OS. Of course your mileage may
+vary depending on your hardware. > > You can influence implementation of this
+feature with pull requests, or [purchase of business support ð¤ and
+sponsorship ð«¶](https://github.com/sponsors/kdeldycke). ## Example
+[https://raw.githubusercontent.com/kdeldycke/mail-deduplicate/main/docs/assets/
+                             cli-coloured-run.png]
+## Installation ### From sources Easiest way is to install `mdedup` from
+sources with [`pipx`](https://pypa.github.io/pipx/): ```shell-session $ pipx
+install mail-deduplicate ``` Other [alternatives installation methods](https://
+kdeldycke.github.io/mail-deduplicate/install.html) are available in the
+documentation. ### Executables Standalone executables of `mdedup`'s latest
+version are available for several platforms and architectures: | Platform |
+`x86_64` | | ----------- | ----------------------------------------------------
+-----------------------------------------------------------------------------
+- | | **Linux** | [Download `mdedup-linux-x64.bin`](https://github.com/
+kdeldycke/mail-deduplicate/releases/latest/download/mdedup-linux-x64.bin) | |
+**macOS** | [Download `mdedup-macos-x64.bin`](https://github.com/kdeldycke/
+mail-deduplicate/releases/latest/download/mdedup-macos-x64.bin) | | **Windows**
+| [Download `mdedup-windows-x64.exe`](https://github.com/kdeldycke/mail-
+deduplicate/releases/latest/download/mdedup-windows-x64.exe) |
```

