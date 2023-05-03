# Comparing `tmp/cspyce-2.0.8.tar.gz` & `tmp/cspyce-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspyce-2.0.8.tar", last modified: Wed Apr 19 20:55:58 2023, max compression
+gzip compressed data, was "cspyce-2.0.9.tar", last modified: Tue May  2 03:37:32 2023, max compression
```

## Comparing `cspyce-2.0.8.tar` & `cspyce-2.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.505477 cspyce-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-04-19 20:55:42.000000 cspyce-2.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 20:55:42.000000 cspyce-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 20:55:58.505477 cspyce-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-04-19 20:55:42.000000 cspyce-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.501477 cspyce-2.0.8/cspyce/
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/alias_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/array_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)   144839 2023-04-19 20:55:57.000000 cspyce-2.0.8/cspyce/cspyce0.py
--rw-r--r--   0 runner    (1001) docker     (123)   392102 2023-04-19 20:55:52.000000 cspyce-2.0.8/cspyce/cspyce0_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    39226 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce1_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce/typemap_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/typemap_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.501477 cspyce-2.0.8/cspyce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   164695 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-19 20:55:42.000000 cspyce-2.0.8/get_spice.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:55:58.505477 cspyce-2.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4167 2023-04-19 20:55:42.000000 cspyce-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.505477 cspyce-2.0.8/swig/
--rw-r--r--   0 runner    (1001) docker     (123)  4109483 2023-04-19 20:55:57.000000 cspyce-2.0.8/swig/cspyce0_wrap.c
--rw-r--r--   0 runner    (1001) docker     (123)   222160 2023-04-19 20:55:58.000000 cspyce-2.0.8/swig/typemap_samples_wrap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:37:32.207097 cspyce-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-02 03:37:10.000000 cspyce-2.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 03:37:10.000000 cspyce-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-05-02 03:37:32.207097 cspyce-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-05-02 03:37:10.000000 cspyce-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:37:32.199096 cspyce-2.0.9/cspyce/
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/alias_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/array_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144839 2023-05-02 03:37:30.000000 cspyce-2.0.9/cspyce/cspyce0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   392102 2023-05-02 03:37:23.000000 cspyce-2.0.9/cspyce/cspyce0_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39226 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/cspyce1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/cspyce1_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/cspyce2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-02 03:37:31.000000 cspyce-2.0.9/cspyce/typemap_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-05-02 03:37:10.000000 cspyce-2.0.9/cspyce/typemap_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:37:32.199096 cspyce-2.0.9/cspyce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-05-02 03:37:31.000000 cspyce-2.0.9/cspyce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   164704 2023-05-02 03:37:32.000000 cspyce-2.0.9/cspyce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:37:31.000000 cspyce-2.0.9/cspyce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 03:37:31.000000 cspyce-2.0.9/cspyce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 03:37:31.000000 cspyce-2.0.9/cspyce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 03:37:10.000000 cspyce-2.0.9/get_spice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 03:37:32.207097 cspyce-2.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3939 2023-05-02 03:37:10.000000 cspyce-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:37:32.207097 cspyce-2.0.9/swig/
+-rw-r--r--   0 runner    (1001) docker     (123)  4109483 2023-05-02 03:37:30.000000 cspyce-2.0.9/swig/cspyce0_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (123)   222160 2023-05-02 03:37:31.000000 cspyce-2.0.9/swig/typemap_samples_wrap.c
```

### Comparing `cspyce-2.0.8/LICENSE.txt` & `cspyce-2.0.9/LICENSE.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,186 +1,194 @@
-Academic Free License ("AFL") v. 3.0
+Apache License
+==============
 
