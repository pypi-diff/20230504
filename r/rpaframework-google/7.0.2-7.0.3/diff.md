# Comparing `tmp/rpaframework_google-7.0.2.tar.gz` & `tmp/rpaframework_google-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_google-7.0.2.tar", max compression
+gzip compressed data, was "rpaframework_google-7.0.3.tar", max compression
```

## Comparing `rpaframework_google-7.0.2.tar` & `rpaframework_google-7.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11358 2022-05-25 11:29:26.067107 rpaframework_google-7.0.2/LICENSE
--rw-r--r--   0        0        0      202 2022-05-25 11:29:26.067378 rpaframework_google-7.0.2/README.rst
--rw-r--r--   0        0        0   114989 2023-04-05 08:31:39.115330 rpaframework_google-7.0.2/RPA_Cloud_Google.libspec
--rw-r--r--   0        0        0     2353 2023-04-05 08:26:05.770866 rpaframework_google-7.0.2/pyproject.toml
--rw-r--r--   0        0        0     8041 2023-02-03 14:24:02.138807 rpaframework_google-7.0.2/src/RPA/Cloud/Google/__init__.py
--rw-r--r--   0        0        0      832 2022-09-27 11:30:02.277133 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/__init__.py
--rw-r--r--   0        0        0     2651 2022-05-25 11:29:26.068930 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/apps_script.py
--rw-r--r--   0        0        0      882 2022-09-27 11:30:02.277226 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/base.py
--rw-r--r--   0        0        0    10487 2022-09-27 11:30:02.277342 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/context.py
--rw-r--r--   0        0        0    11659 2023-02-03 14:24:02.139111 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/document_ai.py
--rw-r--r--   0        0        0    40080 2022-09-09 11:28:10.211864 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/drive.py
--rw-r--r--   0        0        0     2731 2022-09-09 11:28:10.212117 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/enums.py
--rw-r--r--   0        0        0    12499 2022-05-25 11:29:26.069541 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/gmail.py
--rw-r--r--   0        0        0     4226 2022-05-25 11:29:26.069613 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/natural_language.py
--rw-r--r--   0        0        0     7448 2022-05-25 11:29:26.069709 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/sheets.py
--rw-r--r--   0        0        0     3945 2022-05-25 11:29:26.069786 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/speech_to_text.py
--rw-r--r--   0        0        0     8351 2022-05-25 11:29:26.070016 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/storage.py
--rw-r--r--   0        0        0     3401 2022-05-25 11:29:26.070090 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/text_to_speech.py
--rw-r--r--   0        0        0     2608 2022-05-25 11:29:26.070175 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/translation.py
--rw-r--r--   0        0        0     3763 2022-05-25 11:29:26.070249 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/video_intelligence.py
--rw-r--r--   0        0        0     5332 2022-05-25 11:29:26.070322 rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/vision.py
--rw-r--r--   0        0        0     3301 2023-02-03 14:24:02.139397 rpaframework_google-7.0.2/src/RPA/scripts/google_authenticate.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 rpaframework_google-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11560 2022-09-28 13:20:32.478375 rpaframework_google-7.0.3/LICENSE
+-rw-r--r--   0        0        0     2436 2023-05-04 14:34:13.762891 rpaframework_google-7.0.3/pyproject.toml
+-rw-r--r--   0        0        0      209 2022-09-28 13:20:32.479375 rpaframework_google-7.0.3/README.rst
+-rw-r--r--   0        0        0   118394 2023-05-04 14:36:19.988497 rpaframework_google-7.0.3/RPA_Cloud_Google.libspec
+-rw-r--r--   0        0        0     8305 2023-03-06 14:03:56.085715 rpaframework_google-7.0.3/src/RPA/Cloud/Google/__init__.py
+-rw-r--r--   0        0        0      858 2022-09-28 13:20:32.488375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/__init__.py
+-rw-r--r--   0        0        0     2736 2022-09-28 13:20:32.488375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/apps_script.py
+-rw-r--r--   0        0        0      907 2022-09-28 13:20:32.492375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/base.py
+-rw-r--r--   0        0        0    10778 2022-09-28 13:20:32.497374 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/context.py
+-rw-r--r--   0        0        0    11981 2023-01-22 13:06:04.163745 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/document_ai.py
+-rw-r--r--   0        0        0    41274 2023-05-04 13:22:36.846117 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/drive.py
+-rw-r--r--   0        0        0     2830 2022-09-28 13:20:32.502375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/enums.py
+-rw-r--r--   0        0        0    12844 2022-09-28 13:20:32.502375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/gmail.py
+-rw-r--r--   0        0        0     4355 2022-09-28 13:20:32.502375 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/natural_language.py
+-rw-r--r--   0        0        0     7698 2023-01-02 18:36:35.670926 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/sheets.py
+-rw-r--r--   0        0        0     4059 2022-09-28 13:20:32.503374 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/speech_to_text.py
+-rw-r--r--   0        0        0     8628 2022-09-28 13:20:32.504376 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/storage.py
+-rw-r--r--   0        0        0     3514 2022-09-28 13:20:32.504376 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/text_to_speech.py
+-rw-r--r--   0        0        0     2690 2022-09-28 13:20:32.504376 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/translation.py
+-rw-r--r--   0        0        0     3865 2022-09-28 13:20:32.505381 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/video_intelligence.py
+-rw-r--r--   0        0        0     5502 2022-11-24 09:58:33.719283 rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/vision.py
+-rw-r--r--   0        0        0     3418 2023-01-22 13:06:04.164747 rpaframework_google-7.0.3/src/RPA/scripts/google_authenticate.py
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 rpaframework_google-7.0.3/PKG-INFO
```

### Comparing `rpaframework_google-7.0.2/LICENSE` & `rpaframework_google-7.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2020 Robocorp Technologies, Inc.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2020 Robocorp Technologies, Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `rpaframework_google-7.0.2/RPA_Cloud_Google.libspec` & `rpaframework_google-7.0.3/RPA_Cloud_Google.libspec`

 * *Files 15% similar despite different names*

#### Comparing `rpaframework_google-7.0.2/RPA_Cloud_Google.libspec` & `rpaframework_google-7.0.3/RPA_Cloud_Google.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.Cloud.Google" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-04-05T08:31:39Z" specversion="4" source="./RPA/Cloud/Google/__init__.py" lineno="33">
+<keywordspec name="RPA.Cloud.Google" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-05-04T14:36:19Z" specversion="4" source="./RPA/Cloud/Google/__init__.py" lineno="33">
   <version/>
   <doc>`Google` is a library for operating with Google API endpoints.
 
 Usage requires the following steps:
 
 - Create a GCP project
 - Enable approriate APIs
@@ -235,15 +235,15 @@
 :param vault_secret_key: Robocorp secret key
 :param cloud_auth_type: &quot;serviceaccount&quot; or &quot;token&quot;,
  defaults to &quot;serviceaccount&quot;</doc>
       <shortdoc>Library initialization</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Add Drive Share" source="./RPA/Cloud/Google/keywords/drive.py" lineno="716">
+    <kw name="Add Drive Share" source="./RPA/Cloud/Google/keywords/drive.py" lineno="721">
       <arguments repr="file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, source: str | None = None, email: str | None = None, domain: str | None = None, role: DriveRole = READER, share_type: DriveType = USER, notification: bool = False, notification_message: str | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -636,15 +636,15 @@
 
     ${result}=  Copy Sheet   ${SHEET_ID}  ${NEW_SHEET}</doc>
       <shortdoc>Copy spreadsheet to target spreadsheet</shortdoc>
       <tags>
         <tag>sheets</tag>
       </tags>
     </kw>
-    <kw name="Create Drive Directory" source="./RPA/Cloud/Google/keywords/drive.py" lineno="617">
+    <kw name="Create Drive Directory" source="./RPA/Cloud/Google/keywords/drive.py" lineno="622">
       <arguments repr="folder: str | None = None, parent_folder: str | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="folder: str | None = None">
           <name>folder</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -717,15 +717,15 @@
 
     ${result}=   Create Storage Bucket   visionfolder</doc>
       <shortdoc>Create Google Cloud Storage bucket</shortdoc>
       <tags>
         <tag>storage</tag>
       </tags>
     </kw>
-    <kw name="Delete Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="332">
+    <kw name="Delete Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="335">
       <arguments repr="file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, multiple_ok: bool = False, suppress_errors: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -1049,15 +1049,15 @@
 
     ${result}=  Download Storage Files  ${BUCKET_NAME}   test1.txt,test2.txt</doc>
       <shortdoc>Download files from a bucket</shortdoc>
       <tags>
         <tag>storage</tag>
       </tags>
     </kw>
-    <kw name="Export Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="667">
+    <kw name="Export Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="672">
       <arguments repr="file_id: str | None = None, file_dict: dict | None = None, target_file: str | None = None, mimetype: str = application/pdf">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -1175,15 +1175,15 @@
 :return: detected languages in the document response as a list</doc>
       <shortdoc>Helper keyword for getting detected `languages` from a ``Process Document`` response object.</shortdoc>
       <tags>
         <tag>document ai</tag>
         <tag>get</tag>
       </tags>
     </kw>
-    <kw name="Get Drive File By Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="1027">
+    <kw name="Get Drive File By Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="1032">
       <arguments repr="file_id: str, suppress_errors: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="file_id: str">
           <name>file_id</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="suppress_errors: bool = False">
           <name>suppress_errors</name>
@@ -1205,15 +1205,15 @@
     ${file_dict}=  Get Drive File By ID    file_id=${FILE_ID}</doc>
       <shortdoc>Get file dictionary by its file id.</shortdoc>
       <tags>
         <tag>drive</tag>
         <tag>v2.0.0</tag>
       </tags>
     </kw>
-    <kw name="Get Drive Folder Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="377">
+    <kw name="Get Drive Folder Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="380">
       <arguments repr="folder: str | None = None, parent_folder: str | None = None, details: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="folder: str | None = None">
           <name>folder</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -1949,15 +1949,15 @@
         print(f&quot;Processor type: {p.type_}&quot;)
         print(f&quot;Processor name: {p.display_name}&quot;)</doc>
       <shortdoc>List existing document AI processors from given project and region.</shortdoc>
       <tags>
         <tag>document ai</tag>
       </tags>
     </kw>
-    <kw name="List Shared Drive Files" source="./RPA/Cloud/Google/keywords/drive.py" lineno="486">
+    <kw name="List Shared Drive Files" source="./RPA/Cloud/Google/keywords/drive.py" lineno="491">
       <arguments repr="query: str | None = None, source: str | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="query: str | None = None">
           <name>query</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -2096,15 +2096,15 @@
     for ent in entities:
         print(ent)</doc>
       <shortdoc>Loads the binary object saved by ``Save Document Response`` into ``documentai.Document`` format which is accessible by helper keywords.</shortdoc>
       <tags>
         <tag>document ai</tag>
       </tags>
     </kw>
-    <kw name="Move Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="423">
+    <kw name="Move Drive File" source="./RPA/Cloud/Google/keywords/drive.py" lineno="426">
       <arguments repr="file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, source: str | None = None, target: str | None = None, multiple_ok: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -2295,15 +2295,15 @@
 
     ${result}=  Recognize Text From Audio   audio_file=${CURDIR}${/}test.mp3</doc>
       <shortdoc>Recognize text in the audio file</shortdoc>
       <tags>
         <tag>speech to text</tag>
       </tags>
     </kw>
-    <kw name="Remove All Drive Shares" source="./RPA/Cloud/Google/keywords/drive.py" lineno="984">
+    <kw name="Remove All Drive Shares" source="./RPA/Cloud/Google/keywords/drive.py" lineno="989">
       <arguments repr="file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, suppress_errors: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -2343,15 +2343,15 @@
       <shortdoc>Keyword for removing all shares from selected files (only owner permission is retained).</shortdoc>
       <tags>
         <tag>drive</tag>
         <tag>drive share</tag>
         <tag>v2.0.0</tag>
       </tags>
     </kw>
-    <kw name="Remove Drive Share By Criteria" source="./RPA/Cloud/Google/keywords/drive.py" lineno="877">
+    <kw name="Remove Drive Share By Criteria" source="./RPA/Cloud/Google/keywords/drive.py" lineno="882">
       <arguments repr="email: str | None = None, domain: str | None = None, permission_id: str | None = None, file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, source: str | None = None, suppress_errors: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="email: str | None = None">
           <name>email</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -2433,15 +2433,15 @@
       <shortdoc>Keyword for removing share from file or folder based on criteria.</shortdoc>
       <tags>
         <tag>drive</tag>
         <tag>drive share</tag>
         <tag>v2.0.0</tag>
       </tags>
     </kw>
-    <kw name="Remove Drive Share By Permission Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="815">
+    <kw name="Remove Drive Share By Permission Id" source="./RPA/Cloud/Google/keywords/drive.py" lineno="820">
       <arguments repr="permission_id: str, file_id: str | None = None, file_dict: dict | None = None, query: str | None = None, source: str | None = None, suppress_errors: bool = False">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="permission_id: str">
           <name>permission_id</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="file_id: str | None = None">
           <name>file_id</name>
@@ -2583,15 +2583,15 @@
     )
     GOOGLE.save_document_response(document, &quot;receipt.response&quot;)</doc>
       <shortdoc>Save ``Process Document`` response into a binary file.</shortdoc>
       <tags>
         <tag>document ai</tag>
       </tags>
     </kw>
-    <kw name="Search Drive Files" source="./RPA/Cloud/Google/keywords/drive.py" lineno="509">
+    <kw name="Search Drive Files" source="./RPA/Cloud/Google/keywords/drive.py" lineno="514">
       <arguments repr="query: str | None = None, recurse: bool = False, source: str | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="query: str | None = None">
           <name>query</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