-This Academic Free License (the "License") applies to any original
-work of authorship (the "Original Work") whose owner (the "Licensor")
-has placed the following licensing notice adjacent to the copyright
-notice for the Original Work:
-
-Licensed under the Academic Free License version 3.0
-
-1) Grant of Copyright License. Licensor grants You a worldwide,
-royalty-free, non-exclusive, sublicensable license, for the duration
-of the copyright, to do the following:
-
-a) to reproduce the Original Work in copies, either alone or as part
-of a collective work;
-
-b) to translate, adapt, alter, transform, modify, or arrange the
-Original Work, thereby creating derivative works ("Derivative Works")
-based upon the Original Work;
-
-c) to distribute or communicate copies of the Original Work and
-Derivative Works to the public, under any license of your choice that
-does not contradict the terms and conditions, including Licensor's
-reserved rights and remedies, in this Academic Free License;
-
-d) to perform the Original Work publicly; and
-
-e) to display the Original Work publicly.
-
-2) Grant of Patent License. Licensor grants You a worldwide,
-royalty-free, non-exclusive, sublicensable license, under patent
-claims owned or controlled by the Licensor that are embodied in the
-Original Work as furnished by the Licensor, for the duration of the
-patents, to make, use, sell, offer for sale, have made, and import the
-Original Work and Derivative Works.
-
-3) Grant of Source Code License. The term "Source Code" means the
-preferred form of the Original Work for making modifications to it and
-all available documentation describing how to modify the Original
-Work. Licensor agrees to provide a machine-readable copy of the Source
-Code of the Original Work along with each copy of the Original Work
-that Licensor distributes. Licensor reserves the right to satisfy this
-obligation by placing a machine-readable copy of the Source Code in an
-information repository reasonably calculated to permit inexpensive and
-convenient access by You for as long as Licensor continues to
-distribute the Original Work.
-
-4) Exclusions From License Grant. Neither the names of Licensor, nor
-the names of any contributors to the Original Work, nor any of their
-trademarks or service marks, may be used to endorse or promote
-products derived from this Original Work without express prior
-permission of the Licensor. Except as expressly stated herein, nothing
-in this License grants any license to Licensor's trademarks,
-copyrights, patents, trade secrets or any other intellectual
-property. No patent license is granted to make, use, sell, offer for
-sale, have made, or import embodiments of any patent claims other than
-the licensed claims defined in Section 2. No license is granted to the
-trademarks of Licensor even if such marks are included in the Original
-Work. Nothing in this License shall be interpreted to prohibit
-Licensor from licensing under terms different from this License any
-Original Work that Licensor otherwise would have a right to license.
-
-5) External Deployment. The term "External Deployment" means the use,
-distribution, or communication of the Original Work or Derivative
-Works in any way such that the Original Work or Derivative Works may
-be used by anyone other than You, whether those works are distributed
-or communicated to those persons or made available as an application
-intended for use over a network. As an express condition for the
-grants of license hereunder, You must treat any External Deployment by
-You of the Original Work or a Derivative Work as a distribution under
-section 1(c).
-
-6) Attribution Rights. You must retain, in the Source Code of any
-Derivative Works that You create, all copyright, patent, or trademark
-notices from the Source Code of the Original Work, as well as any
-notices of licensing and any descriptive text identified therein as an
-"Attribution Notice." You must cause the Source Code for any
-Derivative Works that You create to carry a prominent Attribution
-Notice reasonably calculated to inform recipients that You have
-modified the Original Work.
-
-7) Warranty of Provenance and Disclaimer of Warranty. Licensor
-warrants that the copyright in and to the Original Work and the patent
-rights granted herein by Licensor are owned by the Licensor or are
-sublicensed to You under the terms of this License with the permission
-of the contributor(s) of those copyrights and patent rights. Except as
-expressly stated in the immediately preceding sentence, the Original
-Work is provided under this License on an "AS IS" BASIS and WITHOUT
-WARRANTY, either express or implied, including, without limitation,
-the warranties of non-infringement, merchantability or fitness for a
-particular purpose. THE ENTIRE RISK AS TO THE QUALITY OF THE ORIGINAL
-WORK IS WITH YOU. This DISCLAIMER OF WARRANTY constitutes an essential
-part of this License. No license to the Original Work is granted by
-this License except under this disclaimer.
-
-8) Limitation of Liability. Under no circumstances and under no legal
-theory, whether in tort (including negligence), contract, or
-otherwise, shall the Licensor be liable to anyone for any indirect,
-special, incidental, or consequential damages of any character arising
-as a result of this License or the use of the Original Work including,
-without limitation, damages for loss of goodwill, work stoppage,
-computer failure or malfunction, or any and all other commercial
-damages or losses. This limitation of liability shall not apply to the
-extent applicable law prohibits such limitation.
-
-9) Acceptance and Termination. If, at any time, You expressly assented
-to this License, that assent indicates your clear and irrevocable
-acceptance of this License and all of its terms and conditions. If You
-distribute or communicate copies of the Original Work or a Derivative
-Work, You must make a reasonable effort under the circumstances to
-obtain the express assent of recipients to the terms of this
-License. This License conditions your rights to undertake the
-activities listed in Section 1, including your right to create
-Derivative Works based upon the Original Work, and doing so without
-honoring these terms and conditions is prohibited by copyright law and
-international treaty. Nothing in this License is intended to affect
-copyright exceptions and limitations (including "fair use" or "fair
-dealing"). This License shall terminate immediately and You may no
-longer exercise any of the rights granted to You by this License upon
-your failure to honor the conditions in Section 1(c).
-
-10) Termination for Patent Action. This License shall terminate
-automatically and You may no longer exercise any of the rights granted
-to You by this License as of the date You commence an action,
-including a cross-claim or counterclaim, against Licensor or any
-licensee alleging that the Original Work infringes a patent. This
-termination provision shall not apply for an action alleging patent
-infringement by combinations of the Original Work with other software
-or hardware.
-
-11) Jurisdiction, Venue and Governing Law. Any action or suit relating
-to this License may be brought only in the courts of a jurisdiction
-wherein the Licensor resides or in which Licensor conducts its primary
-business, and under the laws of that jurisdiction excluding its
-conflict-of-law provisions. The application of the United Nations
-Convention on Contracts for the International Sale of Goods is
-expressly excluded. Any use of the Original Work outside the scope of
-this License or after its termination shall be subject to the
-requirements and penalties of copyright or patent law in the
-appropriate jurisdiction. This section shall survive the termination
-of this License.
-
-12) Attorneys' Fees. In any action to enforce the terms of this
-License or seeking damages relating thereto, the prevailing party
-shall be entitled to recover its costs and expenses, including,
-without limitation, reasonable attorneys' fees and costs incurred in
-connection with such action, including any appeal of such action. This
-section shall survive the termination of this License.
-
-13) Miscellaneous. If any provision of this License is held to be
-unenforceable, such provision shall be reformed only to the extent
-necessary to make it enforceable.
-
-14) Definition of "You" in This License. "You" throughout this
-License, whether in upper or lower case, means an individual or a
-legal entity exercising rights under, and complying with all of the
-terms of, this License. For legal entities, "You" includes any entity
-that controls, is controlled by, or is under common control with
-you. For purposes of this definition, "control" means (i) the power,
-direct or indirect, to cause the direction or management of such
-entity, whether by contract or otherwise, or (ii) ownership of fifty
-percent (50%) or more of the outstanding shares, or (iii) beneficial
-ownership of such entity.
-
-15) Right to Use. You may use the Original Work in all ways not
-otherwise restricted or conditioned by this License or by law, and
-Licensor promises not to interfere with or be responsible for such
-uses by You.
-
-16) Modification of This License. This License is Copyright © 2005
-Lawrence Rosen. Permission is granted to copy, distribute, or
-communicate this License without modification. Nothing in this License
-permits You to modify this License as applied to the Original Work or
-to Derivative Works. However, You may modify the text of this License
-and copy, distribute or communicate your modified version (the
-"Modified License") and apply it to other original works of authorship
-subject to the following conditions: (i) You may not indicate in any
-way that your Modified License is the "Academic Free License" or "AFL"
-and you may not use those names in the name of your Modified License;
-(ii) You must replace the notice specified in the first paragraph
-above with the notice "Licensed under <insert your license name here>"
-or with a notice of your own that is not confusingly similar to the
-notice in this License; and (iii) You may not claim that your original
-works are open source software unless your Modified License has been
-approved by Open Source Initiative (OSI) and You comply with its
-license review and certification process.
+_Version 2.0, January 2004_  
+_&lt;<http://www.apache.org/licenses/>&gt;_
+
+### Terms and Conditions for use, reproduction, and distribution
+
+#### 1. Definitions
+
+“License” shall mean the terms and conditions for use, reproduction, and
+distribution as defined by Sections 1 through 9 of this document.
+
+“Licensor” shall mean the copyright owner or entity authorized by the copyright
+owner that is granting the License.
+
+“Legal Entity” shall mean the union of the acting entity and all other entities
+that control, are controlled by, or are under common control with that entity.
+For the purposes of this definition, “control” means **(i)** the power, direct or
+indirect, to cause the direction or management of such entity, whether by
+contract or otherwise, or **(ii)** ownership of fifty percent (50%) or more of the
+outstanding shares, or **(iii)** beneficial ownership of such entity.
+
+“You” (or “Your”) shall mean an individual or Legal Entity exercising
+permissions granted by this License.
+
+“Source” form shall mean the preferred form for making modifications, including
+but not limited to software source code, documentation source, and configuration
+files.
+
+“Object” form shall mean any form resulting from mechanical transformation or
+translation of a Source form, including but not limited to compiled object code,
+generated documentation, and conversions to other media types.
+
+“Work” shall mean the work of authorship, whether in Source or Object form, made
+available under the License, as indicated by a copyright notice that is included
+in or attached to the work (an example is provided in the Appendix below).
+
+“Derivative Works” shall mean any work, whether in Source or Object form, that
+is based on (or derived from) the Work and for which the editorial revisions,
+annotations, elaborations, or other modifications represent, as a whole, an
+original work of authorship. For the purposes of this License, Derivative Works
+shall not include works that remain separable from, or merely link (or bind by
+name) to the interfaces of, the Work and Derivative Works thereof.
+
+“Contribution” shall mean any work of authorship, including the original version
+of the Work and any modifications or additions to that Work or Derivative Works
+thereof, that is intentionally submitted to Licensor for inclusion in the Work
+by the copyright owner or by an individual or Legal Entity authorized to submit
+on behalf of the copyright owner. For the purposes of this definition,
+“submitted” means any form of electronic, verbal, or written communication sent
+to the Licensor or its representatives, including but not limited to
+communication on electronic mailing lists, source code control systems, and
+issue tracking systems that are managed by, or on behalf of, the Licensor for
+the purpose of discussing and improving the Work, but excluding communication
+that is conspicuously marked or otherwise designated in writing by the copyright
+owner as “Not a Contribution.”
+
+“Contributor” shall mean Licensor and any individual or Legal Entity on behalf
+of whom a Contribution has been received by Licensor and subsequently
+incorporated within the Work.
+
+#### 2. Grant of Copyright License
+
+Subject to the terms and conditions of this License, each Contributor hereby
+grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free,
+irrevocable copyright license to reproduce, prepare Derivative Works of,
+publicly display, publicly perform, sublicense, and distribute the Work and such
+Derivative Works in Source or Object form.
+
+#### 3. Grant of Patent License
+
+Subject to the terms and conditions of this License, each Contributor hereby
+grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free,
+irrevocable (except as stated in this section) patent license to make, have
+made, use, offer to sell, sell, import, and otherwise transfer the Work, where
+such license applies only to those patent claims licensable by such Contributor
+that are necessarily infringed by their Contribution(s) alone or by combination
+of their Contribution(s) with the Work to which such Contribution(s) was
+submitted. If You institute patent litigation against any entity (including a
+cross-claim or counterclaim in a lawsuit) alleging that the Work or a
+Contribution incorporated within the Work constitutes direct or contributory
+patent infringement, then any patent licenses granted to You under this License
+for that Work shall terminate as of the date such litigation is filed.
+
+#### 4. Redistribution
+
+You may reproduce and distribute copies of the Work or Derivative Works thereof
+in any medium, with or without modifications, and in Source or Object form,
+provided that You meet the following conditions:
+
+* **(a)** You must give any other recipients of the Work or Derivative Works a copy of
+this License; and
+* **(b)** You must cause any modified files to carry prominent notices stating that You
+changed the files; and
+* **(c)** You must retain, in the Source form of any Derivative Works that You distribute,
+all copyright, patent, trademark, and attribution notices from the Source form
+of the Work, excluding those notices that do not pertain to any part of the
+Derivative Works; and
+* **(d)** If the Work includes a “NOTICE” text file as part of its distribution, then any
+Derivative Works that You distribute must include a readable copy of the
+attribution notices contained within such NOTICE file, excluding those notices
+that do not pertain to any part of the Derivative Works, in at least one of the
+following places: within a NOTICE text file distributed as part of the
+Derivative Works; within the Source form or documentation, if provided along
+with the Derivative Works; or, within a display generated by the Derivative
+Works, if and wherever such third-party notices normally appear. The contents of
+the NOTICE file are for informational purposes only and do not modify the
+License. You may add Your own attribution notices within Derivative Works that
+You distribute, alongside or as an addendum to the NOTICE text from the Work,
+provided that such additional attribution notices cannot be construed as
+modifying the License.
+
+You may add Your own copyright statement to Your modifications and may provide
+additional or different license terms and conditions for use, reproduction, or
+distribution of Your modifications, or for any such Derivative Works as a whole,
+provided Your use, reproduction, and distribution of the Work otherwise complies
+with the conditions stated in this License.
+
+#### 5. Submission of Contributions
+
+Unless You explicitly state otherwise, any Contribution intentionally submitted
+for inclusion in the Work by You to the Licensor shall be under the terms and
+conditions of this License, without any additional terms or conditions.
+Notwithstanding the above, nothing herein shall supersede or modify the terms of
+any separate license agreement you may have executed with Licensor regarding
+such Contributions.
+
+#### 6. Trademarks
+
+This License does not grant permission to use the trade names, trademarks,
+service marks, or product names of the Licensor, except as required for
+reasonable and customary use in describing the origin of the Work and
+reproducing the content of the NOTICE file.
+
+#### 7. Disclaimer of Warranty
+
+Unless required by applicable law or agreed to in writing, Licensor provides the
+Work (and each Contributor provides its Contributions) on an “AS IS” BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied,
+including, without limitation, any warranties or conditions of TITLE,
+NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are
+solely responsible for determining the appropriateness of using or
+redistributing the Work and assume any risks associated with Your exercise of
+permissions under this License.
+
+#### 8. Limitation of Liability
+
+In no event and under no legal theory, whether in tort (including negligence),
+contract, or otherwise, unless required by applicable law (such as deliberate
+and grossly negligent acts) or agreed to in writing, shall any Contributor be
+liable to You for damages, including any direct, indirect, special, incidental,
+or consequential damages of any character arising as a result of this License or
+out of the use or inability to use the Work (including but not limited to
+damages for loss of goodwill, work stoppage, computer failure or malfunction, or
+any and all other commercial damages or losses), even if such Contributor has
+been advised of the possibility of such damages.
+
+#### 9. Accepting Warranty or Additional Liability
+
+While redistributing the Work or Derivative Works thereof, You may choose to
+offer, and charge a fee for, acceptance of support, warranty, indemnity, or
+other liability obligations and/or rights consistent with this License. However,
+in accepting such obligations, You may act only on Your own behalf and on Your
+sole responsibility, not on behalf of any other Contributor, and only if You
+agree to indemnify, defend, and hold each Contributor harmless for any liability
+incurred by, or claims asserted against, such Contributor by reason of your
+accepting any such warranty or additional liability.
+
+_END OF TERMS AND CONDITIONS_
+
+### APPENDIX: How to apply the Apache License to your work
+
+To apply the Apache License to your work, attach the following boilerplate
+notice, with the fields enclosed by brackets `[]` replaced with your own
+identifying information. (Don't include the brackets!) The text should be
+enclosed in the appropriate comment syntax for the file format. We also
+recommend that a file or class name and description of purpose be included on
+the same “printed page” as the copyright notice for easier identification within
+third-party archives.
+
+    Copyright [yyyy] [name of copyright owner]
+    
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+    
+      http://www.apache.org/licenses/LICENSE-2.0
+    
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
```

### Comparing `cspyce-2.0.8/README.md` & `cspyce-2.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+[![PyPI version](https://badge.fury.io/py/cspyce.svg)](https://badge.fury.io/py/cspyce)
+
 # `cspyce` MODULE OVERVIEW
 Version 2.0
 
 March, 2022
 
 Mark Showalter, PDS Ring-Moon Systems Node, SETI Institute
 
 `cspyce` is a Python module that provides an interface to the C-language CSPICE
 library produced by the Navigation and Ancillary Information Facility
 ([NAIF](https://naif.jpl.nasa.gov/naif/)) of NASA's Planetary Data System (PDS).
-It implements the most widely-used functions of CSPICE in a Python-like way,
-while also supporting numerous enhancements, including support for Python
-exceptions, array inputs, and aliases.
+It implements most functions of CSPICE in a Python-like way, while also
+supporting numerous enhancements, including support for Python exceptions,
+array inputs, and aliases.
+
+`cspyce` may be installed by running `pip install cspyce`.
+
+Python versions 3.8 thru 3.11 are currently supported, with pre-built wheels
+available for Linux, MacOS, and Windows.
 
 If you are looking for information on running or distributing this code from
 the GitHub sources, look at the file `README-developers.md` in this directory.
 
 ## PYTHONIZATION
 
 `cspyce` has been designed to replicate the core features of CSPICE for
```

### Comparing `cspyce-2.0.8/cspyce/__init__.py` & `cspyce-2.0.9/cspyce/__init__.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/alias_support.py` & `cspyce-2.0.9/cspyce/alias_support.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/aliases.py` & `cspyce-2.0.9/cspyce/aliases.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/array_support.py` & `cspyce-2.0.9/cspyce/array_support.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/arrays.py` & `cspyce-2.0.9/cspyce/arrays.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/cspyce0.py` & `cspyce-2.0.9/cspyce/cspyce0.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/cspyce0_info.py` & `cspyce-2.0.9/cspyce/cspyce0_info.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/cspyce1.py` & `cspyce-2.0.9/cspyce/cspyce1.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/cspyce1_info.py` & `cspyce-2.0.9/cspyce/cspyce1_info.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/cspyce2.py` & `cspyce-2.0.9/cspyce/cspyce2.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/typemap_samples.py` & `cspyce-2.0.9/cspyce/typemap_samples.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce/typemap_test.py` & `cspyce-2.0.9/cspyce/typemap_test.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/cspyce.egg-info/SOURCES.txt` & `cspyce-2.0.9/cspyce.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-LICENSE.txt
+LICENSE.md
 MANIFEST.in
 README.md
 get_spice.py
+setup.cfg
 setup.py
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/F77_aloc.c
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/abort_.c
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/accept.c
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/alltru.c
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/ana.c
 /home/runner/work/pds-cspyce/pds-cspyce/cspice/Linux-x86_64/src/appndc.c
```

### Comparing `cspyce-2.0.8/get_spice.py` & `cspyce-2.0.9/get_spice.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/setup.py` & `cspyce-2.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 # distribution or source distribution, and automatically builds it as needed for
 # your machine.
 #
 # If you are doing a build from sources, please read README-developers.md in
 # this directory.
 
 
-# We prefer setuptools, but will use distutils if setuptools isn't available
-import os
 from glob import glob
 import os
 import platform
 import subprocess
 import sys
 
 from setuptools.command.build_ext import build_ext
 
 from get_spice import GetCspice
 
+# We prefer setuptools, but will use distutils if setuptools isn't available
 try:
     from setuptools import Command, setup, Extension
 except ImportError:
     from distutils.core import Command, setup, Extension
 
 try:
     import numpy
@@ -52,82 +51,77 @@
     def run(self):
         if not PYTHON2:
             from swig.make_vectorize import create_vectorize_header_file
             from swig.make_cspyce0_info import make_cspice0_info
             create_vectorize_header_file("swig/vectorize.i")
             make_cspice0_info("cspyce/cspyce0_info.py")
             command = "swig -python -outdir cspyce/. " \
-                      "-o swig/cspyce0_wrap.c swig/cspyce0.i".split(' ')
+                      "-o swig/cspyce0_wrap.c swig/cspyce0.i".split(" ")
             subprocess.check_call(command)
             command = "swig -python -outdir cspyce/. " \
-                      "-o swig/typemap_samples_wrap.c swig/typemap_samples.i".split(' ')
+                      "-o swig/typemap_samples_wrap.c swig/typemap_samples.i".split(" ")
             subprocess.check_call(command)
         else:
-            command = "echo Cannot rebuild files in Python2".split(' ')
+            command = "echo Cannot rebuild files in Python2".split(" ")
             subprocess.check_call(command)
 
 
 # Some linkers seem to have trouble with 2400 files, so we break it up into
 # smaller libraries with a maximum of 250 files apiece.
 
 cspice_directory = GetCspice().download()
 
 def get_c_libraries():
     files = sorted(glob(os.path.join(cspice_directory, "src", "*.c")))
     splits = 1 if IS_LINUX else 1 + (len(files) // 250)
-    compiler_flags = ['-DKR_headers', '-DMSDOS', '/nowarn'] if IS_WINDOWS else ['-w']
+    compiler_flags = ["-DKR_headers", "-DMSDOS", "/nowarn"] if IS_WINDOWS else ["-w"]
     cspice_libraries = [
         ("cspice_" + str(i + 1), {
             "sources": files[i::splits],
             "include_dirs": [os.path.join(cspice_directory, "include")],
             "cflags": compiler_flags
         })
         for i in range(splits)]
     return cspice_libraries
 
 
 def get_extensions():
-    cspyce_cflags = ['/nowarn', '/DSWIG_PYTHON_CAST_MODE'] if IS_WINDOWS \
-        else ['-Wno-incompatible-pointer-types', '-DSWIG_PYTHON_CAST_MODE']
+    cspyce_cflags = ["/nowarn", "/DSWIG_PYTHON_CAST_MODE"] if IS_WINDOWS \
+        else ["-Wno-incompatible-pointer-types", "-DSWIG_PYTHON_CAST_MODE"]
     include_dirs = [os.path.join(cspice_directory, "include"), numpy.get_include()]
 
     cspyce0_module = Extension(
-        'cspyce._cspyce0',
-        sources=['swig/cspyce0_wrap.c'],
+        "cspyce._cspyce0",
+        sources=["swig/cspyce0_wrap.c"],
         include_dirs=include_dirs,
         extra_compile_args=cspyce_cflags)
 
     typemap_samples_module = Extension(
-        'cspyce._typemap_samples',
-        sources=['swig/typemap_samples_wrap.c'],
+        "cspyce._typemap_samples",
+        sources=["swig/typemap_samples_wrap.c"],
         include_dirs=include_dirs,
         extra_compile_args=cspyce_cflags,
     )
     return [cspyce0_module, typemap_samples_module]
 
 
 class MyBuildExt(build_ext):
     def initialize_options(self):
         build_ext.initialize_options(self)
 
 
 def do_setup():
-    prerelease_version = os.getenv('PRERELEASE_VERSION', '')
-    if prerelease_version == 'release':
-        prerelease_version = ''
+    prerelease_version = os.getenv("PRERELEASE_VERSION", "")
+    if prerelease_version == "release":
+        prerelease_version = ""
 
     setup(
-        name='cspyce',
-        version='2.0.8' + prerelease_version,
-        author="Mark Showalter/PDS Ring-Moon Systems Node",
-        description="Low-level SWIG interface to the CSPICE library",
+        version='2.0.9' + prerelease_version,
         ext_modules=get_extensions(),
         libraries=get_c_libraries(),
-        packages=["cspyce"],
-        install_requires=['numpy'],
         cmdclass={
-            'build_ext': MyBuildExt,
-            'generate': GenerateCommand,
+            "build_ext": MyBuildExt,
+            "generate": GenerateCommand,
         }
     )
 
 do_setup()
```

### Comparing `cspyce-2.0.8/swig/cspyce0_wrap.c` & `cspyce-2.0.9/swig/cspyce0_wrap.c`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.8/swig/typemap_samples_wrap.c` & `cspyce-2.0.9/swig/typemap_samples_wrap.c`

 * *Files identical despite different names*