```

### Comparing `rpaframework_google-7.0.2/pyproject.toml` & `rpaframework_google-7.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-[tool.poetry]
-name = "rpaframework-google"
-version = "7.0.2"
-description = "Google library for RPA Framework"
-authors = ["RPA Framework <rpafw@robocorp.com>"]
-license = "Apache-2.0"
-readme = "README.rst"
-
-homepage = "https://rpaframework.org/"
-documentation = "https://rpaframework.org/"
-repository = "https://github.com/robocorp/rpaframework"
-
-keywords = ["robotframework", "rpa", "automation", "google"]
-classifiers = [
-	"License :: OSI Approved :: Apache Software License",
-	"Development Status :: 5 - Production/Stable",
-	"Operating System :: OS Independent",
-	"Intended Audience :: Developers",
-	"Topic :: Software Development :: Libraries :: Python Modules",
-	"Topic :: Software Development :: Libraries",
-	"Framework :: Robot Framework :: Library",
-	"Framework :: Robot Framework",
-	"Programming Language :: Python :: 3.7",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-]
-
-include = ["*.libspec"]
-
-packages = [{ include = "RPA", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.7"
-rpaframework-core = "^11.0.0"
-robotframework = ">=4.0.0,!=4.0.1,<6.0.0"
-robotframework-pythonlibcore = "^4.0.0"
-google-api-python-client = "^2.58.0"
-google-auth-httplib2 = "^0.1.0"
-google-auth-oauthlib = "^0.5.2"
-google-cloud-language = "^2.5.2"
-google-cloud-speech = "^2.15.1"
-google-cloud-storage = "^2.5.0"
-google-cloud-texttospeech = "^2.12.1"
-google-cloud-translate = "^3.8.1"
-google-cloud-videointelligence = "^2.8.1"
-google-cloud-vision = "^3.1.1"
-google-cloud-documentai = "^2.0.1"
-grpcio = "^1.48.1"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-flake8 = "^3.7.9"
-pylint = "^2.4.4, <2.13"
-pytest = "^7.2.0"
-mock = "^5.0.0"
-pytest-cov = "^4.0.0"
-invoke = "^1.6.0"
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.1.1"
-toml = "^0.10.2"
-sphinx-markdown-builder = "^0.5.4"
-robotframework-docgen = "^0.15.0"
-sphinx-issues = "^3.0.1"
-docutils = "0.16"
-colorama = "^0.4.5"
-keyring = "^23.9.0"
-PyYAML = "^5.4.1"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.7"
-
-[tool.poetry.scripts]
-rpa-google-oauth = 'RPA.scripts.google_authenticate:main'
-
-[tool.black]
-target-version = ["py37", "py38", "py39"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-addopts = "-v --cov=src --cov-report term-missing --cov-branch"
-testpaths = ["tests"]
+[tool.poetry]
+name = "rpaframework-google"
+version = "7.0.3"
+description = "Google library for RPA Framework"
+authors = ["RPA Framework <rpafw@robocorp.com>"]
+license = "Apache-2.0"
+readme = "README.rst"
+
+homepage = "https://rpaframework.org/"
+documentation = "https://rpaframework.org/"
+repository = "https://github.com/robocorp/rpaframework"
+
+keywords = ["robotframework", "rpa", "automation", "google"]
+classifiers = [
+	"License :: OSI Approved :: Apache Software License",
+	"Development Status :: 5 - Production/Stable",
+	"Operating System :: OS Independent",
+	"Intended Audience :: Developers",
+	"Topic :: Software Development :: Libraries :: Python Modules",
+	"Topic :: Software Development :: Libraries",
+	"Framework :: Robot Framework :: Library",
+	"Framework :: Robot Framework",
+	"Programming Language :: Python :: 3.7",
+	"Programming Language :: Python :: 3.8",
+	"Programming Language :: Python :: 3.9",
+]
+
+include = ["*.libspec"]
+
+packages = [{ include = "RPA", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.7"
+rpaframework-core = "^11.0.0"
+robotframework = ">=4.0.0,!=4.0.1,<6.0.0"
+robotframework-pythonlibcore = "^4.0.0"
+google-api-python-client = "^2.58.0"
+google-auth-httplib2 = "^0.1.0"
+google-auth-oauthlib = "^0.5.2"
+google-cloud-language = "^2.5.2"
+google-cloud-speech = "^2.15.1"
+google-cloud-storage = "^2.5.0"
+google-cloud-texttospeech = "^2.12.1"
+google-cloud-translate = "^3.8.1"
+google-cloud-videointelligence = "^2.8.1"
+google-cloud-vision = "^3.1.1"
+google-cloud-documentai = "^2.0.1"
+grpcio = "^1.48.1"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.3.0"
+flake8 = "^3.7.9"
+pylint = "^2.4.4, <2.13"
+pytest = "^7.2.0"
+mock = "^5.0.0"
+pytest-cov = "^4.0.0"
+invoke = "^1.6.0"
+sphinx = "^5.3.0"
+sphinx-rtd-theme = "^1.1.1"
+toml = "^0.10.2"
+sphinx-markdown-builder = "^0.5.4"
+robotframework-docgen = "^0.15.0"
+sphinx-issues = "^3.0.1"
+docutils = "0.16"
+colorama = "^0.4.5"
+keyring = "^23.9.0"
+PyYAML = "^5.4.1"
+flake8-docstrings = "^1.6.0"
+flake8-rst-docstrings = "^0.2.7"
+
+[tool.poetry.scripts]
+rpa-google-oauth = 'RPA.scripts.google_authenticate:main'
+
+[tool.black]
+target-version = ["py37", "py38", "py39"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = "-v --cov=src --cov-report term-missing --cov-branch"
+testpaths = ["tests"]
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/__init__.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-import importlib
-import logging
-import os
-from robotlibcore import DynamicCore
-
-
-from .keywords import (
-    AppsScriptKeywords,
-    BaseKeywords,
-    DocumentAIKeywords,
-    DriveKeywords,
-    GmailKeywords,
-    NaturalLanguageKeywords,
-    SheetsKeywords,
-    SpeechToTextKeywords,
-    StorageKeywords,
-    TextToSpeechKeywords,
-    TranslationKeywords,
-    VideoIntelligenceKeywords,
-    VisionKeywords,
-)
-
-
-def import_vault():
-    """Try to import Vault/Secrets library, with the new name."""
-    try:
-        module = importlib.import_module("RPA.Robocorp.Vault")
-        return getattr(module, "Vault")
-    except ModuleNotFoundError:
-        return None
-
-
-class Google(DynamicCore):
-    """`Google` is a library for operating with Google API endpoints.
-
-    Usage requires the following steps:
-
-    - Create a GCP project
-    - Enable approriate APIs
-    - Create credentials (OAuth or service account)
-    - Install rpaframework-google package
-
-    **Google authentication**
-
-    Authentication for Google is set with `service account JSON file` which can be given to the library
-    in three different ways or with `OAuth2 token`, which is used for OAuth authentication.
-
-    Methods when using service account:
-
-    - Method 1 as environment variables, ``GOOGLE_APPLICATION_CREDENTIALS`` with path to service account file.
-    - Method 2 as keyword parameter to ``Init Storage`` for example.
-    - Method 3 as Robocorp vault secret. The vault name and secret key name needs to be given in library init
-      or with keyword ``Set Robocorp Vault``. Secret value should contain JSON file contents.
-
-    Method 1. service account using environment variable
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-
-        *** Tasks ***
-        Init Google services
-            # NO parameters for Init Vision, expecting to get JSON
-            # with GOOGLE_APPLICATION_CREDENTIALS environment variable
-            Init Vision
-
-    Method 2. service account with keyword parameter
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-
-        *** Tasks ***
-        Init Google services
-            Init Speech To Text   /path/to/service_account.json
-
-    Method 3. setting Robocorp Vault in the library init
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-        ...       vault_name=googlecloud
-        ...       vault_secret_key=servicecreds
-
-        *** Tasks ***
-        Init Google services
-            Init Storage
-
-    Method 3. setting Robocorp Vault with keyword
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-
-        *** Tasks ***
-        Init Google services
-            Set Robocorp Vault   vault_name=googlecloud  vault_secret_key=servicecreds
-            Init Storage    use_robocorp_vault=${TRUE}
-
-    Methods when using OAuth token:
-
-    - Method 1 as keyword parameter ``token_file`` to ``Init Storage`` for example.
-    - Method 2 as Robocorp vault secret. The vault name and secret key name needs to be given in library init
-      or with keyword ``Set Robocorp Vault``. Secret value should contain JSON file contents.
-
-    Method 1. The Google Apps Script and Google Drive services are authenticated using this method.
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-
-        *** Variables ***
-        @{SCRIPT_SCOPES}     forms   spreadsheets
-
-        *** Tasks ***
-        Init Google OAuth services
-            Init Apps Script    token_file=oauth_token   ${SCRIPT_SCOPES}
-
-    Method 2. setting Robocorp Vault in the library init
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-        ...       vault_name=googlecloud
-        ...       vault_secret_key=oauth
-        ...       cloud_auth_type=token
-
-        *** Tasks ***
-        Init Google services
-            Init Storage
-
-
-    **Creating and using OAuth token file**
-
-    The token file can be created using `credentials.json` by running command:
-
-    ``rpa-google-oauth --credentials <filepath> --service drive`` or
-    ``rpa-google-oauth --credentials <filepath> --scopes drive.appdata,drive.file,drive.install``
-
-    This will start web based authentication process, which outputs the token at the end.
-    Token could be stored into ``Robocorp Vault``.
-
-    Example Vault content.
-
-    .. code-block:: json
-
-        "googlecloud": {
-            "oauth-token": "gANfd123321aabeedYsc"
-        }
-
-    Using the Vault.
-
-    .. code-block:: robotframework
-
-        *** Keywords ***
-        Set up Google Drive authentication
-            Set Robocorp Vault   vault_name=googlecloud
-            ...  vault_secret_key=oauth-token
-            ...  cloud_auth_type=token
-            Init Drive
-
-
-    **Installation**
-
-    This library, ``RPA.Cloud.Google`` is available via **rpaframework-google** package.
-
-    Check the latest package version from `PyPI`_.
-
-    .. _PyPI: https://pypi.org/project/rpaframework-google/
-
-    **Examples**
-
-    **Robot Framework**
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library   RPA.Cloud.Google
-
-        *** Variables ***
-        ${SERVICE_ACCOUNT}    ${/}path${/}to${/}service_account.json
-        ${BUCKET_NAME}            testbucket12213123123
-
-        *** Tasks ***
-        Upload a file into a new storage bucket
-            [Setup]   Init Storage    ${SERVICE_ACCOUNT}
-            Create Storage Bucket    ${BUCKET_NAME}
-            Upload Storage File      ${BUCKET_NAME}
-            ...   ${/}path${/}to${/}file.pdf
-            ...   myfile.pdf
-            @{files}         List Storage Files   ${BUCKET_NAME}
-            FOR   ${file}  IN   @{files}
-                Log  ${file}
-            END
-
-    **Python**
-
-    .. code-block:: python
-
-        from RPA.Cloud.Google import Google
-
-        library = Google
-        service_account = '/path/to/service_account.json'
-
-        library.init_vision(service_account)
-        library.init_text_to_speech(service_account)
-
-        response = library.detect_text('imagefile.png', 'result.json')
-        library.synthesize_speech('I want this said aloud', target_file='said.mp3')
-    """  # noqa: E501
-
-    ROBOT_LIBRARY_SCOPE = "GLOBAL"
-    ROBOT_LIBRARY_DOC_FORMAT = "REST"
-
-    def __init__(
-        self,
-        service_account: str = None,
-        vault_name: str = None,
-        vault_secret_key: str = None,
-        cloud_auth_type: str = "serviceaccount",
-    ):
-        """Library initialization
-
-        :param service_account: path to service account
-        :param vault_name: Robocorp vault name
-        :param vault_secret_key: Robocorp secret key
-        :param cloud_auth_type: "serviceaccount" or "token",
-         defaults to "serviceaccount"
-        """
-        self.logger = logging.getLogger(__name__)
-        self.service_account_file = service_account
-        self.robocorp_vault_name = vault_name
-        self.robocorp_vault_secret_key = vault_secret_key
-        self.cloud_auth_type = cloud_auth_type
-        self.use_robocorp_vault = False
-        if self.robocorp_vault_name and self.robocorp_vault_secret_key:
-            self.use_robocorp_vault = True
-        if self.service_account_file is None:
-            self.service_account_file = os.getenv("GOOGLE_APPLICATION_CREDENTIALS")
-        self.secrets_library = import_vault()
-
-        # Register keyword libraries to LibCore
-        libraries = [
-            AppsScriptKeywords(self),
-            BaseKeywords(self),
-            DocumentAIKeywords(self),
-            DriveKeywords(self),
-            GmailKeywords(self),
-            NaturalLanguageKeywords(self),
-            SheetsKeywords(self),
-            SpeechToTextKeywords(self),
-            StorageKeywords(self),
-            TextToSpeechKeywords(self),
-            TranslationKeywords(self),
-            VideoIntelligenceKeywords(self),
-            VisionKeywords(self),
-        ]
-        super().__init__(libraries)
+import importlib
+import logging
+import os
+from robotlibcore import DynamicCore
+
+
+from .keywords import (
+    AppsScriptKeywords,
+    BaseKeywords,
+    DocumentAIKeywords,
+    DriveKeywords,
+    GmailKeywords,
+    NaturalLanguageKeywords,
+    SheetsKeywords,
+    SpeechToTextKeywords,
+    StorageKeywords,
+    TextToSpeechKeywords,
+    TranslationKeywords,
+    VideoIntelligenceKeywords,
+    VisionKeywords,
+)
+
+
+def import_vault():
+    """Try to import Vault/Secrets library, with the new name."""
+    try:
+        module = importlib.import_module("RPA.Robocorp.Vault")
+        return getattr(module, "Vault")
+    except ModuleNotFoundError:
+        return None
+
+
+class Google(DynamicCore):
+    """`Google` is a library for operating with Google API endpoints.
+
+    Usage requires the following steps:
+
+    - Create a GCP project
+    - Enable approriate APIs
+    - Create credentials (OAuth or service account)
+    - Install rpaframework-google package
+
+    **Google authentication**
+
+    Authentication for Google is set with `service account JSON file` which can be given to the library
+    in three different ways or with `OAuth2 token`, which is used for OAuth authentication.
+
+    Methods when using service account:
+
+    - Method 1 as environment variables, ``GOOGLE_APPLICATION_CREDENTIALS`` with path to service account file.
+    - Method 2 as keyword parameter to ``Init Storage`` for example.
+    - Method 3 as Robocorp vault secret. The vault name and secret key name needs to be given in library init
+      or with keyword ``Set Robocorp Vault``. Secret value should contain JSON file contents.
+
+    Method 1. service account using environment variable
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+
+        *** Tasks ***
+        Init Google services
+            # NO parameters for Init Vision, expecting to get JSON
+            # with GOOGLE_APPLICATION_CREDENTIALS environment variable
+            Init Vision
+
+    Method 2. service account with keyword parameter
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+
+        *** Tasks ***
+        Init Google services
+            Init Speech To Text   /path/to/service_account.json
+
+    Method 3. setting Robocorp Vault in the library init
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+        ...       vault_name=googlecloud
+        ...       vault_secret_key=servicecreds
+
+        *** Tasks ***
+        Init Google services
+            Init Storage
+
+    Method 3. setting Robocorp Vault with keyword
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+
+        *** Tasks ***
+        Init Google services
+            Set Robocorp Vault   vault_name=googlecloud  vault_secret_key=servicecreds
+            Init Storage    use_robocorp_vault=${TRUE}
+
+    Methods when using OAuth token:
+
+    - Method 1 as keyword parameter ``token_file`` to ``Init Storage`` for example.
+    - Method 2 as Robocorp vault secret. The vault name and secret key name needs to be given in library init
+      or with keyword ``Set Robocorp Vault``. Secret value should contain JSON file contents.
+
+    Method 1. The Google Apps Script and Google Drive services are authenticated using this method.
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+
+        *** Variables ***
+        @{SCRIPT_SCOPES}     forms   spreadsheets
+
+        *** Tasks ***
+        Init Google OAuth services
+            Init Apps Script    token_file=oauth_token   ${SCRIPT_SCOPES}
+
+    Method 2. setting Robocorp Vault in the library init
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+        ...       vault_name=googlecloud
+        ...       vault_secret_key=oauth
+        ...       cloud_auth_type=token
+
+        *** Tasks ***
+        Init Google services
+            Init Storage
+
+
+    **Creating and using OAuth token file**
+
+    The token file can be created using `credentials.json` by running command:
+
+    ``rpa-google-oauth --credentials <filepath> --service drive`` or
+    ``rpa-google-oauth --credentials <filepath> --scopes drive.appdata,drive.file,drive.install``
+
+    This will start web based authentication process, which outputs the token at the end.
+    Token could be stored into ``Robocorp Vault``.
+
+    Example Vault content.
+
+    .. code-block:: json
+
+        "googlecloud": {
+            "oauth-token": "gANfd123321aabeedYsc"
+        }
+
+    Using the Vault.
+
+    .. code-block:: robotframework
+
+        *** Keywords ***
+        Set up Google Drive authentication
+            Set Robocorp Vault   vault_name=googlecloud
+            ...  vault_secret_key=oauth-token
+            ...  cloud_auth_type=token
+            Init Drive
+
+
+    **Installation**
+
+    This library, ``RPA.Cloud.Google`` is available via **rpaframework-google** package.
+
+    Check the latest package version from `PyPI`_.
+
+    .. _PyPI: https://pypi.org/project/rpaframework-google/
+
+    **Examples**
+
+    **Robot Framework**
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library   RPA.Cloud.Google
+
+        *** Variables ***
+        ${SERVICE_ACCOUNT}    ${/}path${/}to${/}service_account.json
+        ${BUCKET_NAME}            testbucket12213123123
+
+        *** Tasks ***
+        Upload a file into a new storage bucket
+            [Setup]   Init Storage    ${SERVICE_ACCOUNT}
+            Create Storage Bucket    ${BUCKET_NAME}
+            Upload Storage File      ${BUCKET_NAME}
+            ...   ${/}path${/}to${/}file.pdf
+            ...   myfile.pdf
+            @{files}         List Storage Files   ${BUCKET_NAME}
+            FOR   ${file}  IN   @{files}
+                Log  ${file}
+            END
+
+    **Python**
+
+    .. code-block:: python
+
+        from RPA.Cloud.Google import Google
+
+        library = Google
+        service_account = '/path/to/service_account.json'
+
+        library.init_vision(service_account)
+        library.init_text_to_speech(service_account)
+
+        response = library.detect_text('imagefile.png', 'result.json')
+        library.synthesize_speech('I want this said aloud', target_file='said.mp3')
+    """  # noqa: E501
+
+    ROBOT_LIBRARY_SCOPE = "GLOBAL"
+    ROBOT_LIBRARY_DOC_FORMAT = "REST"
+
+    def __init__(
+        self,
+        service_account: str = None,
+        vault_name: str = None,
+        vault_secret_key: str = None,
+        cloud_auth_type: str = "serviceaccount",
+    ):
+        """Library initialization
+
+        :param service_account: path to service account
+        :param vault_name: Robocorp vault name
+        :param vault_secret_key: Robocorp secret key
+        :param cloud_auth_type: "serviceaccount" or "token",
+         defaults to "serviceaccount"
+        """
+        self.logger = logging.getLogger(__name__)
+        self.service_account_file = service_account
+        self.robocorp_vault_name = vault_name
+        self.robocorp_vault_secret_key = vault_secret_key
+        self.cloud_auth_type = cloud_auth_type
+        self.use_robocorp_vault = False
+        if self.robocorp_vault_name and self.robocorp_vault_secret_key:
+            self.use_robocorp_vault = True
+        if self.service_account_file is None:
+            self.service_account_file = os.getenv("GOOGLE_APPLICATION_CREDENTIALS")
+        self.secrets_library = import_vault()
+
+        # Register keyword libraries to LibCore
+        libraries = [
+            AppsScriptKeywords(self),
+            BaseKeywords(self),
+            DocumentAIKeywords(self),
+            DriveKeywords(self),
+            GmailKeywords(self),
+            NaturalLanguageKeywords(self),
+            SheetsKeywords(self),
+            SpeechToTextKeywords(self),
+            StorageKeywords(self),
+            TextToSpeechKeywords(self),
+            TranslationKeywords(self),
+            VideoIntelligenceKeywords(self),
+            VisionKeywords(self),
+        ]
+        super().__init__(libraries)
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/__init__.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# flake8: noqa
-
-from robot.api.deco import keyword
-from .context import (
-    LibraryContext,
-    ElementNotFound,
-    MultipleElementsFound,
-    TimeoutException,
-    GoogleOAuthAuthenticationError,
-)
-
-from .enums import TextType, to_texttype, UpdateAction, VideoFeature, to_feature
-from .base import BaseKeywords
-
-from .apps_script import AppsScriptKeywords
-from .document_ai import DocumentAIKeywords
-from .drive import DriveKeywords
-from .gmail import GmailKeywords
-from .natural_language import NaturalLanguageKeywords
-from .sheets import SheetsKeywords
-from .speech_to_text import SpeechToTextKeywords
-from .storage import StorageKeywords
-from .text_to_speech import TextToSpeechKeywords
-from .translation import TranslationKeywords
-from .video_intelligence import VideoIntelligenceKeywords
-from .vision import VisionKeywords
+# flake8: noqa
+
+from robot.api.deco import keyword
+from .context import (
+    LibraryContext,
+    ElementNotFound,
+    MultipleElementsFound,
+    TimeoutException,
+    GoogleOAuthAuthenticationError,
+)
+
+from .enums import TextType, to_texttype, UpdateAction, VideoFeature, to_feature
+from .base import BaseKeywords
+
+from .apps_script import AppsScriptKeywords
+from .document_ai import DocumentAIKeywords
+from .drive import DriveKeywords
+from .gmail import GmailKeywords
+from .natural_language import NaturalLanguageKeywords
+from .sheets import SheetsKeywords
+from .speech_to_text import SpeechToTextKeywords
+from .storage import StorageKeywords
+from .text_to_speech import TextToSpeechKeywords
+from .translation import TranslationKeywords
+from .video_intelligence import VideoIntelligenceKeywords
+from .vision import VisionKeywords
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/apps_script.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/apps_script.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from typing import Optional
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-
-class AppsScriptKeywords(LibraryContext):
-    """Class for Google Apps Script API
-
-    For more information about Google Apps Script API link_.
-
-    .. _link: https://developers.google.com/apps-script/api
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "apps script"])
-    def init_apps_script(
-        self,
-        service_account: str = None,
-        credentials: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        scopes: list = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Apps Script client
-
-        :param service_account: file path to service account file
-        :param credentials: file path to credentials file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param scopes: list of extra authentication scopes
-        :param token_file: file path to token file
-        """
-        apps_scopes = ["script.projects", "drive.scripts", "script.external_request"]
-        if scopes:
-            apps_scopes += scopes
-        self.service = self.init_service(
-            service_name="script",
-            api_version="v1",
-            scopes=apps_scopes,
-            service_account_file=service_account,
-            credentials_file=credentials,
-            use_robocorp_vault=use_robocorp_vault,
-            token_file=token_file,
-        )
-
-    @keyword(tags=["apps script"])
-    def run_script(
-        self, script_id: str, function_name: str, parameters: dict = None
-    ) -> None:
-        """Run the Google Apps Script function
-
-        :param script_id: Google Script identifier
-        :param function_name: name of the script function
-        :param parameters: script function parameters as a dictionary
-        :raises AssertionError: thrown when Google Script returns errors
-
-        Example:
-
-        .. code-block:: robotframework
-
-            &{params}=    Create Dictionary  formid=aaad4232  formvalues=1,2,3
-            ${response}=  Run Script    abc21397283712da  submit_form   ${params}
-            Log Many   ${response}
-        """
-        request = {
-            "function": function_name,
-        }
-        if parameters:
-            request["parameters"] = [parameters]
-        response = (
-            self.service.scripts()
-            .run(
-                body=request,
-                scriptId=script_id,
-            )
-            .execute()
-        )
-        if "error" in response.keys():
-            raise AssertionError(response["error"])
-        return response
+from typing import Optional
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+
+class AppsScriptKeywords(LibraryContext):
+    """Class for Google Apps Script API
+
+    For more information about Google Apps Script API link_.
+
+    .. _link: https://developers.google.com/apps-script/api
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "apps script"])
+    def init_apps_script(
+        self,
+        service_account: str = None,
+        credentials: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        scopes: list = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Apps Script client
+
+        :param service_account: file path to service account file
+        :param credentials: file path to credentials file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param scopes: list of extra authentication scopes
+        :param token_file: file path to token file
+        """
+        apps_scopes = ["script.projects", "drive.scripts", "script.external_request"]
+        if scopes:
+            apps_scopes += scopes
+        self.service = self.init_service(
+            service_name="script",
+            api_version="v1",
+            scopes=apps_scopes,
+            service_account_file=service_account,
+            credentials_file=credentials,
+            use_robocorp_vault=use_robocorp_vault,
+            token_file=token_file,
+        )
+
+    @keyword(tags=["apps script"])
+    def run_script(
+        self, script_id: str, function_name: str, parameters: dict = None
+    ) -> None:
+        """Run the Google Apps Script function
+
+        :param script_id: Google Script identifier
+        :param function_name: name of the script function
+        :param parameters: script function parameters as a dictionary
+        :raises AssertionError: thrown when Google Script returns errors
+
+        Example:
+
+        .. code-block:: robotframework
+
+            &{params}=    Create Dictionary  formid=aaad4232  formvalues=1,2,3
+            ${response}=  Run Script    abc21397283712da  submit_form   ${params}
+            Log Many   ${response}
+        """
+        request = {
+            "function": function_name,
+        }
+        if parameters:
+            request["parameters"] = [parameters]
+        response = (
+            self.service.scripts()
+            .run(
+                body=request,
+                scriptId=script_id,
+            )
+            .execute()
+        )
+        if "error" in response.keys():
+            raise AssertionError(response["error"])
+        return response
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/base.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from . import LibraryContext, keyword
-
-
-class BaseKeywords(LibraryContext):
-    """Base keywords for the Google library"""
-
-    @keyword
-    def set_robocorp_vault(
-        self,
-        vault_name: str = None,
-        vault_secret_key: str = None,
-        auth_type: str = "serviceaccount",
-    ):
-        """Set Robocorp Vault name and secret key name
-        :param vault_name: Robocorp Vault name
-        :param vault_secret_key: Robocorp Vault secret key name
-        :param auth_type: either `serviceaccount` or `token`
-        """
-        if vault_name:
-            self.ctx.robocorp_vault_name = vault_name
-        if vault_secret_key:
-            self.ctx.robocorp_vault_secret_key = vault_secret_key
-        if self.ctx.robocorp_vault_name and self.ctx.robocorp_vault_secret_key:
-            self.ctx.use_robocorp_vault = True
-        self.ctx.cloud_auth_type = auth_type
+from . import LibraryContext, keyword
+
+
+class BaseKeywords(LibraryContext):
+    """Base keywords for the Google library"""
+
+    @keyword
+    def set_robocorp_vault(
+        self,
+        vault_name: str = None,
+        vault_secret_key: str = None,
+        auth_type: str = "serviceaccount",
+    ):
+        """Set Robocorp Vault name and secret key name
+        :param vault_name: Robocorp Vault name
+        :param vault_secret_key: Robocorp Vault secret key name
+        :param auth_type: either `serviceaccount` or `token`
+        """
+        if vault_name:
+            self.ctx.robocorp_vault_name = vault_name
+        if vault_secret_key:
+            self.ctx.robocorp_vault_secret_key = vault_secret_key
+        if self.ctx.robocorp_vault_name and self.ctx.robocorp_vault_secret_key:
+            self.ctx.use_robocorp_vault = True
+        self.ctx.cloud_auth_type = auth_type
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/drive.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/drive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1052 +1,1057 @@
-from io import BytesIO
-import mimetypes
-from pathlib import Path
-import shutil
-import time
-from typing import Dict, List, Optional
-
-from apiclient.errors import HttpError
-from apiclient.http import MediaFileUpload, MediaIoBaseDownload
-
-from . import LibraryContext, keyword, UpdateAction
-from .enums import DriveRole, DriveType, to_drive_role, to_drive_type
-
-
-class GoogleDriveError(Exception):
-    """Raised with errors in Drive API"""
-
-
-class DriveKeywords(LibraryContext):
-    """Class for Google Drive API
-
-    For more information about Google Drive API link_.
-
-    .. _link: https://developers.google.com/drive/api
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "drive"])
-    def init_drive(
-        self,
-        service_account: str = None,
-        credentials: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        scopes: list = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Drive client
-
-        :param service_account: file path to service account file
-        :param credentials: file path to credentials file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param scopes: list of extra authentication scopes
-        :param token_file: file path to token file
-        """
-        drive_scopes = [
-            "drive",
-            "drive.appdata",
-            "drive.file",
-            "drive.install",
-            "drive.metadata",
-        ]
-        if scopes:
-            drive_scopes += scopes
-        self.service = self.init_service(
-            service_name="drive",
-            api_version="v3",
-            scopes=drive_scopes,
-            service_account_file=service_account,
-            credentials_file=credentials,
-            use_robocorp_vault=use_robocorp_vault,
-            token_file=token_file,
-        )
-
-    @keyword(tags=["drive"])
-    def upload_drive_file(
-        self,
-        filename: str = None,
-        folder: str = None,
-        overwrite: bool = False,
-        make_dir: bool = False,
-    ) -> str:
-        """Upload files into Drive
-
-        :param filename: name of the file to upload
-        :param folder: target folder for upload
-        :param overwrite: set to `True` if already existing file should be overwritten
-        :param make_dir: set to `True` if folder should be created if it does not exist
-        :return: uploaded file id
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${file1_id}=  Upload Drive File  data.json  # Upload file to drive root
-            ${file2_id}=  Upload Drive File  newdata.json  new_folder  make_dir=True
-            ${file3_id}=  Upload Drive File  data.json  overwrite=True
-        """
-        folder_id = self.get_drive_folder_id(folder)
-        if folder_id is None and make_dir:
-            folder = self.create_drive_directory(folder)
-            folder_id = folder["id"]
-        if folder_id is None:
-            raise GoogleDriveError(
-                "Target folder '%s' does not exist or could not be created" % folder
-            )
-
-        filepath = Path(filename)
-        if filepath.is_dir():
-            raise GoogleDriveError(
-                "The '%s' is a directory and can not be uploaded" % filename
-            )
-        elif not filepath.is_file():
-            raise GoogleDriveError("Filename '%s' does not exist" % filename)
-
-        query_string = f"name = '{filepath.name}' and '{folder_id}' in parents"
-        self.logger.debug("Upload query_string: '%s'" % query_string)
-        target_file = self.search_drive_files(query=query_string, recurse=True)
-        guess_mimetype = mimetypes.guess_type(str(filepath.absolute()))
-        file_mimetype = guess_mimetype[0] if guess_mimetype else "*/*"
-        media = MediaFileUpload(
-            filepath.absolute(), mimetype=file_mimetype, resumable=True
-        )
-        file_metadata = {
-            "name": filepath.name,
-            "parents": [folder_id],
-            "mimeType": file_mimetype,
-        }
-        self.logger.debug("Upload file_metadata: '%s'" % file_metadata)
-        if len(target_file) == 1 and overwrite:
-            self.logger.info("Overwriting file '%s' with new content", filename)
-            return self._file_update(target_file, media)
-        elif len(target_file) == 1 and not overwrite:
-            self.logger.warn("Not uploading new copy of file '%s'", filepath.name)
-            return target_file[0]["id"]
-        elif len(target_file) > 1:
-            self.logger.warn(
-                "Drive already contains '%s' copies of file '%s'. Not uploading again."
-                % (len(target_file), filepath.name)
-            )
-            return None
-        else:
-            return self._file_create(file_metadata, media)
-
-    def _file_create(self, file_metadata, media):
-        try:
-            result = (
-                self.service.files()
-                .create(
-                    body=file_metadata,
-                    media_body=media,
-                    fields="id",
-                )
-                .execute()
-            )
-            return result.get("id", None)
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-
-    def _file_update(self, target_file, media):
-        try:
-            result = (
-                self.service.files()
-                .update(fileId=target_file[0]["id"], media_body=media, fields="id")
-                .execute()
-            )
-            return result.get("id", None)
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-
-    def _download_with_fileobject(self, file_object):
-        try:
-            request = self.service.files().get_media(fileId=file_object["id"])
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-        fh = BytesIO()
-        downloader = MediaIoBaseDownload(fh, request)
-        done = False
-        while done is False:
-            _, done = downloader.next_chunk()
-        fh.seek(0)
-        with open(file_object["name"], "wb") as f:
-            # pylint: disable=protected-access
-            shutil.copyfileobj(fh, f, length=downloader._total_size)
-
-    @keyword(tags=["drive"])
-    def download_drive_files(
-        self,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        limit: int = None,
-        timeout: float = None,
-    ) -> List:
-        """Download files specified by file dictionary or query string
-
-        Parameters `start`, `limit` and `timeout` are used only when
-        downloading files defined by `query` parameter.
-
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target files, defaults to None
-        :param source: source directory where query is executed
-        :param limit: maximum amount of files that are downloaded, defaults to None
-        :param timeout: maximum allowed time in seconds for download process
-        :return: list of downloaded files
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${files}=    Search Drive Files    query=name contains '.json'
-            FOR    ${f}    IN    @{files}
-                IF  ${f}[size] < 2000
-                    Download Drive Files  file_dict=${f}
-                END
-            END
-
-            ${folder_id}=   Get Drive Folder Id   datafolder
-            Download Drive Files  query=name contains '.json' and '${folder_id}' in parents
-        """  # noqa: E501
-        if query:
-            filelist = self.search_drive_files(query, source=source)
-            files_downloaded = []
-            start_time = time.time()
-
-            for f in filelist:
-                self._download_with_fileobject(f)
-                current_time = time.time()
-                files_downloaded.append(f["name"])
-                if limit and len(files_downloaded) >= limit:
-                    self.logger.info(
-                        "Drive download limit %s reached. Stopping the download.", limit
-                    )
-                    break
-                if timeout and (current_time - start_time) > float(timeout):
-                    self.logger.info(
-                        "Drive download timeout %s seconds reached. "
-                        "Stopping the download.",
-                        timeout,
-                    )
-                    break
-            return files_downloaded
-
-        if file_dict:
-            self._download_with_fileobject(file_dict)
-            return [file_dict]
-        return []
-
-    @keyword(tags=["drive"])
-    def update_drive_file(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        action: UpdateAction = UpdateAction.star,
-        multiple_ok: bool = False,
-    ) -> int:
-        """Update file specified by id, file dictionary or query string
-
-        Possible actions:
-        - star
-        - unstar
-        - trash
-        - untrash
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Drive Search Files`
-        :param query: drive query string to find target file, needs to match 1 file
-        :param source: source directory where query is executed
-        :param action: update action, default star file
-        :param multiple_ok: set to `True` if it is ok to perform update
-         on more than 1 file
-        :return: number of updated files
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${folder_id}=  Get Drive Folder Id   datafolder
-            ${updated}=    Update Drive File  query=name contains '.json' and '${folder_id}' in parents
-            ...            action=star
-            ...            multiple_ok=True
-        """  # noqa: E501
-        target_files = self._get_target_file(
-            file_id, file_dict, query, multiple_ok, source
-        )
-        update_count = 0
-        for tf in target_files:
-            self._drive_files_update(tf, action)
-            update_count += 1
-        return update_count
-
-    def _get_target_file(
-        self, file_id, file_dict, query, multiple_ok, source=None, details=False
-    ):
-        target_files = []
-        if file_id:
-            if details:
-                filedata = self.get_drive_file_by_id(file_id)
-                target_files.append(filedata)
-            else:
-                target_files.append(file_id)
-        elif file_dict:
-            target_files.append(file_dict.get("id", None))
-        else:
-            files = self.search_drive_files(query, source=source, recurse=True)
-            target_files = [tf if details else tf.get("id", None) for tf in files]
-            if not multiple_ok and len(target_files) > 1:
-                raise GoogleDriveError(
-                    "expected search to match 1 file, but it matched %s files"
-                    % len(files)
-                )
-
-        return target_files
-
-    def _drive_files_update(self, file_id: str, action: UpdateAction):
-        body = None
-        if action == UpdateAction.trash:
-            body = {"trashed": True}
-        elif action == UpdateAction.untrash:
-            body = {"trashed": False}
-        elif action == UpdateAction.star:
-            body = {"starred": True}
-        elif action == UpdateAction.unstar:
-            body = {"starred": False}
-        else:
-            # TODO: mypy should handle enum exhaustivity validation
-            raise ValueError(f"Unsupported update action: {action}")
-        self.logger.debug(body)
-        try:
-            updated_file = (
-                self.service.files().update(fileId=file_id, body=body).execute()
-            )
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-        return updated_file
-
-    @keyword(tags=["drive"])
-    def delete_drive_file(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        multiple_ok: bool = False,
-        suppress_errors: bool = False,
-    ) -> int:
-        """Delete file specified by id, file dictionary or query string
-
-        Note. Be extra careful when calling this keyword!
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target file, needs to match 1 file
-         unless parameter `multiple_ok` is set to `True`
-        :param multiple_ok: set to `True` if it is ok to perform delete
-         on more than 1 file
-        :param suppress_errors: on True will log warning message instead of
-         raising an exception, defaults to False
-        :return: how many files where deleted
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${folder_id}=  Get Drive Folder Id   datafolder
-            ${deleted}=    Delete Drive File  query=name contains '.json' and '${folder_id}' in parents
-            ...            multiple_ok=True
-        """  # noqa: E501
-        target_files = self._get_target_file(file_id, file_dict, query, multiple_ok)
-
-        delete_count = 0
-        for tf in target_files:
-            try:
-                self.service.files().delete(fileId=tf).execute()
-            except HttpError as err:
-                if suppress_errors:
-                    self.logger.warn(str(err))
-                else:
-                    raise GoogleDriveError(str(err)) from err
-            delete_count += 1
-        return delete_count
-
-    @keyword(tags=["drive"])
-    def get_drive_folder_id(
-        self, folder: str = None, parent_folder: str = None, details: bool = False
-    ) -> str:
-        """Get file id for the folder
-
-        :param folder: name of the folder to identify, by default returns drive's
-         `root` folder id
-        :param parent_folder: can be used to narrow search by giving parent
-         folder name
-        :param details: on True will return folder dictionary, on False (default)
-         folder id is returned
-        :return: file id of the folder or file dictionary when details = True
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${root_id}=    Get Drive Folder Id   # returns Drive root folder id
-            ${folder_id}=  Get Drive Folder Id  subdir
-        """
-        mime_folder_type = "application/vnd.google-apps.folder"
-        drive_file = None
-        if folder is None:
-            try:
-                drive_file = (
-                    self.service.files().get(fileId="root", fields="id").execute()
-                )
-            except HttpError as err:
-                raise GoogleDriveError(str(err)) from err
-        else:
-            query_string = f"name = '{folder}' AND mimeType = '{mime_folder_type}'"
-            parameters = {"query": query_string, "recurse": True}
-            if parent_folder:
-                parameters["source"] = parent_folder
-            folders = self.search_drive_files(**parameters)
-            if len(folders) == 1:
-                drive_file = folders[0]  # .get("id", None)
-            else:
-                self.logger.info(
-                    "Found %s directories with name '%s'" % (len(folders), folder)
-                )
-        if drive_file:
-            return drive_file if details else drive_file.get("id", None)
-        return None
-
-    @keyword(tags=["drive"])
-    def move_drive_file(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        target: str = None,
-        multiple_ok: bool = False,
-    ) -> List:
-        """Move file specified by id, file dictionary or query string into target folder
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target file, needs to match 1 file
-        :param source: name of the folder to move file from, is by default drive's
-         `root` folder id
-        :param target: name of the folder to move file into, is by default drive's
-         `root` folder id
-        :param multiple_ok: if `True` then moving more than 1 file
-        :return: list of file ids
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${source_id}=  Get Drive Folder Id  sourcefolder
-            ${query}=      Set Variable  name contains '.json' and '${sourceid}' in parents
-            ${files}=      Move Drive File  query=${query}  folder=target_folder  multiple_ok=True
-        """  # noqa: E501
-        result_files = []
-        if file_id or file_dict:
-            target_files = self._get_target_file(file_id, file_dict, query, multiple_ok)
-        else:
-            target_files = self.search_drive_files(query, source=source)
-        target_parent = None
-        if len(target_files) == 0:
-            raise GoogleDriveError("Did not find any files to move")
-        if target:
-            target_parent = self.get_drive_folder_id(target)
-        if target_parent is None:
-            raise GoogleDriveError(
-                "Unable to find target folder: '%s'" % (target if target else "root")
-            )
-        for tf in target_files:
-            file = self.service.files().get(fileId=tf["id"], fields="parents").execute()
-            previous_parents = ",".join(file.get("parents"))
-            try:
-                result_file = (
-                    self.service.files()
-                    .update(
-                        fileId=tf["id"],
-                        addParents=target_parent,
-                        removeParents=previous_parents,
-                        fields="id, parents",
-                    )
-                    .execute()
-                )
-            except HttpError as err:
-                raise GoogleDriveError(str(err)) from err
-            result_files.append(result_file)
-        return result_files
-
-    @keyword(tags=["drive", "drive share", "v2.0.0"])
-    def list_shared_drive_files(self, query: str = None, source: str = None) -> List:
-        """Keyword for listing shared files in the source folder.
-
-        Alias keyword for ``Search Drive Files`` which can be used to list
-        only files which have been shared.
-
-        :param query: drive query string to find target files
-        :param source: source directory where query is executed
-        :return: list of shared files
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${shared}=    List Shared Drive Files    source=subfolder
-            FOR    ${file}    IN    @{shared}
-                Log To Console    ${file}
-            END
-        """
-        files = self.search_drive_files(query=query, source=source)
-        return [f for f in files if f["shared"]]
-
-    @keyword(tags=["drive"])
-    def search_drive_files(
-        self, query: str = None, recurse: bool = False, source: str = None
-    ) -> List:
-        """Search Google Drive for files matching query string
-
-        :param query: search string, defaults to None which means that all files
-         and folders are returned
-        :param recurse: set to `True` if search should recursive
-        :param source: source directory where query is executed
-        :return: list of files
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${files}=  Search Drive Files   query=name contains 'hello'
-            ${files}=  Search Drive Files   query=modifiedTime > '2020-06-04T12:00:00'
-            ${files}=  Search Drive Files   query=mimeType contains 'image/' or mimeType contains 'video/'
-            ${files}=  Search Drive Files   query=name contains '.yaml'  recurse=True
-            ${files}=  Search Drive Files   query=name contains '.yaml'  source=datadirectory
-        """  # noqa: E501
-        page_token = None
-        filelist = []
-
-        parameters = self._set_search_parameters(query, source, recurse)
-
-        while True:
-            if page_token:
-                parameters["pageToken"] = page_token
-            try:
-                self.logger.debug("Searching with parameters: '%s'" % parameters)
-                response = self.service.files().list(**parameters).execute()
-                for file_details in response.get("files", []):
-                    file_dict = self._drive_file_details_into_file_dict(file_details)
-                    filelist.append(file_dict)
-                page_token = response.get("nextPageToken", None)
-                if page_token is None:
-                    break
-            except HttpError as err:
-                raise GoogleDriveError(str(err)) from err
-        return filelist
-
-    def _set_search_parameters(self, query, source, recurse):
-        parameters = {
-            "fields": "*",
-        }
-        if query:
-            parameters["q"] = query
-
-        folder_id = None
-        if source:
-            folder_id = self.get_drive_folder_id(source)
-        elif not recurse:
-            folder_id = "root"
-
-        if folder_id:
-            if "q" in parameters:
-                parameters["q"] += f" and '{folder_id}' in parents"
-            else:
-                parameters["q"] = f"'{folder_id}' in parents"
-        return parameters
-
-    def _drive_file_details_into_file_dict(self, details):
-        filesize = details.get("size")
-        file_id = details.get("id")
-        parents = details.get("parents")
-        kind = details.get("kind")
-        mimetype = details.get("mimeType")
-        is_folder = mimetype == "application/vnd.google-apps.folder"
-        folder_id = (
-            file_id
-            if mimetype == "application/vnd.google-apps.folder"
-            else parents[0]
-            if parents and len(parents) > 0
-            else None
-        )
-        file_link = (
-            None
-            if mimetype == "application/vnd.google-apps.folder"
-            else f"https://drive.google.com/file/d/{file_id}?usp=sharing"
-        )
-        folder_link = (
-            f"https://drive.google.com/drive/folders/{folder_id}?usp=sharing"
-            if folder_id
-            else ""
-        )
-        file_dict = {
-            "name": details.get("name"),
-            "id": file_id,
-            "size": int(filesize) if filesize else None,
-            "kind": kind,
-            "is_folder": is_folder,
-            "parents": parents,
-            "starred": details.get("starred"),
-            "trashed": details.get("trashed"),
-            "shared": details.get("shared"),
-            "permissions": details.get("permissions", []),
-            "mimeType": mimetype,
-            "spaces": details.get("spaces", None),
-            "exportLinks": details.get("exportLinks"),
-            "createdTime": details.get("createdTime"),
-            "modifiedTime": details.get("modifiedTime"),
-            "fileLink": file_link,
-            "folderLink": folder_link,
-        }
-        return file_dict
-
-    @keyword(tags=["drive"])
-    def create_drive_directory(
-        self, folder: str = None, parent_folder: str = None
-    ) -> Dict:
-        """Create new directory to Google Drive
-
-        :param folder: name for the new directory
-        :param parent_folder: top level directory for new directory
-        :return: dictionary containing folder ID and folder URL
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${folder}=  Create Drive Directory   example-folder
-            Log To Console    Google Drive folder ID: ${folder}[id]
-            Log To Console    Google Drive folder URL:  ${folder}[url]
-        """
-        if not folder or len(folder) == 0:
-            raise GoogleDriveError("Can't create Drive directory with empty name")
-
-        folder_id = self.get_drive_folder_id(folder, parent_folder=parent_folder)
-        if folder_id:
-            self.logger.info(
-                "Folder '%s' already exists. Not creating new one.", folder_id
-            )
-            return self._folder_response(folder_id)
-
-        file_metadata = {
-            "name": folder,
-            "mimeType": "application/vnd.google-apps.folder",
-        }
-
-        if parent_folder:
-            parent_folder_id = self.get_drive_folder_id(parent_folder)
-            file_metadata["parents"] = [parent_folder_id]
-        try:
-            added_folder = (
-                self.service.files().create(body=file_metadata, fields="id").execute()
-            )
-            return self._folder_response(added_folder["id"])
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-
-    def _folder_response(self, folder_id):
-        return {
-            "id": folder_id,
-            "url": f"https://drive.google.com/drive/folders/{folder_id}?usp=sharing",
-        }
-
-    @keyword(tags=["drive"])
-    def export_drive_file(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        target_file: str = None,
-        mimetype: str = "application/pdf",
-    ) -> str:
-        """Export Google Drive file using Drive export links
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param target_file: name for the exported file
-        :param mimetype: export mimetype, defaults to "application/pdf"
-        :return: file path to the exported file
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${files}=  Drive Search Files  query=name contains 'my example worksheet'
-            Export Drive File  file_dict=${files}[0]
-        """
-        if target_file is None or len(target_file) == 0:
-            raise AttributeError("The target_file is required parameter for export")
-        if file_id is None and file_dict is None:
-            raise AttributeError("Either file_id or file_dict is required for export")
-        target_files = self._get_target_file(file_id, file_dict, None, False)
-        if len(target_files) != 1:
-            raise ValueError("Did not find the Google Drive file to export")
-        try:
-            request = self.service.files().export(
-                fileId=target_files[0], mimeType=mimetype
-            )
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-
-        fh = BytesIO()
-        downloader = MediaIoBaseDownload(fh, request)
-        done = False
-        while done is False:
-            _, done = downloader.next_chunk()
-
-        fh.seek(0)
-        filepath = Path(target_file).absolute()
-        with open(filepath, "wb") as f:
-            shutil.copyfileobj(fh, f, length=131072)
-        return filepath
-
-    @keyword(tags=["drive", "drive share", "v2.0.0"])
-    def add_drive_share(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        email: str = None,
-        domain: str = None,
-        role: DriveRole = DriveRole.READER,
-        share_type: DriveType = DriveType.USER,
-        notification: bool = False,
-        notification_message: str = None,
-    ) -> Dict:
-        """Keyword for sharing drive file or folder.
-
-        Parameters `file_id`, `file_dict`, `query` and `source` can be
-        used to select files to which sharing is added to.
-
-        If share is added to a folder, all files within that folder get same
-        sharing permissions.
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target file, needs to match 1 file
-        :param source: name of the folder to search files in, is by default drive's
-         `root` folder
-        :param email: user or group email address if share type
-         is DriveType.USER or DriveType.GROUP
-        :param domain: domain name if share type is DriveType.DOMAIN
-        :param role: see ``DriveRole`` enum for possible values,
-         defaults to DriveRole.READER
-        :param share_type: see ``DriveType`` enum for possible values,
-         defaults to DriveType.USER
-        :param notification: whether to send notificatin email, defaults to False
-        :param notification_message: optional message to include with the notification
-        :return: share response dictionary containing 'file_id' and 'permission_id'
-
-        Example:
-
-        .. code-block:: robotframework
-
-            # Add file share for a email address with email notification
-            Add Drive Share
-            ...    query=name = 'okta.png'
-            ...    email=robocorp.tester@gmail.com
-            ...    notification=True
-            ...    notification_message=Hello. I have shared 'okta.png' with you for review.
-            # Add file share for a domain
-            Add Drive Share
-            ...    query=name = 'okta.png'
-            ...    domain=robocorp.com
-            # Add folder share for a email address
-            ${folder}=    Create Drive Directory   attachments-for-the-task
-            ${share}=  Add Drive Share
-            ...   file_id=${folder}[id]
-            ...   email=robocorp.tester@gmail.com
-            ...   role=writer
-            Log To Console  Share details: ${share}[file_id], ${share}[permission_id]
-        """  # noqa: E501
-        target_file = self._get_target_file(
-            file_id, file_dict, query, False, source=source
-        )
-        if not target_file:
-            raise GoogleDriveError("Did not find target file")
-        if domain:
-            share_type = DriveType.DOMAIN
-        user_permission = {
-            "type": to_drive_type(share_type),
-            "role": to_drive_role(role),
-        }
-        if share_type in [DriveType.USER, DriveType.GROUP]:
-            if not email:
-                raise ValueError(
-                    "email parameter is required with share_type = 'user' or 'group'"
-                )
-            user_permission["emailAddress"] = email
-        if share_type == DriveType.DOMAIN:
-            if not domain:
-                raise ValueError(
-                    "domain parameter is required with share_type = 'domain'"
-                )
-            user_permission["domain"] = domain
-
-        request_parameters = {
-            "fileId": target_file[0],
-            "body": user_permission,
-            "fields": "id",
-            "sendNotificationEmail": notification,
-        }
-        if notification and notification_message:
-            request_parameters["emailMessage"] = notification_message
-
-        try:
-            response = self.service.permissions().create(**request_parameters).execute()
-            return {"file_id": target_file[0], "permission_id": response["id"]}
-        except HttpError as err:
-            raise GoogleDriveError(str(err)) from err
-
-    @keyword(tags=["drive", "drive share", "v2.0.0"])
-    def remove_drive_share_by_permission_id(
-        self,
-        permission_id: str,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        suppress_errors: bool = False,
-    ) -> Dict:
-        """Keyword for removing share permission of file or folder
-        permission id.
-
-        Parameters `file_id`, `file_dict`, `query` and `source` can be
-        used to select files from which sharing is removed.
-
-        :param permission_id: id of the permission to remove
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target file, needs to match 1 file
-        :param source: name of the folder to search files in, is by default drive's
-         `root` folder
-        :param suppress_errors: on True will log warning message instead of
-         raising an exception, defaults to False (exception is raised)
-        :return: dictionary of permission response
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${share}=   Add Drive Share
-            ...  query=name = 'sharable-files' and mimeType = 'application/vnd.google-apps.folder'
-            ...  email=robocorp.tester@gmail.com
-            #
-            # actions on shared files in the folder 'shareable-files' ....
-            #
-            Remove Drive Share By Permission Id   ${share}[permission_id]  ${share}[file_id]
-        """  # noqa: E501
-        target_file = self._get_target_file(
-            file_id, file_dict, query, False, source=source
-        )
-        if not target_file:
-            raise GoogleDriveError("Did not find target file")
-
-        self.logger.info(
-            "Removing permission id '%s' for file_id '%s'"
-            % (permission_id, target_file[0])
-        )
-        response = None
-        try:
-            response = (
-                self.service.permissions()
-                .delete(fileId=target_file[0], permissionId=permission_id)
-                .execute()
-            )
-        except HttpError as err:
-            if suppress_errors:
-                self.logger.warn(str(err))
-            else:
-                raise GoogleDriveError(str(err)) from err
-        return response
-
-    @keyword(tags=["drive", "drive share", "v2.0.0"])
-    def remove_drive_share_by_criteria(
-        self,
-        email: str = None,
-        domain: str = None,
-        permission_id: str = None,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        source: str = None,
-        suppress_errors: bool = False,
-    ) -> List:
-        """Keyword for removing share from file or folder
-        based on criteria.
-
-        Parameters `file_id`, `file_dict`, `query` and `source` can be
-        used to select files from which sharing is removed.
-
-        Parameters `email`, `domain` or `permission_id` can be
-        used to select which share is removed from selected files.
-
-        :param email: email address of the permission to remove
-        :param domain: domain name of the permission to remove
-        :param permission_id: id of the permission to remove
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target files
-        :param source: name of the folder to search files in, is by default drive's
-         `root` folder
-        :param suppress_errors: on True will log warning message instead of
-         raising an exception, defaults to False (exception is raised)
-        :return: list of dictionaries containing information of file permissions removed
-
-        Example:
-
-        .. code-block:: robotframework
-
-            # Remove domain shares for files in the folder ${FOLDER_NAME}
-            ${removed}=    Remove Drive Share By Criteria
-            ...    domain=robocorp.com
-            ...    source=${FOLDER_NAME}
-            # Remove email share for a file
-            ${removed}=    Remove Drive Share By Criteria
-            ...    query=name = 'okta.png'
-            ...    email=robocorp.tester@gmail.com
-        """
-        if not email and not domain and permission_id:
-            raise AttributeError(
-                "At least one of the 'email', 'domain' or 'permission_id' "
-                "is required to remove drive share"
-            )
-        target_files = self._get_target_file(
-            file_id, file_dict, query, multiple_ok=True, source=source, details=True
-        )
-        if not target_files or len(target_files) == 0:
-            raise GoogleDriveError("Did not find target files")
-        permissions_removed = []
-        for tf in target_files:
-            file_permissions_removed = []
-            if "permissions" in tf and tf["permissions"]:
-                self.logger.info(
-                    "Removing shares from file '%s' id '%s'" % (tf["name"], tf["id"])
-                )
-                for p in tf["permissions"]:
-                    if self._is_permission_removable(p, email, domain, permission_id):
-                        self._remove_file_permission(
-                            tf, p, file_permissions_removed, suppress_errors
-                        )
-            if file_permissions_removed:
-                permissions_removed.append(
-                    {
-                        "file_id": tf["id"],
-                        "file_name": tf["name"],
-                        "permissions_removed": file_permissions_removed,
-                    }
-                )
-        return permissions_removed
-
-    def _is_permission_removable(self, permission, email, domain, permission_id):
-        return (
-            (
-                email
-                and "emailAddress" in permission.keys()
-                and permission["emailAddress"] == email
-            )
-            or (
-                domain
-                and "domain" in permission.keys()
-                and permission["domain"] == domain
-            )
-            or (permission_id and permission["id"] == permission_id)
-        )
-
-    def _remove_file_permission(
-        self, drive_file, permission, permissions_removed, suppress_errors
-    ):
-        try:
-            self.service.permissions().delete(
-                fileId=drive_file["id"], permissionId=permission["id"]
-            ).execute()
-            permissions_removed.append(permission)
-        except HttpError as err:
-            if suppress_errors:
-                self.logger.warn(str(err))
-            else:
-                raise GoogleDriveError(str(err)) from err
-
-    @keyword(tags=["drive", "drive share", "v2.0.0"])
-    def remove_all_drive_shares(
-        self,
-        file_id: str = None,
-        file_dict: dict = None,
-        query: str = None,
-        suppress_errors: bool = False,
-    ) -> List:
-        """Keyword for removing all shares from selected files (only owner
-        permission is retained).
-
-        :param file_id: drive file id
-        :param file_dict: file dictionary returned by `Search Drive Files`
-        :param query: drive query string to find target files
-        :param suppress_errors: on True will log warning message instead of
-         raising an exception, defaults to False (exception is raised)
-        :return: list of dictionaries containing information of file permissions removed
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${removed}=  Remove All Drive Shares    file_id=${FOLDER_ID}
-        """
-        target_files = self._get_target_file(
-            file_id, file_dict, query, multiple_ok=True, details=True
-        )
-        permissions_removed = []
-        for tf in target_files:
-            if "permissions" in tf and tf["permissions"]:
-                self.logger.info(
-                    "Removing shares from file '%s' id '%s'" % (tf["name"], tf["id"])
-                )
-                for p in tf["permissions"]:
-                    if p["role"] != "owner":
-                        self.remove_drive_share_by_permission_id(
-                            file_id=tf["id"],
-                            permission_id=p["id"],
-                            suppress_errors=suppress_errors,
-                        )
-                        permissions_removed.append(p)
-        return permissions_removed
-
-    @keyword(tags=["drive", "v2.0.0"])
-    def get_drive_file_by_id(self, file_id: str, suppress_errors: bool = False) -> Dict:
-        """Get file dictionary by its file id.
-
-        :param file_id: id of the file in the Google Drive
-        :param suppress_errors: on True will log warning message instead of
-         raising an exception, defaults to False (exception is raised)
-        :return: dictionary containing file information
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${file_dict}=  Get Drive File By ID    file_id=${FILE_ID}
-        """
-        response = None
-        try:
-            raw_response = (
-                self.service.files().get(fileId=file_id, fields="*").execute()
-            )
-            response = self._drive_file_details_into_file_dict(raw_response)
-        except HttpError as err:
-            if suppress_errors:
-                self.logger.warn(str(err))
-            else:
-                raise GoogleDriveError(str(err)) from err
-        return response
+from io import BytesIO
+import mimetypes
+from pathlib import Path
+import shutil
+import time
+from typing import Dict, List, Optional
+
+from apiclient.errors import HttpError
+from apiclient.http import MediaFileUpload, MediaIoBaseDownload
+
+from . import LibraryContext, keyword, UpdateAction
+from .enums import DriveRole, DriveType, to_drive_role, to_drive_type
+
+
+class GoogleDriveError(Exception):
+    """Raised with errors in Drive API"""
+
+
+class DriveKeywords(LibraryContext):
+    """Class for Google Drive API
+
+    For more information about Google Drive API link_.
+
+    .. _link: https://developers.google.com/drive/api
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "drive"])
+    def init_drive(
+        self,
+        service_account: str = None,
+        credentials: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        scopes: list = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Drive client
+
+        :param service_account: file path to service account file
+        :param credentials: file path to credentials file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param scopes: list of extra authentication scopes
+        :param token_file: file path to token file
+        """
+        drive_scopes = [
+            "drive",
+            "drive.appdata",
+            "drive.file",
+            "drive.install",
+            "drive.metadata",
+        ]
+        if scopes:
+            drive_scopes += scopes
+        self.service = self.init_service(
+            service_name="drive",
+            api_version="v3",
+            scopes=drive_scopes,
+            service_account_file=service_account,
+            credentials_file=credentials,
+            use_robocorp_vault=use_robocorp_vault,
+            token_file=token_file,
+        )
+
+    @keyword(tags=["drive"])
+    def upload_drive_file(
+        self,
+        filename: str = None,
+        folder: str = None,
+        overwrite: bool = False,
+        make_dir: bool = False,
+    ) -> str:
+        """Upload files into Drive
+
+        :param filename: name of the file to upload
+        :param folder: target folder for upload
+        :param overwrite: set to `True` if already existing file should be overwritten
+        :param make_dir: set to `True` if folder should be created if it does not exist
+        :return: uploaded file id
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${file1_id}=  Upload Drive File  data.json  # Upload file to drive root
+            ${file2_id}=  Upload Drive File  newdata.json  new_folder  make_dir=True
+            ${file3_id}=  Upload Drive File  data.json  overwrite=True
+        """
+        folder_id = self.get_drive_folder_id(folder)
+        if folder_id is None and make_dir:
+            folder = self.create_drive_directory(folder)
+            folder_id = folder["id"]
+        if folder_id is None:
+            raise GoogleDriveError(
+                "Target folder '%s' does not exist or could not be created" % folder
+            )
+
+        filepath = Path(filename)
+        if filepath.is_dir():
+            raise GoogleDriveError(
+                "The '%s' is a directory and can not be uploaded" % filename
+            )
+        elif not filepath.is_file():
+            raise GoogleDriveError("Filename '%s' does not exist" % filename)
+
+        query_string = f"name = '{filepath.name}' and '{folder_id}' in parents"
+        self.logger.debug("Upload query_string: '%s'" % query_string)
+        target_file = self.search_drive_files(query=query_string, recurse=True)
+        guess_mimetype = mimetypes.guess_type(str(filepath.absolute()))
+        file_mimetype = guess_mimetype[0] if guess_mimetype else "*/*"
+        media = MediaFileUpload(
+            filepath.absolute(), mimetype=file_mimetype, resumable=True
+        )
+        file_metadata = {
+            "name": filepath.name,
+            "parents": [folder_id],
+            "mimeType": file_mimetype,
+        }
+        self.logger.debug("Upload file_metadata: '%s'" % file_metadata)
+        if len(target_file) == 1 and overwrite:
+            self.logger.info("Overwriting file '%s' with new content", filename)
+            return self._file_update(target_file, media)
+        elif len(target_file) == 1 and not overwrite:
+            self.logger.warn("Not uploading new copy of file '%s'", filepath.name)
+            return target_file[0]["id"]
+        elif len(target_file) > 1:
+            self.logger.warn(
+                "Drive already contains '%s' copies of file '%s'. Not uploading again."
+                % (len(target_file), filepath.name)
+            )
+            return None
+        else:
+            return self._file_create(file_metadata, media)
+
+    def _file_create(self, file_metadata, media):
+        try:
+            result = (
+                self.service.files()
+                .create(
+                    body=file_metadata,
+                    media_body=media,
+                    fields="id",
+                )
+                .execute()
+            )
+            return result.get("id", None)
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+
+    def _file_update(self, target_file, media):
+        try:
+            result = (
+                self.service.files()
+                .update(fileId=target_file[0]["id"], media_body=media, fields="id")
+                .execute()
+            )
+            return result.get("id", None)
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+
+    def _download_with_fileobject(self, file_object):
+        try:
+            request = self.service.files().get_media(fileId=file_object["id"])
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+        fh = BytesIO()
+        downloader = MediaIoBaseDownload(fh, request)
+        done = False
+        while done is False:
+            _, done = downloader.next_chunk()
+        fh.seek(0)
+        with open(file_object["name"], "wb") as f:
+            # pylint: disable=protected-access
+            shutil.copyfileobj(fh, f, length=downloader._total_size)
+
+    @keyword(tags=["drive"])
+    def download_drive_files(
+        self,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        limit: int = None,
+        timeout: float = None,
+    ) -> List:
+        """Download files specified by file dictionary or query string
+
+        Parameters `start`, `limit` and `timeout` are used only when
+        downloading files defined by `query` parameter.
+
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target files, defaults to None
+        :param source: source directory where query is executed
+        :param limit: maximum amount of files that are downloaded, defaults to None
+        :param timeout: maximum allowed time in seconds for download process
+        :return: list of downloaded files
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${files}=    Search Drive Files    query=name contains '.json'
+            FOR    ${f}    IN    @{files}
+                IF  ${f}[size] < 2000
+                    Download Drive Files  file_dict=${f}
+                END
+            END
+
+            ${folder_id}=   Get Drive Folder Id   datafolder
+            Download Drive Files  query=name contains '.json' and '${folder_id}' in parents
+        """  # noqa: E501
+        if query:
+            filelist = self.search_drive_files(query, source=source)
+            files_downloaded = []
+            start_time = time.time()
+
+            for f in filelist:
+                self._download_with_fileobject(f)
+                current_time = time.time()
+                files_downloaded.append(f["name"])
+                if limit and len(files_downloaded) >= limit:
+                    self.logger.info(
+                        "Drive download limit %s reached. Stopping the download.", limit
+                    )
+                    break
+                if timeout and (current_time - start_time) > float(timeout):
+                    self.logger.info(
+                        "Drive download timeout %s seconds reached. "
+                        "Stopping the download.",
+                        timeout,
+                    )
+                    break
+            return files_downloaded
+
+        if file_dict:
+            self._download_with_fileobject(file_dict)
+            return [file_dict]
+        return []
+
+    @keyword(tags=["drive"])
+    def update_drive_file(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        action: UpdateAction = UpdateAction.star,
+        multiple_ok: bool = False,
+    ) -> int:
+        """Update file specified by id, file dictionary or query string
+
+        Possible actions:
+        - star
+        - unstar
+        - trash
+        - untrash
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Drive Search Files`
+        :param query: drive query string to find target file, needs to match 1 file
+        :param source: source directory where query is executed
+        :param action: update action, default star file
+        :param multiple_ok: set to `True` if it is ok to perform update
+         on more than 1 file
+        :return: number of updated files
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${folder_id}=  Get Drive Folder Id   datafolder
+            ${updated}=    Update Drive File  query=name contains '.json' and '${folder_id}' in parents
+            ...            action=star
+            ...            multiple_ok=True
+        """  # noqa: E501
+        target_files = self._get_target_file(
+            file_id, file_dict, query, multiple_ok, source
+        )
+        update_count = 0
+        for tf in target_files:
+            self._drive_files_update(tf, action)
+            update_count += 1
+        return update_count
+
+    def _get_target_file(
+        self, file_id, file_dict, query, multiple_ok, source=None, details=False
+    ):
+        target_files = []
+        if file_id:
+            if details:
+                filedata = self.get_drive_file_by_id(file_id)
+                target_files.append(filedata)
+            else:
+                target_files.append(file_id)
+        elif file_dict:
+            if details:
+                target_files.append(file_dict)
+            else:
+                target_files.append(file_dict.get("id", None))
+        else:
+            files = self.search_drive_files(query, source=source, recurse=True)
+            target_files = [tf if details else tf.get("id", None) for tf in files]
+            if not multiple_ok and len(target_files) > 1:
+                raise GoogleDriveError(
+                    "expected search to match 1 file, but it matched %s files"
+                    % len(files)
+                )
+
+        return target_files
+
+    def _drive_files_update(self, file_id: str, action: UpdateAction):
+        body = None
+        if action == UpdateAction.trash:
+            body = {"trashed": True}
+        elif action == UpdateAction.untrash:
+            body = {"trashed": False}
+        elif action == UpdateAction.star:
+            body = {"starred": True}
+        elif action == UpdateAction.unstar:
+            body = {"starred": False}
+        else:
+            # TODO: mypy should handle enum exhaustivity validation
+            raise ValueError(f"Unsupported update action: {action}")
+        self.logger.debug(body)
+        try:
+            updated_file = (
+                self.service.files().update(fileId=file_id, body=body).execute()
+            )
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+        return updated_file
+
+    @keyword(tags=["drive"])
+    def delete_drive_file(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        multiple_ok: bool = False,
+        suppress_errors: bool = False,
+    ) -> int:
+        """Delete file specified by id, file dictionary or query string
+
+        Note. Be extra careful when calling this keyword!
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target file, needs to match 1 file
+         unless parameter `multiple_ok` is set to `True`
+        :param multiple_ok: set to `True` if it is ok to perform delete
+         on more than 1 file
+        :param suppress_errors: on True will log warning message instead of
+         raising an exception, defaults to False
+        :return: how many files where deleted
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${folder_id}=  Get Drive Folder Id   datafolder
+            ${deleted}=    Delete Drive File  query=name contains '.json' and '${folder_id}' in parents
+            ...            multiple_ok=True
+        """  # noqa: E501
+        target_files = self._get_target_file(file_id, file_dict, query, multiple_ok)
+
+        delete_count = 0
+        for tf in target_files:
+            try:
+                self.service.files().delete(fileId=tf).execute()
+            except HttpError as err:
+                if suppress_errors:
+                    self.logger.warn(str(err))
+                else:
+                    raise GoogleDriveError(str(err)) from err
+            delete_count += 1
+        return delete_count
+
+    @keyword(tags=["drive"])
+    def get_drive_folder_id(
+        self, folder: str = None, parent_folder: str = None, details: bool = False
+    ) -> str:
+        """Get file id for the folder
+
+        :param folder: name of the folder to identify, by default returns drive's
+         `root` folder id
+        :param parent_folder: can be used to narrow search by giving parent
+         folder name
+        :param details: on True will return folder dictionary, on False (default)
+         folder id is returned
+        :return: file id of the folder or file dictionary when details = True
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${root_id}=    Get Drive Folder Id   # returns Drive root folder id
+            ${folder_id}=  Get Drive Folder Id  subdir
+        """
+        mime_folder_type = "application/vnd.google-apps.folder"
+        drive_file = None
+        if folder is None:
+            try:
+                drive_file = (
+                    self.service.files().get(fileId="root", fields="id").execute()
+                )
+            except HttpError as err:
+                raise GoogleDriveError(str(err)) from err
+        else:
+            query_string = f"name = '{folder}' AND mimeType = '{mime_folder_type}'"
+            parameters = {"query": query_string, "recurse": True}
+            if parent_folder:
+                parameters["source"] = parent_folder
+            folders = self.search_drive_files(**parameters)
+            if len(folders) == 1:
+                drive_file = folders[0]  # .get("id", None)
+            else:
+                self.logger.info(
+                    "Found %s directories with name '%s'" % (len(folders), folder)
+                )
+        if drive_file:
+            return drive_file if details else drive_file.get("id", None)
+        return None
+
+    @keyword(tags=["drive"])
+    def move_drive_file(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        target: str = None,
+        multiple_ok: bool = False,
+    ) -> List:
+        """Move file specified by id, file dictionary or query string into target folder
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target file, needs to match 1 file
+        :param source: name of the folder to move file from, is by default drive's
+         `root` folder id
+        :param target: name of the folder to move file into, is by default drive's
+         `root` folder id
+        :param multiple_ok: if `True` then moving more than 1 file
+        :return: list of file ids
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${source_id}=  Get Drive Folder Id  sourcefolder
+            ${query}=      Set Variable  name contains '.json' and '${sourceid}' in parents
+            ${files}=      Move Drive File  query=${query}  folder=target_folder  multiple_ok=True
+        """  # noqa: E501
+        result_files = []
+        if file_id or file_dict:
+            target_files = self._get_target_file(
+                file_id, file_dict, query, multiple_ok, details=True
+            )
+        else:
+            target_files = self.search_drive_files(query, source=source)
+        target_parent = None
+        if len(target_files) == 0:
+            raise GoogleDriveError("Did not find any files to move")
+        if target:
+            target_parent = self.get_drive_folder_id(target)
+        if target_parent is None:
+            raise GoogleDriveError(
+                "Unable to find target folder: '%s'" % (target if target else "root")
+            )
+        for tf in target_files:
+            file = self.service.files().get(fileId=tf["id"], fields="parents").execute()
+            previous_parents = ",".join(file.get("parents"))
+            try:
+                result_file = (
+                    self.service.files()
+                    .update(
+                        fileId=tf["id"],
+                        addParents=target_parent,
+                        removeParents=previous_parents,
+                        fields="id, parents",
+                    )
+                    .execute()
+                )
+            except HttpError as err:
+                raise GoogleDriveError(str(err)) from err
+            result_files.append(result_file)
+        return result_files
+
+    @keyword(tags=["drive", "drive share", "v2.0.0"])
+    def list_shared_drive_files(self, query: str = None, source: str = None) -> List:
+        """Keyword for listing shared files in the source folder.
+
+        Alias keyword for ``Search Drive Files`` which can be used to list
+        only files which have been shared.
+
+        :param query: drive query string to find target files
+        :param source: source directory where query is executed
+        :return: list of shared files
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${shared}=    List Shared Drive Files    source=subfolder
+            FOR    ${file}    IN    @{shared}
+                Log To Console    ${file}
+            END
+        """
+        files = self.search_drive_files(query=query, source=source)
+        return [f for f in files if f["shared"]]
+
+    @keyword(tags=["drive"])
+    def search_drive_files(
+        self, query: str = None, recurse: bool = False, source: str = None
+    ) -> List:
+        """Search Google Drive for files matching query string
+
+        :param query: search string, defaults to None which means that all files
+         and folders are returned
+        :param recurse: set to `True` if search should recursive
+        :param source: source directory where query is executed
+        :return: list of files
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${files}=  Search Drive Files   query=name contains 'hello'
+            ${files}=  Search Drive Files   query=modifiedTime > '2020-06-04T12:00:00'
+            ${files}=  Search Drive Files   query=mimeType contains 'image/' or mimeType contains 'video/'
+            ${files}=  Search Drive Files   query=name contains '.yaml'  recurse=True
+            ${files}=  Search Drive Files   query=name contains '.yaml'  source=datadirectory
+        """  # noqa: E501
+        page_token = None
+        filelist = []
+
+        parameters = self._set_search_parameters(query, source, recurse)
+
+        while True:
+            if page_token:
+                parameters["pageToken"] = page_token
+            try:
+                self.logger.debug("Searching with parameters: '%s'" % parameters)
+                response = self.service.files().list(**parameters).execute()
+                for file_details in response.get("files", []):
+                    file_dict = self._drive_file_details_into_file_dict(file_details)
+                    filelist.append(file_dict)
+                page_token = response.get("nextPageToken", None)
+                if page_token is None:
+                    break
+            except HttpError as err:
+                raise GoogleDriveError(str(err)) from err
+        return filelist
+
+    def _set_search_parameters(self, query, source, recurse):
+        parameters = {
+            "fields": "*",
+        }
+        if query:
+            parameters["q"] = query
+
+        folder_id = None
+        if source:
+            folder_id = self.get_drive_folder_id(source)
+        elif not recurse:
+            folder_id = "root"
+
+        if folder_id:
+            if "q" in parameters:
+                parameters["q"] += f" and '{folder_id}' in parents"
+            else:
+                parameters["q"] = f"'{folder_id}' in parents"
+        return parameters
+
+    def _drive_file_details_into_file_dict(self, details):
+        filesize = details.get("size")
+        file_id = details.get("id")
+        parents = details.get("parents")
+        kind = details.get("kind")
+        mimetype = details.get("mimeType")
+        is_folder = mimetype == "application/vnd.google-apps.folder"
+        folder_id = (
+            file_id
+            if mimetype == "application/vnd.google-apps.folder"
+            else parents[0]
+            if parents and len(parents) > 0
+            else None
+        )
+        file_link = (
+            None
+            if mimetype == "application/vnd.google-apps.folder"
+            else f"https://drive.google.com/file/d/{file_id}?usp=sharing"
+        )
+        folder_link = (
+            f"https://drive.google.com/drive/folders/{folder_id}?usp=sharing"
+            if folder_id
+            else ""
+        )
+        file_dict = {
+            "name": details.get("name"),
+            "id": file_id,
+            "size": int(filesize) if filesize else None,
+            "kind": kind,
+            "is_folder": is_folder,
+            "parents": parents,
+            "starred": details.get("starred"),
+            "trashed": details.get("trashed"),
+            "shared": details.get("shared"),
+            "permissions": details.get("permissions", []),
+            "mimeType": mimetype,
+            "spaces": details.get("spaces", None),
+            "exportLinks": details.get("exportLinks"),
+            "createdTime": details.get("createdTime"),
+            "modifiedTime": details.get("modifiedTime"),
+            "fileLink": file_link,
+            "folderLink": folder_link,
+        }
+        return file_dict
+
+    @keyword(tags=["drive"])
+    def create_drive_directory(
+        self, folder: str = None, parent_folder: str = None
+    ) -> Dict:
+        """Create new directory to Google Drive
+
+        :param folder: name for the new directory
+        :param parent_folder: top level directory for new directory
+        :return: dictionary containing folder ID and folder URL
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${folder}=  Create Drive Directory   example-folder
+            Log To Console    Google Drive folder ID: ${folder}[id]
+            Log To Console    Google Drive folder URL:  ${folder}[url]
+        """
+        if not folder or len(folder) == 0:
+            raise GoogleDriveError("Can't create Drive directory with empty name")
+
+        folder_id = self.get_drive_folder_id(folder, parent_folder=parent_folder)
+        if folder_id:
+            self.logger.info(
+                "Folder '%s' already exists. Not creating new one.", folder_id
+            )
+            return self._folder_response(folder_id)
+
+        file_metadata = {
+            "name": folder,
+            "mimeType": "application/vnd.google-apps.folder",
+        }
+
+        if parent_folder:
+            parent_folder_id = self.get_drive_folder_id(parent_folder)
+            file_metadata["parents"] = [parent_folder_id]
+        try:
+            added_folder = (
+                self.service.files().create(body=file_metadata, fields="id").execute()
+            )
+            return self._folder_response(added_folder["id"])
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+
+    def _folder_response(self, folder_id):
+        return {
+            "id": folder_id,
+            "url": f"https://drive.google.com/drive/folders/{folder_id}?usp=sharing",
+        }
+
+    @keyword(tags=["drive"])
+    def export_drive_file(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        target_file: str = None,
+        mimetype: str = "application/pdf",
+    ) -> str:
+        """Export Google Drive file using Drive export links
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param target_file: name for the exported file
+        :param mimetype: export mimetype, defaults to "application/pdf"
+        :return: file path to the exported file
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${files}=  Drive Search Files  query=name contains 'my example worksheet'
+            Export Drive File  file_dict=${files}[0]
+        """
+        if target_file is None or len(target_file) == 0:
+            raise AttributeError("The target_file is required parameter for export")
+        if file_id is None and file_dict is None:
+            raise AttributeError("Either file_id or file_dict is required for export")
+        target_files = self._get_target_file(file_id, file_dict, None, False)
+        if len(target_files) != 1:
+            raise ValueError("Did not find the Google Drive file to export")
+        try:
+            request = self.service.files().export(
+                fileId=target_files[0], mimeType=mimetype
+            )
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+
+        fh = BytesIO()
+        downloader = MediaIoBaseDownload(fh, request)
+        done = False
+        while done is False:
+            _, done = downloader.next_chunk()
+
+        fh.seek(0)
+        filepath = Path(target_file).absolute()
+        with open(filepath, "wb") as f:
+            shutil.copyfileobj(fh, f, length=131072)
+        return filepath
+
+    @keyword(tags=["drive", "drive share", "v2.0.0"])
+    def add_drive_share(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        email: str = None,
+        domain: str = None,
+        role: DriveRole = DriveRole.READER,
+        share_type: DriveType = DriveType.USER,
+        notification: bool = False,
+        notification_message: str = None,
+    ) -> Dict:
+        """Keyword for sharing drive file or folder.
+
+        Parameters `file_id`, `file_dict`, `query` and `source` can be
+        used to select files to which sharing is added to.
+
+        If share is added to a folder, all files within that folder get same
+        sharing permissions.
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target file, needs to match 1 file
+        :param source: name of the folder to search files in, is by default drive's
+         `root` folder
+        :param email: user or group email address if share type
+         is DriveType.USER or DriveType.GROUP
+        :param domain: domain name if share type is DriveType.DOMAIN
+        :param role: see ``DriveRole`` enum for possible values,
+         defaults to DriveRole.READER
+        :param share_type: see ``DriveType`` enum for possible values,
+         defaults to DriveType.USER
+        :param notification: whether to send notificatin email, defaults to False
+        :param notification_message: optional message to include with the notification
+        :return: share response dictionary containing 'file_id' and 'permission_id'
+
+        Example:
+
+        .. code-block:: robotframework
+
+            # Add file share for a email address with email notification
+            Add Drive Share
+            ...    query=name = 'okta.png'
+            ...    email=robocorp.tester@gmail.com
+            ...    notification=True
+            ...    notification_message=Hello. I have shared 'okta.png' with you for review.
+            # Add file share for a domain
+            Add Drive Share
+            ...    query=name = 'okta.png'
+            ...    domain=robocorp.com
+            # Add folder share for a email address
+            ${folder}=    Create Drive Directory   attachments-for-the-task
+            ${share}=  Add Drive Share
+            ...   file_id=${folder}[id]
+            ...   email=robocorp.tester@gmail.com
+            ...   role=writer
+            Log To Console  Share details: ${share}[file_id], ${share}[permission_id]
+        """  # noqa: E501
+        target_file = self._get_target_file(
+            file_id, file_dict, query, False, source=source
+        )
+        if not target_file:
+            raise GoogleDriveError("Did not find target file")
+        if domain:
+            share_type = DriveType.DOMAIN
+        user_permission = {
+            "type": to_drive_type(share_type),
+            "role": to_drive_role(role),
+        }
+        if share_type in [DriveType.USER, DriveType.GROUP]:
+            if not email:
+                raise ValueError(
+                    "email parameter is required with share_type = 'user' or 'group'"
+                )
+            user_permission["emailAddress"] = email
+        if share_type == DriveType.DOMAIN:
+            if not domain:
+                raise ValueError(
+                    "domain parameter is required with share_type = 'domain'"
+                )
+            user_permission["domain"] = domain
+
+        request_parameters = {
+            "fileId": target_file[0],
+            "body": user_permission,
+            "fields": "id",
+            "sendNotificationEmail": notification,
+        }
+        if notification and notification_message:
+            request_parameters["emailMessage"] = notification_message
+
+        try:
+            response = self.service.permissions().create(**request_parameters).execute()
+            return {"file_id": target_file[0], "permission_id": response["id"]}
+        except HttpError as err:
+            raise GoogleDriveError(str(err)) from err
+
+    @keyword(tags=["drive", "drive share", "v2.0.0"])
+    def remove_drive_share_by_permission_id(
+        self,
+        permission_id: str,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        suppress_errors: bool = False,
+    ) -> Dict:
+        """Keyword for removing share permission of file or folder
+        permission id.
+
+        Parameters `file_id`, `file_dict`, `query` and `source` can be
+        used to select files from which sharing is removed.
+
+        :param permission_id: id of the permission to remove
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target file, needs to match 1 file
+        :param source: name of the folder to search files in, is by default drive's
+         `root` folder
+        :param suppress_errors: on True will log warning message instead of
+         raising an exception, defaults to False (exception is raised)
+        :return: dictionary of permission response
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${share}=   Add Drive Share
+            ...  query=name = 'sharable-files' and mimeType = 'application/vnd.google-apps.folder'
+            ...  email=robocorp.tester@gmail.com
+            #
+            # actions on shared files in the folder 'shareable-files' ....
+            #
+            Remove Drive Share By Permission Id   ${share}[permission_id]  ${share}[file_id]
+        """  # noqa: E501
+        target_file = self._get_target_file(
+            file_id, file_dict, query, False, source=source
+        )
+        if not target_file:
+            raise GoogleDriveError("Did not find target file")
+
+        self.logger.info(
+            "Removing permission id '%s' for file_id '%s'"
+            % (permission_id, target_file[0])
+        )
+        response = None
+        try:
+            response = (
+                self.service.permissions()
+                .delete(fileId=target_file[0], permissionId=permission_id)
+                .execute()
+            )
+        except HttpError as err:
+            if suppress_errors:
+                self.logger.warn(str(err))
+            else:
+                raise GoogleDriveError(str(err)) from err
+        return response
+
+    @keyword(tags=["drive", "drive share", "v2.0.0"])
+    def remove_drive_share_by_criteria(
+        self,
+        email: str = None,
+        domain: str = None,
+        permission_id: str = None,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        source: str = None,
+        suppress_errors: bool = False,
+    ) -> List:
+        """Keyword for removing share from file or folder
+        based on criteria.
+
+        Parameters `file_id`, `file_dict`, `query` and `source` can be
+        used to select files from which sharing is removed.
+
+        Parameters `email`, `domain` or `permission_id` can be
+        used to select which share is removed from selected files.
+
+        :param email: email address of the permission to remove
+        :param domain: domain name of the permission to remove
+        :param permission_id: id of the permission to remove
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target files
+        :param source: name of the folder to search files in, is by default drive's
+         `root` folder
+        :param suppress_errors: on True will log warning message instead of
+         raising an exception, defaults to False (exception is raised)
+        :return: list of dictionaries containing information of file permissions removed
+
+        Example:
+
+        .. code-block:: robotframework
+
+            # Remove domain shares for files in the folder ${FOLDER_NAME}
+            ${removed}=    Remove Drive Share By Criteria
+            ...    domain=robocorp.com
+            ...    source=${FOLDER_NAME}
+            # Remove email share for a file
+            ${removed}=    Remove Drive Share By Criteria
+            ...    query=name = 'okta.png'
+            ...    email=robocorp.tester@gmail.com
+        """
+        if not email and not domain and permission_id:
+            raise AttributeError(
+                "At least one of the 'email', 'domain' or 'permission_id' "
+                "is required to remove drive share"
+            )
+        target_files = self._get_target_file(
+            file_id, file_dict, query, multiple_ok=True, source=source, details=True
+        )
+        if not target_files or len(target_files) == 0:
+            raise GoogleDriveError("Did not find target files")
+        permissions_removed = []
+        for tf in target_files:
+            file_permissions_removed = []
+            if "permissions" in tf and tf["permissions"]:
+                self.logger.info(
+                    "Removing shares from file '%s' id '%s'" % (tf["name"], tf["id"])
+                )
+                for p in tf["permissions"]:
+                    if self._is_permission_removable(p, email, domain, permission_id):
+                        self._remove_file_permission(
+                            tf, p, file_permissions_removed, suppress_errors
+                        )
+            if file_permissions_removed:
+                permissions_removed.append(
+                    {
+                        "file_id": tf["id"],
+                        "file_name": tf["name"],
+                        "permissions_removed": file_permissions_removed,
+                    }
+                )
+        return permissions_removed
+
+    def _is_permission_removable(self, permission, email, domain, permission_id):
+        return (
+            (
+                email
+                and "emailAddress" in permission.keys()
+                and permission["emailAddress"] == email
+            )
+            or (
+                domain
+                and "domain" in permission.keys()
+                and permission["domain"] == domain
+            )
+            or (permission_id and permission["id"] == permission_id)
+        )
+
+    def _remove_file_permission(
+        self, drive_file, permission, permissions_removed, suppress_errors
+    ):
+        try:
+            self.service.permissions().delete(
+                fileId=drive_file["id"], permissionId=permission["id"]
+            ).execute()
+            permissions_removed.append(permission)
+        except HttpError as err:
+            if suppress_errors:
+                self.logger.warn(str(err))
+            else:
+                raise GoogleDriveError(str(err)) from err
+
+    @keyword(tags=["drive", "drive share", "v2.0.0"])
+    def remove_all_drive_shares(
+        self,
+        file_id: str = None,
+        file_dict: dict = None,
+        query: str = None,
+        suppress_errors: bool = False,
+    ) -> List:
+        """Keyword for removing all shares from selected files (only owner
+        permission is retained).
+
+        :param file_id: drive file id
+        :param file_dict: file dictionary returned by `Search Drive Files`
+        :param query: drive query string to find target files
+        :param suppress_errors: on True will log warning message instead of
+         raising an exception, defaults to False (exception is raised)
+        :return: list of dictionaries containing information of file permissions removed
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${removed}=  Remove All Drive Shares    file_id=${FOLDER_ID}
+        """
+        target_files = self._get_target_file(
+            file_id, file_dict, query, multiple_ok=True, details=True
+        )
+        permissions_removed = []
+        for tf in target_files:
+            if "permissions" in tf and tf["permissions"]:
+                self.logger.info(
+                    "Removing shares from file '%s' id '%s'" % (tf["name"], tf["id"])
+                )
+                for p in tf["permissions"]:
+                    if p["role"] != "owner":
+                        self.remove_drive_share_by_permission_id(
+                            file_id=tf["id"],
+                            permission_id=p["id"],
+                            suppress_errors=suppress_errors,
+                        )
+                        permissions_removed.append(p)
+        return permissions_removed
+
+    @keyword(tags=["drive", "v2.0.0"])
+    def get_drive_file_by_id(self, file_id: str, suppress_errors: bool = False) -> Dict:
+        """Get file dictionary by its file id.
+
+        :param file_id: id of the file in the Google Drive
+        :param suppress_errors: on True will log warning message instead of
+         raising an exception, defaults to False (exception is raised)
+        :return: dictionary containing file information
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${file_dict}=  Get Drive File By ID    file_id=${FILE_ID}
+        """
+        response = None
+        try:
+            raw_response = (
+                self.service.files().get(fileId=file_id, fields="*").execute()
+            )
+            response = self._drive_file_details_into_file_dict(raw_response)
+        except HttpError as err:
+            if suppress_errors:
+                self.logger.warn(str(err))
+            else:
+                raise GoogleDriveError(str(err)) from err
+        return response
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/enums.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/enums.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from enum import Enum
-from google.cloud import language_v1, videointelligence
-
-
-class TextType(Enum):
-    """Possible text types."""
-
-    TEXT = language_v1.Document.Type.PLAIN_TEXT
-    HTML = language_v1.Document.Type.HTML
-
-
-class UpdateAction(Enum):
-    """Possible file update actions."""
-
-    trash = 1
-    untrash = 2
-    star = 3
-    unstar = 4
-
-
-def to_texttype(value):
-    """Convert value to TextType enum."""
-    if isinstance(value, TextType):
-        return int(value.value)
-
-    sanitized = str(value).upper().strip().replace(" ", "_")
-    try:
-        return int(TextType[sanitized].value)
-    except KeyError as err:
-        raise ValueError(f"Unknown text type: {value}") from err
-
-
-class VideoFeature(Enum):
-    """Possible video features."""
-
-    FEATURE_UNSPECIFIED = videointelligence.Feature.FEATURE_UNSPECIFIED
-    LABEL_DETECTION = videointelligence.Feature.LABEL_DETECTION
-    SHOT_CHANGE_DETECTION = videointelligence.Feature.SHOT_CHANGE_DETECTION
-    EXPLICIT_CONTENT_DETECTION = videointelligence.Feature.EXPLICIT_CONTENT_DETECTION
-    SPEECH_TRANSCRIPTION = videointelligence.Feature.SPEECH_TRANSCRIPTION
-    TEXT_DETECTION = videointelligence.Feature.TEXT_DETECTION
-    OBJECT_TRACKING = videointelligence.Feature.OBJECT_TRACKING
-    LOGO_RECOGNITION = videointelligence.Feature.LOGO_RECOGNITION
-
-
-def to_feature(value):
-    """Convert value to VideoFeature enum."""
-    if isinstance(value, VideoFeature):
-        return int(value.value)
-
-    sanitized = str(value).upper().strip().replace(" ", "_")
-    try:
-        return int(VideoFeature[sanitized].value)
-    except KeyError as err:
-        raise ValueError(f"Unknown video feature: {value}") from err
-
-
-class DriveRole(Enum):
-    """Possible Drive user roles"""
-
-    OWNER = "owner"
-    ORGANIZER = "organizer"
-    FILE_ORGANIZER = "fileOrganizer"
-    WRITER = "writer"
-    COMMENTER = "commenter"
-    READER = "reader"
-
-
-def to_drive_role(value):
-    """Convert value to DriveRole enum."""
-    if isinstance(value, DriveRole):
-        return value.value
-
-    sanitized = str(value).upper().strip().replace(" ", "_")
-    try:
-        return DriveRole[sanitized].value
-    except KeyError as err:
-        raise ValueError(f"Unknown drive role: {value}") from err
-
-
-class DriveType(Enum):
-    """Possible Drive Share types"""
-
-    USER = "user"
-    GROUP = "group"
-    DOMAIN = "domain"
-    ANY = "anyone"
-
-
-def to_drive_type(value):
-    """Convert value to DriveType enum."""
-    if isinstance(value, DriveType):
-        return value.value
-
-    sanitized = str(value).upper().strip().replace(" ", "_")
-    try:
-        return DriveType[sanitized].value
-    except KeyError as err:
-        raise ValueError(f"Unknown drive type: {value}") from err
+from enum import Enum
+from google.cloud import language_v1, videointelligence
+
+
+class TextType(Enum):
+    """Possible text types."""
+
+    TEXT = language_v1.Document.Type.PLAIN_TEXT
+    HTML = language_v1.Document.Type.HTML
+
+
+class UpdateAction(Enum):
+    """Possible file update actions."""
+
+    trash = 1
+    untrash = 2
+    star = 3
+    unstar = 4
+
+
+def to_texttype(value):
+    """Convert value to TextType enum."""
+    if isinstance(value, TextType):
+        return int(value.value)
+
+    sanitized = str(value).upper().strip().replace(" ", "_")
+    try:
+        return int(TextType[sanitized].value)
+    except KeyError as err:
+        raise ValueError(f"Unknown text type: {value}") from err
+
+
+class VideoFeature(Enum):
+    """Possible video features."""
+
+    FEATURE_UNSPECIFIED = videointelligence.Feature.FEATURE_UNSPECIFIED
+    LABEL_DETECTION = videointelligence.Feature.LABEL_DETECTION
+    SHOT_CHANGE_DETECTION = videointelligence.Feature.SHOT_CHANGE_DETECTION
+    EXPLICIT_CONTENT_DETECTION = videointelligence.Feature.EXPLICIT_CONTENT_DETECTION
+    SPEECH_TRANSCRIPTION = videointelligence.Feature.SPEECH_TRANSCRIPTION
+    TEXT_DETECTION = videointelligence.Feature.TEXT_DETECTION
+    OBJECT_TRACKING = videointelligence.Feature.OBJECT_TRACKING
+    LOGO_RECOGNITION = videointelligence.Feature.LOGO_RECOGNITION
+
+
+def to_feature(value):
+    """Convert value to VideoFeature enum."""
+    if isinstance(value, VideoFeature):
+        return int(value.value)
+
+    sanitized = str(value).upper().strip().replace(" ", "_")
+    try:
+        return int(VideoFeature[sanitized].value)
+    except KeyError as err:
+        raise ValueError(f"Unknown video feature: {value}") from err
+
+
+class DriveRole(Enum):
+    """Possible Drive user roles"""
+
+    OWNER = "owner"
+    ORGANIZER = "organizer"
+    FILE_ORGANIZER = "fileOrganizer"
+    WRITER = "writer"
+    COMMENTER = "commenter"
+    READER = "reader"
+
+
+def to_drive_role(value):
+    """Convert value to DriveRole enum."""
+    if isinstance(value, DriveRole):
+        return value.value
+
+    sanitized = str(value).upper().strip().replace(" ", "_")
+    try:
+        return DriveRole[sanitized].value
+    except KeyError as err:
+        raise ValueError(f"Unknown drive role: {value}") from err
+
+
+class DriveType(Enum):
+    """Possible Drive Share types"""
+
+    USER = "user"
+    GROUP = "group"
+    DOMAIN = "domain"
+    ANY = "anyone"
+
+
+def to_drive_type(value):
+    """Convert value to DriveType enum."""
+    if isinstance(value, DriveType):
+        return value.value
+
+    sanitized = str(value).upper().strip().replace(" ", "_")
+    try:
+        return DriveType[sanitized].value
+    except KeyError as err:
+        raise ValueError(f"Unknown drive type: {value}") from err
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/gmail.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/gmail.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,345 +1,345 @@
-import base64
-import mimetypes
-import os
-from pathlib import Path
-from typing import Optional
-
-from email.mime.audio import MIMEAudio
-from email.mime.base import MIMEBase
-from email.mime.image import MIMEImage
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from googleapiclient import errors
-
-
-from . import LibraryContext, keyword
-
-
-def get_size_format(b, factor=1024, suffix="B"):
-    """
-    Scale bytes to its proper byte format
-    e.g:
-        1253656 => '1.20MB'
-        1253656678 => '1.17GB'
-    """
-    for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
-        if b < factor:
-            return f"{b:.2f}{unit}{suffix}"
-        b /= factor
-    return f"{b:.2f}Y{suffix}"
-
-
-def clean(text):
-    # clean text for creating a folder
-    return "".join(c if c.isalnum() else "_" for c in text)
-
-
-class GmailKeywords(LibraryContext):
-    """Class for Google Gmail API
-
-    **Note:** The Gmail API does not work with _service accounts_
-
-    For more information about Google Gmail API link_.
-
-    .. _link: https://developers.google.com/gmail/api
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "gmail"])
-    def init_gmail(
-        self,
-        service_account: str = None,
-        credentials: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        scopes: list = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Gmail client
-
-        :param service_account: file path to service account file
-        :param credentials: file path to credentials file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param scopes: list of extra authentication scopes
-        :param token_file: file path to token file
-        """
-        gmail_scopes = ["gmail.send", "gmail.compose", "gmail.modify", "gmail.labels"]
-        if scopes:
-            gmail_scopes += scopes
-        self.service = self.init_service(
-            service_name="gmail",
-            api_version="v1",
-            scopes=gmail_scopes,
-            service_account_file=service_account,
-            credentials_file=credentials,
-            use_robocorp_vault=use_robocorp_vault,
-            token_file=token_file,
-        )
-
-    def create_message(
-        self,
-        to: str,
-        subject: str,
-        message_text: str,
-        attachments: list = None,
-    ):
-        """Create a message for an email.
-
-        :param to: message recipient
-        :param subject: message subject
-        :param message_text: message body text
-        :param attachment: list of files to add as message attachments
-        :return: An object containing a base64url encoded email object
-        """
-        mimeMessage = MIMEMultipart()
-        mimeMessage["to"] = to
-        mimeMessage["subject"] = subject
-        mimeMessage.attach(MIMEText(message_text, "plain"))
-
-        for at in attachments:
-            self.add_attachment_to_message(mimeMessage, at)
-        return {"raw": base64.urlsafe_b64encode(mimeMessage.as_bytes()).decode()}
-
-    def add_attachment_to_message(self, mimeMessage, attachment):
-        content_type, encoding = mimetypes.guess_type(attachment)
-
-        if content_type is None or encoding is not None:
-            content_type = "application/octet-stream"
-        main_type, sub_type = content_type.split("/", 1)
-        if main_type == "text":
-            with open(attachment, "r") as fp:  # pylint: disable=unspecified-encoding
-                msg = MIMEText(fp.read(), _subtype=sub_type)
-        elif main_type == "image":
-            with open(attachment, "rb") as fp:
-                msg = MIMEImage(fp.read(), _subtype=sub_type)
-        elif main_type == "audio":
-            with open(attachment, "rb") as fp:
-                msg = MIMEAudio(fp.read(), _subtype=sub_type)
-        else:
-            with open(attachment, "rb") as fp:
-                msg = MIMEBase(main_type, sub_type)
-                msg.set_payload(fp.read())
-        filename = os.path.basename(attachment)
-        msg.add_header("Content-Disposition", "attachment", filename=filename)
-        mimeMessage.attach(msg)
-
-    @keyword(tags=["gmail"])
-    def send_message(
-        self,
-        sender: str,
-        to: str,
-        subject: str,
-        message_text: str,
-        attachments: list = None,
-    ):
-        """Send an email message.
-
-        :param sender: message sender
-        :param to: message recipient
-        :param subject: message subject
-        :param message_text: message body text
-        :param attachment: list of files to add as message attachments
-        :return: sent message
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${attachments}=  Create List
-            ...  ${CURDIR}${/}random.txt
-            ...  ${CURDIR}${/}source.png
-            Send Message    me
-            ...    mika@robocorp.com
-            ...    message subject
-            ...    body of the message
-            ...    ${attachments}
-        """
-        if not self.service:
-            raise AssertionError("Gmail service has not been initialized")
-        attachments = attachments or []
-        message = self.create_message(to, subject, message_text, attachments)
-        try:
-            response = (
-                self.service.users()
-                .messages()
-                .send(userId=sender, body=message)
-                .execute()
-            )
-            self.logger.debug("Message Id: %s" % response["id"])
-        except errors.HttpError as he:
-            self.logger.warning(str(he))
-            raise he
-        return response
-
-    def set_list_parameters(self, user_id, query, label_ids, max_results, include_spam):
-        parameters = {"userId": user_id, "q": query}
-        if label_ids:
-            parameters["labelIds"] = ",".join(label_ids)
-        if max_results:
-            parameters["maxResults"] = max_results
-        if include_spam:
-            parameters["includeSpamTrash"] = include_spam
-        return parameters
-
-    def set_headers_to_message_dict(self, payload, message_id, response):
-        headers = payload.get("headers")
-        message_dict = {"id": message_id, "label_ids": response["labelIds"]}
-        for header in headers:
-            name = header.get("name")
-            value = header.get("value")
-            if name.lower() == "from":
-                message_dict["from"] = value
-            if name.lower() == "to":
-                message_dict["to"] = value
-            if name.lower() == "subject":
-                message_dict["subject"] = value
-            if name.lower() == "date":
-                message_dict["date"] = value
-        return message_dict
-
-    def handle_mimetypes(self, parsed_parts, part, msg, folder_name):
-        filename = part.get("filename")
-        mimetype = part.get("mimeType")
-        body = part.get("body")
-        data = body.get("data")
-        filesize = body.get("size")
-        part_headers = part.get("headers")
-        if mimetype == "text/plain":
-            if data:
-                text = base64.urlsafe_b64decode(data).decode()
-                parsed_parts.append({"text/plain": text})
-        elif mimetype == "text/html":
-            if not filename:
-                filename = "message.html"
-            filepath = os.path.join(folder_name, filename)
-
-            with open(filepath, "wb") as f:
-                data = base64.urlsafe_b64decode(data)
-                parsed_parts.append({"text/html": data, "path": filepath})
-                f.write(data)
-        else:
-            for part_header in part_headers:
-                part_header_name = part_header.get("name")
-                part_header_value = part_header.get("value")
-                if part_header_name == "Content-Disposition":
-                    if "attachment" in part_header_value:
-                        # we get the attachment ID
-                        # and make another request to get the attachment itself
-                        self.logger.info(
-                            "Saving the file: %s, size:%s"
-                            % (filename, get_size_format(filesize))
-                        )
-                        attachment_id = body.get("attachmentId")
-                        attachment = (
-                            self.service.users()
-                            .messages()
-                            .attachments()
-                            .get(
-                                id=attachment_id,
-                                userId="me",
-                                messageId=msg["id"],
-                            )
-                            .execute()
-                        )
-                        data = attachment.get("data")
-                        filepath = os.path.join(folder_name, filename)
-                        if data:
-                            parsed_parts.append(
-                                {"attachment": filepath, "id": attachment_id}
-                            )
-                            with open(filepath, "wb") as f:
-                                f.write(base64.urlsafe_b64decode(data))
-
-    @keyword(tags=["gmail"])
-    def list_messages(
-        self,
-        user_id: str,
-        query: str,
-        folder_name: str = None,
-        label_ids: list = None,
-        max_results: int = None,
-        include_json: bool = False,
-        include_spam: bool = False,
-    ):
-        """List messages
-
-        :param user_id: user's email address. The special value me can
-         be used to indicate the authenticated user.
-        :param query: message query
-        :param folder_name: path where attachments are saved, default current
-         directory
-        :param label_ids: message label ids
-        :param max_results: maximum number of message to return
-        :param include_json: include original response json
-        :param include_spam: include messages from SPAM and TRASH
-        :return: messages
-
-        Example:
-
-        .. code-block:: robotframework
-
-            ${messages}=    List Messages    me
-            ...    from:mika@robocorp.com
-            ...    folder_name=${CURDIR}${/}target
-            ...    include_json=True
-            FOR    ${msg}    IN    @{messages}
-                Log Many    ${msg}
-            END
-        """
-        parameters = self.set_list_parameters(
-            user_id, query, label_ids, max_results, include_spam
-        )
-        folder_name = Path(folder_name) if folder_name else Path().absolute()
-        messages = []
-        try:
-            response = self.service.users().messages().list(**parameters).execute()
-            message_ids = [
-                m["id"] for m in response["messages"] if "messages" in response.keys()
-            ]
-            for message_id in message_ids:
-                response = (
-                    self.service.users()
-                    .messages()
-                    .get(userId=user_id, id=message_id)
-                    .execute()
-                )
-                payload = response["payload"]
-                message_dict = self.set_headers_to_message_dict(
-                    payload, message_id, response
-                )
-                if include_json:
-                    message_dict["json"] = response
-                parts = payload.get("parts")
-                parsed_parts = self.parse_parts(
-                    message_id, response, parts, folder_name
-                )
-                message_dict["parts"] = parsed_parts
-                messages.append(message_dict)
-        except errors.HttpError as he:
-            self.logger.warning(str(he))
-            raise he
-        return messages
-
-    def parse_parts(self, msg_id, msg, parts, folder_name):
-        """
-        Utility function that parses the content of an email partition
-        """
-        if msg_id and msg_id not in str(folder_name):
-            try:
-                folder_name = folder_name / msg_id
-                folder_name.mkdir(parents=True, exist_ok=True)
-            except FileExistsError:
-                pass
-
-        parsed_parts = []
-        if parts:
-            for part in parts:
-                if part.get("parts"):
-                    # recursively call this function when we see that a part
-                    # has parts inside
-                    self.parse_parts(None, msg, part.get("parts"), folder_name)
-                self.handle_mimetypes(parsed_parts, part, msg, folder_name)
-
-        return parsed_parts
+import base64
+import mimetypes
+import os
+from pathlib import Path
+from typing import Optional
+
+from email.mime.audio import MIMEAudio
+from email.mime.base import MIMEBase
+from email.mime.image import MIMEImage
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from googleapiclient import errors
+
+
+from . import LibraryContext, keyword
+
+
+def get_size_format(b, factor=1024, suffix="B"):
+    """
+    Scale bytes to its proper byte format
+    e.g:
+        1253656 => '1.20MB'
+        1253656678 => '1.17GB'
+    """
+    for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
+        if b < factor:
+            return f"{b:.2f}{unit}{suffix}"
+        b /= factor
+    return f"{b:.2f}Y{suffix}"
+
+
+def clean(text):
+    # clean text for creating a folder
+    return "".join(c if c.isalnum() else "_" for c in text)
+
+
+class GmailKeywords(LibraryContext):
+    """Class for Google Gmail API
+
+    **Note:** The Gmail API does not work with _service accounts_
+
+    For more information about Google Gmail API link_.
+
+    .. _link: https://developers.google.com/gmail/api
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "gmail"])
+    def init_gmail(
+        self,
+        service_account: str = None,
+        credentials: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        scopes: list = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Gmail client
+
+        :param service_account: file path to service account file
+        :param credentials: file path to credentials file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param scopes: list of extra authentication scopes
+        :param token_file: file path to token file
+        """
+        gmail_scopes = ["gmail.send", "gmail.compose", "gmail.modify", "gmail.labels"]
+        if scopes:
+            gmail_scopes += scopes
+        self.service = self.init_service(
+            service_name="gmail",
+            api_version="v1",
+            scopes=gmail_scopes,
+            service_account_file=service_account,
+            credentials_file=credentials,
+            use_robocorp_vault=use_robocorp_vault,
+            token_file=token_file,
+        )
+
+    def create_message(
+        self,
+        to: str,
+        subject: str,
+        message_text: str,
+        attachments: list = None,
+    ):
+        """Create a message for an email.
+
+        :param to: message recipient
+        :param subject: message subject
+        :param message_text: message body text
+        :param attachment: list of files to add as message attachments
+        :return: An object containing a base64url encoded email object
+        """
+        mimeMessage = MIMEMultipart()
+        mimeMessage["to"] = to
+        mimeMessage["subject"] = subject
+        mimeMessage.attach(MIMEText(message_text, "plain"))
+
+        for at in attachments:
+            self.add_attachment_to_message(mimeMessage, at)
+        return {"raw": base64.urlsafe_b64encode(mimeMessage.as_bytes()).decode()}
+
+    def add_attachment_to_message(self, mimeMessage, attachment):
+        content_type, encoding = mimetypes.guess_type(attachment)
+
+        if content_type is None or encoding is not None:
+            content_type = "application/octet-stream"
+        main_type, sub_type = content_type.split("/", 1)
+        if main_type == "text":
+            with open(attachment, "r") as fp:  # pylint: disable=unspecified-encoding
+                msg = MIMEText(fp.read(), _subtype=sub_type)
+        elif main_type == "image":
+            with open(attachment, "rb") as fp:
+                msg = MIMEImage(fp.read(), _subtype=sub_type)
+        elif main_type == "audio":
+            with open(attachment, "rb") as fp:
+                msg = MIMEAudio(fp.read(), _subtype=sub_type)
+        else:
+            with open(attachment, "rb") as fp:
+                msg = MIMEBase(main_type, sub_type)
+                msg.set_payload(fp.read())
+        filename = os.path.basename(attachment)
+        msg.add_header("Content-Disposition", "attachment", filename=filename)
+        mimeMessage.attach(msg)
+
+    @keyword(tags=["gmail"])
+    def send_message(
+        self,
+        sender: str,
+        to: str,
+        subject: str,
+        message_text: str,
+        attachments: list = None,
+    ):
+        """Send an email message.
+
+        :param sender: message sender
+        :param to: message recipient
+        :param subject: message subject
+        :param message_text: message body text
+        :param attachment: list of files to add as message attachments
+        :return: sent message
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${attachments}=  Create List
+            ...  ${CURDIR}${/}random.txt
+            ...  ${CURDIR}${/}source.png
+            Send Message    me
+            ...    mika@robocorp.com
+            ...    message subject
+            ...    body of the message
+            ...    ${attachments}
+        """
+        if not self.service:
+            raise AssertionError("Gmail service has not been initialized")
+        attachments = attachments or []
+        message = self.create_message(to, subject, message_text, attachments)
+        try:
+            response = (
+                self.service.users()
+                .messages()
+                .send(userId=sender, body=message)
+                .execute()
+            )
+            self.logger.debug("Message Id: %s" % response["id"])
+        except errors.HttpError as he:
+            self.logger.warning(str(he))
+            raise he
+        return response
+
+    def set_list_parameters(self, user_id, query, label_ids, max_results, include_spam):
+        parameters = {"userId": user_id, "q": query}
+        if label_ids:
+            parameters["labelIds"] = ",".join(label_ids)
+        if max_results:
+            parameters["maxResults"] = max_results
+        if include_spam:
+            parameters["includeSpamTrash"] = include_spam
+        return parameters
+
+    def set_headers_to_message_dict(self, payload, message_id, response):
+        headers = payload.get("headers")
+        message_dict = {"id": message_id, "label_ids": response["labelIds"]}
+        for header in headers:
+            name = header.get("name")
+            value = header.get("value")
+            if name.lower() == "from":
+                message_dict["from"] = value
+            if name.lower() == "to":
+                message_dict["to"] = value
+            if name.lower() == "subject":
+                message_dict["subject"] = value
+            if name.lower() == "date":
+                message_dict["date"] = value
+        return message_dict
+
+    def handle_mimetypes(self, parsed_parts, part, msg, folder_name):
+        filename = part.get("filename")
+        mimetype = part.get("mimeType")
+        body = part.get("body")
+        data = body.get("data")
+        filesize = body.get("size")
+        part_headers = part.get("headers")
+        if mimetype == "text/plain":
+            if data:
+                text = base64.urlsafe_b64decode(data).decode()
+                parsed_parts.append({"text/plain": text})
+        elif mimetype == "text/html":
+            if not filename:
+                filename = "message.html"
+            filepath = os.path.join(folder_name, filename)
+
+            with open(filepath, "wb") as f:
+                data = base64.urlsafe_b64decode(data)
+                parsed_parts.append({"text/html": data, "path": filepath})
+                f.write(data)
+        else:
+            for part_header in part_headers:
+                part_header_name = part_header.get("name")
+                part_header_value = part_header.get("value")
+                if part_header_name == "Content-Disposition":
+                    if "attachment" in part_header_value:
+                        # we get the attachment ID
+                        # and make another request to get the attachment itself
+                        self.logger.info(
+                            "Saving the file: %s, size:%s"
+                            % (filename, get_size_format(filesize))
+                        )
+                        attachment_id = body.get("attachmentId")
+                        attachment = (
+                            self.service.users()
+                            .messages()
+                            .attachments()
+                            .get(
+                                id=attachment_id,
+                                userId="me",
+                                messageId=msg["id"],
+                            )
+                            .execute()
+                        )
+                        data = attachment.get("data")
+                        filepath = os.path.join(folder_name, filename)
+                        if data:
+                            parsed_parts.append(
+                                {"attachment": filepath, "id": attachment_id}
+                            )
+                            with open(filepath, "wb") as f:
+                                f.write(base64.urlsafe_b64decode(data))
+
+    @keyword(tags=["gmail"])
+    def list_messages(
+        self,
+        user_id: str,
+        query: str,
+        folder_name: str = None,
+        label_ids: list = None,
+        max_results: int = None,
+        include_json: bool = False,
+        include_spam: bool = False,
+    ):
+        """List messages
+
+        :param user_id: user's email address. The special value me can
+         be used to indicate the authenticated user.
+        :param query: message query
+        :param folder_name: path where attachments are saved, default current
+         directory
+        :param label_ids: message label ids
+        :param max_results: maximum number of message to return
+        :param include_json: include original response json
+        :param include_spam: include messages from SPAM and TRASH
+        :return: messages
+
+        Example:
+
+        .. code-block:: robotframework
+
+            ${messages}=    List Messages    me
+            ...    from:mika@robocorp.com
+            ...    folder_name=${CURDIR}${/}target
+            ...    include_json=True
+            FOR    ${msg}    IN    @{messages}
+                Log Many    ${msg}
+            END
+        """
+        parameters = self.set_list_parameters(
+            user_id, query, label_ids, max_results, include_spam
+        )
+        folder_name = Path(folder_name) if folder_name else Path().absolute()
+        messages = []
+        try:
+            response = self.service.users().messages().list(**parameters).execute()
+            message_ids = [
+                m["id"] for m in response["messages"] if "messages" in response.keys()
+            ]
+            for message_id in message_ids:
+                response = (
+                    self.service.users()
+                    .messages()
+                    .get(userId=user_id, id=message_id)
+                    .execute()
+                )
+                payload = response["payload"]
+                message_dict = self.set_headers_to_message_dict(
+                    payload, message_id, response
+                )
+                if include_json:
+                    message_dict["json"] = response
+                parts = payload.get("parts")
+                parsed_parts = self.parse_parts(
+                    message_id, response, parts, folder_name
+                )
+                message_dict["parts"] = parsed_parts
+                messages.append(message_dict)
+        except errors.HttpError as he:
+            self.logger.warning(str(he))
+            raise he
+        return messages
+
+    def parse_parts(self, msg_id, msg, parts, folder_name):
+        """
+        Utility function that parses the content of an email partition
+        """
+        if msg_id and msg_id not in str(folder_name):
+            try:
+                folder_name = folder_name / msg_id
+                folder_name.mkdir(parents=True, exist_ok=True)
+            except FileExistsError:
+                pass
+
+        parsed_parts = []
+        if parts:
+            for part in parts:
+                if part.get("parts"):
+                    # recursively call this function when we see that a part
+                    # has parts inside
+                    self.parse_parts(None, msg, part.get("parts"), folder_name)
+                self.handle_mimetypes(parsed_parts, part, msg, folder_name)
+
+        return parsed_parts
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/sheets.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/sheets.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from typing import Dict, List, Optional
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-
-class SheetsKeywords(LibraryContext):
-    """Keywords for Google Sheets operations"""
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "sheets"])
-    def init_sheets(
-        self,
-        service_account: str = None,
-        credentials: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        scopes: list = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Sheets client
-
-        :param service_account: file path to service account file
-        :param credentials: file path to credentials file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param scopes: list of extra authentication scopes
-        :param token_file: file path to token file
-        """
-        sheets_scopes = ["drive", "drive.file", "spreadsheets"]
-        if scopes:
-            sheets_scopes += scopes
-        self.service = self.init_service(
-            service_name="sheets",
-            api_version="v4",
-            scopes=sheets_scopes,
-            service_account_file=service_account,
-            credentials_file=credentials,
-            use_robocorp_vault=use_robocorp_vault,
-            token_file=token_file,
-        )
-
-    @keyword(tags=["sheets"])
-    def create_sheet(self, title: str) -> str:
-        """Create empty sheet with a title
-
-        :param title: name as string
-        :return: created `sheet_id`
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=  Create Sheet   Example Sheet
-        """
-        if not title:
-            raise KeyError("title is required for kw: create_sheet")
-
-        data = {"properties": {"title": title}}
-        spreadsheet = (
-            self.service.spreadsheets()
-            .create(body=data, fields="spreadsheetId")
-            .execute()
-        )
-        return spreadsheet.get("spreadsheetId")
-
-    @keyword(tags=["sheets"])
-    def insert_sheet_values(
-        self,
-        sheet_id: str,
-        sheet_range: str,
-        values: list,
-        major_dimension: str = "COLUMNS",
-        value_input_option: str = "USER_ENTERED",
-    ) -> Dict:
-        """Insert values into sheet cells
-
-        :param sheet_id: target sheet
-        :param sheet_range: target sheet range
-        :param values: list of values to insert into sheet
-        :param major_dimension: major dimension of the values, default `COLUMNS`
-        :param value_input_option: controls whether input strings are parsed or not,
-         default `USER_ENTERED`
-        :return: operation result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${values}   Evaluate   [[11, 12, 13], ['aa', 'bb', 'cc']]
-            ${result}=  Insert Sheet Values   ${SHEET_ID}  A:B  ${values}
-            ${result}=  Insert Sheet Values   ${SHEET_ID}  A:B  ${values}  ROWS
-        """
-        resource = {"majorDimension": major_dimension, "values": values}
-        return (
-            self.service.spreadsheets()
-            .values()
-            .append(
-                spreadsheetId=sheet_id,
-                range=sheet_range,
-                body=resource,
-                valueInputOption=value_input_option,
-            )
-            .execute()
-        )
-
-    @keyword(tags=["sheets"])
-    def update_sheet_values(
-        self,
-        sheet_id: str,
-        sheet_range: str,
-        values: list,
-        major_dimension: str = "COLUMNS",
-        value_input_option: str = "USER_ENTERED",
-    ) -> Dict:
-        """Insert values into sheet cells
-
-        :param sheet_id: target sheet
-        :param sheet_range: target sheet range
-        :param values: list of values to insert into sheet
-        :param major_dimension: major dimension of the values, default `COLUMNS`
-        :param value_input_option: controls whether input strings are parsed or not,
-         default `USER_ENTERED`
-        :return: operation result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${row}  Evaluate   [[22, 33 ,44]]
-            ${result}=  Update Sheet Values  ${SHEET_ID}  A6:C6  ${row}   ROWS
-        """
-        resource = {"majorDimension": major_dimension, "values": values}
-        return (
-            self.service.spreadsheets()
-            .values()
-            .update(
-                spreadsheetId=sheet_id,
-                range=sheet_range,
-                body=resource,
-                valueInputOption=value_input_option,
-            )
-            .execute()
-        )
-
-    @keyword(tags=["sheets"])
-    def get_sheet_values(
-        self,
-        sheet_id: str,
-        sheet_range: str,
-        value_render_option: str = "UNFORMATTED_VALUE",
-        datetime_render_option: str = "FORMATTED_STRING",
-    ) -> List:
-        """Get values from the range in the sheet
-
-        :param sheet_id: target sheet
-        :param sheet_range: target sheet range
-        :param value_render_option: how values should be represented
-         in the output defaults to "UNFORMATTED_VALUE"
-        :param datetime_render_option: how dates, times, and durations should be
-         represented in the output, defaults to "FORMATTED_STRING"
-        :return: operation result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${values}=  Get Sheet Values  ${SHEET_ID}  A1:C1
-        """  # noqa: E501
-        return (
-            self.service.spreadsheets()
-            .values()
-            .get(
-                spreadsheetId=sheet_id,
-                range=sheet_range,
-                valueRenderOption=value_render_option,
-                dateTimeRenderOption=datetime_render_option,
-            )
-            .execute()
-        )
-
-    @keyword(tags=["sheets"])
-    def clear_sheet_values(self, sheet_id: str, sheet_range: str) -> Dict:
-        """Clear cell values for range of cells within a sheet
-
-        :param sheet_id: target sheet
-        :param sheet_range: target sheet range
-        :return: operation result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=  Clear Sheet Values  ${SHEET_ID}  A1:C1
-        """
-        return (
-            self.service.spreadsheets()
-            .values()
-            .clear(
-                spreadsheetId=sheet_id,
-                range=sheet_range,
-            )
-            .execute()
-        )
-
-    @keyword(tags=["sheets"])
-    def copy_sheet(self, sheet_id: str, target_sheet_id: str) -> Dict:
-        """Copy spreadsheet to target spreadsheet
-
-        *NOTE:* service account user must have access to
-        target sheet also
-
-        :param sheet_id: ID of the sheet to copy
-        :param target_sheet_id: ID of the target sheet
-        :return: operation result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=  Copy Sheet   ${SHEET_ID}  ${NEW_SHEET}
-        """
-        body = {
-            "destination_spreadsheet_id": target_sheet_id,
-        }
-        return (
-            self.service.spreadsheets()
-            .sheets()
-            .copyTo(
-                spreadsheetId=sheet_id,
-                sheetId=0,
-                body=body,
-            )
-            .execute()
-        )
+from typing import Dict, List, Optional
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+
+class SheetsKeywords(LibraryContext):
+    """Keywords for Google Sheets operations"""
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "sheets"])
+    def init_sheets(
+        self,
+        service_account: str = None,
+        credentials: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        scopes: list = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Sheets client
+
+        :param service_account: file path to service account file
+        :param credentials: file path to credentials file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param scopes: list of extra authentication scopes
+        :param token_file: file path to token file
+        """
+        sheets_scopes = ["drive", "drive.file", "spreadsheets"]
+        if scopes:
+            sheets_scopes += scopes
+        self.service = self.init_service(
+            service_name="sheets",
+            api_version="v4",
+            scopes=sheets_scopes,
+            service_account_file=service_account,
+            credentials_file=credentials,
+            use_robocorp_vault=use_robocorp_vault,
+            token_file=token_file,
+        )
+
+    @keyword(tags=["sheets"])
+    def create_sheet(self, title: str) -> str:
+        """Create empty sheet with a title
+
+        :param title: name as string
+        :return: created `sheet_id`
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=  Create Sheet   Example Sheet
+        """
+        if not title:
+            raise KeyError("title is required for kw: create_sheet")
+
+        data = {"properties": {"title": title}}
+        spreadsheet = (
+            self.service.spreadsheets()
+            .create(body=data, fields="spreadsheetId")
+            .execute()
+        )
+        return spreadsheet.get("spreadsheetId")
+
+    @keyword(tags=["sheets"])
+    def insert_sheet_values(
+        self,
+        sheet_id: str,
+        sheet_range: str,
+        values: list,
+        major_dimension: str = "COLUMNS",
+        value_input_option: str = "USER_ENTERED",
+    ) -> Dict:
+        """Insert values into sheet cells
+
+        :param sheet_id: target sheet
+        :param sheet_range: target sheet range
+        :param values: list of values to insert into sheet
+        :param major_dimension: major dimension of the values, default `COLUMNS`
+        :param value_input_option: controls whether input strings are parsed or not,
+         default `USER_ENTERED`
+        :return: operation result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${values}   Evaluate   [[11, 12, 13], ['aa', 'bb', 'cc']]
+            ${result}=  Insert Sheet Values   ${SHEET_ID}  A:B  ${values}
+            ${result}=  Insert Sheet Values   ${SHEET_ID}  A:B  ${values}  ROWS
+        """
+        resource = {"majorDimension": major_dimension, "values": values}
+        return (
+            self.service.spreadsheets()
+            .values()
+            .append(
+                spreadsheetId=sheet_id,
+                range=sheet_range,
+                body=resource,
+                valueInputOption=value_input_option,
+            )
+            .execute()
+        )
+
+    @keyword(tags=["sheets"])
+    def update_sheet_values(
+        self,
+        sheet_id: str,
+        sheet_range: str,
+        values: list,
+        major_dimension: str = "COLUMNS",
+        value_input_option: str = "USER_ENTERED",
+    ) -> Dict:
+        """Insert values into sheet cells
+
+        :param sheet_id: target sheet
+        :param sheet_range: target sheet range
+        :param values: list of values to insert into sheet
+        :param major_dimension: major dimension of the values, default `COLUMNS`
+        :param value_input_option: controls whether input strings are parsed or not,
+         default `USER_ENTERED`
+        :return: operation result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${row}  Evaluate   [[22, 33 ,44]]
+            ${result}=  Update Sheet Values  ${SHEET_ID}  A6:C6  ${row}   ROWS
+        """
+        resource = {"majorDimension": major_dimension, "values": values}
+        return (
+            self.service.spreadsheets()
+            .values()
+            .update(
+                spreadsheetId=sheet_id,
+                range=sheet_range,
+                body=resource,
+                valueInputOption=value_input_option,
+            )
+            .execute()
+        )
+
+    @keyword(tags=["sheets"])
+    def get_sheet_values(
+        self,
+        sheet_id: str,
+        sheet_range: str,
+        value_render_option: str = "UNFORMATTED_VALUE",
+        datetime_render_option: str = "FORMATTED_STRING",
+    ) -> List:
+        """Get values from the range in the sheet
+
+        :param sheet_id: target sheet
+        :param sheet_range: target sheet range
+        :param value_render_option: how values should be represented
+         in the output defaults to "UNFORMATTED_VALUE"
+        :param datetime_render_option: how dates, times, and durations should be
+         represented in the output, defaults to "FORMATTED_STRING"
+        :return: operation result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${values}=  Get Sheet Values  ${SHEET_ID}  A1:C1
+        """  # noqa: E501
+        return (
+            self.service.spreadsheets()
+            .values()
+            .get(
+                spreadsheetId=sheet_id,
+                range=sheet_range,
+                valueRenderOption=value_render_option,
+                dateTimeRenderOption=datetime_render_option,
+            )
+            .execute()
+        )
+
+    @keyword(tags=["sheets"])
+    def clear_sheet_values(self, sheet_id: str, sheet_range: str) -> Dict:
+        """Clear cell values for range of cells within a sheet
+
+        :param sheet_id: target sheet
+        :param sheet_range: target sheet range
+        :return: operation result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=  Clear Sheet Values  ${SHEET_ID}  A1:C1
+        """
+        return (
+            self.service.spreadsheets()
+            .values()
+            .clear(
+                spreadsheetId=sheet_id,
+                range=sheet_range,
+            )
+            .execute()
+        )
+
+    @keyword(tags=["sheets"])
+    def copy_sheet(self, sheet_id: str, target_sheet_id: str) -> Dict:
+        """Copy spreadsheet to target spreadsheet
+
+        *NOTE:* service account user must have access to
+        target sheet also
+
+        :param sheet_id: ID of the sheet to copy
+        :param target_sheet_id: ID of the target sheet
+        :return: operation result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=  Copy Sheet   ${SHEET_ID}  ${NEW_SHEET}
+        """
+        body = {
+            "destination_spreadsheet_id": target_sheet_id,
+        }
+        return (
+            self.service.spreadsheets()
+            .sheets()
+            .copyTo(
+                spreadsheetId=sheet_id,
+                sheetId=0,
+                body=body,
+            )
+            .execute()
+        )
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/speech_to_text.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/speech_to_text.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from typing import Dict, Optional
-from google.cloud import speech
-from google.cloud.speech_v1.types import RecognitionConfig, RecognitionAudio
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-ENCODING = {
-    "AMR": RecognitionConfig.AudioEncoding.AMR,
-    "AMR_WB": RecognitionConfig.AudioEncoding.AMR_WB,
-    "FLAC": RecognitionConfig.AudioEncoding.FLAC,
-    "LINEAR16": RecognitionConfig.AudioEncoding.LINEAR16,
-    "MULAW": RecognitionConfig.AudioEncoding.MULAW,
-    "OGG": RecognitionConfig.AudioEncoding.OGG_OPUS,
-    "SPEEX": RecognitionConfig.AudioEncoding.SPEEX_WITH_HEADER_BYTE,  # noqa: E501 # pylint: disable=C0301
-    "UNSPECIFIED": RecognitionConfig.AudioEncoding.ENCODING_UNSPECIFIED,  # noqa: E501 # pylint: disable=C0301
-}
-
-
-class SpeechToTextKeywords(LibraryContext):
-    """Class for Google Cloud Speech-To-Text API
-
-    Possible input audio encodings:
-
-    - 'AMR'
-    - 'AMR_WB'
-    - 'ENCODING_UNSPECIFIED'
-    - 'FLAC'
-    - 'LINEAR16'
-    - 'MULAW'
-    - 'OGG_OPUS'
-    - 'SPEEX_WITH_HEADER_BYTE'
-
-    Link to `Speech To Text PyPI`_ page.
-
-    .. _Speech To Text PyPI: https://pypi.org/project/google-cloud-speech/
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "speech to text"])
-    def init_speech_to_text(
-        self,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Speech to Text client
-
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.service = self.init_service_with_object(
-            speech.SpeechClient, service_account, use_robocorp_vault, token_file
-        )
-
-    @keyword(tags=["speech to text"])
-    def recognize_text_from_audio(
-        self,
-        audio_file: str = None,
-        audio_uri: str = None,
-        encoding: str = None,
-        language_code: str = "en_US",
-        audio_channel_count: int = 2,
-        sample_rate: int = None,
-    ) -> Dict:
-        """Recognize text in the audio file
-
-        :param audio_file: local audio file path
-        :param audio_uri: Google Cloud Storage URI
-        :param encoding: audio file encoding
-        :param language_code: language in the audio
-        :param audio_channel_count: number of audio channel
-        :param sample_rate: rate in hertz, for example 16000
-        :return: recognized texts
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=  Recognize Text From Audio   audio_file=${CURDIR}${/}test.mp3
-        """
-        audio = self.set_audio_type(audio_file, audio_uri)
-        parameters = {"use_enhanced": True}
-        # audio_encoding = ENCODING["UNSPECIFIED"]
-        if encoding and encoding.upper() in ENCODING.keys():
-            parameters["encoding"] = ENCODING[encoding.upper()]
-        if sample_rate:
-            parameters["sample_rate_hertz"] = sample_rate
-        if language_code:
-            parameters["language_code"] = language_code
-        if audio_channel_count:
-            parameters["audio_channel_count"] = audio_channel_count
-        config = RecognitionConfig(**parameters)  # pylint: disable=E1101
-        rec = self.service.recognize(config=config, audio=audio)
-        return rec.results
-
-    def set_audio_type(self, audio_file, audio_uri):
-        # flac or wav, does not require encoding type
-        if audio_file:
-            with open(audio_file, "rb") as f:
-                content = f.read()
-                return RecognitionAudio(content=content)  # pylint: disable=E1101
-        elif audio_uri:
-            return RecognitionAudio(uri=audio_uri)  # pylint: disable=E1101
-        else:
-            raise KeyError("'audio_file' or 'audio_uri' is required")
+from typing import Dict, Optional
+from google.cloud import speech
+from google.cloud.speech_v1.types import RecognitionConfig, RecognitionAudio
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+ENCODING = {
+    "AMR": RecognitionConfig.AudioEncoding.AMR,
+    "AMR_WB": RecognitionConfig.AudioEncoding.AMR_WB,
+    "FLAC": RecognitionConfig.AudioEncoding.FLAC,
+    "LINEAR16": RecognitionConfig.AudioEncoding.LINEAR16,
+    "MULAW": RecognitionConfig.AudioEncoding.MULAW,
+    "OGG": RecognitionConfig.AudioEncoding.OGG_OPUS,
+    "SPEEX": RecognitionConfig.AudioEncoding.SPEEX_WITH_HEADER_BYTE,  # noqa: E501 # pylint: disable=C0301
+    "UNSPECIFIED": RecognitionConfig.AudioEncoding.ENCODING_UNSPECIFIED,  # noqa: E501 # pylint: disable=C0301
+}
+
+
+class SpeechToTextKeywords(LibraryContext):
+    """Class for Google Cloud Speech-To-Text API
+
+    Possible input audio encodings:
+
+    - 'AMR'
+    - 'AMR_WB'
+    - 'ENCODING_UNSPECIFIED'
+    - 'FLAC'
+    - 'LINEAR16'
+    - 'MULAW'
+    - 'OGG_OPUS'
+    - 'SPEEX_WITH_HEADER_BYTE'
+
+    Link to `Speech To Text PyPI`_ page.
+
+    .. _Speech To Text PyPI: https://pypi.org/project/google-cloud-speech/
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "speech to text"])
+    def init_speech_to_text(
+        self,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Speech to Text client
+
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.service = self.init_service_with_object(
+            speech.SpeechClient, service_account, use_robocorp_vault, token_file
+        )
+
+    @keyword(tags=["speech to text"])
+    def recognize_text_from_audio(
+        self,
+        audio_file: str = None,
+        audio_uri: str = None,
+        encoding: str = None,
+        language_code: str = "en_US",
+        audio_channel_count: int = 2,
+        sample_rate: int = None,
+    ) -> Dict:
+        """Recognize text in the audio file
+
+        :param audio_file: local audio file path
+        :param audio_uri: Google Cloud Storage URI
+        :param encoding: audio file encoding
+        :param language_code: language in the audio
+        :param audio_channel_count: number of audio channel
+        :param sample_rate: rate in hertz, for example 16000
+        :return: recognized texts
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=  Recognize Text From Audio   audio_file=${CURDIR}${/}test.mp3
+        """
+        audio = self.set_audio_type(audio_file, audio_uri)
+        parameters = {"use_enhanced": True}
+        # audio_encoding = ENCODING["UNSPECIFIED"]
+        if encoding and encoding.upper() in ENCODING.keys():
+            parameters["encoding"] = ENCODING[encoding.upper()]
+        if sample_rate:
+            parameters["sample_rate_hertz"] = sample_rate
+        if language_code:
+            parameters["language_code"] = language_code
+        if audio_channel_count:
+            parameters["audio_channel_count"] = audio_channel_count
+        config = RecognitionConfig(**parameters)  # pylint: disable=E1101
+        rec = self.service.recognize(config=config, audio=audio)
+        return rec.results
+
+    def set_audio_type(self, audio_file, audio_uri):
+        # flac or wav, does not require encoding type
+        if audio_file:
+            with open(audio_file, "rb") as f:
+                content = f.read()
+                return RecognitionAudio(content=content)  # pylint: disable=E1101
+        elif audio_uri:
+            return RecognitionAudio(uri=audio_uri)  # pylint: disable=E1101
+        else:
+            raise KeyError("'audio_file' or 'audio_uri' is required")
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/storage.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/storage.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,277 +1,277 @@
-from typing import Any, Dict, List, Optional
-
-from google.cloud import storage
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-
-class StorageKeywords(LibraryContext):
-    """Class for Google Cloud Storage API
-     and Google Cloud Storage JSON API
-
-    Link to `Google Storage PyPI`_ page.
-
-    .. _Google Storage PyPI: https://pypi.org/project/google-cloud-storage/
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "storage"])
-    def init_storage(
-        self,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Storage client
-
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.service = self.init_service_with_object(
-            storage.Client, service_account, use_robocorp_vault, token_file
-        )
-
-    @keyword(tags=["storage"])
-    def create_storage_bucket(self, bucket_name: str) -> Dict:
-        """Create Google Cloud Storage bucket
-
-        :param bucket_name: name as string
-        :return: bucket
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Create Storage Bucket   visionfolder
-        """
-        bucket = self.service.create_bucket(bucket_name)
-        return bucket
-
-    @keyword(tags=["storage"])
-    def delete_storage_bucket(self, bucket_name: str):
-        """Delete Google Cloud Storage bucket
-
-        Bucket needs to be empty before it can be deleted.
-
-        :param bucket_name: name as string
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Delete Storage Bucket   visionfolder
-        """
-        bucket = self.get_storage_bucket(bucket_name)
-        try:
-            bucket.delete()
-        except Exception as e:
-            raise ValueError("The bucket you tried to delete was not empty") from e
-
-    @keyword(tags=["storage"])
-    def get_storage_bucket(self, bucket_name: str) -> Dict:
-        """Get Google Cloud Storage bucket
-
-        :param bucket_name: name as string
-        :return: bucket
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Get Bucket   visionfolder
-        """
-        bucket = self.service.get_bucket(bucket_name)
-        return bucket
-
-    @keyword(tags=["storage"])
-    def list_storage_buckets(self) -> List:
-        """List Google Cloud Storage buckets
-
-        :return: list of buckets
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${buckets}=   List Storage Buckets
-            FOR  ${bucket}  IN   @{buckets}
-                Log  ${bucket}
-            END
-        """
-        return list(self.service.list_buckets())
-
-    @keyword(tags=["storage"])
-    def delete_storage_files(self, bucket_name: str, files: Any) -> List:
-        """Delete files in the bucket
-
-        Files need to be object name in the bucket.
-
-        :param bucket_name: name as string
-        :param files: single file, list of files or comma separated list of files
-        :return: list of files which could not be deleted
-
-         **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Delete Storage Files   ${BUCKET_NAME}   file1,file2
-        """
-        if not isinstance(files, list):
-            files = files.split(",")
-        bucket = self.get_storage_bucket(bucket_name)
-        notfound = []
-        for filename in files:
-            filename = filename.strip()
-            blob = bucket.get_blob(filename)
-            if blob:
-                blob.delete()
-            else:
-                notfound.append(filename)
-        return notfound if len(notfound) > 0 else True
-
-    @keyword(tags=["storage"])
-    def list_storage_files(self, bucket_name: str) -> List:
-        """List files in the bucket
-
-        :param bucket_name: name as string
-        :return: list of object names in the bucket
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${files}=   List Storage Files  ${BUCKET_NAME}
-            FOR  ${bucket}  IN   @{files}
-                Log  ${file}
-            END
-        """
-        bucket = self.get_storage_bucket(bucket_name)
-        all_blobs = bucket.list_blobs()
-        sorted_blobs = sorted(blob.name for blob in all_blobs)
-        return [
-            {"name": name, "uri": f"gs://{bucket_name}/{name}"} for name in sorted_blobs
-        ]
-
-    @keyword(tags=["storage"])
-    def upload_storage_file(
-        self, bucket_name: str, filename: str, target_name: str
-    ) -> None:
-        """Upload a file into a bucket
-
-        :param bucket_name: name as string
-        :param filename: filepath to upload file
-        :param target_name: target object name
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            Upload Storage File  ${BUCKET_NAME}
-            ...   ${CURDIR}${/}test.txt    test.txt
-        """
-        bucket = self.get_storage_bucket(bucket_name)
-        blob = bucket.blob(target_name)
-        with open(filename, "rb") as f:
-            blob.upload_from_file(f)
-
-    @keyword(tags=["storage"])
-    def upload_storage_files(self, bucket_name: str, files: dict) -> None:
-        """Upload files into a bucket
-
-        Example `files`:
-        files = {"mytestimg": "image1.png", "mydoc": "google.pdf"}
-
-        :param bucket_name: name as string
-        :param files: dictionary of object names and filepaths
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${files}=   Create Dictionary
-            ...   test1.txt   ${CURDIR}${/}test1.txt
-            ...   test2.txt   ${CURDIR}${/}test2.txt
-            Upload Storage Files   ${BUCKET_NAME}   ${files}
-        """
-        if not isinstance(files, dict):
-            raise ValueError("files needs to be an dictionary")
-        bucket = self.get_storage_bucket(bucket_name)
-        for target_name, filename in files.items():
-            blob = bucket.blob(target_name)
-            blob.upload_from_filename(filename)
-
-    @keyword(tags=["storage"])
-    def download_storage_files(self, bucket_name: str, files: Any) -> List:
-        """Download files from a bucket
-
-        Example `files`:
-        files = {"mytestimg": "image1.png", "mydoc": "google.pdf"}
-
-        :param bucket_name: name as string
-        :param files: list of object names or dictionary of
-            object names and target files
-        :return: list of files which could not be downloaded
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=  Download Storage Files  ${BUCKET_NAME}   test1.txt,test2.txt
-        """
-        if isinstance(files, str):
-            files = files.split(",")
-        bucket = self.get_storage_bucket(bucket_name)
-        notfound = []
-        if isinstance(files, dict):
-            for object_name, filename in files.items():
-                blob = bucket.get_blob(object_name)
-                if blob:
-                    with open(filename, "wb") as f:
-                        blob.download_to_file(f)
-                        self.logger.info(
-                            "Downloaded object %s from Google to filepath %s",
-                            object_name,
-                            filename,
-                        )
-                else:
-                    notfound.append(object_name)
-        else:
-            for filename in files:
-                filename = filename.strip()
-                blob = bucket.get_blob(filename)
-                if blob:
-                    with open(filename, "wb") as f:
-                        blob.download_to_file(f)
-                        self.logger.info(
-                            "Downloaded object %s from Google to filepath %s",
-                            filename,
-                            filename,
-                        )
-                else:
-                    notfound.append(filename)
-        return notfound
+from typing import Any, Dict, List, Optional
+
+from google.cloud import storage
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+
+class StorageKeywords(LibraryContext):
+    """Class for Google Cloud Storage API
+     and Google Cloud Storage JSON API
+
+    Link to `Google Storage PyPI`_ page.
+
+    .. _Google Storage PyPI: https://pypi.org/project/google-cloud-storage/
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "storage"])
+    def init_storage(
+        self,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Storage client
+
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.service = self.init_service_with_object(
+            storage.Client, service_account, use_robocorp_vault, token_file
+        )
+
+    @keyword(tags=["storage"])
+    def create_storage_bucket(self, bucket_name: str) -> Dict:
+        """Create Google Cloud Storage bucket
+
+        :param bucket_name: name as string
+        :return: bucket
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Create Storage Bucket   visionfolder
+        """
+        bucket = self.service.create_bucket(bucket_name)
+        return bucket
+
+    @keyword(tags=["storage"])
+    def delete_storage_bucket(self, bucket_name: str):
+        """Delete Google Cloud Storage bucket
+
+        Bucket needs to be empty before it can be deleted.
+
+        :param bucket_name: name as string
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Delete Storage Bucket   visionfolder
+        """
+        bucket = self.get_storage_bucket(bucket_name)
+        try:
+            bucket.delete()
+        except Exception as e:
+            raise ValueError("The bucket you tried to delete was not empty") from e
+
+    @keyword(tags=["storage"])
+    def get_storage_bucket(self, bucket_name: str) -> Dict:
+        """Get Google Cloud Storage bucket
+
+        :param bucket_name: name as string
+        :return: bucket
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Get Bucket   visionfolder
+        """
+        bucket = self.service.get_bucket(bucket_name)
+        return bucket
+
+    @keyword(tags=["storage"])
+    def list_storage_buckets(self) -> List:
+        """List Google Cloud Storage buckets
+
+        :return: list of buckets
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${buckets}=   List Storage Buckets
+            FOR  ${bucket}  IN   @{buckets}
+                Log  ${bucket}
+            END
+        """
+        return list(self.service.list_buckets())
+
+    @keyword(tags=["storage"])
+    def delete_storage_files(self, bucket_name: str, files: Any) -> List:
+        """Delete files in the bucket
+
+        Files need to be object name in the bucket.
+
+        :param bucket_name: name as string
+        :param files: single file, list of files or comma separated list of files
+        :return: list of files which could not be deleted
+
+         **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Delete Storage Files   ${BUCKET_NAME}   file1,file2
+        """
+        if not isinstance(files, list):
+            files = files.split(",")
+        bucket = self.get_storage_bucket(bucket_name)
+        notfound = []
+        for filename in files:
+            filename = filename.strip()
+            blob = bucket.get_blob(filename)
+            if blob:
+                blob.delete()
+            else:
+                notfound.append(filename)
+        return notfound if len(notfound) > 0 else True
+
+    @keyword(tags=["storage"])
+    def list_storage_files(self, bucket_name: str) -> List:
+        """List files in the bucket
+
+        :param bucket_name: name as string
+        :return: list of object names in the bucket
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${files}=   List Storage Files  ${BUCKET_NAME}
+            FOR  ${bucket}  IN   @{files}
+                Log  ${file}
+            END
+        """
+        bucket = self.get_storage_bucket(bucket_name)
+        all_blobs = bucket.list_blobs()
+        sorted_blobs = sorted(blob.name for blob in all_blobs)
+        return [
+            {"name": name, "uri": f"gs://{bucket_name}/{name}"} for name in sorted_blobs
+        ]
+
+    @keyword(tags=["storage"])
+    def upload_storage_file(
+        self, bucket_name: str, filename: str, target_name: str
+    ) -> None:
+        """Upload a file into a bucket
+
+        :param bucket_name: name as string
+        :param filename: filepath to upload file
+        :param target_name: target object name
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            Upload Storage File  ${BUCKET_NAME}
+            ...   ${CURDIR}${/}test.txt    test.txt
+        """
+        bucket = self.get_storage_bucket(bucket_name)
+        blob = bucket.blob(target_name)
+        with open(filename, "rb") as f:
+            blob.upload_from_file(f)
+
+    @keyword(tags=["storage"])
+    def upload_storage_files(self, bucket_name: str, files: dict) -> None:
+        """Upload files into a bucket
+
+        Example `files`:
+        files = {"mytestimg": "image1.png", "mydoc": "google.pdf"}
+
+        :param bucket_name: name as string
+        :param files: dictionary of object names and filepaths
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${files}=   Create Dictionary
+            ...   test1.txt   ${CURDIR}${/}test1.txt
+            ...   test2.txt   ${CURDIR}${/}test2.txt
+            Upload Storage Files   ${BUCKET_NAME}   ${files}
+        """
+        if not isinstance(files, dict):
+            raise ValueError("files needs to be an dictionary")
+        bucket = self.get_storage_bucket(bucket_name)
+        for target_name, filename in files.items():
+            blob = bucket.blob(target_name)
+            blob.upload_from_filename(filename)
+
+    @keyword(tags=["storage"])
+    def download_storage_files(self, bucket_name: str, files: Any) -> List:
+        """Download files from a bucket
+
+        Example `files`:
+        files = {"mytestimg": "image1.png", "mydoc": "google.pdf"}
+
+        :param bucket_name: name as string
+        :param files: list of object names or dictionary of
+            object names and target files
+        :return: list of files which could not be downloaded
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=  Download Storage Files  ${BUCKET_NAME}   test1.txt,test2.txt
+        """
+        if isinstance(files, str):
+            files = files.split(",")
+        bucket = self.get_storage_bucket(bucket_name)
+        notfound = []
+        if isinstance(files, dict):
+            for object_name, filename in files.items():
+                blob = bucket.get_blob(object_name)
+                if blob:
+                    with open(filename, "wb") as f:
+                        blob.download_to_file(f)
+                        self.logger.info(
+                            "Downloaded object %s from Google to filepath %s",
+                            object_name,
+                            filename,
+                        )
+                else:
+                    notfound.append(object_name)
+        else:
+            for filename in files:
+                filename = filename.strip()
+                blob = bucket.get_blob(filename)
+                if blob:
+                    with open(filename, "wb") as f:
+                        blob.download_to_file(f)
+                        self.logger.info(
+                            "Downloaded object %s from Google to filepath %s",
+                            filename,
+                            filename,
+                        )
+                else:
+                    notfound.append(filename)
+        return notfound
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/text_to_speech.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/text_to_speech.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from typing import List, Optional
-
-from google.cloud import texttospeech_v1
-from google.cloud.texttospeech_v1.types import (
-    AudioConfig,
-    VoiceSelectionParams,
-    SynthesisInput,
-)
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-
-class TextToSpeechKeywords(LibraryContext):
-    """Class for Google Cloud Text-to-Speech API
-
-    Link to `Text To Speech PyPI`_ page.
-
-    .. _Text To Speech PyPI: https://pypi.org/project/google-cloud-texttospeech/
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "text to speech"])
-    def init_text_to_speech(
-        self,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Text to Speech client
-
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.service = self.init_service_with_object(
-            texttospeech_v1.TextToSpeechClient,
-            service_account,
-            use_robocorp_vault,
-            token_file,
-        )
-
-    @keyword(tags=["text to speech"])
-    def list_supported_voices(self, language_code: str = None) -> List:
-        """List supported voices for the speech
-
-        :param language_code: voice languages to list, defaults to None (all)
-        :return: list of supported voices
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   List Supported Voices   en-US
-        """
-        if language_code:
-            voices = self.service.list_voices(language_code)
-        else:
-            voices = self.service.list_voices()
-        return voices.voices
-
-    @keyword(tags=["text to speech"])
-    def synthesize_speech(
-        self,
-        text: str,
-        language: str = "en-US",
-        name: str = "en-US-Standard-B",
-        gender: str = "MALE",
-        encoding: str = "MP3",
-        target_file: str = "synthesized.mp3",
-    ) -> List:
-        """Synthesize speech synchronously
-
-        :param text: input text to synthesize
-        :param language: voice language, defaults to "en-US"
-        :param name: voice name, defaults to "en-US-Standard-B"
-        :param gender: voice gender, defaults to "MALE"
-        :param encoding: result encoding type, defaults to "MP3"
-        :param target_file: save synthesized output to file,
-            defaults to "synthesized.mp3"
-        :return: synthesized output in bytes
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Synthesize Speech   ${text}
-        """
-        synth_input = SynthesisInput(text=text)
-        voice_selection = VoiceSelectionParams(
-            language_code=language, name=name, ssml_gender=gender
-        )
-        audio_config = AudioConfig(audio_encoding=encoding)
-        response = self.service.synthesize_speech(
-            request={
-                "input": synth_input,
-                "voice": voice_selection,
-                "audio_config": audio_config,
-            }
-        )
-        if target_file:
-            with open(target_file, "wb") as f:
-                f.write(response.audio_content)
-        return response.audio_content
+from typing import List, Optional
+
+from google.cloud import texttospeech_v1
+from google.cloud.texttospeech_v1.types import (
+    AudioConfig,
+    VoiceSelectionParams,
+    SynthesisInput,
+)
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+
+class TextToSpeechKeywords(LibraryContext):
+    """Class for Google Cloud Text-to-Speech API
+
+    Link to `Text To Speech PyPI`_ page.
+
+    .. _Text To Speech PyPI: https://pypi.org/project/google-cloud-texttospeech/
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "text to speech"])
+    def init_text_to_speech(
+        self,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Text to Speech client
+
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.service = self.init_service_with_object(
+            texttospeech_v1.TextToSpeechClient,
+            service_account,
+            use_robocorp_vault,
+            token_file,
+        )
+
+    @keyword(tags=["text to speech"])
+    def list_supported_voices(self, language_code: str = None) -> List:
+        """List supported voices for the speech
+
+        :param language_code: voice languages to list, defaults to None (all)
+        :return: list of supported voices
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   List Supported Voices   en-US
+        """
+        if language_code:
+            voices = self.service.list_voices(language_code)
+        else:
+            voices = self.service.list_voices()
+        return voices.voices
+
+    @keyword(tags=["text to speech"])
+    def synthesize_speech(
+        self,
+        text: str,
+        language: str = "en-US",
+        name: str = "en-US-Standard-B",
+        gender: str = "MALE",
+        encoding: str = "MP3",
+        target_file: str = "synthesized.mp3",
+    ) -> List:
+        """Synthesize speech synchronously
+
+        :param text: input text to synthesize
+        :param language: voice language, defaults to "en-US"
+        :param name: voice name, defaults to "en-US-Standard-B"
+        :param gender: voice gender, defaults to "MALE"
+        :param encoding: result encoding type, defaults to "MP3"
+        :param target_file: save synthesized output to file,
+            defaults to "synthesized.mp3"
+        :return: synthesized output in bytes
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Synthesize Speech   ${text}
+        """
+        synth_input = SynthesisInput(text=text)
+        voice_selection = VoiceSelectionParams(
+            language_code=language, name=name, ssml_gender=gender
+        )
+        audio_config = AudioConfig(audio_encoding=encoding)
+        response = self.service.synthesize_speech(
+            request={
+                "input": synth_input,
+                "voice": voice_selection,
+                "audio_config": audio_config,
+            }
+        )
+        if target_file:
+            with open(target_file, "wb") as f:
+                f.write(response.audio_content)
+        return response.audio_content
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/translation.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/translation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import Dict, Union, Optional
-
-from google.cloud import translate_v3
-
-from . import LibraryContext, keyword, TextType, to_texttype
-
-
-class TranslationKeywords(LibraryContext):
-    """Class for Google Cloud Translation API
-
-    Link to `Translation PyPI`_ page.
-
-    .. _Translation PyPI: https://pypi.org/project/google-cloud-translate/
-    """
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-        self.project_id = None
-
-    @keyword(tags=["init", "translation"])
-    def init_translation(
-        self,
-        project_identifier: str,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Translation client
-
-        :param project_identifier: identifier for Translation project
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.project_id = project_identifier
-        self.service = self.init_service_with_object(
-            translate_v3.TranslationServiceClient,
-            service_account,
-            use_robocorp_vault,
-            token_file,
-        )
-
-    @keyword(tags=["translation"])
-    def translate(
-        self,
-        text: Union[list, str],
-        source_language: str = None,
-        target_language: str = None,
-        mime_type: TextType = None,
-    ) -> Dict:
-        """Translate text
-
-        :param text: text to translate
-        :param source_language: language code
-        :param target_language: language code
-        :param mime_type: text or html
-        :return: translated text
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Translate   ${TEXT}  target_language=de
-        """
-        if not text and not target_language:
-            raise KeyError("text and target_language are required parameters")
-        parent = f"projects/{self.project_id}"
-        contents = [text] if not isinstance(text, list) else text
-
-        parameters = {"parent": parent, "contents": contents}
-        if source_language:
-            parameters["source_language_code"] = source_language
-        if target_language:
-            parameters["target_language_code"] = target_language
-        if mime_type:
-            mimetype = to_texttype(mime_type)
-            parameters["mime_type"] = mimetype
-        response = self.service.translate_text(**parameters)
-        return response
+from typing import Dict, Union, Optional
+
+from google.cloud import translate_v3
+
+from . import LibraryContext, keyword, TextType, to_texttype
+
+
+class TranslationKeywords(LibraryContext):
+    """Class for Google Cloud Translation API
+
+    Link to `Translation PyPI`_ page.
+
+    .. _Translation PyPI: https://pypi.org/project/google-cloud-translate/
+    """
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+        self.project_id = None
+
+    @keyword(tags=["init", "translation"])
+    def init_translation(
+        self,
+        project_identifier: str,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Translation client
+
+        :param project_identifier: identifier for Translation project
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.project_id = project_identifier
+        self.service = self.init_service_with_object(
+            translate_v3.TranslationServiceClient,
+            service_account,
+            use_robocorp_vault,
+            token_file,
+        )
+
+    @keyword(tags=["translation"])
+    def translate(
+        self,
+        text: Union[list, str],
+        source_language: str = None,
+        target_language: str = None,
+        mime_type: TextType = None,
+    ) -> Dict:
+        """Translate text
+
+        :param text: text to translate
+        :param source_language: language code
+        :param target_language: language code
+        :param mime_type: text or html
+        :return: translated text
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Translate   ${TEXT}  target_language=de
+        """
+        if not text and not target_language:
+            raise KeyError("text and target_language are required parameters")
+        parent = f"projects/{self.project_id}"
+        contents = [text] if not isinstance(text, list) else text
+
+        parameters = {"parent": parent, "contents": contents}
+        if source_language:
+            parameters["source_language_code"] = source_language
+        if target_language:
+            parameters["target_language_code"] = target_language
+        if mime_type:
+            mimetype = to_texttype(mime_type)
+            parameters["mime_type"] = mimetype
+        response = self.service.translate_text(**parameters)
+        return response
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/video_intelligence.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/video_intelligence.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from typing import Dict, Optional
-
-from google.cloud import videointelligence
-
-from . import LibraryContext, keyword, to_feature
-
-
-class VideoIntelligenceKeywords(LibraryContext):
-    """Keywords for Google Video Intelligence API"""
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "video intelligence"])
-    def init_video_intelligence(
-        self,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Video Intelligence client
-
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.service = self.init_service_with_object(
-            videointelligence.VideoIntelligenceServiceClient,
-            service_account,
-            use_robocorp_vault,
-            token_file,
-        )
-
-    @keyword(tags=["video intelligence"])
-    def annotate_video(
-        self,
-        video_file: str = None,
-        video_uri: str = None,
-        features: str = None,
-        output_uri: str = None,
-        json_file: str = None,
-        timeout: int = 300,
-    ) -> Dict:
-        """Annotate video
-
-        Possible values for features:
-
-        - FEATURE_UNSPECIFIED, Unspecified.
-        - LABEL_DETECTION, Label detection. Detect objects, such as dog or flower.
-        - SHOT_CHANGE_DETECTION, Shot change detection.
-        - EXPLICIT_CONTENT_DETECTION, Explicit content detection.
-        - SPEECH_TRANSCRIPTION, Speech transcription.
-        - TEXT_DETECTION, OCR text detection and tracking.
-        - OBJECT_TRACKING, Object detection and tracking.
-        - LOGO_RECOGNITION, Logo detection, tracking, and recognition.
-
-        If `video_uri` is given then that is used even if `video_file` is given.
-
-        :param video_file: local file path to input video
-        :param video_uri: Google Cloud Storage URI to input video
-        :param features: list of annotation features to detect,
-            defaults to LABEL_DETECTION,SHOT_CHANGE_DETECTION
-        :param output_uri: Google Cloud Storage URI to store response json
-        :param json_file: json target to save result
-        :param timeout: timeout for operation in seconds
-        :return: annotate result
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Annotate Video   video_uri=gs://videointelligence/movie.mp4
-            ...  features=TEXT_DETECTION,LABEL_DETECTION
-            ...  output_uri=gs://videointelligence/movie_annotations.json
-            ...  json_file=${CURDIR}${/}videoannotations.json
-        """
-        if features is None:
-            features_in = [
-                videointelligence.Feature.LABEL_DETECTION,
-                videointelligence.Feature.SHOT_CHANGE_DETECTION,
-            ]
-        else:
-            features_in = [to_feature(feature) for feature in features.split(",")]
-        parameters = {"features": features_in}
-        if video_uri:
-            parameters["input_uri"] = video_uri
-        elif video_file:
-            video_context = videointelligence.VideoContext()
-            with open(video_file, "rb") as file:
-                input_content = file.read()
-                parameters["input_content"] = input_content
-                parameters["video_context"] = video_context
-        if output_uri:
-            parameters["output_uri"] = output_uri
-
-        operation = self.service.annotate_video(request=parameters)
-        result = operation.result(timeout=timeout)
-        self.write_json(json_file, result)
-        return result
+from typing import Dict, Optional
+
+from google.cloud import videointelligence
+
+from . import LibraryContext, keyword, to_feature
+
+
+class VideoIntelligenceKeywords(LibraryContext):
+    """Keywords for Google Video Intelligence API"""
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "video intelligence"])
+    def init_video_intelligence(
+        self,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Video Intelligence client
+
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.service = self.init_service_with_object(
+            videointelligence.VideoIntelligenceServiceClient,
+            service_account,
+            use_robocorp_vault,
+            token_file,
+        )
+
+    @keyword(tags=["video intelligence"])
+    def annotate_video(
+        self,
+        video_file: str = None,
+        video_uri: str = None,
+        features: str = None,
+        output_uri: str = None,
+        json_file: str = None,
+        timeout: int = 300,
+    ) -> Dict:
+        """Annotate video
+
+        Possible values for features:
+
+        - FEATURE_UNSPECIFIED, Unspecified.
+        - LABEL_DETECTION, Label detection. Detect objects, such as dog or flower.
+        - SHOT_CHANGE_DETECTION, Shot change detection.
+        - EXPLICIT_CONTENT_DETECTION, Explicit content detection.
+        - SPEECH_TRANSCRIPTION, Speech transcription.
+        - TEXT_DETECTION, OCR text detection and tracking.
+        - OBJECT_TRACKING, Object detection and tracking.
+        - LOGO_RECOGNITION, Logo detection, tracking, and recognition.
+
+        If `video_uri` is given then that is used even if `video_file` is given.
+
+        :param video_file: local file path to input video
+        :param video_uri: Google Cloud Storage URI to input video
+        :param features: list of annotation features to detect,
+            defaults to LABEL_DETECTION,SHOT_CHANGE_DETECTION
+        :param output_uri: Google Cloud Storage URI to store response json
+        :param json_file: json target to save result
+        :param timeout: timeout for operation in seconds
+        :return: annotate result
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Annotate Video   video_uri=gs://videointelligence/movie.mp4
+            ...  features=TEXT_DETECTION,LABEL_DETECTION
+            ...  output_uri=gs://videointelligence/movie_annotations.json
+            ...  json_file=${CURDIR}${/}videoannotations.json
+        """
+        if features is None:
+            features_in = [
+                videointelligence.Feature.LABEL_DETECTION,
+                videointelligence.Feature.SHOT_CHANGE_DETECTION,
+            ]
+        else:
+            features_in = [to_feature(feature) for feature in features.split(",")]
+        parameters = {"features": features_in}
+        if video_uri:
+            parameters["input_uri"] = video_uri
+        elif video_file:
+            video_context = videointelligence.VideoContext()
+            with open(video_file, "rb") as file:
+                input_content = file.read()
+                parameters["input_content"] = input_content
+                parameters["video_context"] = video_context
+        if output_uri:
+            parameters["output_uri"] = output_uri
+
+        operation = self.service.annotate_video(request=parameters)
+        result = operation.result(timeout=timeout)
+        self.write_json(json_file, result)
+        return result
```

### Comparing `rpaframework_google-7.0.2/src/RPA/Cloud/Google/keywords/vision.py` & `rpaframework_google-7.0.3/src/RPA/Cloud/Google/keywords/vision.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-from typing import Dict, Optional
-from google.cloud import vision
-
-from . import (
-    LibraryContext,
-    keyword,
-)
-
-
-class VisionKeywords(LibraryContext):
-    """Keywords for Google Vision operations"""
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-        self.service = None
-
-    @keyword(tags=["init", "vision"])
-    def init_vision(
-        self,
-        service_account: str = None,
-        use_robocorp_vault: Optional[bool] = None,
-        token_file: str = None,
-    ) -> None:
-        """Initialize Google Cloud Vision client
-
-        :param service_account: file path to service account file
-        :param use_robocorp_vault: use credentials in `Robocorp Vault`
-        :param token_file: file path to token file
-        """
-        self.service = self.init_service_with_object(
-            vision.ImageAnnotatorClient,
-            service_account,
-            use_robocorp_vault,
-            token_file,
-        )
-
-    def set_image_type(self, image_file: str = None, image_uri: str = None):
-        if image_file:
-            with open(image_file, "rb") as f:
-                content = f.read()
-                return {"image": {"content": content}}
-        elif image_uri:
-            return {"image": {"source": {"image_uri": image_uri}}}
-        else:
-            raise KeyError("'image_file' or 'image_uri' is required")
-
-    @keyword(tags=["vision"])
-    def detect_labels(
-        self, image_file: str = None, image_uri: str = None, json_file: str = None
-    ) -> Dict:
-        """Detect labels in the image
-
-        :param image_file: source image file path
-        :param image_uri: source image uri
-        :param json_file: json target to save result
-        :return: detection response
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Detect Labels   image_file=${CURDIR}${/}test.png
-            ...  json_file=${CURDIR}${/}result.json
-        """
-        parameters = self.set_image_type(image_file, image_uri)
-        response = self.service.label_detection(**parameters)
-        self.write_json(json_file, response)
-        return response
-
-    @keyword(tags=["vision"])
-    def detect_text(
-        self, image_file: str = None, image_uri: str = None, json_file: str = None
-    ) -> Dict:
-        """Detect text in the image
-
-        :param image_file: source image file path
-        :param image_uri: Google Cloud Storage URI
-        :param json_file: json target to save result
-        :return: detection response
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Detect Text   image_file=${CURDIR}${/}test.png
-            ...  json_file=${CURDIR}${/}result.json
-        """
-        parameters = self.set_image_type(image_file, image_uri)
-        response = self.service.text_detection(**parameters)
-        self.write_json(json_file, response)
-        return response
-
-    @keyword(tags=["vision"])
-    def detect_document(
-        self, image_file: str = None, image_uri: str = None, json_file: str = None
-    ) -> Dict:
-        """Detect document
-
-        :param image_file: source image file path
-        :param image_uri: Google Cloud Storage URI
-        :param json_file: json target to save result
-        :return: detection response
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Detect Document   image_file=${CURDIR}${/}test.png
-            ...  json_file=${CURDIR}${/}result.json
-        """
-        parameters = self.set_image_type(image_file, image_uri)
-        response = self.service.document_text_detection(**parameters)
-        self.write_json(json_file, response)
-        return response
-
-    @keyword(tags=["vision"])
-    def annotate_image(
-        self, image_file: str, image_uri: str, json_file: str = None
-    ) -> Dict:
-        """Annotate image
-
-        :param image_file: source image file path
-        :param image_uri: Google Cloud Storage URI
-        :param json_file: json target to save result
-        :return: detection response
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Annotate Image   image_file=${CURDIR}${/}test.png
-            ...  json_file=${CURDIR}${/}result.json
-        """
-        parameters = self.set_image_type(image_file, image_uri)
-        response = self.service.annotate_image(**parameters)
-        self.write_json(json_file, response)
-        return response
-
-    @keyword(tags=["vision"])
-    def face_detection(
-        self, image_file: str = None, image_uri: str = None, json_file: str = None
-    ) -> Dict:
-        """Detect faces
-
-        :param image_file: source image file path
-        :param image_uri: Google Cloud Storage URI
-        :param json_file: json target to save result
-        :return: detection response
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            ${result}=   Face Detection   image_uri=gs://vision/faces.png
-            ...  json_file=${CURDIR}${/}result.json
-        """
-        parameters = self.set_image_type(image_file, image_uri)
-        response = self.service.face_detection(**parameters)
-        self.write_json(json_file, response)
-        return response
+from typing import Dict, Optional
+from google.cloud import vision
+
+from . import (
+    LibraryContext,
+    keyword,
+)
+
+
+class VisionKeywords(LibraryContext):
+    """Keywords for Google Vision operations"""
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+        self.service = None
+
+    @keyword(tags=["init", "vision"])
+    def init_vision(
+        self,
+        service_account: str = None,
+        use_robocorp_vault: Optional[bool] = None,
+        token_file: str = None,
+    ) -> None:
+        """Initialize Google Cloud Vision client
+
+        :param service_account: file path to service account file
+        :param use_robocorp_vault: use credentials in `Robocorp Vault`
+        :param token_file: file path to token file
+        """
+        self.service = self.init_service_with_object(
+            vision.ImageAnnotatorClient,
+            service_account,
+            use_robocorp_vault,
+            token_file,
+        )
+
+    def set_image_type(self, image_file: str = None, image_uri: str = None):
+        if image_file:
+            with open(image_file, "rb") as f:
+                content = f.read()
+                return {"image": {"content": content}}
+        elif image_uri:
+            return {"image": {"source": {"image_uri": image_uri}}}
+        else:
+            raise KeyError("'image_file' or 'image_uri' is required")
+
+    @keyword(tags=["vision"])
+    def detect_labels(
+        self, image_file: str = None, image_uri: str = None, json_file: str = None
+    ) -> Dict:
+        """Detect labels in the image
+
+        :param image_file: source image file path
+        :param image_uri: source image uri
+        :param json_file: json target to save result
+        :return: detection response
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Detect Labels   image_file=${CURDIR}${/}test.png
+            ...  json_file=${CURDIR}${/}result.json
+        """
+        parameters = self.set_image_type(image_file, image_uri)
+        response = self.service.label_detection(**parameters)
+        self.write_json(json_file, response)
+        return response
+
+    @keyword(tags=["vision"])
+    def detect_text(
+        self, image_file: str = None, image_uri: str = None, json_file: str = None
+    ) -> Dict:
+        """Detect text in the image
+
+        :param image_file: source image file path
+        :param image_uri: Google Cloud Storage URI
+        :param json_file: json target to save result
+        :return: detection response
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Detect Text   image_file=${CURDIR}${/}test.png
+            ...  json_file=${CURDIR}${/}result.json
+        """
+        parameters = self.set_image_type(image_file, image_uri)
+        response = self.service.text_detection(**parameters)
+        self.write_json(json_file, response)
+        return response
+
+    @keyword(tags=["vision"])
+    def detect_document(
+        self, image_file: str = None, image_uri: str = None, json_file: str = None
+    ) -> Dict:
+        """Detect document
+
+        :param image_file: source image file path
+        :param image_uri: Google Cloud Storage URI
+        :param json_file: json target to save result
+        :return: detection response
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Detect Document   image_file=${CURDIR}${/}test.png
+            ...  json_file=${CURDIR}${/}result.json
+        """
+        parameters = self.set_image_type(image_file, image_uri)
+        response = self.service.document_text_detection(**parameters)
+        self.write_json(json_file, response)
+        return response
+
+    @keyword(tags=["vision"])
+    def annotate_image(
+        self, image_file: str, image_uri: str, json_file: str = None
+    ) -> Dict:
+        """Annotate image
+
+        :param image_file: source image file path
+        :param image_uri: Google Cloud Storage URI
+        :param json_file: json target to save result
+        :return: detection response
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Annotate Image   image_file=${CURDIR}${/}test.png
+            ...  json_file=${CURDIR}${/}result.json
+        """
+        parameters = self.set_image_type(image_file, image_uri)
+        response = self.service.annotate_image(**parameters)
+        self.write_json(json_file, response)
+        return response
+
+    @keyword(tags=["vision"])
+    def face_detection(
+        self, image_file: str = None, image_uri: str = None, json_file: str = None
+    ) -> Dict:
+        """Detect faces
+
+        :param image_file: source image file path
+        :param image_uri: Google Cloud Storage URI
+        :param json_file: json target to save result
+        :return: detection response
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            ${result}=   Face Detection   image_uri=gs://vision/faces.png
+            ...  json_file=${CURDIR}${/}result.json
+        """
+        parameters = self.set_image_type(image_file, image_uri)
+        response = self.service.face_detection(**parameters)
+        self.write_json(json_file, response)
+        return response
```

### Comparing `rpaframework_google-7.0.2/src/RPA/scripts/google_authenticate.py` & `rpaframework_google-7.0.3/src/RPA/scripts/google_authenticate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import argparse
-import base64
-import os
-import pickle
-import sys
-
-from google_auth_oauthlib.flow import InstalledAppFlow
-
-
-DESCRIPTION = """
-Command-line utility for converting Google OAuth
-authorization credentials to an access token, which can be kept
-in a secret storage such as Robocorp Vault. This allows calling Google
-APIs without user interaction.
-
-example usage:
-> rpa-google-oauth --credentials drive_credentials.json --service drive
-"""
-
-CREDENTIALS = """
-Copy these credentials into Robocorp Vault:
-
--------------------------------------------
-{}
--------------------------------------------
-"""
-
-SERVICE_SCOPES = {
-    "drive": ["drive.appdata", "drive.file", "drive.install", "drive"],
-    "natural-language": ["cloud-language", "cloud-platform"],
-    "sheets": ["spreadsheets"],
-    "apps-script": ["script.projects"],
-    "vision": ["cloud-vision", "cloud-platform"],
-    "gmail": ["gmail.send", "gmail.compose", "gmail.modify", "gmail.labels"],
-}
-
-
-def create_parser():
-    parser = argparse.ArgumentParser(
-        description=DESCRIPTION.strip(), formatter_class=argparse.RawTextHelpFormatter
-    )
-    parser.add_argument(
-        "--credentials",
-        dest="credentials_file",
-        default="credentials.json",
-        help="project credentials file (default: %(default)s)",
-    )
-    parser.add_argument(
-        "--scopes",
-        dest="scopes",
-        help="authentication scopes as comma separated list",
-    )
-    parser.add_argument(
-        "--service",
-        dest="service",
-        help="set authentication scopes for the given service",
-    )
-    parser.add_argument(
-        "--console",
-        dest="console_flow",
-        action="store_true",
-        help="run console based auth flow (default: %(default)s)",
-    )
-    return parser
-
-
-def main():
-    parser = create_parser()
-    args = parser.parse_args()
-
-    def error(msg):
-        parser.print_help()
-        print(f"\nERROR: {msg}\n")
-        sys.exit(1)
-
-    # if Google.GOOGLECLOUD_IMPORT_ERROR:
-    #     error(
-    #         "Please install the 'google' optional extra to use this script:\n"
-    #         "> pip install rpaframework-google"
-    #     )
-
-    if (
-        not os.path.exists(args.credentials_file)
-        or os.stat(args.credentials_file).st_size == 0
-    ):
-        error(f"Credentials file '{args.credentials_file}' does not exist or is empty")
-
-    scopes = []
-
-    if args.service:  # and args.service in SERVICE_SCOPES:
-        services = args.service.split(",")
-        for service in services:
-            if service in SERVICE_SCOPES.keys():
-                scopes += SERVICE_SCOPES[service]
-
-    if args.scopes:
-        scopes.extend(args.scopes.split(","))
-
-    if not scopes:
-        error("No authentication scopes have been defined")
-
-    print(scopes)
-    uris = [f"https://www.googleapis.com/auth/{scope}" for scope in scopes]
-    print("Google OAuth Flow for scopes: {}".format(", ".join(scopes)))
-
-    flow = InstalledAppFlow.from_client_secrets_file(args.credentials_file, uris)
-    if args.console_flow:
-        credentials = flow.run_console()
-    else:
-        credentials = flow.run_local_server()
-
-    serialized = base64.b64encode(pickle.dumps(credentials)).decode("utf-8")
-    print(CREDENTIALS.format(serialized))
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+import base64
+import os
+import pickle
+import sys
+
+from google_auth_oauthlib.flow import InstalledAppFlow
+
+
+DESCRIPTION = """
+Command-line utility for converting Google OAuth
+authorization credentials to an access token, which can be kept
+in a secret storage such as Robocorp Vault. This allows calling Google
+APIs without user interaction.
+
+example usage:
+> rpa-google-oauth --credentials drive_credentials.json --service drive
+"""
+
+CREDENTIALS = """
+Copy these credentials into Robocorp Vault:
+
+-------------------------------------------
+{}
+-------------------------------------------
+"""
+
+SERVICE_SCOPES = {
+    "drive": ["drive.appdata", "drive.file", "drive.install", "drive"],
+    "natural-language": ["cloud-language", "cloud-platform"],
+    "sheets": ["spreadsheets"],
+    "apps-script": ["script.projects"],
+    "vision": ["cloud-vision", "cloud-platform"],
+    "gmail": ["gmail.send", "gmail.compose", "gmail.modify", "gmail.labels"],
+}
+
+
+def create_parser():
+    parser = argparse.ArgumentParser(
+        description=DESCRIPTION.strip(), formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument(
+        "--credentials",
+        dest="credentials_file",
+        default="credentials.json",
+        help="project credentials file (default: %(default)s)",
+    )
+    parser.add_argument(
+        "--scopes",
+        dest="scopes",
+        help="authentication scopes as comma separated list",
+    )
+    parser.add_argument(
+        "--service",
+        dest="service",
+        help="set authentication scopes for the given service",
+    )
+    parser.add_argument(
+        "--console",
+        dest="console_flow",
+        action="store_true",
+        help="run console based auth flow (default: %(default)s)",
+    )
+    return parser
+
+
+def main():
+    parser = create_parser()
+    args = parser.parse_args()
+
+    def error(msg):
+        parser.print_help()
+        print(f"\nERROR: {msg}\n")
+        sys.exit(1)
+
+    # if Google.GOOGLECLOUD_IMPORT_ERROR:
+    #     error(
+    #         "Please install the 'google' optional extra to use this script:\n"
+    #         "> pip install rpaframework-google"
+    #     )
+
+    if (
+        not os.path.exists(args.credentials_file)
+        or os.stat(args.credentials_file).st_size == 0
+    ):
+        error(f"Credentials file '{args.credentials_file}' does not exist or is empty")
+
+    scopes = []
+
+    if args.service:  # and args.service in SERVICE_SCOPES:
+        services = args.service.split(",")
+        for service in services:
+            if service in SERVICE_SCOPES.keys():
+                scopes += SERVICE_SCOPES[service]
+
+    if args.scopes:
+        scopes.extend(args.scopes.split(","))
+
+    if not scopes:
+        error("No authentication scopes have been defined")
+
+    print(scopes)
+    uris = [f"https://www.googleapis.com/auth/{scope}" for scope in scopes]
+    print("Google OAuth Flow for scopes: {}".format(", ".join(scopes)))
+
+    flow = InstalledAppFlow.from_client_secrets_file(args.credentials_file, uris)
+    if args.console_flow:
+        credentials = flow.run_console()
+    else:
+        credentials = flow.run_local_server()
+
+    serialized = base64.b64encode(pickle.dumps(credentials)).decode("utf-8")
+    print(CREDENTIALS.format(serialized))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `rpaframework_google-7.0.2/PKG-INFO` & `rpaframework_google-7.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-google
-Version: 7.0.2
+Version: 7.0.3
 Summary: Google library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,google
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.7,<4.0
```

