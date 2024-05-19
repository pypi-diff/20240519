# Comparing `tmp/hydromodel-0.2.2.tar.gz` & `tmp/hydromodel-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromodel-0.2.2.tar", last modified: Thu Mar 28 04:46:34 2024, max compression
+gzip compressed data, was "hydromodel-0.2.3.tar", last modified: Sun May 19 05:51:41 2024, max compression
```

## Comparing `hydromodel-0.2.2.tar` & `hydromodel-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.352724 hydromodel-0.2.2/
--rw-rw-rw-   0        0        0      174 2024-03-28 03:17:25.000000 hydromodel-0.2.2/AUTHORS.rst
--rw-rw-rw-   0        0        0    35823 2021-09-26 09:37:40.000000 hydromodel-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      129 2024-03-28 03:17:25.000000 hydromodel-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14236 2024-03-28 04:46:34.350737 hydromodel-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13235 2024-03-28 03:17:25.000000 hydromodel-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:33.888890 hydromodel-0.2.2/hydromodel/
--rw-rw-rw-   0        0        0     2648 2024-03-28 04:40:46.000000 hydromodel-0.2.2/hydromodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.012413 hydromodel-0.2.2/hydromodel/datasets/
--rw-rw-rw-   0        0        0     1345 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/datasets/__init__.py
--rw-rw-rw-   0        0        0    17994 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/datasets/data_preprocess.py
--rw-rw-rw-   0        0        0    12663 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/datasets/data_visualize.py
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.112977 hydromodel-0.2.2/hydromodel/models/
--rw-rw-rw-   0        0        0        0 2021-12-10 15:01:02.000000 hydromodel-0.2.2/hydromodel/models/__init__.py
--rw-rw-rw-   0        0        0     8453 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/gr4j.py
--rw-rw-rw-   0        0        0     5213 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/hymod.py
--rw-rw-rw-   0        0        0     5789 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/model_config.py
--rw-rw-rw-   0        0        0     1417 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/model_dict.py
--rw-rw-rw-   0        0        0    32781 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/xaj.py
--rw-rw-rw-   0        0        0     9665 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/models/xaj_bmi.py
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.171546 hydromodel-0.2.2/hydromodel/trainers/
--rw-rw-rw-   0        0        0        0 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/trainers/__init__.py
--rw-rw-rw-   0        0        0    12193 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/trainers/calibrate_ga.py
--rw-rw-rw-   0        0        0     8200 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/trainers/calibrate_sceua.py
--rw-rw-rw-   0        0        0    12718 2024-03-28 03:17:25.000000 hydromodel-0.2.2/hydromodel/trainers/evaluate.py
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.337117 hydromodel-0.2.2/hydromodel.egg-info/
--rw-rw-rw-   0        0        0    14236 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      104 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-10-28 09:37:05.000000 hydromodel-0.2.2/hydromodel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      101 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-28 04:46:33.000000 hydromodel-0.2.2/hydromodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      116 2024-03-28 03:17:25.000000 hydromodel-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0      481 2024-03-28 04:46:34.362733 hydromodel-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2098 2024-03-28 04:40:46.000000 hydromodel-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 04:46:34.302090 hydromodel-0.2.2/test/
--rw-rw-rw-   0        0        0     1683 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_calibrate.py
--rw-rw-rw-   0        0        0     9185 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_data_preprocess.py
--rw-rw-rw-   0        0        0     3893 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_data_visualize.py
--rw-rw-rw-   0        0        0      710 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_gr4j.py
--rw-rw-rw-   0        0        0      722 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_hymod.py
--rw-rw-rw-   0        0        0      281 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_show_results.py
--rw-rw-rw-   0        0        0     2432 2024-03-28 03:17:25.000000 hydromodel-0.2.2/test/test_xaj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-19 05:51:33.000000 hydromodel-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 05:51:33.000000 hydromodel-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 05:51:33.000000 hydromodel-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-19 05:51:41.673990 hydromodel-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-05-19 05:51:33.000000 hydromodel-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.669990 hydromodel-0.2.3/hydromodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/data_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/gr4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/hymod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/xaj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/xaj_bmi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/calibrate_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/calibrate_sceua.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.669990 hydromodel-0.2.3/hydromodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 05:51:33.000000 hydromodel-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 05:51:41.673990 hydromodel-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-19 05:51:33.000000 hydromodel-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_data_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_gr4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_hymod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_show_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_xaj.py
```

### Comparing `hydromodel-0.2.2/LICENSE` & `hydromodel-0.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `hydromodel-0.2.2/PKG-INFO` & `hydromodel-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,261 +1,250 @@
-Metadata-Version: 2.1
-Name: hydromodel
-Version: 0.2.2
-Summary: hydrological models starting from XinAnJiang
-Home-page: https://github.com/OuyangWenyu/hydromodel
-Author: Wenyu Ouyang
-Author-email: wenyuouyang@outlook.com
-License: GNU General Public License v3
-Keywords: hydromodel
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: ipykernel
-Requires-Dist: numba
-Requires-Dist: scikit-learn
-Requires-Dist: deap
-Requires-Dist: spotpy
-Requires-Dist: pytest
-Requires-Dist: bmipy
-Requires-Dist: pyyaml
-Requires-Dist: requests
-Requires-Dist: muskingumcunge
-Requires-Dist: hydrodatasource
-
-# hydromodel
-
-[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
-[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
-
-[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
-
--   Free software: GNU General Public License v3
--   Documentation: https://OuyangWenyu.github.io/hydromodel
-
-## What is hydromodel
-
-**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
-
-**Not an official version, just for learning**
-
-This is a Python console program (no graphic interface now). It is **still developing**.
-
-## How to run
-
-### Install
-
-We provided a pip package. You can install it with pip:
-
-
-```Shell
-# create python environment
-$ conda create -n hydromodel python=3.10
-$ conda activate hydromodel
-# install hydromodel
-$ pip install hydromodel
-```
-
-If you want to run the model as a developer, you can clone the repository
-
-```Shell
-# fork hydromodel to your GitHub, and clone it to your computer
-$ git clone <address of hydromodel in your github>
-# move to it
-$ cd hydromodel
-# if updating from upstream, pull the new version to local
-$ git pull
-# create python environment
-$ mamba env create -f env-dev.yml
-# if mamba is not installed:
-# $ conda install -c conda-forge mamba
-# activate it
-$ conda activate hydromodel
-```
-
-### Prepare data
-
-You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
-
-If CAMELS is used, you can skip this step.
-
-To use your own data to run the model, you need prepare the data in the required format.
-
-We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
-
-But you still need to do some manual work before transformation. Here are the steps:
-
-1. Put all data in one directory and check if it is organized as the following format:
-```
-your_data_directory_for_hydromodel/
-# one attribute csv file for all basins
-├─ basin_attributes.csv
-# one timeseries csv file for one basin, xxx and yyy are the basin ids
-├─ basin_xxx.csv
-├─ basin_yyy.csv
-├─ basin_zzz.csv
-├─ ...
-```
-basin_attributes.csv should have the following columns:
-```csv
-id     name  area(km^2)
-xxx  Basin A         100
-yyy  Basin B         200
-zzz  Basin C         300
-```
-basin_xxx.csv should have the following columns:
-```csv
-time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
-2022-01-01 00:00:00            1                 10                 13                 16                 19
-2022-01-02 00:00:00            2                 11                 14                 17                 20
-2022-01-03 00:00:00            3                 12                 15                 18                 21
-```
-The sequence of the columns is not important, but the column names should be the same as the above.
-No more unnecessary columns are allowed.
-For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
-The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
-
-1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
-```Shell
-$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
-```
-
-### Run the model
-
-To run calibration with CAMLES dataset, you can use the following code:
-
-```Shell
-# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
-$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-```
-
-To use your own data, run the following code:
-
-```Shell
-# you can change the algorithm parameters:
-$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
-```
-
-**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
-
-Then you can evaluate the calibrated model with the following code:
-
-```Shell
-# $ python evaluate_xaj.py --exp expcamels001
-# for your own data
-$ python evaluate_xaj.py --exp expbiliuhe001
-```
-
-### See the results
-
-Run the following code to see the results of the evaluation:
-
-```Shell
-# $ python visualize.py --exp expcamels001
-# for your own data
-$ python visualize.py --exp expbiliuhe001
-```
-
-You will see the results in the `example` directory.
-
-## Why does hydro-model-xaj exist
-
-When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
-models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
-model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
-provided.
-
-Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
-popular now as they are public with great performance and readable documents; as more and more people use them, they
-become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
-and develop it. I think hydro-model-xaj is a good start.
-
-## What are the main features
-
-We basically implement the formula in this book
--- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
-
-Other reference Chinese books：
-
-- ["*Principles of
-  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
-- ["*Hydrologic
-  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
-- ["*Engineering
-  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
-
-More English references could be seen at the end of this README file.
-
-The model mainly includes three parts:
-
-![](docs/img/xaj.jpg)
-
-For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
-evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
-because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
-you use pan evaporation, just treat K as Kc.
-
-For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
-little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
-
-For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
-CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
-from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
-, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
-
-We provide two common calibration methods to optimize XAJ's parameters:
-
-- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
-- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
-  is used, but no completed case is provided yet. We will provide one soon.
-
-Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
-for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
-needed, and it is not implemented yet. The following links may be useful:
-
-- https://github.com/ecoon/watershed-workflow
-- https://github.com/ConnectedSystems/Streamfall.jl
-
-**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
-
-The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
-
-Other implementations for XAJ:
-
-- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
-- Java: https://github.com/wfxr/xaj-hydrological-model
-- R, C++: https://github.com/Sibada/XAJ
-
-## How to contribute
-
-If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
-git branch for your feature and send me a pull request.
-
-If you find any problems in hydro-model-xaj, please post your questions
-on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
-
-## References
-
-- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
-  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
-- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
-  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
-- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
-  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
-  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
-  DOI:https://doi.org/10.1145/2330784.2330799
-- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
-  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
-- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
-  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
-  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
-- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
-  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
-- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
+Metadata-Version: 2.1
+Name: hydromodel
+Version: 0.2.3
+Summary: hydrological models starting from XinAnJiang
+Home-page: https://github.com/OuyangWenyu/hydromodel
+Author: Wenyu Ouyang
+Author-email: wenyuouyang@outlook.com
+License: GNU General Public License v3
+Keywords: hydromodel
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# hydromodel
+
+[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
+[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
+
+[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
+
+-   Free software: GNU General Public License v3
+-   Documentation: https://OuyangWenyu.github.io/hydromodel
+
+## What is hydromodel
+
+**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
+
+**Not an official version, just for learning**
+
+This is a Python console program (no graphic interface now). It is **still developing**.
+
+## How to run
+
+### Install
+
+We provided a pip package. You can install it with pip:
+
+
+```Shell
+# create python environment
+$ conda create -n hydromodel python=3.10
+$ conda activate hydromodel
+# install hydromodel
+$ pip install hydromodel
+```
+
+If you want to run the model as a developer, you can clone the repository
+
+```Shell
+# fork hydromodel to your GitHub, and clone it to your computer
+$ git clone <address of hydromodel in your github>
+# move to it
+$ cd hydromodel
+# if updating from upstream, pull the new version to local
+$ git pull
+# create python environment
+$ mamba env create -f env-dev.yml
+# if mamba is not installed:
+# $ conda install -c conda-forge mamba
+# activate it
+$ conda activate hydromodel
+```
+
+### Prepare data
+
+You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
+
+If CAMELS is used, you can skip this step.
+
+To use your own data to run the model, you need prepare the data in the required format.
+
+We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
+
+But you still need to do some manual work before transformation. Here are the steps:
+
+1. Put all data in one directory and check if it is organized as the following format:
+```
+your_data_directory_for_hydromodel/
+# one attribute csv file for all basins
+├─ basin_attributes.csv
+# one timeseries csv file for one basin, xxx and yyy are the basin ids
+├─ basin_xxx.csv
+├─ basin_yyy.csv
+├─ basin_zzz.csv
+├─ ...
+```
+basin_attributes.csv should have the following columns:
+```csv
+id     name  area(km^2)
+xxx  Basin A         100
+yyy  Basin B         200
+zzz  Basin C         300
+```
+basin_xxx.csv should have the following columns:
+```csv
+time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
+2022-01-01 00:00:00            1                 10                 13                 16                 19
+2022-01-02 00:00:00            2                 11                 14                 17                 20
+2022-01-03 00:00:00            3                 12                 15                 18                 21
+```
+The sequence of the columns is not important, but the column names should be the same as the above.
+No more unnecessary columns are allowed.
+For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
+The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
+
+1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
+```Shell
+$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
+```
+
+### Run the model
+
+To run calibration with CAMLES dataset, you can use the following code:
+
+```Shell
+# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
+$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+```
+
+To use your own data, run the following code:
+
+```Shell
+# you can change the algorithm parameters:
+$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
+```
+
+**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
+
+Then you can evaluate the calibrated model with the following code:
+
+```Shell
+# $ python evaluate_xaj.py --exp expcamels001
+# for your own data
+$ python evaluate_xaj.py --exp expbiliuhe001
+```
+
+### See the results
+
+Run the following code to see the results of the evaluation:
+
+```Shell
+# $ python visualize.py --exp expcamels001
+# for your own data
+$ python visualize.py --exp expbiliuhe001
+```
+
+You will see the results in the `example` directory.
+
+## Why does hydro-model-xaj exist
+
+When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
+models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
+model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
+provided.
+
+Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
+popular now as they are public with great performance and readable documents; as more and more people use them, they
+become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
+and develop it. I think hydro-model-xaj is a good start.
+
+## What are the main features
+
+We basically implement the formula in this book
+-- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
+
+Other reference Chinese books：
+
+- ["*Principles of
+  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
+- ["*Hydrologic
+  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
+- ["*Engineering
+  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
+
+More English references could be seen at the end of this README file.
+
+The model mainly includes three parts:
+
+![](docs/img/xaj.jpg)
+
+For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
+evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
+because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
+you use pan evaporation, just treat K as Kc.
+
+For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
+little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
+
+For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
+CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
+from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
+, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
+
+We provide two common calibration methods to optimize XAJ's parameters:
+
+- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
+- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
+  is used, but no completed case is provided yet. We will provide one soon.
+
+Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
+for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
+needed, and it is not implemented yet. The following links may be useful:
+
+- https://github.com/ecoon/watershed-workflow
+- https://github.com/ConnectedSystems/Streamfall.jl
+
+**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
+
+The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
+
+Other implementations for XAJ:
+
+- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
+- Java: https://github.com/wfxr/xaj-hydrological-model
+- R, C++: https://github.com/Sibada/XAJ
+
+## How to contribute
+
+If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
+git branch for your feature and send me a pull request.
+
+If you find any problems in hydro-model-xaj, please post your questions
+on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
+
+## References
+
+- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
+  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
+- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
+  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
+- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
+  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
+  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
+  DOI:https://doi.org/10.1145/2330784.2330799
+- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
+  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
+- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
+  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
+  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
+- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
+  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
+- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
```

### Comparing `hydromodel-0.2.2/README.md` & `hydromodel-0.2.3/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-# hydromodel
-
-[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
-[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
-
-[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
-
--   Free software: GNU General Public License v3
--   Documentation: https://OuyangWenyu.github.io/hydromodel
-
-## What is hydromodel
-
-**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
-
-**Not an official version, just for learning**
-
-This is a Python console program (no graphic interface now). It is **still developing**.
-
-## How to run
-
-### Install
-
-We provided a pip package. You can install it with pip:
-
-
-```Shell
-# create python environment
-$ conda create -n hydromodel python=3.10
-$ conda activate hydromodel
-# install hydromodel
-$ pip install hydromodel
-```
-
-If you want to run the model as a developer, you can clone the repository
-
-```Shell
-# fork hydromodel to your GitHub, and clone it to your computer
-$ git clone <address of hydromodel in your github>
-# move to it
-$ cd hydromodel
-# if updating from upstream, pull the new version to local
-$ git pull
-# create python environment
-$ mamba env create -f env-dev.yml
-# if mamba is not installed:
-# $ conda install -c conda-forge mamba
-# activate it
-$ conda activate hydromodel
-```
-
-### Prepare data
-
-You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
-
-If CAMELS is used, you can skip this step.
-
-To use your own data to run the model, you need prepare the data in the required format.
-
-We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
-
-But you still need to do some manual work before transformation. Here are the steps:
-
-1. Put all data in one directory and check if it is organized as the following format:
-```
-your_data_directory_for_hydromodel/
-# one attribute csv file for all basins
-├─ basin_attributes.csv
-# one timeseries csv file for one basin, xxx and yyy are the basin ids
-├─ basin_xxx.csv
-├─ basin_yyy.csv
-├─ basin_zzz.csv
-├─ ...
-```
-basin_attributes.csv should have the following columns:
-```csv
-id     name  area(km^2)
-xxx  Basin A         100
-yyy  Basin B         200
-zzz  Basin C         300
-```
-basin_xxx.csv should have the following columns:
-```csv
-time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
-2022-01-01 00:00:00            1                 10                 13                 16                 19
-2022-01-02 00:00:00            2                 11                 14                 17                 20
-2022-01-03 00:00:00            3                 12                 15                 18                 21
-```
-The sequence of the columns is not important, but the column names should be the same as the above.
-No more unnecessary columns are allowed.
-For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
-The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
-
-1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
-```Shell
-$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
-```
-
-### Run the model
-
-To run calibration with CAMLES dataset, you can use the following code:
-
-```Shell
-# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
-$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-```
-
-To use your own data, run the following code:
-
-```Shell
-# you can change the algorithm parameters:
-$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
-```
-
-**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
-
-Then you can evaluate the calibrated model with the following code:
-
-```Shell
-# $ python evaluate_xaj.py --exp expcamels001
-# for your own data
-$ python evaluate_xaj.py --exp expbiliuhe001
-```
-
-### See the results
-
-Run the following code to see the results of the evaluation:
-
-```Shell
-# $ python visualize.py --exp expcamels001
-# for your own data
-$ python visualize.py --exp expbiliuhe001
-```
-
-You will see the results in the `example` directory.
-
-## Why does hydro-model-xaj exist
-
-When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
-models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
-model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
-provided.
-
-Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
-popular now as they are public with great performance and readable documents; as more and more people use them, they
-become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
-and develop it. I think hydro-model-xaj is a good start.
-
-## What are the main features
-
-We basically implement the formula in this book
--- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
-
-Other reference Chinese books：
-
-- ["*Principles of
-  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
-- ["*Hydrologic
-  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
-- ["*Engineering
-  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
-
-More English references could be seen at the end of this README file.
-
-The model mainly includes three parts:
-
-![](docs/img/xaj.jpg)
-
-For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
-evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
-because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
-you use pan evaporation, just treat K as Kc.
-
-For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
-little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
-
-For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
-CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
-from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
-, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
-
-We provide two common calibration methods to optimize XAJ's parameters:
-
-- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
-- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
-  is used, but no completed case is provided yet. We will provide one soon.
-
-Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
-for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
-needed, and it is not implemented yet. The following links may be useful:
-
-- https://github.com/ecoon/watershed-workflow
-- https://github.com/ConnectedSystems/Streamfall.jl
-
-**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
-
-The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
-
-Other implementations for XAJ:
-
-- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
-- Java: https://github.com/wfxr/xaj-hydrological-model
-- R, C++: https://github.com/Sibada/XAJ
-
-## How to contribute
-
-If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
-git branch for your feature and send me a pull request.
-
-If you find any problems in hydro-model-xaj, please post your questions
-on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
-
-## References
-
-- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
-  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
-- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
-  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
-- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
-  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
-  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
-  DOI:https://doi.org/10.1145/2330784.2330799
-- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
-  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
-- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
-  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
-  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
-- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
-  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
-- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
+# hydromodel
+
+[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
+[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
+
+[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
+
+-   Free software: GNU General Public License v3
+-   Documentation: https://OuyangWenyu.github.io/hydromodel
+
+## What is hydromodel
+
+**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
+
+**Not an official version, just for learning**
+
+This is a Python console program (no graphic interface now). It is **still developing**.
+
+## How to run
+
+### Install
+
+We provided a pip package. You can install it with pip:
+
+
+```Shell
+# create python environment
+$ conda create -n hydromodel python=3.10
+$ conda activate hydromodel
+# install hydromodel
+$ pip install hydromodel
+```
+
+If you want to run the model as a developer, you can clone the repository
+
+```Shell
+# fork hydromodel to your GitHub, and clone it to your computer
+$ git clone <address of hydromodel in your github>
+# move to it
+$ cd hydromodel
+# if updating from upstream, pull the new version to local
+$ git pull
+# create python environment
+$ mamba env create -f env-dev.yml
+# if mamba is not installed:
+# $ conda install -c conda-forge mamba
+# activate it
+$ conda activate hydromodel
+```
+
+### Prepare data
+
+You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
+
+If CAMELS is used, you can skip this step.
+
+To use your own data to run the model, you need prepare the data in the required format.
+
+We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
+
+But you still need to do some manual work before transformation. Here are the steps:
+
+1. Put all data in one directory and check if it is organized as the following format:
+```
+your_data_directory_for_hydromodel/
+# one attribute csv file for all basins
+├─ basin_attributes.csv
+# one timeseries csv file for one basin, xxx and yyy are the basin ids
+├─ basin_xxx.csv
+├─ basin_yyy.csv
+├─ basin_zzz.csv
+├─ ...
+```
+basin_attributes.csv should have the following columns:
+```csv
+id     name  area(km^2)
+xxx  Basin A         100
+yyy  Basin B         200
+zzz  Basin C         300
+```
+basin_xxx.csv should have the following columns:
+```csv
+time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
+2022-01-01 00:00:00            1                 10                 13                 16                 19
+2022-01-02 00:00:00            2                 11                 14                 17                 20
+2022-01-03 00:00:00            3                 12                 15                 18                 21
+```
+The sequence of the columns is not important, but the column names should be the same as the above.
+No more unnecessary columns are allowed.
+For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
+The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
+
+1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
+```Shell
+$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
+```
+
+### Run the model
+
+To run calibration with CAMLES dataset, you can use the following code:
+
+```Shell
+# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
+$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+```
+
+To use your own data, run the following code:
+
+```Shell
+# you can change the algorithm parameters:
+$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
+```
+
+**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
+
+Then you can evaluate the calibrated model with the following code:
+
+```Shell
+# $ python evaluate_xaj.py --exp expcamels001
+# for your own data
+$ python evaluate_xaj.py --exp expbiliuhe001
+```
+
+### See the results
+
+Run the following code to see the results of the evaluation:
+
+```Shell
+# $ python visualize.py --exp expcamels001
+# for your own data
+$ python visualize.py --exp expbiliuhe001
+```
+
+You will see the results in the `example` directory.
+
+## Why does hydro-model-xaj exist
+
+When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
+models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
+model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
+provided.
+
+Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
+popular now as they are public with great performance and readable documents; as more and more people use them, they
+become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
+and develop it. I think hydro-model-xaj is a good start.
+
+## What are the main features
+
+We basically implement the formula in this book
+-- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
+
+Other reference Chinese books：
+
+- ["*Principles of
+  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
+- ["*Hydrologic
+  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
+- ["*Engineering
+  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
+
+More English references could be seen at the end of this README file.
+
+The model mainly includes three parts:
+
+![](docs/img/xaj.jpg)
+
+For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
+evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
+because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
+you use pan evaporation, just treat K as Kc.
+
+For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
+little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
+
+For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
+CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
+from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
+, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
+
+We provide two common calibration methods to optimize XAJ's parameters:
+
+- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
+- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
+  is used, but no completed case is provided yet. We will provide one soon.
+
+Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
+for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
+needed, and it is not implemented yet. The following links may be useful:
+
+- https://github.com/ecoon/watershed-workflow
+- https://github.com/ConnectedSystems/Streamfall.jl
+
+**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
+
+The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
+
+Other implementations for XAJ:
+
+- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
+- Java: https://github.com/wfxr/xaj-hydrological-model
+- R, C++: https://github.com/Sibada/XAJ
+
+## How to contribute
+
+If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
+git branch for your feature and send me a pull request.
+
+If you find any problems in hydro-model-xaj, please post your questions
+on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
+
+## References
+
+- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
+  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
+- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
+  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
+- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
+  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
+  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
+  DOI:https://doi.org/10.1145/2330784.2330799
+- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
+  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
+- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
+  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
+  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
+- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
+  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
+- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
```

### Comparing `hydromodel-0.2.2/hydromodel/datasets/__init__.py` & `hydromodel-0.2.3/hydromodel/datasets/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-PRCP_NAME = "prcp(mm/day)"
-PET_NAME = "pet(mm/day)"
-ET_NAME = "et(mm/day)"
-FLOW_NAME = "flow(m^3/s)"
-NODE_FLOW_NAME = "node1_flow(m^3/s)"
-AREA_NAME = "area(km^2)"
-TIME_NAME = "time"
-POSSIBLE_TIME_FORMATS = [
-    "%Y-%m-%d %H:%M:%S",  # 完整的日期和时间
-    "%Y-%m-%d",  # 只有日期
-    "%d/%m/%Y",  # 不同的日期格式
-    "%m/%d/%Y %H:%M",  # 月/日/年 小时:分钟
-    "%d/%m/%Y %H:%M",  # 日/月/年 小时:分钟
-    # ... 可以根据需要添加更多格式 ...
-]
-ID_NAME = "id"
-NAME_NAME = "name"
-
-
-def remove_unit_from_name(name_with_unit):
-    """
-    Remove the unit from a variable name.
-
-    Parameters
-    ----------
-    name_with_unit : str
-        The name of the variable including its unit, e.g., "prcp(mm/day)".
-
-    Returns
-    -------
-    str
-        The name of the variable without the unit, e.g., "prcp".
-    """
-    return name_with_unit.split("(")[0]
-
-
-def get_unit_from_name(name_with_unit):
-    """
-    Extract the unit from a variable name.
-
-    Parameters
-    ----------
-    name_with_unit : str
-        The name of the variable including its unit, e.g., "prcp(mm/day)".
-
-    Returns
-    -------
-    str
-        The unit of the variable, e.g., "mm/day".
-    """
-    return name_with_unit.split("(")[1].strip(")") if "(" in name_with_unit else ""
+PRCP_NAME = "prcp(mm/day)"
+PET_NAME = "pet(mm/day)"
+ET_NAME = "et(mm/day)"
+FLOW_NAME = "flow(m^3/s)"
+NODE_FLOW_NAME = "node1_flow(m^3/s)"
+AREA_NAME = "area(km^2)"
+TIME_NAME = "time"
+POSSIBLE_TIME_FORMATS = [
+    "%Y-%m-%d %H:%M:%S",  # 完整的日期和时间
+    "%Y-%m-%d",  # 只有日期
+    "%d/%m/%Y",  # 不同的日期格式
+    "%m/%d/%Y %H:%M",  # 月/日/年 小时:分钟
+    "%d/%m/%Y %H:%M",  # 日/月/年 小时:分钟
+    # ... 可以根据需要添加更多格式 ...
+]
+ID_NAME = "id"
+NAME_NAME = "name"
+
+
+def remove_unit_from_name(name_with_unit):
+    """
+    Remove the unit from a variable name.
+
+    Parameters
+    ----------
+    name_with_unit : str
+        The name of the variable including its unit, e.g., "prcp(mm/day)".
+
+    Returns
+    -------
+    str
+        The name of the variable without the unit, e.g., "prcp".
+    """
+    return name_with_unit.split("(")[0]
+
+
+def get_unit_from_name(name_with_unit):
+    """
+    Extract the unit from a variable name.
+
+    Parameters
+    ----------
+    name_with_unit : str
+        The name of the variable including its unit, e.g., "prcp(mm/day)".
+
+    Returns
+    -------
+    str
+        The unit of the variable, e.g., "mm/day".
+    """
+    return name_with_unit.split("(")[1].strip(")") if "(" in name_with_unit else ""
```

### Comparing `hydromodel-0.2.2/hydromodel/datasets/data_preprocess.py` & `hydromodel-0.2.3/hydromodel/datasets/data_preprocess.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,544 +1,544 @@
-"""
-Author: Wenyu Ouyang
-Date: 2022-10-25 21:16:22
-LastEditTime: 2024-03-27 18:17:14
-LastEditors: Wenyu Ouyang
-Description: preprocess data for models in hydro-model-xaj
-FilePath: \hydro-model-xaj\hydromodel\datasets\data_preprocess.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import re
-import numpy as np
-import pandas as pd
-from pint import UnitRegistry
-from sklearn.model_selection import KFold
-import xarray as xr
-
-from hydrodataset import Camels
-from hydrodatasource.utils.utils import streamflow_unit_conv
-from hydrodatasource.cleaner.dmca_esr import rainfall_runoff_event_identify
-
-from hydromodel import CACHE_DIR, SETTING
-from hydromodel.datasets import *
-
-
-def check_tsdata_format(file_path):
-    """
-    Checks the time-series data for required and optional columns
-    used in hydrological modeling.
-
-    Parameters
-    ----------
-    file_path : str
-        Path to the hydrological data file.
-
-    Returns
-    -------
-    bool
-        True if the data file format is correct, False otherwise.
-    """
-    # prcp means precipitation, pet means potential evapotranspiration, flow means streamflow
-    required_columns = [
-        remove_unit_from_name(TIME_NAME),
-        remove_unit_from_name(PRCP_NAME),
-        remove_unit_from_name(PET_NAME),
-        remove_unit_from_name(FLOW_NAME),
-    ]
-    # et means evapotranspiration, node_flow means upstream streamflow
-    # node1 means the first upstream node, node2 means the second upstream node, etc.
-    # these nodes are the nearest upstream nodes of the target node
-    # meaning: if node1_flow, node2_flow, and more upstream nodes are parellel.
-    # No serial relationship
-    optional_columns = [
-        remove_unit_from_name(ET_NAME),
-        remove_unit_from_name(NODE_FLOW_NAME),
-    ]
-
-    try:
-        data = pd.read_csv(file_path)
-
-        data_columns = [remove_unit_from_name(col) for col in data.columns]
-        # Check required columns
-        missing_required_columns = [
-            column for column in required_columns if column not in data_columns
-        ]
-
-        if missing_required_columns:
-            print(
-                f"Missing required columns in file: {file_path}: {missing_required_columns}"
-            )
-            return False
-
-        # Check optional columns
-        for column in optional_columns:
-            if column not in data_columns:
-                print(
-                    f"Optional column '{column}' not found in file: {file_path}, but it's okay."
-                )
-
-        # Check node_flow columns (flexible number of nodes)
-        node_flow_columns = [
-            col for col in data.columns if re.match(r"node\d+_flow", col)
-        ]
-        if not node_flow_columns:
-            print(f"No 'node_flow' columns found in file: {file_path}, but it's okay.")
-
-        # Check time format and sorting
-        time_parsed = False
-        for time_format in POSSIBLE_TIME_FORMATS:
-            try:
-                data[TIME_NAME] = pd.to_datetime(data[TIME_NAME], format=time_format)
-                time_parsed = True
-                break
-            except ValueError:
-                continue
-
-        if not time_parsed:
-            print(f"Time format is incorrect in file: {file_path}")
-            return False
-
-        if not data[TIME_NAME].is_monotonic_increasing:
-            print(f"Data is not sorted by time in file: {file_path}")
-            return False
-
-        # Check for consistent time intervals
-        time_differences = (
-            data[TIME_NAME].diff().dropna()
-        )  # Calculate differences and remove NaN
-        if not all(time_differences == time_differences.iloc[0]):
-            print(f"Time series is not at consistent intervals in file: {file_path}")
-            return False
-
-        return True
-
-    except Exception as e:
-        print(f"Error reading file {file_path}: {e}")
-        return False
-
-
-def check_basin_attr_format(file_path):
-    """
-    Checks the basin attributes data for required columns.
-
-    Parameters
-    ----------
-    file_path : str
-        Path to the basin attributes data file.
-
-    Returns
-    -------
-    bool
-        True if the basin attributes file format is correct, False otherwise.
-    """
-    required_columns = [ID_NAME, NAME_NAME, AREA_NAME]
-
-    try:
-        data = pd.read_csv(file_path)
-
-        if missing_required_columns := [
-            col for col in required_columns if col not in data.columns
-        ]:
-            print(
-                f"Missing required columns in basin attributes file: {file_path}: {missing_required_columns}"
-            )
-            return False
-
-        # Additional checks (e.g., datatype checks, non-empty rows) can be added here
-
-        return True
-
-    except Exception as e:
-        print(f"Error reading basin attributes file {file_path}: {e}")
-        return False
-
-
-def check_folder_contents(folder_path, basin_attr_file="basin_attributes.csv"):
-    """
-    Checks all time series data files in a folder and a single basin attributes file.
-
-    Parameters
-    ----------
-    folder_path : str
-        Path to the folder containing the time series data files.
-    basin_attr_file : str
-        Filename of the basin attributes file, default is "basin_attributes.csv".
-
-    Returns
-    -------
-    bool
-        True if all files in the folder and the basin attributes file are correct, False otherwise.
-    """
-    # 检查流域属性文件
-    if not check_basin_attr_format(os.path.join(folder_path, basin_attr_file)):
-        return False
-
-    # 获取流域ID列表
-    basin_ids = pd.read_csv(
-        os.path.join(folder_path, basin_attr_file), dtype={ID_NAME: str}
-    )[ID_NAME].tolist()
-
-    # 检查每个流域的时序文件
-    for basin_id in basin_ids:
-        file_name = f"basin_{basin_id}.csv"
-        file_path = os.path.join(folder_path, file_name)
-
-        if not os.path.exists(file_path):
-            print(f"Missing time series data file for basin {basin_id}: {file_path}")
-            return False
-
-        if not check_tsdata_format(file_path):
-            print(f"Time series data format check failed for file: {file_path}")
-            return False
-
-    return True
-
-
-def process_and_save_data_as_nc(
-    folder_path,
-    save_folder=CACHE_DIR,
-    nc_attrs_file="attributes.nc",
-    nc_ts_file="timeseries.nc",
-):
-    # 验证文件夹内容
-    if not check_folder_contents(folder_path):
-        print("Folder contents validation failed.")
-        return False
-
-    # 读取流域属性
-    basin_attr_file = os.path.join(folder_path, "basin_attributes.csv")
-    # id must be str
-    basin_attrs = pd.read_csv(basin_attr_file, dtype={ID_NAME: str})
-
-    # 创建属性数据集
-    ds_attrs = xr.Dataset.from_dataframe(basin_attrs.set_index(ID_NAME))
-    new_column_names = {}
-    units = {}
-
-    for col in basin_attrs.columns:
-        new_name = remove_unit_from_name(col)
-        unit = get_unit_from_name(col)
-        new_column_names[col] = new_name
-        if unit:
-            units[new_name] = unit
-
-    basin_attrs.rename(columns=new_column_names, inplace=True)
-
-    # 创建不带单位的数据集
-    ds_attrs = xr.Dataset.from_dataframe(basin_attrs.set_index(ID_NAME))
-
-    # 为有单位的变量添加单位属性
-    for var_name, unit in units.items():
-        ds_attrs[var_name].attrs["units"] = unit
-    # 初始化时序数据集
-    ds_ts = xr.Dataset()
-
-    # 初始化用于保存单位的字典
-    units = {}
-
-    # id must be str
-    basin_ids = basin_attrs[ID_NAME].astype(str).tolist()
-
-    # 为每个流域读取并处理时序数据
-    for i, basin_id in enumerate(basin_ids):
-        file_name = f"basin_{basin_id}.csv"
-        file_path = os.path.join(folder_path, file_name)
-        data = pd.read_csv(file_path)
-        for time_format in POSSIBLE_TIME_FORMATS:
-            try:
-                data[TIME_NAME] = pd.to_datetime(data[TIME_NAME], format=time_format)
-                break
-            except ValueError:
-                continue
-        # 在处理第一个流域时构建单位字典
-        if i == 0:
-            for col in data.columns:
-                new_name = remove_unit_from_name(col)
-                if unit := get_unit_from_name(col):
-                    units[new_name] = unit
-
-        # 修改列名以移除单位
-        renamed_columns = {col: remove_unit_from_name(col) for col in data.columns}
-        data.rename(columns=renamed_columns, inplace=True)
-
-        # 将 DataFrame 转换为 xarray Dataset
-        ds_basin = xr.Dataset.from_dataframe(data.set_index(TIME_NAME))
-
-        # 为每个变量设置单位属性
-        for var in ds_basin.data_vars:
-            if var in units:
-                ds_basin[var].attrs["units"] = units[var]
-        # 添加 basin 坐标
-        ds_basin = ds_basin.expand_dims({"basin": [basin_id]})
-        # 合并到主数据集
-        ds_ts = xr.merge([ds_ts, ds_basin], compat="no_conflicts")
-
-    # 保存为 NetCDF 文件
-    ds_attrs.to_netcdf(os.path.join(save_folder, nc_attrs_file))
-    ds_ts.to_netcdf(os.path.join(save_folder, nc_ts_file))
-
-    return True
-
-
-def split_train_test(ts_data, train_period, test_period):
-    """
-    Split all data to train and test parts with same format
-
-    Parameters
-    ----------
-    ts_data: xr.Dataset
-        time series data
-    train_period
-        training period
-    test_period
-        testing period
-
-    Returns
-    -------
-    tuple of xr.Dataset
-        A tuple of xr.Dataset for training and testing data
-    """
-    # Convert date strings to pandas datetime objects
-    train_start, train_end = pd.to_datetime(train_period[0]), pd.to_datetime(
-        train_period[1]
-    )
-    test_start, test_end = pd.to_datetime(test_period[0]), pd.to_datetime(
-        test_period[1]
-    )
-
-    # Select data for training and testing periods
-    train_data = ts_data.sel(time=slice(train_start, train_end))
-    test_data = ts_data.sel(time=slice(test_start, test_end))
-
-    return train_data, test_data
-
-
-def validate_freq(freq):
-    """
-    Validate if the freq string is a valid pandas frequency.
-
-    Parameters
-    ----------
-    freq : str
-        Frequency string to validate.
-
-    Returns
-    -------
-    bool
-        True if the freq string is valid, False otherwise.
-    """
-    try:
-        pd.to_timedelta("1" + freq)
-        return True
-    except ValueError:
-        return False
-
-
-def cross_valid_data(ts_data, period, warmup, cv_fold, freq="1D"):
-    """
-    Split all data to train and test parts with same format for cross validation.
-
-    Parameters
-    ----------
-    ts_data : xr.Dataset
-        time series data.
-    period : tuple of str
-        The whole period in the format ("start_date", "end_date").
-    warmup : int
-        Warmup period length in days.
-    cv_fold : int
-        Number of folds for cross-validation.
-    freq : str
-        len of one period.
-
-    Returns
-    -------
-    list of tuples
-        Each tuple contains training and testing datasets for a fold.
-    """
-    if not validate_freq(freq):
-        raise ValueError(
-            "Time unit must be number with either 'Y','M','W','D','h','m' or 's', such as 3D."
-        )
-
-    # Convert the whole period to pandas datetime
-    start_date, end_date = pd.to_datetime(period[0]), pd.to_datetime(period[1])
-    date_lst = pd.date_range(start=start_date, end=end_date, freq=freq)
-    date_rm_warmup = date_lst[warmup:]
-
-    # Initialize lists to store train and test datasets for each fold
-    train_test_data = []
-
-    # KFold split
-    kf = KFold(n_splits=cv_fold, shuffle=False)
-    for train_index, test_index in kf.split(date_rm_warmup):
-        train_period = date_rm_warmup[train_index]
-        test_period = date_rm_warmup[test_index]
-        # Create warmup periods using the specified frequency
-        train_period_warmup = pd.date_range(
-            end=train_period[0], periods=warmup + 1, freq=freq
-        )[:-1]
-        test_period_warmup = pd.date_range(
-            end=test_period[0], periods=warmup + 1, freq=freq
-        )[:-1]
-
-        # Select data from ts_data based on train and test periods
-        train_data = ts_data.sel(time=train_period.union(train_period_warmup))
-        test_data = ts_data.sel(time=test_period.union(test_period_warmup))
-
-        # Add the datasets to the list
-        train_test_data.append((train_data, test_data))
-
-    return train_test_data
-
-
-def get_basin_area(data_type, data_dir, basin_ids) -> xr.Dataset:
-    """_summary_
-
-    Parameters
-    ----------
-    data_type : _type_
-        _description_
-    data_dir : _type_
-        _description_
-    basin_ids : _type_
-        _description_
-
-    Returns
-    -------
-    xr.Dataset
-        _description_
-    """
-    area_name = remove_unit_from_name(AREA_NAME)
-    if data_type == "camels":
-        camels_data_dir = os.path.join(
-            SETTING["local_data_path"]["datasets-origin"], "camels", data_dir
-        )
-        camels = Camels(camels_data_dir)
-        basin_area = camels.read_area(basin_ids)
-    elif data_type == "owndata":
-        attr_data = xr.open_dataset(os.path.join(data_dir, "attributes.nc"))
-        # to guarantee the column name is same as the column name in the time series data
-        basin_area = attr_data[[area_name]].rename({"id": "basin"})
-    return basin_area
-
-
-def get_ts_from_diffsource(data_type, data_dir, periods, basin_ids):
-    """Get time series data from different sources and unify the format and unit of streamflow.
-
-    Parameters
-    ----------
-    data_type
-        The type of the data source, 'camels' or 'owndata'
-    data_dir
-        The directory of the data source
-    periods
-        The periods of the time series data, [start_date, end_date]
-    basin_ids
-        The ids of the basins
-
-    Returns
-    -------
-    xr.Dataset
-        The time series data
-
-    Raises
-    ------
-    NotImplementedError
-        The data type is not 'camels' or 'owndata'
-    """
-    prcp_name = remove_unit_from_name(PRCP_NAME)
-    pet_name = remove_unit_from_name(PET_NAME)
-    flow_name = remove_unit_from_name(FLOW_NAME)
-    basin_area = get_basin_area(data_type, data_dir, basin_ids)
-    if data_type == "camels":
-        camels_data_dir = os.path.join(
-            SETTING["local_data_path"]["datasets-origin"], "camels", data_dir
-        )
-        camels = Camels(camels_data_dir)
-        ts_data = camels.read_ts_xrdataset(
-            basin_ids, periods, ["prcp", "PET", "streamflow"]
-        )
-        # trans unit to mm/day
-        qobs_ = ts_data[["streamflow"]]
-        target_unit = ts_data["prcp"].attrs.get("units", "unknown")
-        r_mmd = streamflow_unit_conv(qobs_, basin_area, target_unit=target_unit)
-        ts_data[flow_name] = r_mmd["streamflow"]
-        ts_data[flow_name].attrs["units"] = target_unit
-        ts_data = ts_data.rename({"PET": pet_name})
-        # ts_data = ts_data.drop_vars('streamflow')
-    elif data_type == "owndata":
-        ts_data = xr.open_dataset(os.path.join(data_dir, "timeseries.nc"))
-        target_unit = ts_data[prcp_name].attrs.get("units", "unknown")
-        qobs_ = ts_data[[flow_name]]
-        r_mmd = streamflow_unit_conv(qobs_, basin_area, target_unit=target_unit)
-        ts_data[flow_name] = r_mmd[flow_name]
-        ts_data[flow_name].attrs["units"] = target_unit
-        ts_data = ts_data.sel(time=slice(periods[0], periods[1]))
-    else:
-        raise NotImplementedError(
-            "You should set the data type as 'camels' or 'owndata'"
-        )
-
-    return ts_data
-
-
-def _get_pe_q_from_ts(ts_xr_dataset):
-    """Transform the time series data to the format that can be used in the calibration process
-
-    Parameters
-    ----------
-    ts_xr_dataset : xr.Dataset
-        The time series data
-
-    Returns
-    -------
-    tuple[np.ndarray, np.ndarray]
-        The tuple contains the precipitation and evaporation data and the observed streamflow data
-    """
-    prcp_name = remove_unit_from_name(PRCP_NAME)
-    pet_name = remove_unit_from_name(PET_NAME)
-    flow_name = remove_unit_from_name(FLOW_NAME)
-    p_and_e = (
-        ts_xr_dataset[[prcp_name, pet_name]].to_array().to_numpy().transpose(2, 1, 0)
-    )
-    qobs = np.expand_dims(ts_xr_dataset[flow_name].to_numpy().transpose(1, 0), axis=2)
-
-    return p_and_e, qobs
-
-
-def cross_val_split_tsdata(
-    data_type, data_dir, cv_fold, train_period, test_period, periods, warmup, basin_ids
-):
-    ts_data = get_ts_from_diffsource(data_type, data_dir, periods, basin_ids)
-    if cv_fold <= 1:
-        # no cross validation
-        periods = np.sort(
-            [train_period[0], train_period[1], test_period[0], test_period[1]]
-        )
-        train_and_test_data = split_train_test(ts_data, train_period, test_period)
-    else:
-        # cross validation
-        train_and_test_data = cross_valid_data(ts_data, periods, warmup, cv_fold)
-    return train_and_test_data
-
-
-def get_rr_events(rain, flow, basin_area):
-    ureg = UnitRegistry()
-    # trans unit to mm/day
-    flow_threshold = streamflow_unit_conv(
-        np.array([100]) * ureg.m**3 / ureg.s,
-        basin_area.isel(basin=0).to_array().to_numpy() * ureg.km**2,
-        target_unit="mm/h",
-    )
-    rr_events = {}
-    for basin in basin_area.basin.values:
-        rr_event = rainfall_runoff_event_identify(
-            rain.sel(basin=basin).to_series(),
-            flow.sel(basin=basin).to_series(),
-            multiple=1,
-            flow_threshold=flow_threshold[0],
-        )
-        rr_events[basin] = rr_event
-    return rr_events
+"""
+Author: Wenyu Ouyang
+Date: 2022-10-25 21:16:22
+LastEditTime: 2024-03-27 18:17:14
+LastEditors: Wenyu Ouyang
+Description: preprocess data for models in hydro-model-xaj
+FilePath: \hydro-model-xaj\hydromodel\datasets\data_preprocess.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import re
+import numpy as np
+import pandas as pd
+from pint import UnitRegistry
+from sklearn.model_selection import KFold
+import xarray as xr
+
+from hydrodataset import Camels
+from hydrodatasource.utils.utils import streamflow_unit_conv
+from hydrodatasource.cleaner.dmca_esr import rainfall_runoff_event_identify
+
+from hydromodel import CACHE_DIR, SETTING
+from hydromodel.datasets import *
+
+
+def check_tsdata_format(file_path):
+    """
+    Checks the time-series data for required and optional columns
+    used in hydrological modeling.
+
+    Parameters
+    ----------
+    file_path : str
+        Path to the hydrological data file.
+
+    Returns
+    -------
+    bool
+        True if the data file format is correct, False otherwise.
+    """
+    # prcp means precipitation, pet means potential evapotranspiration, flow means streamflow
+    required_columns = [
+        remove_unit_from_name(TIME_NAME),
+        remove_unit_from_name(PRCP_NAME),
+        remove_unit_from_name(PET_NAME),
+        remove_unit_from_name(FLOW_NAME),
+    ]
+    # et means evapotranspiration, node_flow means upstream streamflow
+    # node1 means the first upstream node, node2 means the second upstream node, etc.
+    # these nodes are the nearest upstream nodes of the target node
+    # meaning: if node1_flow, node2_flow, and more upstream nodes are parellel.
+    # No serial relationship
+    optional_columns = [
+        remove_unit_from_name(ET_NAME),
+        remove_unit_from_name(NODE_FLOW_NAME),
+    ]
+
+    try:
+        data = pd.read_csv(file_path)
+
+        data_columns = [remove_unit_from_name(col) for col in data.columns]
+        # Check required columns
+        missing_required_columns = [
+            column for column in required_columns if column not in data_columns
+        ]
+
+        if missing_required_columns:
+            print(
+                f"Missing required columns in file: {file_path}: {missing_required_columns}"
+            )
+            return False
+
+        # Check optional columns
+        for column in optional_columns:
+            if column not in data_columns:
+                print(
+                    f"Optional column '{column}' not found in file: {file_path}, but it's okay."
+                )
+
+        # Check node_flow columns (flexible number of nodes)
+        node_flow_columns = [
+            col for col in data.columns if re.match(r"node\d+_flow", col)
+        ]
+        if not node_flow_columns:
+            print(f"No 'node_flow' columns found in file: {file_path}, but it's okay.")
+
+        # Check time format and sorting
+        time_parsed = False
+        for time_format in POSSIBLE_TIME_FORMATS:
+            try:
+                data[TIME_NAME] = pd.to_datetime(data[TIME_NAME], format=time_format)
+                time_parsed = True
+                break
+            except ValueError:
+                continue
+
+        if not time_parsed:
+            print(f"Time format is incorrect in file: {file_path}")
+            return False
+
+        if not data[TIME_NAME].is_monotonic_increasing:
+            print(f"Data is not sorted by time in file: {file_path}")
+            return False
+
+        # Check for consistent time intervals
+        time_differences = (
+            data[TIME_NAME].diff().dropna()
+        )  # Calculate differences and remove NaN
+        if not all(time_differences == time_differences.iloc[0]):
+            print(f"Time series is not at consistent intervals in file: {file_path}")
+            return False
+
+        return True
+
+    except Exception as e:
+        print(f"Error reading file {file_path}: {e}")
+        return False
+
+
+def check_basin_attr_format(file_path):
+    """
+    Checks the basin attributes data for required columns.
+
+    Parameters
+    ----------
+    file_path : str
+        Path to the basin attributes data file.
+
+    Returns
+    -------
+    bool
+        True if the basin attributes file format is correct, False otherwise.
+    """
+    required_columns = [ID_NAME, NAME_NAME, AREA_NAME]
+
+    try:
+        data = pd.read_csv(file_path)
+
+        if missing_required_columns := [
+            col for col in required_columns if col not in data.columns
+        ]:
+            print(
+                f"Missing required columns in basin attributes file: {file_path}: {missing_required_columns}"
+            )
+            return False
+
+        # Additional checks (e.g., datatype checks, non-empty rows) can be added here
+
+        return True
+
+    except Exception as e:
+        print(f"Error reading basin attributes file {file_path}: {e}")
+        return False
+
+
+def check_folder_contents(folder_path, basin_attr_file="basin_attributes.csv"):
+    """
+    Checks all time series data files in a folder and a single basin attributes file.
+
+    Parameters
+    ----------
+    folder_path : str
+        Path to the folder containing the time series data files.
+    basin_attr_file : str
+        Filename of the basin attributes file, default is "basin_attributes.csv".
+
+    Returns
+    -------
+    bool
+        True if all files in the folder and the basin attributes file are correct, False otherwise.
+    """
+    # 检查流域属性文件
+    if not check_basin_attr_format(os.path.join(folder_path, basin_attr_file)):
+        return False
+
+    # 获取流域ID列表
+    basin_ids = pd.read_csv(
+        os.path.join(folder_path, basin_attr_file), dtype={ID_NAME: str}
+    )[ID_NAME].tolist()
+
+    # 检查每个流域的时序文件
+    for basin_id in basin_ids:
+        file_name = f"basin_{basin_id}.csv"
+        file_path = os.path.join(folder_path, file_name)
+
+        if not os.path.exists(file_path):
+            print(f"Missing time series data file for basin {basin_id}: {file_path}")
+            return False
+
+        if not check_tsdata_format(file_path):
+            print(f"Time series data format check failed for file: {file_path}")
+            return False
+
+    return True
+
+
+def process_and_save_data_as_nc(
+    folder_path,
+    save_folder=CACHE_DIR,
+    nc_attrs_file="attributes.nc",
+    nc_ts_file="timeseries.nc",
+):
+    # 验证文件夹内容
+    if not check_folder_contents(folder_path):
+        print("Folder contents validation failed.")
+        return False
+
+    # 读取流域属性
+    basin_attr_file = os.path.join(folder_path, "basin_attributes.csv")
+    # id must be str
+    basin_attrs = pd.read_csv(basin_attr_file, dtype={ID_NAME: str})
+
+    # 创建属性数据集
+    ds_attrs = xr.Dataset.from_dataframe(basin_attrs.set_index(ID_NAME))
+    new_column_names = {}
+    units = {}
+
+    for col in basin_attrs.columns:
+        new_name = remove_unit_from_name(col)
+        unit = get_unit_from_name(col)
+        new_column_names[col] = new_name
+        if unit:
+            units[new_name] = unit
+
+    basin_attrs.rename(columns=new_column_names, inplace=True)
+
+    # 创建不带单位的数据集
+    ds_attrs = xr.Dataset.from_dataframe(basin_attrs.set_index(ID_NAME))
+
+    # 为有单位的变量添加单位属性
+    for var_name, unit in units.items():
+        ds_attrs[var_name].attrs["units"] = unit
+    # 初始化时序数据集
+    ds_ts = xr.Dataset()
+
+    # 初始化用于保存单位的字典
+    units = {}
+
+    # id must be str
+    basin_ids = basin_attrs[ID_NAME].astype(str).tolist()
+
+    # 为每个流域读取并处理时序数据
+    for i, basin_id in enumerate(basin_ids):
+        file_name = f"basin_{basin_id}.csv"
+        file_path = os.path.join(folder_path, file_name)
+        data = pd.read_csv(file_path)
+        for time_format in POSSIBLE_TIME_FORMATS:
+            try:
+                data[TIME_NAME] = pd.to_datetime(data[TIME_NAME], format=time_format)
+                break
+            except ValueError:
+                continue
+        # 在处理第一个流域时构建单位字典
+        if i == 0:
+            for col in data.columns:
+                new_name = remove_unit_from_name(col)
+                if unit := get_unit_from_name(col):
+                    units[new_name] = unit
+
+        # 修改列名以移除单位
+        renamed_columns = {col: remove_unit_from_name(col) for col in data.columns}
+        data.rename(columns=renamed_columns, inplace=True)
+
+        # 将 DataFrame 转换为 xarray Dataset
+        ds_basin = xr.Dataset.from_dataframe(data.set_index(TIME_NAME))
+
+        # 为每个变量设置单位属性
+        for var in ds_basin.data_vars:
+            if var in units:
+                ds_basin[var].attrs["units"] = units[var]
+        # 添加 basin 坐标
+        ds_basin = ds_basin.expand_dims({"basin": [basin_id]})
+        # 合并到主数据集
+        ds_ts = xr.merge([ds_ts, ds_basin], compat="no_conflicts")
+
+    # 保存为 NetCDF 文件
+    ds_attrs.to_netcdf(os.path.join(save_folder, nc_attrs_file))
+    ds_ts.to_netcdf(os.path.join(save_folder, nc_ts_file))
+
+    return True
+
+
+def split_train_test(ts_data, train_period, test_period):
+    """
+    Split all data to train and test parts with same format
+
+    Parameters
+    ----------
+    ts_data: xr.Dataset
+        time series data
+    train_period
+        training period
+    test_period
+        testing period
+
+    Returns
+    -------
+    tuple of xr.Dataset
+        A tuple of xr.Dataset for training and testing data
+    """
+    # Convert date strings to pandas datetime objects
+    train_start, train_end = pd.to_datetime(train_period[0]), pd.to_datetime(
+        train_period[1]
+    )
+    test_start, test_end = pd.to_datetime(test_period[0]), pd.to_datetime(
+        test_period[1]
+    )
+
+    # Select data for training and testing periods
+    train_data = ts_data.sel(time=slice(train_start, train_end))
+    test_data = ts_data.sel(time=slice(test_start, test_end))
+
+    return train_data, test_data
+
+
+def validate_freq(freq):
+    """
+    Validate if the freq string is a valid pandas frequency.
+
+    Parameters
+    ----------
+    freq : str
+        Frequency string to validate.
+
+    Returns
+    -------
+    bool
+        True if the freq string is valid, False otherwise.
+    """
+    try:
+        pd.to_timedelta("1" + freq)
+        return True
+    except ValueError:
+        return False
+
+
+def cross_valid_data(ts_data, period, warmup, cv_fold, freq="1D"):
+    """
+    Split all data to train and test parts with same format for cross validation.
+
+    Parameters
+    ----------
+    ts_data : xr.Dataset
+        time series data.
+    period : tuple of str
+        The whole period in the format ("start_date", "end_date").
+    warmup : int
+        Warmup period length in days.
+    cv_fold : int
+        Number of folds for cross-validation.
+    freq : str
+        len of one period.
+
+    Returns
+    -------
+    list of tuples
+        Each tuple contains training and testing datasets for a fold.
+    """
+    if not validate_freq(freq):
+        raise ValueError(
+            "Time unit must be number with either 'Y','M','W','D','h','m' or 's', such as 3D."
+        )
+
+    # Convert the whole period to pandas datetime
+    start_date, end_date = pd.to_datetime(period[0]), pd.to_datetime(period[1])
+    date_lst = pd.date_range(start=start_date, end=end_date, freq=freq)
+    date_rm_warmup = date_lst[warmup:]
+
+    # Initialize lists to store train and test datasets for each fold
+    train_test_data = []
+
+    # KFold split
+    kf = KFold(n_splits=cv_fold, shuffle=False)
+    for train_index, test_index in kf.split(date_rm_warmup):
+        train_period = date_rm_warmup[train_index]
+        test_period = date_rm_warmup[test_index]
+        # Create warmup periods using the specified frequency
+        train_period_warmup = pd.date_range(
+            end=train_period[0], periods=warmup + 1, freq=freq
+        )[:-1]
+        test_period_warmup = pd.date_range(
+            end=test_period[0], periods=warmup + 1, freq=freq
+        )[:-1]
+
+        # Select data from ts_data based on train and test periods
+        train_data = ts_data.sel(time=train_period.union(train_period_warmup))
+        test_data = ts_data.sel(time=test_period.union(test_period_warmup))
+
+        # Add the datasets to the list
+        train_test_data.append((train_data, test_data))
+
+    return train_test_data
+
+
+def get_basin_area(data_type, data_dir, basin_ids) -> xr.Dataset:
+    """_summary_
+
+    Parameters
+    ----------
+    data_type : _type_
+        _description_
+    data_dir : _type_
+        _description_
+    basin_ids : _type_
+        _description_
+
+    Returns
+    -------
+    xr.Dataset
+        _description_
+    """
+    area_name = remove_unit_from_name(AREA_NAME)
+    if data_type == "camels":
+        camels_data_dir = os.path.join(
+            SETTING["local_data_path"]["datasets-origin"], "camels", data_dir
+        )
+        camels = Camels(camels_data_dir)
+        basin_area = camels.read_area(basin_ids)
+    elif data_type == "owndata":
+        attr_data = xr.open_dataset(os.path.join(data_dir, "attributes.nc"))
+        # to guarantee the column name is same as the column name in the time series data
+        basin_area = attr_data[[area_name]].rename({"id": "basin"})
+    return basin_area
+
+
+def get_ts_from_diffsource(data_type, data_dir, periods, basin_ids):
+    """Get time series data from different sources and unify the format and unit of streamflow.
+
+    Parameters
+    ----------
+    data_type
+        The type of the data source, 'camels' or 'owndata'
+    data_dir
+        The directory of the data source
+    periods
+        The periods of the time series data, [start_date, end_date]
+    basin_ids
+        The ids of the basins
+
+    Returns
+    -------
+    xr.Dataset
+        The time series data
+
+    Raises
+    ------
+    NotImplementedError
+        The data type is not 'camels' or 'owndata'
+    """
+    prcp_name = remove_unit_from_name(PRCP_NAME)
+    pet_name = remove_unit_from_name(PET_NAME)
+    flow_name = remove_unit_from_name(FLOW_NAME)
+    basin_area = get_basin_area(data_type, data_dir, basin_ids)
+    if data_type == "camels":
+        camels_data_dir = os.path.join(
+            SETTING["local_data_path"]["datasets-origin"], "camels", data_dir
+        )
+        camels = Camels(camels_data_dir)
+        ts_data = camels.read_ts_xrdataset(
+            basin_ids, periods, ["prcp", "PET", "streamflow"]
+        )
+        # trans unit to mm/day
+        qobs_ = ts_data[["streamflow"]]
+        target_unit = ts_data["prcp"].attrs.get("units", "unknown")
+        r_mmd = streamflow_unit_conv(qobs_, basin_area, target_unit=target_unit)
+        ts_data[flow_name] = r_mmd["streamflow"]
+        ts_data[flow_name].attrs["units"] = target_unit
+        ts_data = ts_data.rename({"PET": pet_name})
+        # ts_data = ts_data.drop_vars('streamflow')
+    elif data_type == "owndata":
+        ts_data = xr.open_dataset(os.path.join(data_dir, "timeseries.nc"))
+        target_unit = ts_data[prcp_name].attrs.get("units", "unknown")
+        qobs_ = ts_data[[flow_name]]
+        r_mmd = streamflow_unit_conv(qobs_, basin_area, target_unit=target_unit)
+        ts_data[flow_name] = r_mmd[flow_name]
+        ts_data[flow_name].attrs["units"] = target_unit
+        ts_data = ts_data.sel(time=slice(periods[0], periods[1]))
+    else:
+        raise NotImplementedError(
+            "You should set the data type as 'camels' or 'owndata'"
+        )
+
+    return ts_data
+
+
+def _get_pe_q_from_ts(ts_xr_dataset):
+    """Transform the time series data to the format that can be used in the calibration process
+
+    Parameters
+    ----------
+    ts_xr_dataset : xr.Dataset
+        The time series data
+
+    Returns
+    -------
+    tuple[np.ndarray, np.ndarray]
+        The tuple contains the precipitation and evaporation data and the observed streamflow data
+    """
+    prcp_name = remove_unit_from_name(PRCP_NAME)
+    pet_name = remove_unit_from_name(PET_NAME)
+    flow_name = remove_unit_from_name(FLOW_NAME)
+    p_and_e = (
+        ts_xr_dataset[[prcp_name, pet_name]].to_array().to_numpy().transpose(2, 1, 0)
+    )
+    qobs = np.expand_dims(ts_xr_dataset[flow_name].to_numpy().transpose(1, 0), axis=2)
+
+    return p_and_e, qobs
+
+
+def cross_val_split_tsdata(
+    data_type, data_dir, cv_fold, train_period, test_period, periods, warmup, basin_ids
+):
+    ts_data = get_ts_from_diffsource(data_type, data_dir, periods, basin_ids)
+    if cv_fold <= 1:
+        # no cross validation
+        periods = np.sort(
+            [train_period[0], train_period[1], test_period[0], test_period[1]]
+        )
+        train_and_test_data = split_train_test(ts_data, train_period, test_period)
+    else:
+        # cross validation
+        train_and_test_data = cross_valid_data(ts_data, periods, warmup, cv_fold)
+    return train_and_test_data
+
+
+def get_rr_events(rain, flow, basin_area):
+    ureg = UnitRegistry()
+    # trans unit to mm/day
+    flow_threshold = streamflow_unit_conv(
+        np.array([100]) * ureg.m**3 / ureg.s,
+        basin_area.isel(basin=0).to_array().to_numpy() * ureg.km**2,
+        target_unit="mm/h",
+    )
+    rr_events = {}
+    for basin in basin_area.basin.values:
+        rr_event = rainfall_runoff_event_identify(
+            rain.sel(basin=basin).to_series(),
+            flow.sel(basin=basin).to_series(),
+            multiple=1,
+            flow_threshold=flow_threshold[0],
+        )
+        rr_events[basin] = rr_event
+    return rr_events
```

### Comparing `hydromodel-0.2.2/hydromodel/datasets/data_visualize.py` & `hydromodel-0.2.3/hydromodel/datasets/data_visualize.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,338 +1,338 @@
-"""Show results of calibration and validation."""
-
-import os
-from matplotlib import dates, pyplot as plt
-import numpy as np
-import pandas as pd
-
-from hydroutils import hydro_file, hydro_stat, hydro_plot
-
-
-def plot_sim_and_obs(
-    date,
-    sim,
-    obs,
-    save_fig,
-    xlabel="Date",
-    ylabel=None,
-):
-    # matplotlib.use("Agg")
-    fig = plt.figure(figsize=(9, 6))
-    ax = fig.subplots()
-    ax.plot(
-        date,
-        sim,
-        color="black",
-        linestyle="solid",
-        label="Simulation",
-    )
-    ax.plot(
-        date,
-        obs,
-        "r.",
-        markersize=3,
-        label="Observation",
-    )
-    ax.set_xlabel(xlabel)
-    ax.set_ylabel(ylabel)
-    plt.legend(loc="upper right")
-    plt.tight_layout()
-    plt.savefig(save_fig, bbox_inches="tight")
-    # plt.cla()
-    plt.close()
-
-
-def plot_train_iteration(likelihood, save_fig):
-    # matplotlib.use("Agg")
-    fig = plt.figure(figsize=(9, 6))
-    ax = fig.subplots()
-    ax.plot(likelihood)
-    ax.set_ylabel("RMSE")
-    ax.set_xlabel("Iteration")
-    plt.savefig(save_fig, bbox_inches="tight")
-    # plt.cla()
-    plt.close()
-
-
-def plot_rr_events(rr_events, rain, flow, save_dir=None):
-    for i in range(len(rr_events)):
-        beginning_time = rr_events["BEGINNING_RAIN"].iloc[i]
-        end_time = rr_events["END_FLOW"].iloc[i]  # Ensure this column exists
-
-        # Filter data for the specific time period
-        filtered_rain_data = rain.sel(time=slice(beginning_time, end_time))
-        filter_flow_data = flow.sel(time=slice(beginning_time, end_time))
-
-        # Plotting
-        hydro_plot.plot_rainfall_runoff(
-            filtered_rain_data.time.values,
-            filtered_rain_data.values,
-            [filter_flow_data.values],
-            title=f"Rainfall-Runoff Event {i}",
-            leg_lst=["Flow"],
-            xlabel="Time",
-            ylabel="Flow (mm/h)",
-        )
-        if save_dir:
-            if not os.path.exists(save_dir):
-                os.makedirs(save_dir)
-            save_fig = os.path.join(save_dir, f"rr_event_{i}.png")
-            plt.savefig(save_fig, bbox_inches="tight")
-
-
-def show_events_result(
-    warmup_length,
-    save_dir,
-    train_period,
-    basin_area=None,
-    prcp=None,
-):
-    """
-    Plot all events result to see the effect of optimized parameters
-
-    Parameters
-    ----------
-    sceua_calibrated_file
-        the result file saved after optimizing
-    basin_id
-        id of the basin
-    train_period
-        the period of training data
-    result_unit
-        the unit of result, default is mm/day, we will convert it to m3/s
-    basin_area
-        the area of the basin, its unit must be km2
-
-    Returns
-    -------
-    None
-    """
-    # TODO: not finished
-    time = pd.read_excel(
-        "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/洪水率定时间.xlsx"
-    )
-    calibrate_starttime = pd.to_datetime("2012-06-10 0:00:00")
-    calibrate_endtime = pd.to_datetime("2019-12-31 23:00:00")
-    basin_area = float(basin_area)
-    best_simulation = [
-        x * (basin_area * 1000000 / 1000 / 3600) for x in best_simulation
-    ]
-    obs = [x * (basin_area * 1000000 / 1000 / 3600) for x in spot_setup.evaluation()]
-    time["starttime"] = pd.to_datetime(time["starttime"])
-    time["endtime"] = pd.to_datetime(time["endtime"])
-    Prcp_list = []
-    W_obs_list = []
-    W_sim_list = []
-    W_bias_abs_list = []
-    W_bias_rela_list = []
-    Q_max_obs_list = []
-    Q_max_sim_list = []
-    Q_bias_rela_list = []
-    time_bias_list = []
-    DC_list = []
-    ID_list = []
-    for i, row in time.iterrows():
-        # for i in range(len(time)):
-        if row["starttime"] < calibrate_endtime:
-            # if(time["starttime",0]<calibrate_endtime):
-            start_num = (
-                row["starttime"]
-                - calibrate_starttime
-                - pd.Timedelta(hours=warmup_length)
-            ) / pd.Timedelta(hours=1)
-            end_num = (
-                row["endtime"] - calibrate_starttime - pd.Timedelta(hours=warmup_length)
-            ) / pd.Timedelta(hours=1)
-            start_period = (row["endtime"] - calibrate_starttime) / pd.Timedelta(
-                hours=1
-            )
-            end_period = (row["endtime"] - calibrate_starttime) / pd.Timedelta(hours=1)
-            start_period = int(start_period)
-            end_period = int(end_period)
-            start_num = int(start_num)
-            end_num = int(end_num)
-            t_range_train_changci = pd.date_range(
-                row["starttime"], row["endtime"], freq="H"
-            )
-            save_fig = os.path.join(save_dir, "train_results" + str(i) + ".png")
-            best_simulation_changci = best_simulation[start_num : end_num + 1]
-            plot_sim_and_obs(
-                t_range_train_changci,
-                best_simulation[start_num : end_num + 1],
-                obs[start_num : end_num + 1],
-                prcp[start_num : end_num + 1],
-                save_fig,
-            )
-            Prcp = sum(prcp[start_num : end_num + 1])
-            W_obs = (
-                sum(obs[start_num : end_num + 1]) * 3600 * 1000 / basin_area / 1000000
-            )
-            W_sim = sum(best_simulation_changci) * 3600 * 1000 / basin_area / 1000000
-            W_bias_abs = W_sim - W_obs
-            W_bias_rela = W_bias_abs / W_obs
-            Q_max_obs = np.max(obs[start_num : end_num + 1])
-            Q_max_sim = np.max(best_simulation_changci)
-            Q_bias_rela = (Q_max_sim - Q_max_obs) / Q_max_obs
-            t1 = np.argmax(best_simulation_changci)
-            t2 = np.argmax(obs[start_num : end_num + 1])
-            time_bias = t1 - t2
-            DC = NSE(obs[start_num : end_num + 1], best_simulation_changci)
-            ID = row["starttime"].strftime("%Y%m%d")
-            Prcp_list.append(Prcp)
-            W_obs_list.append(W_obs)
-            W_sim_list.append(W_sim)
-            W_bias_abs_list.append(W_bias_abs)
-            W_bias_rela_list.append(W_bias_rela)
-            Q_max_obs_list.append(Q_max_obs)
-            Q_max_sim_list.append(Q_max_sim)
-            Q_bias_rela_list.append(Q_bias_rela)
-            time_bias_list.append(time_bias)
-
-            DC_list.append(DC)
-            ID_list.append(ID)
-
-    bias = pd.DataFrame(
-        {
-            "Prcp(mm)": Prcp_list,
-            "W_obs(mm)": W_obs_list,
-            "W_sim(mm)": W_sim_list,
-            "W_bias_abs": W_bias_abs_list,
-            "W_bias_rela": W_bias_rela_list,
-            "Q_max_obs(m3/s)": Q_max_obs_list,
-            "Q_max_sim(m3/s)": Q_max_sim_list,
-            "Q_bias_rela": Q_bias_rela_list,
-            "time_bias": time_bias_list,
-            "DC": DC_list,
-            "ID": ID_list,
-        }
-    )
-    bias.to_csv(
-        os.path.join(
-            "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/train_metrics.csv"
-        )
-    )
-    t_range_train = pd.to_datetime(train_period[warmup_length:]).values.astype(
-        "datetime64[h]"
-    )
-    save_fig = os.path.join(save_dir, "train_results.png")  # 生成结果图
-    plot_sim_and_obs(t_range_train, best_simulation, obs, prcp[:], save_fig)
-
-
-def show_ts_result(basin_id, test_date, qsim, obs, save_dir):
-    stat_error = hydro_stat.stat_error(obs.reshape(1, -1), qsim.reshape(1, -1))
-    print("Test Metrics:", basin_id, stat_error)
-    hydro_file.serialize_json_np(
-        stat_error, os.path.join(save_dir, "test_metrics.json")
-    )
-    time = pd.read_excel(
-        "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/洪水率定时间.xlsx"
-    )
-    test_starttime = pd.to_datetime("2020-01-01 00:00:00")
-    test_endtime = pd.to_datetime("2022-08-31 23:00:00")
-    # for i in range(len(time)):
-    #     if(test_starttime<time.iloc[i,0]<test_endtime):
-    #             start_num = (time.iloc[i,0]-test_starttime-pd.Timedelta(hours=warmup_length))/pd.Timedelta(hours=1)
-    #             end_num = (time.iloc[i,1]-test_starttime-pd.Timedelta(hours=warmup_length))/pd.Timedelta(hours=1)
-    #             start_period = (time.iloc[i,0]-test_starttime)/pd.Timedelta(hours=1)
-    #             end_period = (time.iloc[i,1]-test_starttime)/pd.Timedelta(hours=1)
-    #             start_period = int(start_period)
-    #             end_period = int(end_period)
-    #             start_num = int(start_num)
-    #             end_num = int(end_num)
-    #             t_range_test_changci = pd.to_datetime(test_date[start_period:end_period]).values.astype("datetime64[h]")
-    #             save_fig = os.path.join(save_dir, "test_results"+str(i)+".png")
-    #             plot_sim_and_obs(t_range_test_changci, qsim.flatten()[start_num:end_num],obs.flatten()[start_num:end_num], prcp[start_num:end_num],save_fig)
-    Prcp_list = []
-    W_obs_list = []
-    W_sim_list = []
-    W_bias_abs_list = []
-    W_bias_rela_list = []
-    Q_max_obs_list = []
-    Q_max_sim_list = []
-    Q_bias_rela_list = []
-    time_bias_list = []
-    DC_list = []
-    ID_list = []
-    for i, row in time.iterrows():
-        if test_starttime < row["starttime"] < test_endtime:
-            start_num = (
-                row["starttime"] - test_starttime - pd.Timedelta(hours=warmup_length)
-            ) / pd.Timedelta(hours=1)
-            end_num = (
-                row["endtime"] - test_starttime - pd.Timedelta(hours=warmup_length)
-            ) / pd.Timedelta(hours=1)
-            start_period = (row["endtime"] - test_starttime) / pd.Timedelta(hours=1)
-            end_period = (row["endtime"] - test_starttime) / pd.Timedelta(hours=1)
-            start_period = int(start_period)
-            end_period = int(end_period)
-            start_num = int(start_num)
-            end_num = int(end_num)
-            t_range_train_changci = pd.date_range(
-                row["starttime"], row["endtime"], freq="H"
-            )
-            save_fig = os.path.join(save_dir, "test_results" + str(i) + ".png")
-            plot_sim_and_obs(
-                t_range_train_changci,
-                qsim.flatten()[start_num : end_num + 1],
-                obs.flatten()[start_num : end_num + 1],
-                prcp[start_num : end_num + 1],
-                save_fig,
-            )
-            Prcp = sum(prcp[start_num : end_num + 1])
-            W_obs = sum(obs.flatten()[start_num : end_num + 1])
-            W_sim = sum(qsim.flatten()[start_num : end_num + 1])
-            W_bias_abs = W_sim - W_obs
-            W_bias_rela = W_bias_abs / W_obs
-            Q_max_obs = np.max(obs[start_num : end_num + 1])
-            Q_max_sim = np.max(qsim.flatten()[start_num : end_num + 1])
-            Q_bias_rela = (Q_max_sim - Q_max_obs) / Q_max_obs
-            t1 = np.argmax(qsim.flatten()[start_num : end_num + 1])
-            t2 = np.argmax(obs[start_num : end_num + 1])
-            time_bias = t1 - t2
-            DC = NSE(
-                obs.flatten()[start_num : end_num + 1],
-                qsim.flatten()[start_num : end_num + 1],
-            )
-            ID = row["starttime"].strftime("%Y%m%d")
-            Prcp_list.append(Prcp)
-            W_obs_list.append(W_obs)
-            W_sim_list.append(W_sim)
-            W_bias_abs_list.append(W_bias_abs)
-            W_bias_rela_list.append(W_bias_rela)
-            Q_max_obs_list.append(Q_max_obs)
-            Q_max_sim_list.append(Q_max_sim)
-            Q_bias_rela_list.append(Q_bias_rela)
-            time_bias_list.append(time_bias)
-            DC_list.append(DC)
-            ID_list.append(ID)
-
-    bias = pd.DataFrame(
-        {
-            "Prcp(mm)": Prcp_list,
-            "W_obs(mm)": W_obs_list,
-            "W_sim(mm)": W_sim_list,
-            "W_bias_abs": W_bias_abs_list,
-            "W_bias_rela": W_bias_rela_list,
-            "Q_max_obs(m3/s)": Q_max_obs_list,
-            "Q_max_sim(m3/s)": Q_max_sim_list,
-            "Q_bias_rela": Q_bias_rela_list,
-            "time_bias": time_bias_list,
-            "DC": DC_list,
-            "ID": ID_list,
-        }
-    )
-    bias.to_csv(
-        os.path.join(
-            "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/test_metrics.csv"
-        )
-    )
-
-    save_fig = os.path.join(save_dir, "test_results.png")
-
-    plot_sim_and_obs(
-        test_date[365:],
-        qsim.flatten(),
-        obs.flatten(),
-        prcp[:],
-        save_fig,
-    )
+"""Show results of calibration and validation."""
+
+import os
+from matplotlib import dates, pyplot as plt
+import numpy as np
+import pandas as pd
+
+from hydroutils import hydro_file, hydro_stat, hydro_plot
+
+
+def plot_sim_and_obs(
+    date,
+    sim,
+    obs,
+    save_fig,
+    xlabel="Date",
+    ylabel=None,
+):
+    # matplotlib.use("Agg")
+    fig = plt.figure(figsize=(9, 6))
+    ax = fig.subplots()
+    ax.plot(
+        date,
+        sim,
+        color="black",
+        linestyle="solid",
+        label="Simulation",
+    )
+    ax.plot(
+        date,
+        obs,
+        "r.",
+        markersize=3,
+        label="Observation",
+    )
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
+    plt.legend(loc="upper right")
+    plt.tight_layout()
+    plt.savefig(save_fig, bbox_inches="tight")
+    # plt.cla()
+    plt.close()
+
+
+def plot_train_iteration(likelihood, save_fig):
+    # matplotlib.use("Agg")
+    fig = plt.figure(figsize=(9, 6))
+    ax = fig.subplots()
+    ax.plot(likelihood)
+    ax.set_ylabel("RMSE")
+    ax.set_xlabel("Iteration")
+    plt.savefig(save_fig, bbox_inches="tight")
+    # plt.cla()
+    plt.close()
+
+
+def plot_rr_events(rr_events, rain, flow, save_dir=None):
+    for i in range(len(rr_events)):
+        beginning_time = rr_events["BEGINNING_RAIN"].iloc[i]
+        end_time = rr_events["END_FLOW"].iloc[i]  # Ensure this column exists
+
+        # Filter data for the specific time period
+        filtered_rain_data = rain.sel(time=slice(beginning_time, end_time))
+        filter_flow_data = flow.sel(time=slice(beginning_time, end_time))
+
+        # Plotting
+        hydro_plot.plot_rainfall_runoff(
+            filtered_rain_data.time.values,
+            filtered_rain_data.values,
+            [filter_flow_data.values],
+            title=f"Rainfall-Runoff Event {i}",
+            leg_lst=["Flow"],
+            xlabel="Time",
+            ylabel="Flow (mm/h)",
+        )
+        if save_dir:
+            if not os.path.exists(save_dir):
+                os.makedirs(save_dir)
+            save_fig = os.path.join(save_dir, f"rr_event_{i}.png")
+            plt.savefig(save_fig, bbox_inches="tight")
+
+
+def show_events_result(
+    warmup_length,
+    save_dir,
+    train_period,
+    basin_area=None,
+    prcp=None,
+):
+    """
+    Plot all events result to see the effect of optimized parameters
+
+    Parameters
+    ----------
+    sceua_calibrated_file
+        the result file saved after optimizing
+    basin_id
+        id of the basin
+    train_period
+        the period of training data
+    result_unit
+        the unit of result, default is mm/day, we will convert it to m3/s
+    basin_area
+        the area of the basin, its unit must be km2
+
+    Returns
+    -------
+    None
+    """
+    # TODO: not finished
+    time = pd.read_excel(
+        "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/洪水率定时间.xlsx"
+    )
+    calibrate_starttime = pd.to_datetime("2012-06-10 0:00:00")
+    calibrate_endtime = pd.to_datetime("2019-12-31 23:00:00")
+    basin_area = float(basin_area)
+    best_simulation = [
+        x * (basin_area * 1000000 / 1000 / 3600) for x in best_simulation
+    ]
+    obs = [x * (basin_area * 1000000 / 1000 / 3600) for x in spot_setup.evaluation()]
+    time["starttime"] = pd.to_datetime(time["starttime"])
+    time["endtime"] = pd.to_datetime(time["endtime"])
+    Prcp_list = []
+    W_obs_list = []
+    W_sim_list = []
+    W_bias_abs_list = []
+    W_bias_rela_list = []
+    Q_max_obs_list = []
+    Q_max_sim_list = []
+    Q_bias_rela_list = []
+    time_bias_list = []
+    DC_list = []
+    ID_list = []
+    for i, row in time.iterrows():
+        # for i in range(len(time)):
+        if row["starttime"] < calibrate_endtime:
+            # if(time["starttime",0]<calibrate_endtime):
+            start_num = (
+                row["starttime"]
+                - calibrate_starttime
+                - pd.Timedelta(hours=warmup_length)
+            ) / pd.Timedelta(hours=1)
+            end_num = (
+                row["endtime"] - calibrate_starttime - pd.Timedelta(hours=warmup_length)
+            ) / pd.Timedelta(hours=1)
+            start_period = (row["endtime"] - calibrate_starttime) / pd.Timedelta(
+                hours=1
+            )
+            end_period = (row["endtime"] - calibrate_starttime) / pd.Timedelta(hours=1)
+            start_period = int(start_period)
+            end_period = int(end_period)
+            start_num = int(start_num)
+            end_num = int(end_num)
+            t_range_train_changci = pd.date_range(
+                row["starttime"], row["endtime"], freq="H"
+            )
+            save_fig = os.path.join(save_dir, "train_results" + str(i) + ".png")
+            best_simulation_changci = best_simulation[start_num : end_num + 1]
+            plot_sim_and_obs(
+                t_range_train_changci,
+                best_simulation[start_num : end_num + 1],
+                obs[start_num : end_num + 1],
+                prcp[start_num : end_num + 1],
+                save_fig,
+            )
+            Prcp = sum(prcp[start_num : end_num + 1])
+            W_obs = (
+                sum(obs[start_num : end_num + 1]) * 3600 * 1000 / basin_area / 1000000
+            )
+            W_sim = sum(best_simulation_changci) * 3600 * 1000 / basin_area / 1000000
+            W_bias_abs = W_sim - W_obs
+            W_bias_rela = W_bias_abs / W_obs
+            Q_max_obs = np.max(obs[start_num : end_num + 1])
+            Q_max_sim = np.max(best_simulation_changci)
+            Q_bias_rela = (Q_max_sim - Q_max_obs) / Q_max_obs
+            t1 = np.argmax(best_simulation_changci)
+            t2 = np.argmax(obs[start_num : end_num + 1])
+            time_bias = t1 - t2
+            DC = NSE(obs[start_num : end_num + 1], best_simulation_changci)
+            ID = row["starttime"].strftime("%Y%m%d")
+            Prcp_list.append(Prcp)
+            W_obs_list.append(W_obs)
+            W_sim_list.append(W_sim)
+            W_bias_abs_list.append(W_bias_abs)
+            W_bias_rela_list.append(W_bias_rela)
+            Q_max_obs_list.append(Q_max_obs)
+            Q_max_sim_list.append(Q_max_sim)
+            Q_bias_rela_list.append(Q_bias_rela)
+            time_bias_list.append(time_bias)
+
+            DC_list.append(DC)
+            ID_list.append(ID)
+
+    bias = pd.DataFrame(
+        {
+            "Prcp(mm)": Prcp_list,
+            "W_obs(mm)": W_obs_list,
+            "W_sim(mm)": W_sim_list,
+            "W_bias_abs": W_bias_abs_list,
+            "W_bias_rela": W_bias_rela_list,
+            "Q_max_obs(m3/s)": Q_max_obs_list,
+            "Q_max_sim(m3/s)": Q_max_sim_list,
+            "Q_bias_rela": Q_bias_rela_list,
+            "time_bias": time_bias_list,
+            "DC": DC_list,
+            "ID": ID_list,
+        }
+    )
+    bias.to_csv(
+        os.path.join(
+            "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/train_metrics.csv"
+        )
+    )
+    t_range_train = pd.to_datetime(train_period[warmup_length:]).values.astype(
+        "datetime64[h]"
+    )
+    save_fig = os.path.join(save_dir, "train_results.png")  # 生成结果图
+    plot_sim_and_obs(t_range_train, best_simulation, obs, prcp[:], save_fig)
+
+
+def show_ts_result(basin_id, test_date, qsim, obs, save_dir):
+    stat_error = hydro_stat.stat_error(obs.reshape(1, -1), qsim.reshape(1, -1))
+    print("Test Metrics:", basin_id, stat_error)
+    hydro_file.serialize_json_np(
+        stat_error, os.path.join(save_dir, "test_metrics.json")
+    )
+    time = pd.read_excel(
+        "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/洪水率定时间.xlsx"
+    )
+    test_starttime = pd.to_datetime("2020-01-01 00:00:00")
+    test_endtime = pd.to_datetime("2022-08-31 23:00:00")
+    # for i in range(len(time)):
+    #     if(test_starttime<time.iloc[i,0]<test_endtime):
+    #             start_num = (time.iloc[i,0]-test_starttime-pd.Timedelta(hours=warmup_length))/pd.Timedelta(hours=1)
+    #             end_num = (time.iloc[i,1]-test_starttime-pd.Timedelta(hours=warmup_length))/pd.Timedelta(hours=1)
+    #             start_period = (time.iloc[i,0]-test_starttime)/pd.Timedelta(hours=1)
+    #             end_period = (time.iloc[i,1]-test_starttime)/pd.Timedelta(hours=1)
+    #             start_period = int(start_period)
+    #             end_period = int(end_period)
+    #             start_num = int(start_num)
+    #             end_num = int(end_num)
+    #             t_range_test_changci = pd.to_datetime(test_date[start_period:end_period]).values.astype("datetime64[h]")
+    #             save_fig = os.path.join(save_dir, "test_results"+str(i)+".png")
+    #             plot_sim_and_obs(t_range_test_changci, qsim.flatten()[start_num:end_num],obs.flatten()[start_num:end_num], prcp[start_num:end_num],save_fig)
+    Prcp_list = []
+    W_obs_list = []
+    W_sim_list = []
+    W_bias_abs_list = []
+    W_bias_rela_list = []
+    Q_max_obs_list = []
+    Q_max_sim_list = []
+    Q_bias_rela_list = []
+    time_bias_list = []
+    DC_list = []
+    ID_list = []
+    for i, row in time.iterrows():
+        if test_starttime < row["starttime"] < test_endtime:
+            start_num = (
+                row["starttime"] - test_starttime - pd.Timedelta(hours=warmup_length)
+            ) / pd.Timedelta(hours=1)
+            end_num = (
+                row["endtime"] - test_starttime - pd.Timedelta(hours=warmup_length)
+            ) / pd.Timedelta(hours=1)
+            start_period = (row["endtime"] - test_starttime) / pd.Timedelta(hours=1)
+            end_period = (row["endtime"] - test_starttime) / pd.Timedelta(hours=1)
+            start_period = int(start_period)
+            end_period = int(end_period)
+            start_num = int(start_num)
+            end_num = int(end_num)
+            t_range_train_changci = pd.date_range(
+                row["starttime"], row["endtime"], freq="H"
+            )
+            save_fig = os.path.join(save_dir, "test_results" + str(i) + ".png")
+            plot_sim_and_obs(
+                t_range_train_changci,
+                qsim.flatten()[start_num : end_num + 1],
+                obs.flatten()[start_num : end_num + 1],
+                prcp[start_num : end_num + 1],
+                save_fig,
+            )
+            Prcp = sum(prcp[start_num : end_num + 1])
+            W_obs = sum(obs.flatten()[start_num : end_num + 1])
+            W_sim = sum(qsim.flatten()[start_num : end_num + 1])
+            W_bias_abs = W_sim - W_obs
+            W_bias_rela = W_bias_abs / W_obs
+            Q_max_obs = np.max(obs[start_num : end_num + 1])
+            Q_max_sim = np.max(qsim.flatten()[start_num : end_num + 1])
+            Q_bias_rela = (Q_max_sim - Q_max_obs) / Q_max_obs
+            t1 = np.argmax(qsim.flatten()[start_num : end_num + 1])
+            t2 = np.argmax(obs[start_num : end_num + 1])
+            time_bias = t1 - t2
+            DC = NSE(
+                obs.flatten()[start_num : end_num + 1],
+                qsim.flatten()[start_num : end_num + 1],
+            )
+            ID = row["starttime"].strftime("%Y%m%d")
+            Prcp_list.append(Prcp)
+            W_obs_list.append(W_obs)
+            W_sim_list.append(W_sim)
+            W_bias_abs_list.append(W_bias_abs)
+            W_bias_rela_list.append(W_bias_rela)
+            Q_max_obs_list.append(Q_max_obs)
+            Q_max_sim_list.append(Q_max_sim)
+            Q_bias_rela_list.append(Q_bias_rela)
+            time_bias_list.append(time_bias)
+            DC_list.append(DC)
+            ID_list.append(ID)
+
+    bias = pd.DataFrame(
+        {
+            "Prcp(mm)": Prcp_list,
+            "W_obs(mm)": W_obs_list,
+            "W_sim(mm)": W_sim_list,
+            "W_bias_abs": W_bias_abs_list,
+            "W_bias_rela": W_bias_rela_list,
+            "Q_max_obs(m3/s)": Q_max_obs_list,
+            "Q_max_sim(m3/s)": Q_max_sim_list,
+            "Q_bias_rela": Q_bias_rela_list,
+            "time_bias": time_bias_list,
+            "DC": DC_list,
+            "ID": ID_list,
+        }
+    )
+    bias.to_csv(
+        os.path.join(
+            "D:/研究生/毕业论文/new毕业论文/预答辩/碧流河水库/站点信息/test_metrics.csv"
+        )
+    )
+
+    save_fig = os.path.join(save_dir, "test_results.png")
+
+    plot_sim_and_obs(
+        test_date[365:],
+        qsim.flatten(),
+        obs.flatten(),
+        prcp[:],
+        save_fig,
+    )
```

### Comparing `hydromodel-0.2.2/hydromodel/models/gr4j.py` & `hydromodel-0.2.3/hydromodel/models/gr4j.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-import math
-from typing import Optional, Tuple
-import numpy as np
-from numba import jit
-
-from hydromodel.models.model_config import read_model_param_dict
-from hydromodel.models.xaj import uh_conv
-
-
-# @jit
-@jit(nopython=True)
-def calculate_precip_store(s, precip_net, x1):
-    """Calculates the amount of rainfall which enters the storage reservoir."""
-    n = x1 * (1.0 - (s / x1) ** 2) * np.tanh(precip_net / x1)
-    d = 1.0 + (s / x1) * np.tanh(precip_net / x1)
-    return n / d
-
-
-# @jit
-@jit(nopython=True)
-def calculate_evap_store(s, evap_net, x1):
-    """Determines the evaporation loss from the production store"""
-    n = s * (2.0 - s / x1) * np.tanh(evap_net / x1)
-    d = 1.0 + (1.0 - s / x1) * np.tanh(evap_net / x1)
-    return n / d
-
-
-# @jit
-@jit(nopython=True)
-def calculate_perc(current_store, x1):
-    """Determines how much water percolates out of the production store to streamflow"""
-    return current_store * (
-        1.0 - (1.0 + (4.0 / 9.0 * current_store / x1) ** 4) ** -0.25
-    )
-
-
-def production(
-    p_and_e: np.array, x1: np.array, s_level: Optional[np.array] = None
-) -> Tuple[np.array, np.array]:
-    """
-    an one-step calculation for production store in GR4J
-    the dimension of the cell: [batch, feature]
-    Parameters
-    ----------
-    p_and_e
-        P is pe[:, 0] and E is pe[:, 1]; similar with the "input" in the RNNCell
-    x1:
-        Storage reservoir parameter;
-    s_level
-        s_level means S in the GR4J Model; similar with the "hx" in the RNNCell
-        Initial value of storage in the storage reservoir.
-    Returns
-    -------
-    tuple
-        contains the Pr and updated S
-    """
-    # Calculate net precipitation and evapotranspiration
-    precip_difference = p_and_e[:, 0] - p_and_e[:, 1]
-    precip_net = np.maximum(precip_difference, 0.0)
-    evap_net = np.maximum(-precip_difference, 0.0)
-
-    if s_level is None:
-        s_level = 0.6 * x1
-
-    # s_level should not be larger than x1
-    s_level = np.clip(s_level, a_min=np.full(s_level.shape, 0.0), a_max=x1)
-
-    # Calculate the fraction of net precipitation that is stored
-    precip_store = calculate_precip_store(s_level, precip_net, x1)
-
-    # Calculate the amount of evaporation from storage
-    evap_store = calculate_evap_store(s_level, evap_net, x1)
-
-    # Update the storage by adding effective precipitation and
-    # removing evaporation
-    s_update = s_level - evap_store + precip_store
-    # s_level should not be larger than self.x1
-    s_update = np.clip(s_update, a_min=np.full(s_update.shape, 0.0), a_max=x1)
-
-    # Update the storage again to reflect percolation out of the store
-    perc = calculate_perc(s_update, x1)
-    s_update = s_update - perc
-    # perc is always lower than S because of the calculation itself, so we don't need clamp here anymore.
-
-    # The precip. for routing is the sum of the rainfall which
-    # did not make it to storage and the percolation from the store
-    current_runoff = perc + (precip_net - precip_store)
-    # TODO: check if evap_store is the real ET
-    return current_runoff, evap_store, s_update
-
-
-# @jit
-@jit(nopython=True)
-def s_curves1(t, x4):
-    """
-    Unit hydrograph ordinates for UH1 derived from S-curves.
-    """
-
-    if t <= 0:
-        return 0
-    elif t < x4:
-        return (t / x4) ** 2.5
-    else:  # t >= x4
-        return 1
-
-
-# @jit
-@jit(nopython=True)
-def s_curves2(t, x4):
-    """
-    Unit hydrograph ordinates for UH2 derived from S-curves.
-    """
-
-    if t <= 0:
-        return 0
-    elif t < x4:
-        return 0.5 * (t / x4) ** 2.5
-    elif t < 2 * x4:
-        return 1 - 0.5 * (2 - t / x4) ** 2.5
-    else:  # t >= x4
-        return 1
-
-
-def uh_gr4j(x4):
-    """
-    Generate the convolution kernel for the convolution operation in routing module of GR4J
-
-    Parameters
-    ----------
-    x4
-        the dim of x4 is [batch]
-    Returns
-    -------
-    list
-        UH1s and UH2s for all basins
-    """
-    uh1_ordinates = []
-    uh2_ordinates = []
-    for i in range(len(x4)):
-        n_uh1 = int(math.ceil(x4[i]))
-        n_uh2 = int(math.ceil(2.0 * x4[i]))
-        uh1_ordinate = np.zeros(n_uh1)
-        uh2_ordinate = np.zeros(n_uh2)
-        for t in range(1, n_uh1 + 1):
-            uh1_ordinate[t - 1] = s_curves1(t, x4[i]) - s_curves1(t - 1, x4[i])
-
-        for t in range(1, n_uh2 + 1):
-            uh2_ordinate[t - 1] = s_curves2(t, x4[i]) - s_curves2(t - 1, x4[i])
-        uh1_ordinates.append(uh1_ordinate)
-        uh2_ordinates.append(uh2_ordinate)
-
-    return uh1_ordinates, uh2_ordinates
-
-
-def routing(q9: np.array, q1: np.array, x2, x3, r_level: Optional[np.array] = None):
-    """
-    the GR4J routing-module unit cell for time-sequence loop
-    Parameters
-    ----------
-    q9
-    q1
-    x2
-        Catchment water exchange parameter
-    x3
-        Routing reservoir parameters
-    r_level
-        Beginning value of storage in the routing reservoir.
-    Returns
-    -------
-    """
-    if r_level is None:
-        r_level = 0.7 * x3
-    # r_level should not be larger than self.x3
-    r_level = np.clip(r_level, a_min=np.full(r_level.shape, 0.0), a_max=x3)
-    groundwater_ex = x2 * (r_level / x3) ** 3.5
-    r_updated = np.maximum(np.full(r_level.shape, 0.0), r_level + q9 + groundwater_ex)
-
-    qr = r_updated * (1.0 - (1.0 + (r_updated / x3) ** 4) ** -0.25)
-    r_updated = r_updated - qr
-
-    qd = np.maximum(np.full(groundwater_ex.shape, 0.0), q1 + groundwater_ex)
-    q = qr + qd
-    return q, r_updated
-
-
-def gr4j(p_and_e, parameters, warmup_length: int, return_state=False, **kwargs):
-    """
-    run GR4J model
-
-    Parameters
-    ----------
-    p_and_e: ndarray
-        3-dim input -- [time, basin, variable]: precipitation and potential evaporation
-    parameters
-        2-dim variable -- [basin, parameter]:
-        the parameters are x1, x2, x3 and x4
-    warmup_length
-        length of warmup period
-    return_state
-        if True, return state values, mainly for warmup periods
-
-    Returns
-    -------
-    Union[np.array, tuple]
-        streamflow or (streamflow, states)
-    """
-    pr_file = kwargs.get("param_range_file", None)
-    model_param_dict = read_model_param_dict(pr_file)
-    x1_scale = model_param_dict["gr4j"]["param_range"]["x1"]
-    x2_sacle = model_param_dict["gr4j"]["param_range"]["x2"]
-    x3_scale = model_param_dict["gr4j"]["param_range"]["x3"]
-    x4_scale = model_param_dict["gr4j"]["param_range"]["x4"]
-    x1 = x1_scale[0] + parameters[:, 0] * (x1_scale[1] - x1_scale[0])
-    x2 = x2_sacle[0] + parameters[:, 1] * (x2_sacle[1] - x2_sacle[0])
-    x3 = x3_scale[0] + parameters[:, 2] * (x3_scale[1] - x3_scale[0])
-    x4 = x4_scale[0] + parameters[:, 3] * (x4_scale[1] - x4_scale[0])
-
-    if warmup_length > 0:
-        # set no_grad for warmup periods
-        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
-        _, _, s0, r0 = gr4j(
-            p_and_e_warmup, parameters, warmup_length=0, return_state=True, **kwargs
-        )
-    else:
-        s0 = 0.5 * x1
-        r0 = 0.5 * x3
-    inputs = p_and_e[warmup_length:, :, :]
-    streamflow_ = np.full(inputs.shape[:2], 0.0)
-    prs = np.full(inputs.shape[:2], 0.0)
-    ets = np.full(inputs.shape[:2], 0.0)
-    for i in range(inputs.shape[0]):
-        if i == 0:
-            pr, et, s = production(inputs[i, :, :], x1, s0)
-        else:
-            pr, et, s = production(inputs[i, :, :], x1, s)
-        prs[i, :] = pr
-        ets[i, :] = et
-    prs_x = np.expand_dims(prs, axis=2)
-    conv_q9, conv_q1 = uh_gr4j(x4)
-    q9 = np.full([inputs.shape[0], inputs.shape[1], 1], 0.0)
-    q1 = np.full([inputs.shape[0], inputs.shape[1], 1], 0.0)
-    for j in range(inputs.shape[1]):
-        q9[:, j : j + 1, :] = uh_conv(
-            prs_x[:, j : j + 1, :], conv_q9[j].reshape(-1, 1, 1)
-        )
-        q1[:, j : j + 1, :] = uh_conv(
-            prs_x[:, j : j + 1, :], conv_q1[j].reshape(-1, 1, 1)
-        )
-    for i in range(inputs.shape[0]):
-        if i == 0:
-            q, r = routing(q9[i, :, 0], q1[i, :, 0], x2, x3, r0)
-        else:
-            q, r = routing(q9[i, :, 0], q1[i, :, 0], x2, x3, r)
-        streamflow_[i, :] = q
-    streamflow = np.expand_dims(streamflow_, axis=2)
-    if return_state:
-        return streamflow, ets, s, r
-    return streamflow, ets
+import math
+from typing import Optional, Tuple
+import numpy as np
+from numba import jit
+
+from hydromodel.models.model_config import read_model_param_dict
+from hydromodel.models.xaj import uh_conv
+
+
+# @jit
+@jit(nopython=True)
+def calculate_precip_store(s, precip_net, x1):
+    """Calculates the amount of rainfall which enters the storage reservoir."""
+    n = x1 * (1.0 - (s / x1) ** 2) * np.tanh(precip_net / x1)
+    d = 1.0 + (s / x1) * np.tanh(precip_net / x1)
+    return n / d
+
+
+# @jit
+@jit(nopython=True)
+def calculate_evap_store(s, evap_net, x1):
+    """Determines the evaporation loss from the production store"""
+    n = s * (2.0 - s / x1) * np.tanh(evap_net / x1)
+    d = 1.0 + (1.0 - s / x1) * np.tanh(evap_net / x1)
+    return n / d
+
+
+# @jit
+@jit(nopython=True)
+def calculate_perc(current_store, x1):
+    """Determines how much water percolates out of the production store to streamflow"""
+    return current_store * (
+        1.0 - (1.0 + (4.0 / 9.0 * current_store / x1) ** 4) ** -0.25
+    )
+
+
+def production(
+    p_and_e: np.array, x1: np.array, s_level: Optional[np.array] = None
+) -> Tuple[np.array, np.array]:
+    """
+    an one-step calculation for production store in GR4J
+    the dimension of the cell: [batch, feature]
+    Parameters
+    ----------
+    p_and_e
+        P is pe[:, 0] and E is pe[:, 1]; similar with the "input" in the RNNCell
+    x1:
+        Storage reservoir parameter;
+    s_level
+        s_level means S in the GR4J Model; similar with the "hx" in the RNNCell
+        Initial value of storage in the storage reservoir.
+    Returns
+    -------
+    tuple
+        contains the Pr and updated S
+    """
+    # Calculate net precipitation and evapotranspiration
+    precip_difference = p_and_e[:, 0] - p_and_e[:, 1]
+    precip_net = np.maximum(precip_difference, 0.0)
+    evap_net = np.maximum(-precip_difference, 0.0)
+
+    if s_level is None:
+        s_level = 0.6 * x1
+
+    # s_level should not be larger than x1
+    s_level = np.clip(s_level, a_min=np.full(s_level.shape, 0.0), a_max=x1)
+
+    # Calculate the fraction of net precipitation that is stored
+    precip_store = calculate_precip_store(s_level, precip_net, x1)
+
+    # Calculate the amount of evaporation from storage
+    evap_store = calculate_evap_store(s_level, evap_net, x1)
+
+    # Update the storage by adding effective precipitation and
+    # removing evaporation
+    s_update = s_level - evap_store + precip_store
+    # s_level should not be larger than self.x1
+    s_update = np.clip(s_update, a_min=np.full(s_update.shape, 0.0), a_max=x1)
+
+    # Update the storage again to reflect percolation out of the store
+    perc = calculate_perc(s_update, x1)
+    s_update = s_update - perc
+    # perc is always lower than S because of the calculation itself, so we don't need clamp here anymore.
+
+    # The precip. for routing is the sum of the rainfall which
+    # did not make it to storage and the percolation from the store
+    current_runoff = perc + (precip_net - precip_store)
+    # TODO: check if evap_store is the real ET
+    return current_runoff, evap_store, s_update
+
+
+# @jit
+@jit(nopython=True)
+def s_curves1(t, x4):
+    """
+    Unit hydrograph ordinates for UH1 derived from S-curves.
+    """
+
+    if t <= 0:
+        return 0
+    elif t < x4:
+        return (t / x4) ** 2.5
+    else:  # t >= x4
+        return 1
+
+
+# @jit
+@jit(nopython=True)
+def s_curves2(t, x4):
+    """
+    Unit hydrograph ordinates for UH2 derived from S-curves.
+    """
+
+    if t <= 0:
+        return 0
+    elif t < x4:
+        return 0.5 * (t / x4) ** 2.5
+    elif t < 2 * x4:
+        return 1 - 0.5 * (2 - t / x4) ** 2.5
+    else:  # t >= x4
+        return 1
+
+
+def uh_gr4j(x4):
+    """
+    Generate the convolution kernel for the convolution operation in routing module of GR4J
+
+    Parameters
+    ----------
+    x4
+        the dim of x4 is [batch]
+    Returns
+    -------
+    list
+        UH1s and UH2s for all basins
+    """
+    uh1_ordinates = []
+    uh2_ordinates = []
+    for i in range(len(x4)):
+        n_uh1 = int(math.ceil(x4[i]))
+        n_uh2 = int(math.ceil(2.0 * x4[i]))
+        uh1_ordinate = np.zeros(n_uh1)
+        uh2_ordinate = np.zeros(n_uh2)
+        for t in range(1, n_uh1 + 1):
+            uh1_ordinate[t - 1] = s_curves1(t, x4[i]) - s_curves1(t - 1, x4[i])
+
+        for t in range(1, n_uh2 + 1):
+            uh2_ordinate[t - 1] = s_curves2(t, x4[i]) - s_curves2(t - 1, x4[i])
+        uh1_ordinates.append(uh1_ordinate)
+        uh2_ordinates.append(uh2_ordinate)
+
+    return uh1_ordinates, uh2_ordinates
+
+
+def routing(q9: np.array, q1: np.array, x2, x3, r_level: Optional[np.array] = None):
+    """
+    the GR4J routing-module unit cell for time-sequence loop
+    Parameters
+    ----------
+    q9
+    q1
+    x2
+        Catchment water exchange parameter
+    x3
+        Routing reservoir parameters
+    r_level
+        Beginning value of storage in the routing reservoir.
+    Returns
+    -------
+    """
+    if r_level is None:
+        r_level = 0.7 * x3
+    # r_level should not be larger than self.x3
+    r_level = np.clip(r_level, a_min=np.full(r_level.shape, 0.0), a_max=x3)
+    groundwater_ex = x2 * (r_level / x3) ** 3.5
+    r_updated = np.maximum(np.full(r_level.shape, 0.0), r_level + q9 + groundwater_ex)
+
+    qr = r_updated * (1.0 - (1.0 + (r_updated / x3) ** 4) ** -0.25)
+    r_updated = r_updated - qr
+
+    qd = np.maximum(np.full(groundwater_ex.shape, 0.0), q1 + groundwater_ex)
+    q = qr + qd
+    return q, r_updated
+
+
+def gr4j(p_and_e, parameters, warmup_length: int, return_state=False, **kwargs):
+    """
+    run GR4J model
+
+    Parameters
+    ----------
+    p_and_e: ndarray
+        3-dim input -- [time, basin, variable]: precipitation and potential evaporation
+    parameters
+        2-dim variable -- [basin, parameter]:
+        the parameters are x1, x2, x3 and x4
+    warmup_length
+        length of warmup period
+    return_state
+        if True, return state values, mainly for warmup periods
+
+    Returns
+    -------
+    Union[np.array, tuple]
+        streamflow or (streamflow, states)
+    """
+    pr_file = kwargs.get("param_range_file", None)
+    model_param_dict = read_model_param_dict(pr_file)
+    x1_scale = model_param_dict["gr4j"]["param_range"]["x1"]
+    x2_sacle = model_param_dict["gr4j"]["param_range"]["x2"]
+    x3_scale = model_param_dict["gr4j"]["param_range"]["x3"]
+    x4_scale = model_param_dict["gr4j"]["param_range"]["x4"]
+    x1 = x1_scale[0] + parameters[:, 0] * (x1_scale[1] - x1_scale[0])
+    x2 = x2_sacle[0] + parameters[:, 1] * (x2_sacle[1] - x2_sacle[0])
+    x3 = x3_scale[0] + parameters[:, 2] * (x3_scale[1] - x3_scale[0])
+    x4 = x4_scale[0] + parameters[:, 3] * (x4_scale[1] - x4_scale[0])
+
+    if warmup_length > 0:
+        # set no_grad for warmup periods
+        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
+        _, _, s0, r0 = gr4j(
+            p_and_e_warmup, parameters, warmup_length=0, return_state=True, **kwargs
+        )
+    else:
+        s0 = 0.5 * x1
+        r0 = 0.5 * x3
+    inputs = p_and_e[warmup_length:, :, :]
+    streamflow_ = np.full(inputs.shape[:2], 0.0)
+    prs = np.full(inputs.shape[:2], 0.0)
+    ets = np.full(inputs.shape[:2], 0.0)
+    for i in range(inputs.shape[0]):
+        if i == 0:
+            pr, et, s = production(inputs[i, :, :], x1, s0)
+        else:
+            pr, et, s = production(inputs[i, :, :], x1, s)
+        prs[i, :] = pr
+        ets[i, :] = et
+    prs_x = np.expand_dims(prs, axis=2)
+    conv_q9, conv_q1 = uh_gr4j(x4)
+    q9 = np.full([inputs.shape[0], inputs.shape[1], 1], 0.0)
+    q1 = np.full([inputs.shape[0], inputs.shape[1], 1], 0.0)
+    for j in range(inputs.shape[1]):
+        q9[:, j : j + 1, :] = uh_conv(
+            prs_x[:, j : j + 1, :], conv_q9[j].reshape(-1, 1, 1)
+        )
+        q1[:, j : j + 1, :] = uh_conv(
+            prs_x[:, j : j + 1, :], conv_q1[j].reshape(-1, 1, 1)
+        )
+    for i in range(inputs.shape[0]):
+        if i == 0:
+            q, r = routing(q9[i, :, 0], q1[i, :, 0], x2, x3, r0)
+        else:
+            q, r = routing(q9[i, :, 0], q1[i, :, 0], x2, x3, r)
+        streamflow_[i, :] = q
+    streamflow = np.expand_dims(streamflow_, axis=2)
+    if return_state:
+        return streamflow, ets, s, r
+    return streamflow, ets
```

### Comparing `hydromodel-0.2.2/hydromodel/models/hymod.py` & `hydromodel-0.2.3/hydromodel/models/hymod.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-from numba import jit
-
-from hydromodel.models.model_config import read_model_param_dict
-
-
-def hymod(p_and_e, parameters, warmup_length=30, return_state=False, **kwargs):
-    """
-    Run Hymod model
-
-    See https://www.proc-iahs.net/368/180/2015/piahs-368-180-2015.pdf for a scientific paper:
-    Quan, Z.; Teng, J.; Sun, W.; Cheng, T. & Zhang, J. (2015): Evaluation of the HYMOD model
-    for rainfall–runoff simulation using the GLUE method. Remote Sensing and GIS for Hydrology
-    and Water Resources, 180 - 185, IAHS Publ. 368. DOI: 10.5194/piahs-368-180-2015.
-
-    Parameters
-    ----------
-    p_and_e
-        precipitation and potential evapotranspiration, 3-dim variable: [time, basin, feature=1]
-    parameters
-         five parameters: cmax, bexp, alpha, ks, kq
-    warmup_length
-        the length of warmup period
-    return_state
-        if True, return x_slow, x_quick, x_loss, else only return streamflow
-
-    Returns
-    -------
-    Union[list, np.array]
-        streamflow, x_slow, x_quick, x_loss or streamflow
-    """
-    pr_file = kwargs.get("param_range_file", None)
-    model_param_dict = read_model_param_dict(pr_file)
-    # parameter, 2-dim variable: [parameter=1, basin]
-    cmax_scale = model_param_dict["hymod"]["param_range"]["cmax"]
-    bexp_sacle = model_param_dict["hymod"]["param_range"]["bexp"]
-    alpha_scale = model_param_dict["hymod"]["param_range"]["alpha"]
-    ks_scale = model_param_dict["hymod"]["param_range"]["ks"]
-    kq_scale = model_param_dict["hymod"]["param_range"]["kq"]
-    cmax = cmax_scale[0] + parameters[:, 0] * (cmax_scale[1] - cmax_scale[0])
-    bexp = bexp_sacle[0] + parameters[:, 1] * (bexp_sacle[1] - bexp_sacle[0])
-    alpha = alpha_scale[0] + parameters[:, 2] * (alpha_scale[1] - alpha_scale[0])
-    ks = ks_scale[0] + parameters[:, 3] * (ks_scale[1] - ks_scale[0])
-    kq = kq_scale[0] + parameters[:, 4] * (kq_scale[1] - kq_scale[0])
-    if warmup_length > 0:
-        # set no_grad for warmup periods
-        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
-        _, _, x_slow, x_quick, x_loss = hymod(
-            p_and_e_warmup,
-            parameters,
-            warmup_length=0,
-            return_state=True,
-            **kwargs,
-        )
-    else:
-        # Initialize slow tank state
-        # x_slow = 2.3503 / (ks * 22.5)
-        x_slow = np.full(
-            (p_and_e.shape[1], 1), 0.0
-        )  # --> works ok if calibration data starts with low discharge
-        # Initialize state(s) of quick tank(s)
-        x_quick = np.full((p_and_e.shape[1], 3), 0.0)
-        # HYMOD PROGRAM IS SIMPLE RAINFALL RUNOFF MODEL
-        x_loss = np.full((p_and_e.shape[1], 1), 0.0)
-    precip = p_and_e[warmup_length:, :, 0]
-    pet = p_and_e[warmup_length:, :, 1]
-    t = 0
-    output = np.full(precip.shape, 0.0)
-    # START PROGRAMMING LOOP WITH DETERMINING RAINFALL - RUNOFF AMOUNTS
-    while t <= precip.shape[0] - 1:
-        pval = precip[t, :]
-        pet_val = pet[t, :]
-        # Compute excess precipitation and evaporation
-        er1, er2, x_loss = excess(x_loss, cmax, bexp, pval, pet_val)
-        # Calculate total effective rainfall
-        et = er1 + er2
-        #  Now partition ER between quick and slow flow reservoirs
-        uq = alpha * et
-        us = (1 - alpha) * et
-        # Route slow flow component with single linear reservoir
-        x_slow, qs = linres(x_slow, us, ks)
-        # Route quick flow component with linear reservoirs
-        inflow = uq
-
-        for i in range(3):
-            # Linear reservoir
-            x_quick[:, i], outflow = linres(x_quick[:, i], inflow, kq)
-            inflow = outflow
-
-        # Compute total flow for timestep
-        output[t, :] = qs + outflow
-        t += 1
-    streamflow = np.expand_dims(output, axis=2)
-    if return_state:
-        return streamflow, et, x_slow, x_quick, x_loss
-    return streamflow, et
-
-
-# @jit
-@jit(nopython=True)
-def power(x, y):
-    x = np.abs(x)  # Needed to capture invalid overflow with negative values
-    return x**y
-
-
-# @jit
-@jit(nopython=True)
-def linres(x_slow, inflow, rs):
-    # Linear reservoir
-    x_slow = (1 - rs) * x_slow + (1 - rs) * inflow
-    outflow = (rs / (1 - rs)) * x_slow
-    return x_slow, outflow
-
-
-# @jit
-@jit(nopython=True)
-def excess(x_loss, cmax, bexp, pval, pet_val):
-    # this function calculates excess precipitation and evaporation
-    xn_prev = x_loss
-    ct_prev = cmax * (
-        1 - power((1 - ((bexp + 1) * (xn_prev) / cmax)), (1 / (bexp + 1)))
-    )
-    # Calculate Effective rainfall 1
-    er1 = np.maximum((pval - cmax + ct_prev), 0.0)
-    pval = pval - er1
-    dummy = np.minimum(((ct_prev + pval) / cmax), 1)
-    xn = (cmax / (bexp + 1)) * (1 - power((1 - dummy), (bexp + 1)))
-
-    # Calculate Effective rainfall 2
-    er2 = np.maximum(pval - (xn - xn_prev), 0)
-
-    # Alternative approach
-    evap = (
-        1 - (((cmax / (bexp + 1)) - xn) / (cmax / (bexp + 1)))
-    ) * pet_val  # actual ET is linearly related to the soil moisture state
-    xn = np.maximum(xn - evap, 0)  # update state
-
-    return er1, er2, xn
+# -*- coding: utf-8 -*-
+import numpy as np
+from numba import jit
+
+from hydromodel.models.model_config import read_model_param_dict
+
+
+def hymod(p_and_e, parameters, warmup_length=30, return_state=False, **kwargs):
+    """
+    Run Hymod model
+
+    See https://www.proc-iahs.net/368/180/2015/piahs-368-180-2015.pdf for a scientific paper:
+    Quan, Z.; Teng, J.; Sun, W.; Cheng, T. & Zhang, J. (2015): Evaluation of the HYMOD model
+    for rainfall–runoff simulation using the GLUE method. Remote Sensing and GIS for Hydrology
+    and Water Resources, 180 - 185, IAHS Publ. 368. DOI: 10.5194/piahs-368-180-2015.
+
+    Parameters
+    ----------
+    p_and_e
+        precipitation and potential evapotranspiration, 3-dim variable: [time, basin, feature=1]
+    parameters
+         five parameters: cmax, bexp, alpha, ks, kq
+    warmup_length
+        the length of warmup period
+    return_state
+        if True, return x_slow, x_quick, x_loss, else only return streamflow
+
+    Returns
+    -------
+    Union[list, np.array]
+        streamflow, x_slow, x_quick, x_loss or streamflow
+    """
+    pr_file = kwargs.get("param_range_file", None)
+    model_param_dict = read_model_param_dict(pr_file)
+    # parameter, 2-dim variable: [parameter=1, basin]
+    cmax_scale = model_param_dict["hymod"]["param_range"]["cmax"]
+    bexp_sacle = model_param_dict["hymod"]["param_range"]["bexp"]
+    alpha_scale = model_param_dict["hymod"]["param_range"]["alpha"]
+    ks_scale = model_param_dict["hymod"]["param_range"]["ks"]
+    kq_scale = model_param_dict["hymod"]["param_range"]["kq"]
+    cmax = cmax_scale[0] + parameters[:, 0] * (cmax_scale[1] - cmax_scale[0])
+    bexp = bexp_sacle[0] + parameters[:, 1] * (bexp_sacle[1] - bexp_sacle[0])
+    alpha = alpha_scale[0] + parameters[:, 2] * (alpha_scale[1] - alpha_scale[0])
+    ks = ks_scale[0] + parameters[:, 3] * (ks_scale[1] - ks_scale[0])
+    kq = kq_scale[0] + parameters[:, 4] * (kq_scale[1] - kq_scale[0])
+    if warmup_length > 0:
+        # set no_grad for warmup periods
+        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
+        _, _, x_slow, x_quick, x_loss = hymod(
+            p_and_e_warmup,
+            parameters,
+            warmup_length=0,
+            return_state=True,
+            **kwargs,
+        )
+    else:
+        # Initialize slow tank state
+        # x_slow = 2.3503 / (ks * 22.5)
+        x_slow = np.full(
+            (p_and_e.shape[1], 1), 0.0
+        )  # --> works ok if calibration data starts with low discharge
+        # Initialize state(s) of quick tank(s)
+        x_quick = np.full((p_and_e.shape[1], 3), 0.0)
+        # HYMOD PROGRAM IS SIMPLE RAINFALL RUNOFF MODEL
+        x_loss = np.full((p_and_e.shape[1], 1), 0.0)
+    precip = p_and_e[warmup_length:, :, 0]
+    pet = p_and_e[warmup_length:, :, 1]
+    t = 0
+    output = np.full(precip.shape, 0.0)
+    # START PROGRAMMING LOOP WITH DETERMINING RAINFALL - RUNOFF AMOUNTS
+    while t <= precip.shape[0] - 1:
+        pval = precip[t, :]
+        pet_val = pet[t, :]
+        # Compute excess precipitation and evaporation
+        er1, er2, x_loss = excess(x_loss, cmax, bexp, pval, pet_val)
+        # Calculate total effective rainfall
+        et = er1 + er2
+        #  Now partition ER between quick and slow flow reservoirs
+        uq = alpha * et
+        us = (1 - alpha) * et
+        # Route slow flow component with single linear reservoir
+        x_slow, qs = linres(x_slow, us, ks)
+        # Route quick flow component with linear reservoirs
+        inflow = uq
+
+        for i in range(3):
+            # Linear reservoir
+            x_quick[:, i], outflow = linres(x_quick[:, i], inflow, kq)
+            inflow = outflow
+
+        # Compute total flow for timestep
+        output[t, :] = qs + outflow
+        t += 1
+    streamflow = np.expand_dims(output, axis=2)
+    if return_state:
+        return streamflow, et, x_slow, x_quick, x_loss
+    return streamflow, et
+
+
+# @jit
+@jit(nopython=True)
+def power(x, y):
+    x = np.abs(x)  # Needed to capture invalid overflow with negative values
+    return x**y
+
+
+# @jit
+@jit(nopython=True)
+def linres(x_slow, inflow, rs):
+    # Linear reservoir
+    x_slow = (1 - rs) * x_slow + (1 - rs) * inflow
+    outflow = (rs / (1 - rs)) * x_slow
+    return x_slow, outflow
+
+
+# @jit
+@jit(nopython=True)
+def excess(x_loss, cmax, bexp, pval, pet_val):
+    # this function calculates excess precipitation and evaporation
+    xn_prev = x_loss
+    ct_prev = cmax * (
+        1 - power((1 - ((bexp + 1) * (xn_prev) / cmax)), (1 / (bexp + 1)))
+    )
+    # Calculate Effective rainfall 1
+    er1 = np.maximum((pval - cmax + ct_prev), 0.0)
+    pval = pval - er1
+    dummy = np.minimum(((ct_prev + pval) / cmax), 1)
+    xn = (cmax / (bexp + 1)) * (1 - power((1 - dummy), (bexp + 1)))
+
+    # Calculate Effective rainfall 2
+    er2 = np.maximum(pval - (xn - xn_prev), 0)
+
+    # Alternative approach
+    evap = (
+        1 - (((cmax / (bexp + 1)) - xn) / (cmax / (bexp + 1)))
+    ) * pet_val  # actual ET is linearly related to the soil moisture state
+    xn = np.maximum(xn - evap, 0)  # update state
+
+    return er1, er2, xn
```

### Comparing `hydromodel-0.2.2/hydromodel/models/model_config.py` & `hydromodel-0.2.3/hydromodel/models/model_config.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-"""
-Author: Wenyu Ouyang
-Date: 2022-10-25 21:16:22
-LastEditTime: 2024-03-27 16:16:25
-LastEditors: Wenyu Ouyang
-Description: some basic config for hydro-model-xaj models
-FilePath: \hydro-model-xaj\hydromodel\models\model_config.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-
-from collections import OrderedDict
-
-import yaml
-
-
-def read_model_param_dict(file_path="param.yaml"):
-    try:
-        with open(file_path, "r") as file:
-            data = yaml.safe_load(file)
-
-        return {
-            model: {
-                "param_name": contents["param_name"],
-                "param_range": OrderedDict(contents["param_range"]),
-            }
-            for model, contents in data.items()
-        }
-    except Exception as e:
-        print(f"Error: {e}, we directly use the default MODEL_PARAM_DICT.")
-        return MODEL_PARAM_DICT
-
-
-MODEL_PARAM_DICT = {
-    "xaj": {
-        "param_name": [
-            # Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998.
-            # Crop Evapotranspiration, Food and Agriculture Organization of the United Nations,
-            # Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
-            "K",  # ratio of potential evapotranspiration to reference crop evaporation generally from Allen, 1998
-            "B",  # The exponent of the tension water capacity curve
-            "IM",  # The ratio of the impervious to the total area of the basin
-            "UM",  # Tension water capacity in the upper layer
-            "LM",  # Tension water capacity in the lower layer
-            "DM",  # Tension water capacity in the deepest layer
-            "C",  # The coefficient of deep evapotranspiration
-            "SM",  # The areal mean of the free water capacity of surface soil layer
-            "EX",  # The exponent of the free water capacity curve
-            "KI",  # Outflow coefficients of interflow
-            "KG",  # Outflow coefficients of groundwater
-            "CS",  # The recession constant of channel system
-            "L",  # Lag time
-            "CI",  # The recession constant of the lower interflow
-            "CG",  # The recession constant of groundwater storage
-        ],
-        "param_range": OrderedDict(
-            {
-                "K": [0.1, 1.0],
-                "B": [0.1, 0.4],
-                "IM": [0.01, 0.1],
-                "UM": [0.0, 20.0],
-                "LM": [60.0, 90.0],
-                "DM": [60.0, 120.0],
-                "C": [0.0, 0.2],
-                "SM": [1, 100.0],
-                # "SM": [50, 100.0],
-                "EX": [1.0, 1.5],
-                "KI": [0.0, 0.7],
-                "KG": [0.0, 0.7],
-                "CS": [0.0, 1.0],
-                "L": [1.0, 10.0],  # unit is same as your time step
-                "CI": [0.0, 0.9],
-                "CG": [0.98, 0.998],
-            }
-        ),
-    },
-    "xaj_mz": {
-        "param_name": [
-            # Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998.
-            # Crop Evapotranspiration, Food and Agriculture Organization of the United Nations,
-            # Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
-            "K",  # ratio of potential evapotranspiration to reference crop evaporation generally from Allen, 1998
-            "B",  # The exponent of the tension water capacity curve
-            "IM",  # The ratio of the impervious to the total area of the basin
-            "UM",  # Tension water capacity in the upper layer
-            "LM",  # Tension water capacity in the lower layer
-            "DM",  # Tension water capacity in the deepest layer
-            "C",  # The coefficient of deep evapotranspiration
-            "SM",  # The areal mean of the free water capacity of surface soil layer
-            "EX",  # The exponent of the free water capacity curve
-            "KI",  # Outflow coefficients of interflow
-            "KG",  # Outflow coefficients of groundwater
-            "A",  # parameter of mizuRoute
-            "THETA",  # parameter of mizuRoute
-            "CI",  # The recession constant of the lower interflow
-            "CG",  # The recession constant of groundwater storage
-            "KERNEL",  # kernel size of mizuRoute unit hydrograph when using convolution method
-        ],
-        "param_range": OrderedDict(
-            {
-                "K": [0.1, 1.0],
-                # "K": [0.5, 1.0],
-                "B": [0.1, 0.4],
-                # "B": [0.2, 0.4],
-                "IM": [0.01, 0.1],
-                # "IM": [0.07, 0.1],
-                "UM": [0.0, 20.0],
-                "LM": [60.0, 90.0],
-                "DM": [60.0, 120.0],
-                "C": [0.0, 0.2],
-                "SM": [1.0, 100.0],
-                # "SM": [5, 10],
-                "EX": [1.0, 1.5],
-                "KI": [0.0, 0.7],
-                "KG": [0.0, 0.7],
-                "A": [0.0, 2.9],
-                "THETA": [0.0, 6.5],
-                "CI": [0.0, 0.9],
-                "CG": [0.98, 0.998],
-                "KERNEL": [1, 15],
-            }
-        ),
-    },
-    "gr4j": {
-        "param_name": ["x1", "x2", "x3", "x4"],
-        "param_range": OrderedDict(
-            {
-                "x1": [100.0, 1200.0],
-                "x2": [-5.0, 3.0],
-                "x3": [20.0, 300.0],
-                "x4": [1.1, 2.9],
-            }
-        ),
-    },
-    "hymod": {
-        "param_name": ["cmax", "bexp", "alpha", "ks", "kq"],
-        "param_range": OrderedDict(
-            {
-                "cmax": [1.0, 500.0],
-                "bexp": [0.1, 2.0],
-                "alpha": [0.1, 0.99],
-                "ks": [0.001, 0.10],
-                "kq": [0.1, 0.99],
-            }
-        ),
-    },
-}
+"""
+Author: Wenyu Ouyang
+Date: 2022-10-25 21:16:22
+LastEditTime: 2024-03-27 16:16:25
+LastEditors: Wenyu Ouyang
+Description: some basic config for hydro-model-xaj models
+FilePath: \hydro-model-xaj\hydromodel\models\model_config.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+from collections import OrderedDict
+
+import yaml
+
+
+def read_model_param_dict(file_path="param.yaml"):
+    try:
+        with open(file_path, "r") as file:
+            data = yaml.safe_load(file)
+
+        return {
+            model: {
+                "param_name": contents["param_name"],
+                "param_range": OrderedDict(contents["param_range"]),
+            }
+            for model, contents in data.items()
+        }
+    except Exception as e:
+        print(f"Error: {e}, we directly use the default MODEL_PARAM_DICT.")
+        return MODEL_PARAM_DICT
+
+
+MODEL_PARAM_DICT = {
+    "xaj": {
+        "param_name": [
+            # Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998.
+            # Crop Evapotranspiration, Food and Agriculture Organization of the United Nations,
+            # Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
+            "K",  # ratio of potential evapotranspiration to reference crop evaporation generally from Allen, 1998
+            "B",  # The exponent of the tension water capacity curve
+            "IM",  # The ratio of the impervious to the total area of the basin
+            "UM",  # Tension water capacity in the upper layer
+            "LM",  # Tension water capacity in the lower layer
+            "DM",  # Tension water capacity in the deepest layer
+            "C",  # The coefficient of deep evapotranspiration
+            "SM",  # The areal mean of the free water capacity of surface soil layer
+            "EX",  # The exponent of the free water capacity curve
+            "KI",  # Outflow coefficients of interflow
+            "KG",  # Outflow coefficients of groundwater
+            "CS",  # The recession constant of channel system
+            "L",  # Lag time
+            "CI",  # The recession constant of the lower interflow
+            "CG",  # The recession constant of groundwater storage
+        ],
+        "param_range": OrderedDict(
+            {
+                "K": [0.1, 1.0],
+                "B": [0.1, 0.4],
+                "IM": [0.01, 0.1],
+                "UM": [0.0, 20.0],
+                "LM": [60.0, 90.0],
+                "DM": [60.0, 120.0],
+                "C": [0.0, 0.2],
+                "SM": [1, 100.0],
+                # "SM": [50, 100.0],
+                "EX": [1.0, 1.5],
+                "KI": [0.0, 0.7],
+                "KG": [0.0, 0.7],
+                "CS": [0.0, 1.0],
+                "L": [1.0, 10.0],  # unit is same as your time step
+                "CI": [0.0, 0.9],
+                "CG": [0.98, 0.998],
+            }
+        ),
+    },
+    "xaj_mz": {
+        "param_name": [
+            # Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998.
+            # Crop Evapotranspiration, Food and Agriculture Organization of the United Nations,
+            # Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
+            "K",  # ratio of potential evapotranspiration to reference crop evaporation generally from Allen, 1998
+            "B",  # The exponent of the tension water capacity curve
+            "IM",  # The ratio of the impervious to the total area of the basin
+            "UM",  # Tension water capacity in the upper layer
+            "LM",  # Tension water capacity in the lower layer
+            "DM",  # Tension water capacity in the deepest layer
+            "C",  # The coefficient of deep evapotranspiration
+            "SM",  # The areal mean of the free water capacity of surface soil layer
+            "EX",  # The exponent of the free water capacity curve
+            "KI",  # Outflow coefficients of interflow
+            "KG",  # Outflow coefficients of groundwater
+            "A",  # parameter of mizuRoute
+            "THETA",  # parameter of mizuRoute
+            "CI",  # The recession constant of the lower interflow
+            "CG",  # The recession constant of groundwater storage
+            "KERNEL",  # kernel size of mizuRoute unit hydrograph when using convolution method
+        ],
+        "param_range": OrderedDict(
+            {
+                "K": [0.1, 1.0],
+                # "K": [0.5, 1.0],
+                "B": [0.1, 0.4],
+                # "B": [0.2, 0.4],
+                "IM": [0.01, 0.1],
+                # "IM": [0.07, 0.1],
+                "UM": [0.0, 20.0],
+                "LM": [60.0, 90.0],
+                "DM": [60.0, 120.0],
+                "C": [0.0, 0.2],
+                "SM": [1.0, 100.0],
+                # "SM": [5, 10],
+                "EX": [1.0, 1.5],
+                "KI": [0.0, 0.7],
+                "KG": [0.0, 0.7],
+                "A": [0.0, 2.9],
+                "THETA": [0.0, 6.5],
+                "CI": [0.0, 0.9],
+                "CG": [0.98, 0.998],
+                "KERNEL": [1, 15],
+            }
+        ),
+    },
+    "gr4j": {
+        "param_name": ["x1", "x2", "x3", "x4"],
+        "param_range": OrderedDict(
+            {
+                "x1": [100.0, 1200.0],
+                "x2": [-5.0, 3.0],
+                "x3": [20.0, 300.0],
+                "x4": [1.1, 2.9],
+            }
+        ),
+    },
+    "hymod": {
+        "param_name": ["cmax", "bexp", "alpha", "ks", "kq"],
+        "param_range": OrderedDict(
+            {
+                "cmax": [1.0, 500.0],
+                "bexp": [0.1, 2.0],
+                "alpha": [0.1, 0.99],
+                "ks": [0.001, 0.10],
+                "kq": [0.1, 0.99],
+            }
+        ),
+    },
+}
```

### Comparing `hydromodel-0.2.2/hydromodel/models/model_dict.py` & `hydromodel-0.2.3/hydromodel/models/model_dict.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-Author: Wenyu Ouyang
-Date: 2024-03-23 08:25:49
-LastEditTime: 2024-03-26 20:41:22
-LastEditors: Wenyu Ouyang
-Description: LOSS_DICT and MODEL_DICT
-FilePath: \hydro-model-xaj\hydromodel\models\model_dict.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import numpy as np
-from spotpy.objectivefunctions import rmse
-from hydromodel.models.xaj import xaj
-from hydromodel.models.gr4j import gr4j
-from hydromodel.models.hymod import hymod
-
-
-def rmse43darr(obs, sim):
-    """RMSE for 3D array
-
-    Parameters
-    ----------
-    obs : np.ndarray
-        observation data
-    sim : np.ndarray
-        simulation data
-
-    Returns
-    -------
-    _type_
-        _description_
-
-    Raises
-    ------
-    ValueError
-        _description_
-    """
-    rmses = np.sqrt(np.nanmean((sim - obs) ** 2, axis=0))
-    rmse = rmses.mean(axis=0)
-    if np.isnan(rmse) or any(np.isnan(sim)):
-        raise ValueError(
-            "RMSE is nan or there are nan values in the simulation data, please check the input data."
-        )
-    # tolist is necessary for spotpy to get the value
-    # otherwise the print will incur to an issue https://github.com/thouska/spotpy/issues/319
-    return rmse.tolist()
-
-
-LOSS_DICT = {
-    "RMSE": rmse43darr,
-    "spotpy_rmse": rmse,
-}
-
-MODEL_DICT = {
-    "xaj_mz": xaj,
-    "xaj": xaj,
-    "gr4j": gr4j,
-    "hymod": hymod,
-}
+"""
+Author: Wenyu Ouyang
+Date: 2024-03-23 08:25:49
+LastEditTime: 2024-03-26 20:41:22
+LastEditors: Wenyu Ouyang
+Description: LOSS_DICT and MODEL_DICT
+FilePath: \hydro-model-xaj\hydromodel\models\model_dict.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import numpy as np
+from spotpy.objectivefunctions import rmse
+from hydromodel.models.xaj import xaj
+from hydromodel.models.gr4j import gr4j
+from hydromodel.models.hymod import hymod
+
+
+def rmse43darr(obs, sim):
+    """RMSE for 3D array
+
+    Parameters
+    ----------
+    obs : np.ndarray
+        observation data
+    sim : np.ndarray
+        simulation data
+
+    Returns
+    -------
+    _type_
+        _description_
+
+    Raises
+    ------
+    ValueError
+        _description_
+    """
+    rmses = np.sqrt(np.nanmean((sim - obs) ** 2, axis=0))
+    rmse = rmses.mean(axis=0)
+    if np.isnan(rmse) or any(np.isnan(sim)):
+        raise ValueError(
+            "RMSE is nan or there are nan values in the simulation data, please check the input data."
+        )
+    # tolist is necessary for spotpy to get the value
+    # otherwise the print will incur to an issue https://github.com/thouska/spotpy/issues/319
+    return rmse.tolist()
+
+
+LOSS_DICT = {
+    "RMSE": rmse43darr,
+    "spotpy_rmse": rmse,
+}
+
+MODEL_DICT = {
+    "xaj_mz": xaj,
+    "xaj": xaj,
+    "gr4j": gr4j,
+    "hymod": hymod,
+}
```

### Comparing `hydromodel-0.2.2/hydromodel/models/xaj.py` & `hydromodel-0.2.3/hydromodel/models/xaj.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,903 +1,905 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-10 23:01:02
-LastEditTime: 2024-03-27 15:09:11
-LastEditors: Wenyu Ouyang
-Description: Core code for XinAnJiang model
-FilePath: /hydro-model-xaj/hydromodel/models/xaj.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import logging
-from typing import Union
-import numpy as np
-from numba import jit
-from scipy.special import gamma
-
-from hydromodel.models.model_config import read_model_param_dict
-
-PRECISION = 1e-5
-
-
-# @jit
-# @jit(nopython=True)
-def calculate_evap(lm, c, wu0, wl0, prcp, pet) -> tuple[np.array, np.array, np.array]:
-    """
-    Three-layers evaporation model from "Watershed Hydrologic Simulation" written by Prof. RenJun Zhao.
-    The book is Chinese, and its name is 《流域水文模拟》;
-    The three-layers evaporation model is described in Page 76;
-    The method is same with that in Page 22-23 in "Hydrologic Forecasting (5-th version)" written by Prof. Weimin Bao.
-    This book's Chinese name is 《水文预报》
-
-    Parameters
-    ----------
-    lm
-        average soil moisture storage capacity of lower layer
-    c
-        coefficient of deep layer
-    wu0
-        initial soil moisture of upper layer; update in each time step
-    wl0
-        initial soil moisture of lower layer; update in each time step
-    prcp
-        basin mean precipitation
-    pet
-        potential evapotranspiration
-
-    Returns
-    -------
-    tuple[np.array,np.array,np.array]
-        eu/el/ed are evaporation from upper/lower/deeper layer, respectively
-    """
-    eu = np.where(wu0 + prcp >= pet, pet, wu0 + prcp)
-    ed = np.where((wl0 < c * lm) & (wl0 < c * (pet - eu)), c * (pet - eu) - wl0, 0.0)
-    el = np.where(
-        wu0 + prcp >= pet,
-        0.0,
-        np.where(
-            wl0 >= c * lm,
-            (pet - eu) * wl0 / lm,
-            np.where(wl0 >= c * (pet - eu), c * (pet - eu), wl0),
-        ),
-    )
-    return eu, el, ed
-
-
-# @jit
-# @jit(nopython=True)
-def calculate_prcp_runoff(b, im, wm, w0, pe) -> tuple[np.array, np.array]:
-    """
-    Calculates the amount of runoff generated from rainfall after entering the underlying surface.
-
-    Same in "Watershed Hydrologic Simulation" and "Hydrologic Forecasting (5-th version)"
-
-    Parameters
-    ----------
-    b
-        B; exponent coefficient
-    im
-        IMP; imperiousness coefficient
-    wm
-        average soil moisture storage capacity
-    w0
-        initial soil moisture
-    pe
-        net precipitation
-
-    Returns
-    -------
-    tuple[np.array,np.array]
-        r -- runoff; r_im -- runoff of impervious part
-    """
-    wmm = wm * (1.0 + b)
-    a = wmm * (1.0 - (1.0 - w0 / wm) ** (1.0 / (1.0 + b)))
-    if np.isnan(a).any():
-        raise ArithmeticError("Please check if w0>wm or b is a negative value!")
-    r_cal = np.where(
-        pe > 0.0,
-        np.where(
-            pe + a < wmm,
-            # 1e-5 is a precision which we set to guarantee float's calculation is correct
-            pe - (wm - w0) + wm * (1.0 - np.minimum(a + pe, wmm) / wmm) ** (1.0 + b),
-            pe - (wm - w0),
-        ),
-        np.full(pe.shape, 0.0),
-    )
-    r = np.maximum(r_cal, 0.0)
-    # separate impervious part with the other
-    r_im_cal = pe * im
-    r_im = np.maximum(r_im_cal, 0.0)
-    return r, r_im
-
-
-def calculate_w_storage(
-    um, lm, dm, wu0, wl0, wd0, eu, el, ed, pe, r
-) -> tuple[np.array, np.array, np.array]:
-    """
-    Update the soil moisture values of the three layers.
-
-    According to the equation 2.60 in the book《水文预报》
-
-    Parameters
-    ----------
-    um
-        average soil moisture storage capacity of the upper layer
-    lm
-        average soil moisture storage capacity of the lower layer
-    dm
-        average soil moisture storage capacity of the deep layer
-    wu0
-        initial values of soil moisture in upper layer
-    wl0
-        initial values of soil moisture in lower layer
-    wd0
-        initial values of soil moisture in deep layer
-    eu
-        evaporation of the upper layer; it isn't used in this function
-    el
-        evaporation of the lower layer
-    ed
-        evaporation of the deep layer
-    pe
-        net precipitation; it is able to be negative value in this function
-    r
-        runoff
-
-    Returns
-    -------
-    tuple[np.array,np.array,np.array]
-        wu,wl,wd -- soil moisture in upper, lower and deep layer
-    """
-    # pe>0: the upper soil moisture was added firstly, then lower layer, and the final is deep layer
-    # pe<=0: no additional water, just remove evapotranspiration,
-    # but note the case: e >= p > 0
-    # (1) if wu0 + p > e, then e = eu (2) else, wu must be zero
-    wu = np.where(
-        pe > 0.0,
-        np.where(wu0 + pe - r < um, wu0 + pe - r, um),
-        np.where(wu0 + pe > 0.0, wu0 + pe, 0.0),
-    )
-    # calculate wd before wl because it is easier to cal using where statement
-    wd = np.where(
-        pe > 0.0,
-        np.where(wu0 + wl0 + pe - r > um + lm, wu0 + wl0 + wd0 + pe - r - um - lm, wd0),
-        wd0 - ed,
-    )
-    # water balance (equation 2.2 in Page 13, also shown in Page 23)
-    # if wu0 + p > e, then e = eu; else p must be used in upper layer,
-    # so no matter what the case is, el didn't include p, neither ed
-    wl = np.where(pe > 0.0, wu0 + wl0 + wd0 + pe - r - wu - wd, wl0 - el)
-    # the water storage should be in reasonable range
-    wu_ = np.clip(wu, a_min=0.0, a_max=um)
-    wl_ = np.clip(wl, a_min=0.0, a_max=lm)
-    wd_ = np.clip(wd, a_min=0.0, a_max=dm)
-    return wu_, wl_, wd_
-
-
-def generation(p_and_e, k, b, im, um, lm, dm, c, wu0=None, wl0=None, wd0=None) -> tuple:
-    """
-    Single-step runoff generation in XAJ.
-
-    Parameters
-    ----------
-    p_and_e
-        precipitation and potential evapotranspiration
-    k
-        ratio of potential evapotranspiration to reference crop evaporation
-    b
-        exponent parameter
-    um
-        average soil moisture storage capacity of the upper layer
-    lm
-        average soil moisture storage capacity of the lower layer
-    dm
-        average soil moisture storage capacity of the deep layer
-    im
-        impermeability coefficient
-    c
-        coefficient of deep layer
-    wu0
-        initial values of soil moisture in upper layer
-    wl0
-        initial values of soil moisture in lower layer
-    wd0
-        initial values of soil moisture in deep layer
-
-    Returns
-    -------
-    tuple[tuple, tuple]
-        (r, rim, e, pe), (wu, wl, wd); all variables are np.array
-    """
-    # make sure physical variables' value ranges are correct
-    prcp = np.maximum(p_and_e[:, 0], 0.0)
-    # get potential evapotranspiration
-    pet = np.maximum(p_and_e[:, 1] * k, 0.0)
-    # wm
-    wm = um + lm + dm
-    if wu0 is None:
-        # just an initial value
-        wu0 = 0.6 * um
-    if wl0 is None:
-        wl0 = 0.6 * lm
-    if wd0 is None:
-        wd0 = 0.6 * dm
-    w0_ = wu0 + wl0 + wd0
-
-    # w0 need locate in correct range so that following calculation could be right
-    # To make sure float data's calculation is correct, we'd better minus a precision (1e-5)
-    w0 = np.minimum(w0_, wm - 1e-5)
-
-    # Calculate the amount of evaporation from storage
-    eu, el, ed = calculate_evap(lm, c, wu0, wl0, prcp, pet)
-    e = eu + el + ed
-
-    # Calculate the runoff generated by net precipitation
-    prcp_difference = prcp - e
-    pe = np.maximum(prcp_difference, 0.0)
-    r, rim = calculate_prcp_runoff(b, im, wm, w0, pe)
-    # Update wu, wl, wd
-    wu, wl, wd = calculate_w_storage(
-        um, lm, dm, wu0, wl0, wd0, eu, el, ed, prcp_difference, r
-    )
-
-    return (r, rim, e, pe), (wu, wl, wd)
-
-
-def sources(pe, r, sm, ex, ki, kg, s0=None, fr0=None, book="HF") -> tuple:
-    """
-    Divide the runoff to different sources
-
-    We use the initial version from the paper of the inventor of the XAJ model -- Prof. Renjun Zhao:
-    "Analysis of parameters of the XinAnJiang model". Its Chinese name is <<新安江模型参数的分析>>,
-    which could be found by searching in "Baidu Xueshu".
-    The module's code can also be found in "Watershed Hydrologic Simulation" (WHS) Page 174.
-    It is nearly same with that in "Hydrologic Forecasting" (HF) Page 148-149
-    We use the period average runoff as input and the unit period is day so we don't need to difference it as books show
-
-    We also provide code for formula from《水文预报》"Hydrologic Forecasting" (HF) the fifth version. Page 40-41 and 150-151;
-    the procedures in 《工程水文学》"Engineering Hydrology" (EH) the third version are different we also provide.
-    they are in the "sources5mm" function.
-
-    Parameters
-    ------------
-    pe
-        net precipitation
-    r
-        runoff from xaj_generation
-    sm
-        areal mean free water capacity of the surface layer
-    ex
-        exponent of the free water capacity curve
-    ki
-        outflow coefficients of the free water storage to interflow relationships
-    kg
-        outflow coefficients of the free water storage to groundwater relationships
-    s0
-        free water capacity of last period
-    fr0
-        runoff area of last period
-
-    Return
-    ------------
-    tuple[tuple, tuple]
-        rs -- surface runoff; ri-- interflow runoff; rg -- groundwater runoff;
-        s1 -- final free water capacity;
-        all variables are numpy array
-
-    """
-    # maximum free water storage capacity in a basin
-    ms = sm * (1.0 + ex)
-    if fr0 is None:
-        fr0 = 0.1
-    if s0 is None:
-        s0 = 0.5 * sm
-    # For free water storage, because s is related to fr and s0 and fr0 are both values of last period,
-    # we have to trans the initial value of s from last period to this one.
-    # both WHS（流域水文模拟）'s sample code and HF（水文预报） use s = fr0 * s0 / fr.
-    # I think they both think free water reservoir as a cubic tank. Its height is s and area of bottom rectangle is fr
-    # we will have a cubic tank with varying bottom and height,
-    # and fixed boundary (in HF sm is fixed) or none-fixed boundary (in EH smmf is not fixed)
-    # but notice r's list like" [1,0] which 1 is the 1st period's runoff and 0 is the 2nd period's runoff
-    # after 1st period, the s1 could not be zero, but in the 2nd period, fr=0, then we cannot set s=0, because some water still in the tank
-    # fr's formula could be found in Eq. 9 in "Analysis of parameters of the XinAnJiang model",
-    # Here our r doesn't include rim, so there is no need to remove rim from r; this is also the method in 《水文预报》（HF）
-
-    # NOTE: when r is 0, fr should be 0, however, s1 may not be zero and it still hold some water,
-    # then fr can not be 0, otherwise when fr is used as denominator it lead to error,
-    # so we have to deal with this case later, for example, when r=0, we cannot use pe * fr to replace r
-    # because fr get the value of last period, and it is not 0
-    fr = np.copy(fr0)
-    if any(fr == 0.0):
-        raise ArithmeticError(
-            "Please check fr's value, fr==0.0 will cause error in the next step!"
-        )
-    # r=0, then r/pe must be 0
-    fr_mask = r > 0.0
-    fr[fr_mask] = r[fr_mask] / pe[fr_mask]
-    if np.isnan(fr).any():
-        raise ArithmeticError("Please check pe's data! there may be 0.0")
-
-    # if fr=0, then we cannot get ss, but ss should not be 0, because s1 of last period may not be 0 and it still hold some water
-    ss = np.copy(s0)
-    # same initialization for s
-    s = np.copy(s0)
-
-    ss[fr_mask] = fr0[fr_mask] * s0[fr_mask] / fr[fr_mask]
-
-    if book == "HF":
-        ss = np.minimum(ss, sm)
-        au = ms * (1.0 - (1.0 - ss / sm) ** (1.0 / (1.0 + ex)))
-        if np.isnan(au).any():
-            raise ValueError(
-                "Error: NaN values detected. Try set clip function or check your data!!!"
-            )
-        # the first condition should be r > 0.0, when r=0, rs must be 0, fig 6-12 in EH or fig 5-4 in HF
-        # so we have to use "pe" carefully!!! when r>0.0, we use pe, otherwise we don't use it!!!
-        rs = np.full(r.shape, 0.0)
-        rs[fr_mask] = np.where(
-            pe[fr_mask] + au[fr_mask] < ms[fr_mask],
-            # equation 2-85 in HF
-            fr[fr_mask]
-            * (
-                pe[fr_mask]
-                - sm[fr_mask]
-                + ss[fr_mask]
-                + sm[fr_mask]
-                * (
-                    (
-                        1
-                        - np.minimum(pe[fr_mask] + au[fr_mask], ms[fr_mask])
-                        / ms[fr_mask]
-                    )
-                    ** (1 + ex[fr_mask])
-                )
-            ),
-            # equation 2-86 in HF
-            fr[fr_mask] * (pe[fr_mask] + ss[fr_mask] - sm[fr_mask]),
-        )
-        rs = np.minimum(rs, r)
-
-        # ri's mask is not same as rs's, because last period's s may not be 0
-        # and in this time, ri and rg could be larger than 0
-        # we need firstly calculate the updated s, s's mask is same as fr_mask,
-        # when r==0, then s will be equal to last period's
-        # equation 2-87 in HF, some free water leave or save, so we update free water storage
-        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
-        s = np.minimum(s, sm)
-        if np.isnan(s).any():
-            raise ArithmeticError("Please check fr's data! there may be 0.0")
-
-    elif book == "EH":
-        # smmf should be with correpond with s
-        smmf = ms * (1 - (1 - fr) ** (1 / ex))
-        smf = smmf / (1 + ex)
-        ss = np.minimum(ss, smf)
-        au = smmf * (1 - (1 - ss / smf) ** (1 / (1 + ex)))
-        if np.isnan(au).any():
-            raise ValueError(
-                "Error: NaN values detected. Try set clip function or check your data!!!"
-            )
-
-        # rs's mask is keep with fr_mask
-        rs = np.full(r.shape, 0.0)
-        rs[fr_mask] = np.where(
-            pe[fr_mask] + au[fr_mask] < smmf[fr_mask],
-            (
-                pe[fr_mask]
-                - smf[fr_mask]
-                + ss[fr_mask]
-                + smf[fr_mask]
-                * (
-                    1
-                    - np.minimum(pe[fr_mask] + au[fr_mask], smmf[fr_mask])
-                    / smmf[fr_mask]
-                )
-                ** (ex[fr_mask] + 1)
-            )
-            * fr[fr_mask],
-            (pe[fr_mask] + ss[fr_mask] - smf[fr_mask]) * fr[fr_mask],
-        )
-        rs = np.minimum(rs, r)
-        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
-        s = np.minimum(s, smf)
-    else:
-        raise ValueError("Please set book as 'HF' or 'EH'!")
-    # the following part is same for both HF and EH. Even the formula is different, but their meaning is same
-    # equation 2-88 in HF, next interflow and ground water will be released from the updated free water storage
-    # We use the period average runoff as input and the general unit period is day.
-    # Hence, we directly use ki and kg rather than ki_{Δt} in books.
-    ri = ki * s * fr
-    rg = kg * s * fr
-    # ri = np.where(s < PRECISION, np.full(r.shape, 0.0), ki * s * fr)
-    # rg = np.where(s < PRECISION, np.full(r.shape, 0.0), kg * s * fr)
-    # equation 2-89 in HF; although it looks different with that in WHS, they are actually same
-    # Finally, calculate the final free water storage
-    s1 = s * (1 - ki - kg)
-    # s1 = np.where(s1 < PRECISION, np.full(s1.shape, 0.0), s1)
-    return (rs, ri, rg), (s1, fr)
-
-
-def sources5mm(
-    pe,
-    runoff,
-    sm,
-    ex,
-    ki,
-    kg,
-    s0=None,
-    fr0=None,
-    time_interval_hours=1,
-    book="HF",
-):
-    """
-    Divide the runoff to different sources according to books -- 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition
-
-    Parameters
-    ----------
-    pe
-        net precipitation
-    runoff
-        runoff from xaj_generation
-    sm
-        areal mean free water capacity of the surface layer
-    ex
-        exponent of the free water capacity curve
-    ki
-        outflow coefficients of the free water storage to interflow relationships
-    kg
-        outflow coefficients of the free water storage to groundwater relationships
-    s0
-        initial free water capacity
-    fr0
-        initial area of generation
-    time_interval_hours
-        由于Ki、Kg、Ci、Cg都是以24小时为时段长定义的,需根据时段长转换
-    book
-        the methods in 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition are different,
-        hence, both are provided, and the default is the former -- "ShuiWenYuBao";
-        the other one is "GongChengShuiWenXue"
-
-    Returns
-    -------
-    tuple[tuple, tuple]
-        rs_s -- surface runoff; rss_s-- interflow runoff; rg_s -- groundwater runoff;
-        (fr_ds[-1], s_ds[-1]): state variables' final value;
-        all variables are numpy array
-    """
-    # 由于Ki、Kg都是以24小时为时段长定义的，需根据时段长转换
-    hours_per_day = 24
-    # 非整除情况，时段+1
-    residue_temp = hours_per_day % time_interval_hours
-    if residue_temp != 0:
-        residue_temp = 1
-    period_num_1d = int(hours_per_day / time_interval_hours) + residue_temp
-    # 当kss+kg>1时，根式为偶数运算时，kss_period会成为复数，这里会报错；另外注意分母可能为0，kss不可取0
-    # 对kss+kg的取值进行限制
-    kss_period = (1 - (1 - (ki + kg)) ** (1 / period_num_1d)) / (1 + kg / ki)
-    kg_period = kss_period * kg / ki
-
-    # 流域最大点自由水蓄水容量深
-    smm = sm * (1 + ex)
-    if s0 is None:
-        s0 = 0.50 * sm
-    if fr0 is None:
-        fr0 = 0.1
-    # don't use np.where here, because it will cause some warning
-    fr = np.copy(fr0)
-    fr_mask = runoff > 0.0
-    fr[fr_mask] = runoff[fr_mask] / pe[fr_mask]
-    if np.all(runoff < 5):
-        n = 1
-    else:
-        # when modeling multiple basins, the number of divides is not the same, so we use the maximum number
-        r_max = np.max(runoff)
-        residue_temp = r_max % 5
-        if residue_temp != 0:
-            residue_temp = 1
-        n = int(r_max / 5) + residue_temp
-    rn = runoff / n
-    pen = pe / n
-    kss_d = (1 - (1 - (kss_period + kg_period)) ** (1 / n)) / (
-        1 + kg_period / kss_period
-    )
-    kg_d = kss_d * kg_period / kss_period
-    # kss_d = kss_period
-    # kg_d = kg_period
-    rs = np.full(runoff.shape, 0.0)
-    rss = np.full(runoff.shape, 0.0)
-    rg = np.full(runoff.shape, 0.0)
-
-    s_ds = []
-    fr_ds = []
-    s_ds.append(s0)
-    fr_ds.append(fr0)
-
-    for j in range(n):
-        fr0_d = fr_ds[j]
-        s0_d = s_ds[j]
-        # equation 5-32 in HF, but strange, cause each period, rn/pen is same, fr_d should be same
-        # fr_d = 1 - (1 - fr) ** (1 / n)
-        fr_d = fr
-
-        ss_d = np.copy(s0_d)
-        s_d = np.copy(s0_d)
-        s1_d = np.copy(s0_d)
-
-        ss_d[fr_mask] = fr0_d[fr_mask] * s0_d[fr_mask] / fr_d[fr_mask]
-
-        if book == "HF":
-            ss_d = np.minimum(ss_d, sm)
-            # ms = smm
-            au = smm * (1.0 - (1.0 - ss_d / sm) ** (1.0 / (1.0 + ex)))
-            if np.isnan(au).any():
-                raise ValueError(
-                    "Error: NaN values detected. Try set clip function or check your data!!!"
-                )
-            rs_j = np.full(rn.shape, 0.0)
-            rs_j[fr_mask] = np.where(
-                pen[fr_mask] + au[fr_mask] < smm[fr_mask],
-                # equation 5-26 in HF
-                fr_d[fr_mask]
-                * (
-                    pen[fr_mask]
-                    - sm[fr_mask]
-                    + ss_d[fr_mask]
-                    + sm[fr_mask]
-                    * (
-                        (
-                            1
-                            - np.minimum(pen[fr_mask] + au[fr_mask], smm[fr_mask])
-                            / smm[fr_mask]
-                        )
-                        ** (1 + ex[fr_mask])
-                    )
-                ),
-                # equation 5-27 in HF
-                fr_d[fr_mask] * (pen[fr_mask] + ss_d[fr_mask] - sm[fr_mask]),
-            )
-            rs_j = np.minimum(rs_j, rn)
-            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
-            s_d = np.minimum(s_d, sm)
-
-        elif book == "EH":
-            smmf = smm * (1 - (1 - fr_d) ** (1 / ex))
-            smf = smmf / (1 + ex)
-            ss_d = np.minimum(ss_d, smf)
-            au = smmf * (1 - (1 - ss_d / smf) ** (1 / (1 + ex)))
-            if np.isnan(au).any():
-                raise ValueError(
-                    "Error: NaN values detected. Try set clip function or check your data!!!"
-                )
-            rs_j = np.full(rn.shape, 0.0)
-            rs_j[fr_mask] = np.where(
-                pen[fr_mask] + au[fr_mask] < smmf[fr_mask],
-                (
-                    pen[fr_mask]
-                    - smf[fr_mask]
-                    + ss_d[fr_mask]
-                    + smf[fr_mask]
-                    * (
-                        1
-                        - np.minimum(pen[fr_mask] + au[fr_mask], smmf[fr_mask])
-                        / smmf[fr_mask]
-                    )
-                    ** (ex[fr_mask] + 1)
-                )
-                * fr_d[fr_mask],
-                (pen[fr_mask] + ss_d[fr_mask] - smf[fr_mask]) * fr_d[fr_mask],
-            )
-            rs_j = np.minimum(rs_j, rn)
-            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
-            s_d = np.minimum(s_d, smf)
-
-        else:
-            raise NotImplementedError(
-                "We don't have this implementation! Please chose 'HF' or 'EH'!!"
-            )
-        rss_j = s_d * kss_d * fr_d
-        rg_j = s_d * kg_d * fr_d
-        s1_d = s_d * (1 - kss_d - kg_d)
-
-        rs = rs + rs_j
-        rss = rss + rss_j
-        rg = rg + rg_j
-        # 赋值s_d和fr_d到数组中，以给下一段做初值
-        s_ds.append(s1_d)
-        fr_ds.append(fr_d)
-
-    return (rs, rss, rg), (s_ds[-1], fr_ds[-1])
-
-
-# @jit
-# @jit(nopython=True)
-def linear_reservoir(x, weight, last_y=None) -> np.array:
-    """
-    Linear reservoir's release function
-
-    Parameters
-    ----------
-    x
-        the input to the linear reservoir
-    weight
-        the coefficient of linear reservoir
-    last_y
-        the output of last period
-
-    Returns
-    -------
-    np.array
-        one-step forward result
-    """
-    weight1 = 1 - weight
-    if last_y is None:
-        last_y = np.full(weight.shape, 0.001)
-    return weight * last_y + weight1 * x
-
-
-def uh_conv(x, uh_from_gamma):
-    """
-    Function for 1d-convolution calculation
-
-    Parameters
-    ----------
-    x
-        x is a sequence-first variable; the dim of x is [seq, batch, feature=1];
-        feature must be 1
-    uh_from_gamma
-        unit hydrograph from uh_gamma; the dim: [len_uh, batch, feature=1];
-        feature must be 1
-
-    Returns
-    -------
-    np.array
-        convolution
-    """
-    outputs = np.full(x.shape, 0.0)
-    time_length, batch_size, feature_size = x.shape
-    if feature_size > 1:
-        logging.error("We only support one-dim convolution now!!!")
-    for i in range(batch_size):
-        uh = uh_from_gamma[:, i, 0]
-        inputs = x[:, i, 0]
-        outputs[:, i, 0] = np.convolve(inputs, uh)[:time_length]
-    return outputs
-
-
-def uh_gamma(a, theta, len_uh=15):
-    """
-    A simple two-parameter Gamma distribution as a unit-hydrograph to route instantaneous runoff from a hydrologic model
-    The method comes from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
-
-    Parameters
-    ----------
-    a
-        shape parameter
-    theta
-        timescale parameter
-    len_uh
-        the time length of the unit hydrograph
-    Returns
-    -------
-    torch.Tensor
-        the unit hydrograph, dim: [seq, batch, feature]
-    """
-    # dims of a: time_seq (same all time steps), batch, feature=1
-    m = a.shape
-    if len_uh > m[0]:
-        raise RuntimeError(
-            "length of unit hydrograph should be smaller than the whole length of input"
-        )
-    # aa > 0, here we set minimum 0.1 (min of a is 0, set when calling this func); First dimension of a is repeat
-    aa = np.maximum(0.0, a[0:len_uh, :, :]) + 0.1
-    # theta > 0, here set minimum 0.5
-    theta = np.maximum(0.0, theta[0:len_uh, :, :]) + 0.5
-    # len_f, batch, feature
-    t = np.expand_dims(
-        np.swapaxes(np.tile(np.arange(0.5, len_uh * 1.0), (m[1], 1)), 0, 1), axis=-1
-    )
-    denominator = gamma(aa) * (theta**aa)
-    # [len_f, m[1], m[2]]
-    w = 1 / denominator * (t ** (aa - 1)) * (np.exp(-t / theta))
-    w = w / w.sum(0)  # scale to 1 for each UH
-    return w
-
-
-def xaj(
-    p_and_e,
-    params: Union[np.array, list],
-    return_state=False,
-    warmup_length=365,
-    **kwargs,
-) -> Union[tuple, np.array]:
-    """
-    run XAJ model
-
-    Parameters
-    ----------
-    p_and_e
-        prcp and pet; sequence-first (time is the first dim) 3-d np array: [time, basin, feature=2]
-    params
-        parameters of XAJ model for basin(s);
-        2-dim variable -- [basin, parameter]:
-        the parameters are B IM UM LM DM C SM EX KI KG A THETA CI CG (notice the sequence)
-    return_state
-        if True, return state values, mainly for warmup periods
-    warmup_length
-        hydro models need a warm-up period to get good initial state values
-    kwargs
-        route_method
-            now we provide two ways: "CSL" (recession constant + lag time) and "MZ" (method from mizuRoute)
-        source_type
-            default is "sources" and it will call "sources" function; the other is "sources5mm",
-            and we will divide the runoff to some <5mm pieces according to the books in this case
-        source_book
-            When source_type is "sources5mm" there are two implementions for dividing sources,
-            as the methods in "ShuiWenYuBao" and "GongChengShuiWenXue"" are different.
-            Hence, both are provided, and the default is the former.
-
-    Returns
-    -------
-    Union[np.array, tuple]
-        streamflow or (streamflow, states)
-    """
-    # default values for some function parameters
-    model_name = kwargs.get("name", "xaj")
-    source_type = kwargs.get("source_type", "sources")
-    source_book = kwargs.get("source_book", "HF")
-    pr_file = kwargs.get("param_range_file", None)
-    model_param_dict = read_model_param_dict(pr_file)
-    # params
-    param_ranges = model_param_dict[model_name]["param_range"]
-    if model_name == "xaj":
-        route_method = "CSL"
-    elif model_name == "xaj_mz":
-        route_method = "MZ"
-    else:
-        raise NotImplementedError(
-            "We don't provide this route method now! Please use 'CSL' or 'MZ'!"
-        )
-    if np.isnan(params).any():
-        raise ValueError(
-            "Parameters contain NaN values. Please check your opt algorithm"
-        )
-    xaj_params = [
-        (value[1] - value[0]) * params[:, i] + value[0]
-        for i, (key, value) in enumerate(param_ranges.items())
-    ]
-
-    k = xaj_params[0]
-    b = xaj_params[1]
-    im = xaj_params[2]
-    um = xaj_params[3]
-    lm = xaj_params[4]
-    dm = xaj_params[5]
-    c = xaj_params[6]
-    sm = xaj_params[7]
-    ex = xaj_params[8]
-    ki_ = xaj_params[9]
-    kg_ = xaj_params[10]
-    # ki+kg should be smaller than 1; if not, we scale them
-    ki = np.where(ki_ + kg_ < 1.0, ki_, (1.0 - PRECISION) / (ki_ + kg_) * ki_)
-    kg = np.where(ki_ + kg_ < 1.0, kg_, (1.0 - PRECISION) / (ki_ + kg_) * kg_)
-    if route_method == "CSL":
-        cs = xaj_params[11]
-        l = xaj_params[12]
-    elif route_method == "MZ":
-        # we will use routing method from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
-        a = xaj_params[11]
-        theta = xaj_params[12]
-        # make it as a parameter
-        kernel_size = int(xaj_params[15])
-    else:
-        raise NotImplementedError(
-            "We don't provide this route method now! Please use 'CSL' or 'MZ'!"
-        )
-    ci = xaj_params[13]
-    cg = xaj_params[14]
-
-    # initialize state values
-    if warmup_length > 0:
-        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
-        _q, _e, *w0, s0, fr0, qi0, qg0 = xaj(
-            p_and_e_warmup,
-            params,
-            return_state=True,
-            warmup_length=0,
-            **kwargs,
-        )
-    else:
-        w0 = (0.5 * um, 0.5 * lm, 0.5 * dm)
-        s0 = 0.5 * sm
-        fr0 = np.full(ex.shape, 0.1)
-        qi0 = np.full(ci.shape, 0.1)
-        qg0 = np.full(cg.shape, 0.1)
-
-    # state_variables
-    inputs = p_and_e[warmup_length:, :, :]
-    runoff_ims_ = np.full(inputs.shape[:2], 0.0)
-    rss_ = np.full(inputs.shape[:2], 0.0)
-    ris_ = np.full(inputs.shape[:2], 0.0)
-    rgs_ = np.full(inputs.shape[:2], 0.0)
-    es_ = np.full(inputs.shape[:2], 0.0)
-    for i in range(inputs.shape[0]):
-        if i == 0:
-            (r, rim, e, pe), w = generation(
-                inputs[i, :, :], k, b, im, um, lm, dm, c, *w0
-            )
-            if source_type == "sources":
-                (rs, ri, rg), (s, fr) = sources(
-                    pe, r, sm, ex, ki, kg, s0, fr0, book=source_book
-                )
-            elif source_type == "sources5mm":
-                (rs, ri, rg), (s, fr) = sources5mm(
-                    pe, r, sm, ex, ki, kg, s0, fr0, book=source_book
-                )
-            else:
-                raise NotImplementedError("No such divide-sources method")
-        else:
-            (r, rim, e, pe), w = generation(
-                inputs[i, :, :], k, b, im, um, lm, dm, c, *w
-            )
-            if source_type == "sources":
-                (rs, ri, rg), (s, fr) = sources(
-                    pe, r, sm, ex, ki, kg, s, fr, book=source_book
-                )
-            elif source_type == "sources5mm":
-                (rs, ri, rg), (s, fr) = sources5mm(
-                    pe, r, sm, ex, ki, kg, s, fr, book=source_book
-                )
-            else:
-                raise NotImplementedError("No such divide-sources method")
-        # impevious part is pe * im
-        runoff_ims_[i, :] = rim
-        # so for non-imprvious part, the result should be corrected
-        rss_[i, :] = rs * (1 - im)
-        ris_[i, :] = ri * (1 - im)
-        rgs_[i, :] = rg * (1 - im)
-        es_[i, :] = e
-    # seq, batch, feature
-    runoff_im = np.expand_dims(runoff_ims_, axis=2)
-    rss = np.expand_dims(rss_, axis=2)
-    es = np.expand_dims(es_, axis=2)
-
-    qs = np.full(inputs.shape[:2], 0.0)
-    if route_method == "CSL":
-        qt = np.full(inputs.shape[:2], 0.0)
-        for i in range(inputs.shape[0]):
-            if i == 0:
-                qi = linear_reservoir(ris_[i], ci, qi0)
-                qg = linear_reservoir(rgs_[i], cg, qg0)
-            else:
-                qi = linear_reservoir(ris_[i], ci, qi)
-                qg = linear_reservoir(rgs_[i], cg, qg)
-            qs_ = rss_[i]
-            qt[i, :] = qs_ + qi + qg
-        for j in range(len(l)):
-            lag = int(l[j])
-            for i in range(lag):
-                qs[i, j] = qt[i, j]
-            for i in range(lag, inputs.shape[0]):
-                qs[i, j] = cs[j] * qs[i - 1, j] + (1 - cs[j]) * qt[i - lag, j]
-    elif route_method == "MZ":
-        rout_a = a.repeat(rss.shape[0]).reshape(rss.shape)
-        rout_b = theta.repeat(rss.shape[0]).reshape(rss.shape)
-        conv_uh = uh_gamma(rout_a, rout_b, kernel_size)
-        qs_ = uh_conv(runoff_im + rss, conv_uh)
-        for i in range(inputs.shape[0]):
-            if i == 0:
-                qi = linear_reservoir(ris_[i], ci, qi0)
-                qg = linear_reservoir(rgs_[i], cg, qg0)
-            else:
-                qi = linear_reservoir(ris_[i], ci, qi)
-                qg = linear_reservoir(rgs_[i], cg, qg)
-            qs[i, :] = qs_[i, :, 0] + qi + qg
-    else:
-        raise NotImplementedError(
-            "We don't provide this route method now! Please use 'CS' or 'MZ'!"
-        )
-
-    # seq, batch, feature
-    q_sim = np.expand_dims(qs, axis=2)
-    if return_state:
-        return q_sim, es, *w, s, fr, qi, qg
-    return q_sim, es
+"""
+Author: Wenyu Ouyang
+Date: 2021-12-10 23:01:02
+LastEditTime: 2024-05-19 11:41:06
+LastEditors: Wenyu Ouyang
+Description: Core code for XinAnJiang model
+FilePath: /hydro-model-xaj/hydromodel/models/xaj.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import logging
+from typing import Union
+import numpy as np
+from numba import jit
+from scipy.special import gamma
+
+from hydromodel.models.model_config import read_model_param_dict
+
+PRECISION = 1e-5
+
+
+# @jit
+# @jit(nopython=True)
+def calculate_evap(lm, c, wu0, wl0, prcp, pet) -> tuple[np.array, np.array, np.array]:
+    """
+    Three-layers evaporation model from "Watershed Hydrologic Simulation" written by Prof. RenJun Zhao.
+    The book is Chinese, and its name is 《流域水文模拟》;
+    The three-layers evaporation model is described in Page 76;
+    The method is same with that in Page 22-23 in "Hydrologic Forecasting (5-th version)" written by Prof. Weimin Bao.
+    This book's Chinese name is 《水文预报》
+
+    Parameters
+    ----------
+    lm
+        average soil moisture storage capacity of lower layer
+    c
+        coefficient of deep layer
+    wu0
+        initial soil moisture of upper layer; update in each time step
+    wl0
+        initial soil moisture of lower layer; update in each time step
+    prcp
+        basin mean precipitation
+    pet
+        potential evapotranspiration
+
+    Returns
+    -------
+    tuple[np.array,np.array,np.array]
+        eu/el/ed are evaporation from upper/lower/deeper layer, respectively
+    """
+    eu = np.where(wu0 + prcp >= pet, pet, wu0 + prcp)
+    ed = np.where((wl0 < c * lm) & (wl0 < c * (pet - eu)), c * (pet - eu) - wl0, 0.0)
+    el = np.where(
+        wu0 + prcp >= pet,
+        0.0,
+        np.where(
+            wl0 >= c * lm,
+            (pet - eu) * wl0 / lm,
+            np.where(wl0 >= c * (pet - eu), c * (pet - eu), wl0),
+        ),
+    )
+    return eu, el, ed
+
+
+# @jit
+# @jit(nopython=True)
+def calculate_prcp_runoff(b, im, wm, w0, pe) -> tuple[np.array, np.array]:
+    """
+    Calculates the amount of runoff generated from rainfall after entering the underlying surface.
+
+    Same in "Watershed Hydrologic Simulation" and "Hydrologic Forecasting (5-th version)"
+
+    Parameters
+    ----------
+    b
+        B; exponent coefficient
+    im
+        IMP; imperiousness coefficient
+    wm
+        average soil moisture storage capacity
+    w0
+        initial soil moisture
+    pe
+        net precipitation
+
+    Returns
+    -------
+    tuple[np.array,np.array]
+        r -- runoff; r_im -- runoff of impervious part
+    """
+    wmm = wm * (1.0 + b)
+    a = wmm * (1.0 - (1.0 - w0 / wm) ** (1.0 / (1.0 + b)))
+    if np.isnan(a).any():
+        raise ArithmeticError("Please check if w0>wm or b is a negative value!")
+    r_cal = np.where(
+        pe > 0.0,
+        np.where(
+            pe + a < wmm,
+            # 1e-5 is a precision which we set to guarantee float's calculation is correct
+            pe - (wm - w0) + wm * (1.0 - np.minimum(a + pe, wmm) / wmm) ** (1.0 + b),
+            pe - (wm - w0),
+        ),
+        np.full(pe.shape, 0.0),
+    )
+    r = np.maximum(r_cal, 0.0)
+    # separate impervious part with the other
+    r_im_cal = pe * im
+    r_im = np.maximum(r_im_cal, 0.0)
+    return r, r_im
+
+
+def calculate_w_storage(
+    um, lm, dm, wu0, wl0, wd0, eu, el, ed, pe, r
+) -> tuple[np.array, np.array, np.array]:
+    """
+    Update the soil moisture values of the three layers.
+
+    According to the equation 2.60 in the book《水文预报》
+
+    Parameters
+    ----------
+    um
+        average soil moisture storage capacity of the upper layer
+    lm
+        average soil moisture storage capacity of the lower layer
+    dm
+        average soil moisture storage capacity of the deep layer
+    wu0
+        initial values of soil moisture in upper layer
+    wl0
+        initial values of soil moisture in lower layer
+    wd0
+        initial values of soil moisture in deep layer
+    eu
+        evaporation of the upper layer; it isn't used in this function
+    el
+        evaporation of the lower layer
+    ed
+        evaporation of the deep layer
+    pe
+        net precipitation; it is able to be negative value in this function
+    r
+        runoff
+
+    Returns
+    -------
+    tuple[np.array,np.array,np.array]
+        wu,wl,wd -- soil moisture in upper, lower and deep layer
+    """
+    # pe>0: the upper soil moisture was added firstly, then lower layer, and the final is deep layer
+    # pe<=0: no additional water, just remove evapotranspiration,
+    # but note the case: e >= p > 0
+    # (1) if wu0 + p > e, then e = eu (2) else, wu must be zero
+    wu = np.where(
+        pe > 0.0,
+        np.where(wu0 + pe - r < um, wu0 + pe - r, um),
+        np.where(wu0 + pe > 0.0, wu0 + pe, 0.0),
+    )
+    # calculate wd before wl because it is easier to cal using where statement
+    wd = np.where(
+        pe > 0.0,
+        np.where(wu0 + wl0 + pe - r > um + lm, wu0 + wl0 + wd0 + pe - r - um - lm, wd0),
+        wd0 - ed,
+    )
+    # water balance (equation 2.2 in Page 13, also shown in Page 23)
+    # if wu0 + p > e, then e = eu; else p must be used in upper layer,
+    # so no matter what the case is, el didn't include p, neither ed
+    wl = np.where(pe > 0.0, wu0 + wl0 + wd0 + pe - r - wu - wd, wl0 - el)
+    # the water storage should be in reasonable range
+    wu_ = np.clip(wu, a_min=0.0, a_max=um)
+    wl_ = np.clip(wl, a_min=0.0, a_max=lm)
+    wd_ = np.clip(wd, a_min=0.0, a_max=dm)
+    return wu_, wl_, wd_
+
+
+def generation(p_and_e, k, b, im, um, lm, dm, c, wu0=None, wl0=None, wd0=None) -> tuple:
+    """
+    Single-step runoff generation in XAJ.
+
+    Parameters
+    ----------
+    p_and_e
+        precipitation and potential evapotranspiration
+    k
+        ratio of potential evapotranspiration to reference crop evaporation
+    b
+        exponent parameter
+    um
+        average soil moisture storage capacity of the upper layer
+    lm
+        average soil moisture storage capacity of the lower layer
+    dm
+        average soil moisture storage capacity of the deep layer
+    im
+        impermeability coefficient
+    c
+        coefficient of deep layer
+    wu0
+        initial values of soil moisture in upper layer
+    wl0
+        initial values of soil moisture in lower layer
+    wd0
+        initial values of soil moisture in deep layer
+
+    Returns
+    -------
+    tuple[tuple, tuple]
+        (r, rim, e, pe), (wu, wl, wd); all variables are np.array
+    """
+    # make sure physical variables' value ranges are correct
+    prcp = np.maximum(p_and_e[:, 0], 0.0)
+    # get potential evapotranspiration
+    pet = np.maximum(p_and_e[:, 1] * k, 0.0)
+    # wm
+    wm = um + lm + dm
+    if wu0 is None:
+        # just an initial value
+        wu0 = 0.6 * um
+    if wl0 is None:
+        wl0 = 0.6 * lm
+    if wd0 is None:
+        wd0 = 0.6 * dm
+    w0_ = wu0 + wl0 + wd0
+
+    # w0 need locate in correct range so that following calculation could be right
+    # To make sure float data's calculation is correct, we'd better minus a precision (1e-5)
+    w0 = np.minimum(w0_, wm - 1e-5)
+
+    # Calculate the amount of evaporation from storage
+    eu, el, ed = calculate_evap(lm, c, wu0, wl0, prcp, pet)
+    e = eu + el + ed
+
+    # Calculate the runoff generated by net precipitation
+    prcp_difference = prcp - e
+    pe = np.maximum(prcp_difference, 0.0)
+    r, rim = calculate_prcp_runoff(b, im, wm, w0, pe)
+    # Update wu, wl, wd
+    wu, wl, wd = calculate_w_storage(
+        um, lm, dm, wu0, wl0, wd0, eu, el, ed, prcp_difference, r
+    )
+
+    return (r, rim, e, pe), (wu, wl, wd)
+
+
+def sources(pe, r, sm, ex, ki, kg, s0=None, fr0=None, book="HF") -> tuple:
+    """
+    Divide the runoff to different sources
+
+    We use the initial version from the paper of the inventor of the XAJ model -- Prof. Renjun Zhao:
+    "Analysis of parameters of the XinAnJiang model". Its Chinese name is <<新安江模型参数的分析>>,
+    which could be found by searching in "Baidu Xueshu".
+    The module's code can also be found in "Watershed Hydrologic Simulation" (WHS) Page 174.
+    It is nearly same with that in "Hydrologic Forecasting" (HF) Page 148-149
+    We use the period average runoff as input and the unit period is day so we don't need to difference it as books show
+
+    We also provide code for formula from《水文预报》"Hydrologic Forecasting" (HF) the fifth version. Page 40-41 and 150-151;
+    the procedures in 《工程水文学》"Engineering Hydrology" (EH) the third version are different we also provide.
+    they are in the "sources5mm" function.
+
+    Parameters
+    ------------
+    pe
+        net precipitation
+    r
+        runoff from xaj_generation
+    sm
+        areal mean free water capacity of the surface layer
+    ex
+        exponent of the free water capacity curve
+    ki
+        outflow coefficients of the free water storage to interflow relationships
+    kg
+        outflow coefficients of the free water storage to groundwater relationships
+    s0
+        free water capacity of last period
+    fr0
+        runoff area of last period
+
+    Return
+    ------------
+    tuple[tuple, tuple]
+        rs -- surface runoff; ri-- interflow runoff; rg -- groundwater runoff;
+        s1 -- final free water capacity;
+        all variables are numpy array
+
+    """
+    # maximum free water storage capacity in a basin
+    ms = sm * (1.0 + ex)
+    if fr0 is None:
+        fr0 = 0.1
+    if s0 is None:
+        s0 = 0.5 * sm
+    # For free water storage, because s is related to fr and s0 and fr0 are both values of last period,
+    # we have to trans the initial value of s from last period to this one.
+    # both WHS（流域水文模拟）'s sample code and HF（水文预报） use s = fr0 * s0 / fr.
+    # I think they both think free water reservoir as a cubic tank. Its height is s and area of bottom rectangle is fr
+    # we will have a cubic tank with varying bottom and height,
+    # and fixed boundary (in HF sm is fixed) or none-fixed boundary (in EH smmf is not fixed)
+    # but notice r's list like" [1,0] which 1 is the 1st period's runoff and 0 is the 2nd period's runoff
+    # after 1st period, the s1 could not be zero, but in the 2nd period, fr=0, then we cannot set s=0, because some water still in the tank
+    # fr's formula could be found in Eq. 9 in "Analysis of parameters of the XinAnJiang model",
+    # Here our r doesn't include rim, so there is no need to remove rim from r; this is also the method in 《水文预报》（HF）
+
+    # NOTE: when r is 0, fr should be 0, however, s1 may not be zero and it still hold some water,
+    # then fr can not be 0, otherwise when fr is used as denominator it lead to error,
+    # so we have to deal with this case later, for example, when r=0, we cannot use pe * fr to replace r
+    # because fr get the value of last period, and it is not 0
+    fr = np.copy(fr0)
+    if any(fr == 0.0):
+        raise ArithmeticError(
+            "Please check fr's value, fr==0.0 will cause error in the next step!"
+        )
+    # r=0, then r/pe must be 0
+    fr_mask = r > 0.0
+    fr[fr_mask] = r[fr_mask] / pe[fr_mask]
+    if np.isnan(fr).any():
+        raise ArithmeticError("Please check pe's data! there may be 0.0")
+
+    # if fr=0, then we cannot get ss, but ss should not be 0, because s1 of last period may not be 0 and it still hold some water
+    ss = np.copy(s0)
+    # same initialization for s
+    s = np.copy(s0)
+
+    ss[fr_mask] = fr0[fr_mask] * s0[fr_mask] / fr[fr_mask]
+
+    if book == "HF":
+        ss = np.minimum(ss, sm)
+        au = ms * (1.0 - (1.0 - ss / sm) ** (1.0 / (1.0 + ex)))
+        if np.isnan(au).any():
+            raise ValueError(
+                "Error: NaN values detected. Try set clip function or check your data!!!"
+            )
+        # the first condition should be r > 0.0, when r=0, rs must be 0, fig 6-12 in EH or fig 5-4 in HF
+        # so we have to use "pe" carefully!!! when r>0.0, we use pe, otherwise we don't use it!!!
+        rs = np.full(r.shape, 0.0)
+        rs[fr_mask] = np.where(
+            pe[fr_mask] + au[fr_mask] < ms[fr_mask],
+            # equation 2-85 in HF
+            fr[fr_mask]
+            * (
+                pe[fr_mask]
+                - sm[fr_mask]
+                + ss[fr_mask]
+                + sm[fr_mask]
+                * (
+                    (
+                        1
+                        - np.minimum(pe[fr_mask] + au[fr_mask], ms[fr_mask])
+                        / ms[fr_mask]
+                    )
+                    ** (1 + ex[fr_mask])
+                )
+            ),
+            # equation 2-86 in HF
+            fr[fr_mask] * (pe[fr_mask] + ss[fr_mask] - sm[fr_mask]),
+        )
+        rs = np.minimum(rs, r)
+
+        # ri's mask is not same as rs's, because last period's s may not be 0
+        # and in this time, ri and rg could be larger than 0
+        # we need firstly calculate the updated s, s's mask is same as fr_mask,
+        # when r==0, then s will be equal to last period's
+        # equation 2-87 in HF, some free water leave or save, so we update free water storage
+        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
+        s = np.minimum(s, sm)
+        if np.isnan(s).any():
+            raise ArithmeticError("Please check fr's data! there may be 0.0")
+
+    elif book == "EH":
+        # smmf should be with correpond with s
+        smmf = ms * (1 - (1 - fr) ** (1 / ex))
+        smf = smmf / (1 + ex)
+        ss = np.minimum(ss, smf)
+        au = smmf * (1 - (1 - ss / smf) ** (1 / (1 + ex)))
+        if np.isnan(au).any():
+            raise ValueError(
+                "Error: NaN values detected. Try set clip function or check your data!!!"
+            )
+
+        # rs's mask is keep with fr_mask
+        rs = np.full(r.shape, 0.0)
+        rs[fr_mask] = np.where(
+            pe[fr_mask] + au[fr_mask] < smmf[fr_mask],
+            (
+                pe[fr_mask]
+                - smf[fr_mask]
+                + ss[fr_mask]
+                + smf[fr_mask]
+                * (
+                    1
+                    - np.minimum(pe[fr_mask] + au[fr_mask], smmf[fr_mask])
+                    / smmf[fr_mask]
+                )
+                ** (ex[fr_mask] + 1)
+            )
+            * fr[fr_mask],
+            (pe[fr_mask] + ss[fr_mask] - smf[fr_mask]) * fr[fr_mask],
+        )
+        rs = np.minimum(rs, r)
+        s[fr_mask] = ss[fr_mask] + (r[fr_mask] - rs[fr_mask]) / fr[fr_mask]
+        s = np.minimum(s, smf)
+    else:
+        raise ValueError("Please set book as 'HF' or 'EH'!")
+    # the following part is same for both HF and EH. Even the formula is different, but their meaning is same
+    # equation 2-88 in HF, next interflow and ground water will be released from the updated free water storage
+    # We use the period average runoff as input and the general unit period is day.
+    # Hence, we directly use ki and kg rather than ki_{Δt} in books.
+    ri = ki * s * fr
+    rg = kg * s * fr
+    # ri = np.where(s < PRECISION, np.full(r.shape, 0.0), ki * s * fr)
+    # rg = np.where(s < PRECISION, np.full(r.shape, 0.0), kg * s * fr)
+    # equation 2-89 in HF; although it looks different with that in WHS, they are actually same
+    # Finally, calculate the final free water storage
+    s1 = s * (1 - ki - kg)
+    # s1 = np.where(s1 < PRECISION, np.full(s1.shape, 0.0), s1)
+    return (rs, ri, rg), (s1, fr)
+
+
+def sources5mm(
+    pe,
+    runoff,
+    sm,
+    ex,
+    ki,
+    kg,
+    s0=None,
+    fr0=None,
+    time_interval_hours=1,
+    book="HF",
+):
+    """
+    Divide the runoff to different sources according to books -- 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition
+
+    Parameters
+    ----------
+    pe
+        net precipitation
+    runoff
+        runoff from xaj_generation
+    sm
+        areal mean free water capacity of the surface layer
+    ex
+        exponent of the free water capacity curve
+    ki
+        outflow coefficients of the free water storage to interflow relationships
+    kg
+        outflow coefficients of the free water storage to groundwater relationships
+    s0
+        initial free water capacity
+    fr0
+        initial area of generation
+    time_interval_hours
+        由于Ki、Kg、Ci、Cg都是以24小时为时段长定义的,需根据时段长转换
+    book
+        the methods in 《水文预报》HF 5th edition and 《工程水文学》EH 3rd edition are different,
+        hence, both are provided, and the default is the former -- "ShuiWenYuBao";
+        the other one is "GongChengShuiWenXue"
+
+    Returns
+    -------
+    tuple[tuple, tuple]
+        rs_s -- surface runoff; rss_s-- interflow runoff; rg_s -- groundwater runoff;
+        (fr_ds[-1], s_ds[-1]): state variables' final value;
+        all variables are numpy array
+    """
+    # Convert Ki and Kg according to the time interval, as they are defined based on a 24-hour time interval
+    hours_per_day = 24
+    # Non-divisible case, add 1 to the period
+    residue_temp = hours_per_day % time_interval_hours
+    if residue_temp != 0:
+        residue_temp = 1
+    period_num_1d = int(hours_per_day / time_interval_hours) + residue_temp
+    # When kss+kg>1, the square root becomes a complex number during even root calculation, which will cause an error here.
+    # Also, be aware that the denominator may be 0, kss cannot be 0.
+    # Restrict the value of kss+kg.
+    kss_period = (1 - (1 - (ki + kg)) ** (1 / period_num_1d)) / (1 + kg / ki)
+    kg_period = kss_period * kg / ki
+
+    # Maximum free water storage capacity depth of the basin
+    smm = sm * (1 + ex)
+    if s0 is None:
+        s0 = 0.50 * sm
+    if fr0 is None:
+        fr0 = 0.1
+    # don't use np.where here, because it will cause some warning
+    fr = np.copy(fr0)
+    fr_mask = runoff > 0.0
+    fr[fr_mask] = runoff[fr_mask] / pe[fr_mask]
+    if np.all(runoff < 5):
+        n = 1
+    else:
+        # when modeling multiple basins, the number of divides is not the same, so we use the maximum number
+        r_max = np.max(runoff)
+        residue_temp = r_max % 5
+        if residue_temp != 0:
+            residue_temp = 1
+        n = int(r_max / 5) + residue_temp
+    rn = runoff / n
+    pen = pe / n
+    kss_d = (1 - (1 - (kss_period + kg_period)) ** (1 / n)) / (
+        1 + kg_period / kss_period
+    )
+    kg_d = kss_d * kg_period / kss_period
+    # kss_d = kss_period
+    # kg_d = kg_period
+    rs = np.full(runoff.shape, 0.0)
+    rss = np.full(runoff.shape, 0.0)
+    rg = np.full(runoff.shape, 0.0)
+
+    s_ds = []
+    fr_ds = []
+    s_ds.append(s0)
+    fr_ds.append(fr0)
+
+    for j in range(n):
+        fr0_d = fr_ds[j]
+        s0_d = s_ds[j]
+        # equation 5-32 in HF, but strange, cause each period, rn/pen is same, fr_d should be same
+        # fr_d = 1 - (1 - fr) ** (1 / n)
+        fr_d = fr
+
+        ss_d = np.copy(s0_d)
+        s_d = np.copy(s0_d)
+        s1_d = np.copy(s0_d)
+
+        ss_d[fr_mask] = fr0_d[fr_mask] * s0_d[fr_mask] / fr_d[fr_mask]
+
+        if book == "HF":
+            ss_d = np.minimum(ss_d, sm)
+            # ms = smm
+            au = smm * (1.0 - (1.0 - ss_d / sm) ** (1.0 / (1.0 + ex)))
+            if np.isnan(au).any():
+                raise ValueError(
+                    "Error: NaN values detected. Try set clip function or check your data!!!"
+                )
+            rs_j = np.full(rn.shape, 0.0)
+            rs_j[fr_mask] = np.where(
+                pen[fr_mask] + au[fr_mask] < smm[fr_mask],
+                # equation 5-26 in HF
+                fr_d[fr_mask]
+                * (
+                    pen[fr_mask]
+                    - sm[fr_mask]
+                    + ss_d[fr_mask]
+                    + sm[fr_mask]
+                    * (
+                        (
+                            1
+                            - np.minimum(pen[fr_mask] + au[fr_mask], smm[fr_mask])
+                            / smm[fr_mask]
+                        )
+                        ** (1 + ex[fr_mask])
+                    )
+                ),
+                # equation 5-27 in HF
+                fr_d[fr_mask] * (pen[fr_mask] + ss_d[fr_mask] - sm[fr_mask]),
+            )
+            rs_j = np.minimum(rs_j, rn)
+            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
+            s_d = np.minimum(s_d, sm)
+
+        elif book == "EH":
+            smmf = smm * (1 - (1 - fr_d) ** (1 / ex))
+            smf = smmf / (1 + ex)
+            ss_d = np.minimum(ss_d, smf)
+            au = smmf * (1 - (1 - ss_d / smf) ** (1 / (1 + ex)))
+            if np.isnan(au).any():
+                raise ValueError(
+                    "Error: NaN values detected. Try set clip function or check your data!!!"
+                )
+            rs_j = np.full(rn.shape, 0.0)
+            rs_j[fr_mask] = np.where(
+                pen[fr_mask] + au[fr_mask] < smmf[fr_mask],
+                (
+                    pen[fr_mask]
+                    - smf[fr_mask]
+                    + ss_d[fr_mask]
+                    + smf[fr_mask]
+                    * (
+                        1
+                        - np.minimum(pen[fr_mask] + au[fr_mask], smmf[fr_mask])
+                        / smmf[fr_mask]
+                    )
+                    ** (ex[fr_mask] + 1)
+                )
+                * fr_d[fr_mask],
+                (pen[fr_mask] + ss_d[fr_mask] - smf[fr_mask]) * fr_d[fr_mask],
+            )
+            rs_j = np.minimum(rs_j, rn)
+            s_d[fr_mask] = ss_d[fr_mask] + (rn[fr_mask] - rs_j[fr_mask]) / fr_d[fr_mask]
+            s_d = np.minimum(s_d, smf)
+
+        else:
+            raise NotImplementedError(
+                "We don't have this implementation! Please chose 'HF' or 'EH'!!"
+            )
+        rss_j = s_d * kss_d * fr_d
+        rg_j = s_d * kg_d * fr_d
+        s1_d = s_d * (1 - kss_d - kg_d)
+
+        rs = rs + rs_j
+        rss = rss + rss_j
+        rg = rg + rg_j
+        # Assign s_d and fr_d to the arrays as initial values for the next segment
+        s_ds.append(s1_d)
+        fr_ds.append(fr_d)
+
+    return (rs, rss, rg), (s_ds[-1], fr_ds[-1])
+
+
+# @jit
+# @jit(nopython=True)
+def linear_reservoir(x, weight, last_y=None) -> np.array:
+    """
+    Linear reservoir's release function
+
+    Parameters
+    ----------
+    x
+        the input to the linear reservoir
+    weight
+        the coefficient of linear reservoir
+    last_y
+        the output of last period
+
+    Returns
+    -------
+    np.array
+        one-step forward result
+    """
+    weight1 = 1 - weight
+    if last_y is None:
+        last_y = np.full(weight.shape, 0.001)
+    return weight * last_y + weight1 * x
+
+
+def uh_conv(x, uh_from_gamma):
+    """
+    Function for 1d-convolution calculation
+
+    Parameters
+    ----------
+    x
+        x is a sequence-first variable; the dim of x is [seq, batch, feature=1];
+        feature must be 1
+    uh_from_gamma
+        unit hydrograph from uh_gamma; the dim: [len_uh, batch, feature=1];
+        feature must be 1
+
+    Returns
+    -------
+    np.array
+        convolution
+    """
+    outputs = np.full(x.shape, 0.0)
+    time_length, batch_size, feature_size = x.shape
+    if feature_size > 1:
+        logging.error("We only support one-dim convolution now!!!")
+    for i in range(batch_size):
+        uh = uh_from_gamma[:, i, 0]
+        inputs = x[:, i, 0]
+        outputs[:, i, 0] = np.convolve(inputs, uh)[:time_length]
+    return outputs
+
+
+def uh_gamma(a, theta, len_uh=15):
+    """
+    A simple two-parameter Gamma distribution as a unit-hydrograph to route instantaneous runoff from a hydrologic model
+    The method comes from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
+
+    Parameters
+    ----------
+    a
+        shape parameter
+    theta
+        timescale parameter
+    len_uh
+        the time length of the unit hydrograph
+    Returns
+    -------
+    torch.Tensor
+        the unit hydrograph, dim: [seq, batch, feature]
+    """
+    # dims of a: time_seq (same all time steps), batch, feature=1
+    m = a.shape
+    if len_uh > m[0]:
+        raise RuntimeError(
+            "length of unit hydrograph should be smaller than the whole length of input"
+        )
+    # aa > 0, here we set minimum 0.1 (min of a is 0, set when calling this func); First dimension of a is repeat
+    aa = np.maximum(0.0, a[0:len_uh, :, :]) + 0.1
+    # theta > 0, here set minimum 0.5
+    theta = np.maximum(0.0, theta[0:len_uh, :, :]) + 0.5
+    # len_f, batch, feature
+    t = np.expand_dims(
+        np.swapaxes(np.tile(np.arange(0.5, len_uh * 1.0), (m[1], 1)), 0, 1), axis=-1
+    )
+    denominator = gamma(aa) * (theta**aa)
+    # [len_f, m[1], m[2]]
+    w = 1 / denominator * (t ** (aa - 1)) * (np.exp(-t / theta))
+    w = w / w.sum(0)  # scale to 1 for each UH
+    return w
+
+
+def xaj(
+    p_and_e,
+    params: Union[np.array, list],
+    return_state=False,
+    warmup_length=365,
+    **kwargs,
+) -> Union[tuple, np.array]:
+    """
+    run XAJ model
+
+    Parameters
+    ----------
+    p_and_e
+        prcp and pet; sequence-first (time is the first dim) 3-d np array: [time, basin, feature=2]
+    params
+        parameters of XAJ model for basin(s);
+        2-dim variable -- [basin, parameter]:
+        the parameters are B IM UM LM DM C SM EX KI KG A THETA CI CG (notice the sequence)
+    return_state
+        if True, return state values, mainly for warmup periods
+    warmup_length
+        hydro models need a warm-up period to get good initial state values
+    kwargs
+        route_method
+            now we provide two ways: "CSL" (recession constant + lag time) and "MZ" (method from mizuRoute)
+        source_type
+            default is "sources" and it will call "sources" function; the other is "sources5mm",
+            and we will divide the runoff to some <5mm pieces according to the books in this case
+        source_book
+            When source_type is "sources5mm" there are two implementions for dividing sources,
+            as the methods in "ShuiWenYuBao" and "GongChengShuiWenXue"" are different.
+            Hence, both are provided, and the default is the former.
+
+    Returns
+    -------
+    Union[np.array, tuple]
+        streamflow or (streamflow, states)
+    """
+    # default values for some function parameters
+    model_name = kwargs.get("name", "xaj")
+    source_type = kwargs.get("source_type", "sources")
+    source_book = kwargs.get("source_book", "HF")
+    time_interval_hours = kwargs.get("time_interval_hours", 1)
+    pr_file = kwargs.get("param_range_file", None)
+    model_param_dict = read_model_param_dict(pr_file)
+    # params
+    param_ranges = model_param_dict[model_name]["param_range"]
+    if model_name == "xaj":
+        route_method = "CSL"
+    elif model_name == "xaj_mz":
+        route_method = "MZ"
+    else:
+        raise NotImplementedError(
+            "We don't provide this route method now! Please use 'CSL' or 'MZ'!"
+        )
+    if np.isnan(params).any():
+        raise ValueError(
+            "Parameters contain NaN values. Please check your opt algorithm"
+        )
+    xaj_params = [
+        (value[1] - value[0]) * params[:, i] + value[0]
+        for i, (key, value) in enumerate(param_ranges.items())
+    ]
+
+    k = xaj_params[0]
+    b = xaj_params[1]
+    im = xaj_params[2]
+    um = xaj_params[3]
+    lm = xaj_params[4]
+    dm = xaj_params[5]
+    c = xaj_params[6]
+    sm = xaj_params[7]
+    ex = xaj_params[8]
+    ki_ = xaj_params[9]
+    kg_ = xaj_params[10]
+    # ki+kg should be smaller than 1; if not, we scale them
+    ki = np.where(ki_ + kg_ < 1.0, ki_, (1.0 - PRECISION) / (ki_ + kg_) * ki_)
+    kg = np.where(ki_ + kg_ < 1.0, kg_, (1.0 - PRECISION) / (ki_ + kg_) * kg_)
+    if route_method == "CSL":
+        cs = xaj_params[11]
+        l = xaj_params[12]
+    elif route_method == "MZ":
+        # we will use routing method from mizuRoute -- http://www.geosci-model-dev.net/9/2223/2016/
+        a = xaj_params[11]
+        theta = xaj_params[12]
+        # make it as a parameter
+        kernel_size = int(xaj_params[15])
+    else:
+        raise NotImplementedError(
+            "We don't provide this route method now! Please use 'CSL' or 'MZ'!"
+        )
+    ci = xaj_params[13]
+    cg = xaj_params[14]
+
+    # initialize state values
+    if warmup_length > 0:
+        p_and_e_warmup = p_and_e[0:warmup_length, :, :]
+        _q, _e, *w0, s0, fr0, qi0, qg0 = xaj(
+            p_and_e_warmup,
+            params,
+            return_state=True,
+            warmup_length=0,
+            **kwargs,
+        )
+    else:
+        w0 = (0.5 * um, 0.5 * lm, 0.5 * dm)
+        s0 = 0.5 * sm
+        fr0 = np.full(ex.shape, 0.1)
+        qi0 = np.full(ci.shape, 0.1)
+        qg0 = np.full(cg.shape, 0.1)
+
+    # state_variables
+    inputs = p_and_e[warmup_length:, :, :]
+    runoff_ims_ = np.full(inputs.shape[:2], 0.0)
+    rss_ = np.full(inputs.shape[:2], 0.0)
+    ris_ = np.full(inputs.shape[:2], 0.0)
+    rgs_ = np.full(inputs.shape[:2], 0.0)
+    es_ = np.full(inputs.shape[:2], 0.0)
+    for i in range(inputs.shape[0]):
+        if i == 0:
+            (r, rim, e, pe), w = generation(
+                inputs[i, :, :], k, b, im, um, lm, dm, c, *w0
+            )
+            if source_type == "sources":
+                (rs, ri, rg), (s, fr) = sources(
+                    pe, r, sm, ex, ki, kg, s0, fr0, book=source_book
+                )
+            elif source_type == "sources5mm":
+                (rs, ri, rg), (s, fr) = sources5mm(
+                    pe, r, sm, ex, ki, kg, s0, fr0, time_interval_hours=time_interval_hours, book=source_book
+                )
+            else:
+                raise NotImplementedError("No such divide-sources method")
+        else:
+            (r, rim, e, pe), w = generation(
+                inputs[i, :, :], k, b, im, um, lm, dm, c, *w
+            )
+            if source_type == "sources":
+                (rs, ri, rg), (s, fr) = sources(
+                    pe, r, sm, ex, ki, kg, s, fr, book=source_book
+                )
+            elif source_type == "sources5mm":
+                (rs, ri, rg), (s, fr) = sources5mm(
+                    pe, r, sm, ex, ki, kg, s, fr, time_interval_hours=time_interval_hours, book=source_book
+                )
+            else:
+                raise NotImplementedError("No such divide-sources method")
+        # impevious part is pe * im
+        runoff_ims_[i, :] = rim
+        # so for non-imprvious part, the result should be corrected
+        rss_[i, :] = rs * (1 - im)
+        ris_[i, :] = ri * (1 - im)
+        rgs_[i, :] = rg * (1 - im)
+        es_[i, :] = e
+    # seq, batch, feature
+    runoff_im = np.expand_dims(runoff_ims_, axis=2)
+    rss = np.expand_dims(rss_, axis=2)
+    es = np.expand_dims(es_, axis=2)
+
+    qs = np.full(inputs.shape[:2], 0.0)
+    if route_method == "CSL":
+        qt = np.full(inputs.shape[:2], 0.0)
+        for i in range(inputs.shape[0]):
+            if i == 0:
+                qi = linear_reservoir(ris_[i], ci, qi0)
+                qg = linear_reservoir(rgs_[i], cg, qg0)
+            else:
+                qi = linear_reservoir(ris_[i], ci, qi)
+                qg = linear_reservoir(rgs_[i], cg, qg)
+            qs_ = rss_[i]
+            qt[i, :] = qs_ + qi + qg
+        for j in range(len(l)):
+            lag = int(l[j])
+            for i in range(lag):
+                qs[i, j] = qt[i, j]
+            for i in range(lag, inputs.shape[0]):
+                qs[i, j] = cs[j] * qs[i - 1, j] + (1 - cs[j]) * qt[i - lag, j]
+    elif route_method == "MZ":
+        rout_a = a.repeat(rss.shape[0]).reshape(rss.shape)
+        rout_b = theta.repeat(rss.shape[0]).reshape(rss.shape)
+        conv_uh = uh_gamma(rout_a, rout_b, kernel_size)
+        qs_ = uh_conv(runoff_im + rss, conv_uh)
+        for i in range(inputs.shape[0]):
+            if i == 0:
+                qi = linear_reservoir(ris_[i], ci, qi0)
+                qg = linear_reservoir(rgs_[i], cg, qg0)
+            else:
+                qi = linear_reservoir(ris_[i], ci, qi)
+                qg = linear_reservoir(rgs_[i], cg, qg)
+            qs[i, :] = qs_[i, :, 0] + qi + qg
+    else:
+        raise NotImplementedError(
+            "We don't provide this route method now! Please use 'CS' or 'MZ'!"
+        )
+
+    # seq, batch, feature
+    q_sim = np.expand_dims(qs, axis=2)
+    if return_state:
+        return q_sim, es, *w, s, fr, qi, qg
+    return q_sim, es
```

### Comparing `hydromodel-0.2.2/hydromodel/models/xaj_bmi.py` & `hydromodel-0.2.3/hydromodel/models/xaj_bmi.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,292 +1,292 @@
-from typing import Tuple
-from bmipy import Bmi
-import numpy as np
-
-import datetime
-import pandas as pd
-import logging
-
-logger = logging.getLogger(__name__)
-
-PRECISION = 1e-5
-
-
-class xajBmi(Bmi):
-    """Empty model wrapped in a BMI interface.
-    TODO: not implemented yet
-    """
-
-    name = "hydro-model-xaj"
-    input_var_names = ("precipitation", "ETp")
-    output_var_names = ("ET", "discharge")
-    var_units = {
-        "precipitation": "mm/day",
-        "ETp": "mm/day",
-        "discharge": "mm/day",
-        "ET": "mm/day",
-    }
-
-    def __init__(self):
-        """Create a BmiHeat model that is ready for initialization."""
-        self.time_step = 0
-
-    def initialize(self, config_file):
-        try:
-            logger.info("xaj: initialize_model")
-            config = configuration.read_config(config_file)
-            forcing_data = pd.read_csv(config["forcing_file"])
-            p_and_e_df, p_and_e = configuration.extract_forcing(forcing_data)
-            p_and_e_warmup = p_and_e[0 : config["warmup_length"], :, :]
-            params = np.tile([0.5], (1, 15))
-            (
-                self.q_sim_state,
-                self.es_state,
-                self.w0,
-                self.w1,
-                self.w2,
-                self.s0,
-                self.fr0,
-                self.qi0,
-                self.qg0,
-            ) = configuration.warmup(p_and_e_warmup, params, config["warmup_length"])
-
-            self._start_time_str, self._end_time_str, self._time_units = (
-                configuration.get_time_config(config)
-            )
-
-            self.params = params
-            self.warmup_length = config["warmup_length"]
-            self.p_and_e_df = p_and_e_df
-            self.p_and_e = p_and_e
-            self.config = config
-            self.basin_area = config["basin_area"]
-
-        except:
-            import traceback
-
-            traceback.print_exc()
-            raise
-
-    def update(self):
-        """Update model for a single time step."""
-
-        self.time_step += 1
-        # p_and_e_sim = self.p_and_e[self.warmup_length+1:self.time_step+self.warmup_length+1]
-        p_and_e_sim = self.p_and_e[1 : self.time_step + 1]
-        self.runoff_im, self.rss_, self.ris_, self.rgs_, self.es_runoff, self.rss = (
-            xaj_runoff(
-                p_and_e_sim,
-                w0=self.w0,
-                s0=self.s0,
-                fr0=self.fr0,
-                params_runoff=self.params,
-                return_state=False,
-            )
-        )
-        if self.time_step + self.warmup_length + 1 >= self.p_and_e.shape[0]:
-            q_sim, es = xaj_route(
-                p_and_e_sim,
-                params_route=self.params,
-                model_name="xaj",
-                runoff_im=self.runoff_im,
-                rss_=self.rss_,
-                ris_=self.ris_,
-                rgs_=self.rgs_,
-                rss=self.rss,
-                qi0=self.qi0,
-                qg0=self.qg0,
-                es=self.es_runoff,
-            )
-            self.p_sim = p_and_e_sim[:, :, 0]
-            self.e_sim = p_and_e_sim[:, :, 1]
-            q_sim = convert_unit(
-                q_sim,
-                unit_now="mm/day",
-                unit_final=unit["streamflow"],
-                basin_area=float(self.basin_area),
-            )
-            self.q_sim = q_sim
-            self.es = es
-
-    def update_until(self, time):
-        while self.get_current_time() + 0.001 < time:
-            self.update()
-
-    def finalize(self) -> None:
-        """Finalize model."""
-        self.model = None
-
-    def get_component_name(self) -> str:
-        return "xaj"
-
-    def get_input_item_count(self) -> int:
-        return len(self.input_var_names)
-
-    def get_output_item_count(self) -> int:
-        return len(self.output_var_names)
-
-    def get_input_var_names(self) -> Tuple[str]:
-        return self.input_var_names
-
-    def get_output_var_names(self) -> Tuple[str]:
-        return self.output_var_names
-
-    def get_var_grid(self, name: str) -> int:
-        raise NotImplementedError()
-
-    def get_var_type(self, name: str) -> str:
-        return "float64"
-
-    def get_var_units(self, name: str) -> str:
-        return self.var_units[name]
-
-    def get_var_itemsize(self, name: str) -> int:
-        return np.dtype(self.get_var_type(name)).itemsize
-
-    def get_var_nbytes(self, name: str) -> int:
-        return self.get_value_ptr(name).nbytes
-
-    def get_var_location(self, name: str) -> str:
-        raise NotImplementedError()
-
-    def get_start_time(self):
-        return self.start_Time(self._start_time_str)
-
-    def get_current_time(self):
-        # return self.start_Time(self._start_time_str) + datetime.timedelta(self.time_step+self.warmup_length)
-        if self._time_units == "hours":
-            time_step = datetime.timedelta(hours=self.time_step)
-        elif self._time_units == "days":
-            time_step = datetime.timedelta(days=self.time_step)
-        return self.start_Time(self._start_time_str) + time_step
-
-    def get_end_time(self):
-        return self.end_Time(self._end_time_str)
-
-    def get_time_units(self) -> str:
-        return self._time_units
-
-    def get_time_step(self) -> float:
-        return 1
-
-    def get_value(self, name: str) -> None:
-        logger.info("getting value for var %s", name)
-        return self.get_value_ptr(name).flatten()
-
-    def get_value_ptr(self, name: str) -> np.ndarray:
-        if name == "discharge":
-            return self.q_sim
-        elif name == "ET":
-            return self.es
-
-    def get_value_at_indices(self, name: str, inds: np.ndarray) -> np.ndarray:
-
-        return self.get_value_ptr(name).take(inds)
-
-    def set_value(self, name: str, src: np.ndarray):
-
-        val = self.get_value_ptr(name)
-        val[:] = src.reshape(val.shape)
-
-    def set_value_at_indices(
-        self, name: str, inds: np.ndarray, src: np.ndarray
-    ) -> None:
-        val = self.get_value_ptr(name)
-        val.flat[inds] = src
-
-    # Grid information
-    def get_grid_rank(self, grid: int) -> int:
-        raise NotImplementedError()
-
-    def get_grid_size(self, grid: int) -> int:
-        raise NotImplementedError()
-
-    def get_grid_type(self, grid: int) -> str:
-        raise NotImplementedError()
-
-    # Uniform rectilinear
-    def get_grid_shape(self, grid: int, shape: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_spacing(self, grid: int, spacing: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_origin(self, grid: int, origin: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    # Non-uniform rectilinear, curvilinear
-    def get_grid_x(self, grid: int, x: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_y(self, grid: int, y: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_z(self, grid: int, z: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_node_count(self, grid: int) -> int:
-        raise NotImplementedError()
-
-    def get_grid_edge_count(self, grid: int) -> int:
-        raise NotImplementedError()
-
-    def get_grid_face_count(self, grid: int) -> int:
-        raise NotImplementedError()
-
-    def get_grid_edge_nodes(self, grid: int, edge_nodes: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_face_edges(self, grid: int, face_edges: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_face_nodes(self, grid: int, face_nodes: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    def get_grid_nodes_per_face(
-        self, grid: int, nodes_per_face: np.ndarray
-    ) -> np.ndarray:
-        raise NotImplementedError()
-
-    def start_Time(self, _start_time_str):
-
-        try:
-            if " " in _start_time_str:
-                date, time = _start_time_str.split(" ")
-            else:
-                date = _start_time_str
-                time = None
-            year, month, day = date.split("-")
-            self._startTime = datetime.date(int(year), int(month), int(day))
-
-            if time:
-                hour, minute, second = time.split(":")
-                # self._startTime = self._startTime.replace(hour=int(hour),
-                #                                       minute=int(minute),
-                #                                       second=int(second))
-                self._startTime = datetime.datetime(
-                    int(year), int(month), int(day), int(hour), int(minute), int(second)
-                )
-        except ValueError:
-            raise ValueError("Invalid start date format!")
-
-        return self._startTime
-
-    def end_Time(self, _end_time_str):
-
-        try:
-            if " " in _end_time_str:
-                date, time = _end_time_str.split(" ")
-            else:
-                date = _end_time_str
-                time = None
-            year, month, day = date.split("-")
-            self._endTime = datetime.date(int(year), int(month), int(day))
-
-            if time:
-                hour, minute, second = time.split(":")
-                self._endTime = datetime.datetime(
-                    int(year), int(month), int(day), int(hour), int(minute), int(second)
-                )
-        except ValueError:
-            raise ValueError("Invalid start date format!")
-        return self._endTime
+from typing import Tuple
+from bmipy import Bmi
+import numpy as np
+
+import datetime
+import pandas as pd
+import logging
+
+logger = logging.getLogger(__name__)
+
+PRECISION = 1e-5
+
+
+class xajBmi(Bmi):
+    """Empty model wrapped in a BMI interface.
+    TODO: not implemented yet
+    """
+
+    name = "hydro-model-xaj"
+    input_var_names = ("precipitation", "ETp")
+    output_var_names = ("ET", "discharge")
+    var_units = {
+        "precipitation": "mm/day",
+        "ETp": "mm/day",
+        "discharge": "mm/day",
+        "ET": "mm/day",
+    }
+
+    def __init__(self):
+        """Create a BmiHeat model that is ready for initialization."""
+        self.time_step = 0
+
+    def initialize(self, config_file):
+        try:
+            logger.info("xaj: initialize_model")
+            config = configuration.read_config(config_file)
+            forcing_data = pd.read_csv(config["forcing_file"])
+            p_and_e_df, p_and_e = configuration.extract_forcing(forcing_data)
+            p_and_e_warmup = p_and_e[0 : config["warmup_length"], :, :]
+            params = np.tile([0.5], (1, 15))
+            (
+                self.q_sim_state,
+                self.es_state,
+                self.w0,
+                self.w1,
+                self.w2,
+                self.s0,
+                self.fr0,
+                self.qi0,
+                self.qg0,
+            ) = configuration.warmup(p_and_e_warmup, params, config["warmup_length"])
+
+            self._start_time_str, self._end_time_str, self._time_units = (
+                configuration.get_time_config(config)
+            )
+
+            self.params = params
+            self.warmup_length = config["warmup_length"]
+            self.p_and_e_df = p_and_e_df
+            self.p_and_e = p_and_e
+            self.config = config
+            self.basin_area = config["basin_area"]
+
+        except:
+            import traceback
+
+            traceback.print_exc()
+            raise
+
+    def update(self):
+        """Update model for a single time step."""
+
+        self.time_step += 1
+        # p_and_e_sim = self.p_and_e[self.warmup_length+1:self.time_step+self.warmup_length+1]
+        p_and_e_sim = self.p_and_e[1 : self.time_step + 1]
+        self.runoff_im, self.rss_, self.ris_, self.rgs_, self.es_runoff, self.rss = (
+            xaj_runoff(
+                p_and_e_sim,
+                w0=self.w0,
+                s0=self.s0,
+                fr0=self.fr0,
+                params_runoff=self.params,
+                return_state=False,
+            )
+        )
+        if self.time_step + self.warmup_length + 1 >= self.p_and_e.shape[0]:
+            q_sim, es = xaj_route(
+                p_and_e_sim,
+                params_route=self.params,
+                model_name="xaj",
+                runoff_im=self.runoff_im,
+                rss_=self.rss_,
+                ris_=self.ris_,
+                rgs_=self.rgs_,
+                rss=self.rss,
+                qi0=self.qi0,
+                qg0=self.qg0,
+                es=self.es_runoff,
+            )
+            self.p_sim = p_and_e_sim[:, :, 0]
+            self.e_sim = p_and_e_sim[:, :, 1]
+            q_sim = convert_unit(
+                q_sim,
+                unit_now="mm/day",
+                unit_final=unit["streamflow"],
+                basin_area=float(self.basin_area),
+            )
+            self.q_sim = q_sim
+            self.es = es
+
+    def update_until(self, time):
+        while self.get_current_time() + 0.001 < time:
+            self.update()
+
+    def finalize(self) -> None:
+        """Finalize model."""
+        self.model = None
+
+    def get_component_name(self) -> str:
+        return "xaj"
+
+    def get_input_item_count(self) -> int:
+        return len(self.input_var_names)
+
+    def get_output_item_count(self) -> int:
+        return len(self.output_var_names)
+
+    def get_input_var_names(self) -> Tuple[str]:
+        return self.input_var_names
+
+    def get_output_var_names(self) -> Tuple[str]:
+        return self.output_var_names
+
+    def get_var_grid(self, name: str) -> int:
+        raise NotImplementedError()
+
+    def get_var_type(self, name: str) -> str:
+        return "float64"
+
+    def get_var_units(self, name: str) -> str:
+        return self.var_units[name]
+
+    def get_var_itemsize(self, name: str) -> int:
+        return np.dtype(self.get_var_type(name)).itemsize
+
+    def get_var_nbytes(self, name: str) -> int:
+        return self.get_value_ptr(name).nbytes
+
+    def get_var_location(self, name: str) -> str:
+        raise NotImplementedError()
+
+    def get_start_time(self):
+        return self.start_Time(self._start_time_str)
+
+    def get_current_time(self):
+        # return self.start_Time(self._start_time_str) + datetime.timedelta(self.time_step+self.warmup_length)
+        if self._time_units == "hours":
+            time_step = datetime.timedelta(hours=self.time_step)
+        elif self._time_units == "days":
+            time_step = datetime.timedelta(days=self.time_step)
+        return self.start_Time(self._start_time_str) + time_step
+
+    def get_end_time(self):
+        return self.end_Time(self._end_time_str)
+
+    def get_time_units(self) -> str:
+        return self._time_units
+
+    def get_time_step(self) -> float:
+        return 1
+
+    def get_value(self, name: str) -> None:
+        logger.info("getting value for var %s", name)
+        return self.get_value_ptr(name).flatten()
+
+    def get_value_ptr(self, name: str) -> np.ndarray:
+        if name == "discharge":
+            return self.q_sim
+        elif name == "ET":
+            return self.es
+
+    def get_value_at_indices(self, name: str, inds: np.ndarray) -> np.ndarray:
+
+        return self.get_value_ptr(name).take(inds)
+
+    def set_value(self, name: str, src: np.ndarray):
+
+        val = self.get_value_ptr(name)
+        val[:] = src.reshape(val.shape)
+
+    def set_value_at_indices(
+        self, name: str, inds: np.ndarray, src: np.ndarray
+    ) -> None:
+        val = self.get_value_ptr(name)
+        val.flat[inds] = src
+
+    # Grid information
+    def get_grid_rank(self, grid: int) -> int:
+        raise NotImplementedError()
+
+    def get_grid_size(self, grid: int) -> int:
+        raise NotImplementedError()
+
+    def get_grid_type(self, grid: int) -> str:
+        raise NotImplementedError()
+
+    # Uniform rectilinear
+    def get_grid_shape(self, grid: int, shape: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_spacing(self, grid: int, spacing: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_origin(self, grid: int, origin: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    # Non-uniform rectilinear, curvilinear
+    def get_grid_x(self, grid: int, x: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_y(self, grid: int, y: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_z(self, grid: int, z: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_node_count(self, grid: int) -> int:
+        raise NotImplementedError()
+
+    def get_grid_edge_count(self, grid: int) -> int:
+        raise NotImplementedError()
+
+    def get_grid_face_count(self, grid: int) -> int:
+        raise NotImplementedError()
+
+    def get_grid_edge_nodes(self, grid: int, edge_nodes: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_face_edges(self, grid: int, face_edges: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_face_nodes(self, grid: int, face_nodes: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    def get_grid_nodes_per_face(
+        self, grid: int, nodes_per_face: np.ndarray
+    ) -> np.ndarray:
+        raise NotImplementedError()
+
+    def start_Time(self, _start_time_str):
+
+        try:
+            if " " in _start_time_str:
+                date, time = _start_time_str.split(" ")
+            else:
+                date = _start_time_str
+                time = None
+            year, month, day = date.split("-")
+            self._startTime = datetime.date(int(year), int(month), int(day))
+
+            if time:
+                hour, minute, second = time.split(":")
+                # self._startTime = self._startTime.replace(hour=int(hour),
+                #                                       minute=int(minute),
+                #                                       second=int(second))
+                self._startTime = datetime.datetime(
+                    int(year), int(month), int(day), int(hour), int(minute), int(second)
+                )
+        except ValueError:
+            raise ValueError("Invalid start date format!")
+
+        return self._startTime
+
+    def end_Time(self, _end_time_str):
+
+        try:
+            if " " in _end_time_str:
+                date, time = _end_time_str.split(" ")
+            else:
+                date = _end_time_str
+                time = None
+            year, month, day = date.split("-")
+            self._endTime = datetime.date(int(year), int(month), int(day))
+
+            if time:
+                hour, minute, second = time.split(":")
+                self._endTime = datetime.datetime(
+                    int(year), int(month), int(day), int(hour), int(minute), int(second)
+                )
+        except ValueError:
+            raise ValueError("Invalid start date format!")
+        return self._endTime
```

### Comparing `hydromodel-0.2.2/hydromodel/trainers/calibrate_ga.py` & `hydromodel-0.2.3/hydromodel/trainers/calibrate_ga.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,375 +1,375 @@
-"""
-Author: Wenyu Ouyang
-Date: 2021-12-10 23:01:02
-LastEditTime: 2024-03-27 15:11:04
-LastEditors: Wenyu Ouyang
-Description: Calibrate XAJ model using DEAP
-FilePath: \hydro-model-xaj\hydromodel\trainers\calibrate_ga.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import pickle
-from deap import base, creator
-import random
-from deap import tools
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-
-from hydroutils import hydro_file, hydro_stat
-
-
-from datasets.data_visualize import plot_sim_and_obs, plot_train_iteration
-from hydromodel.models.model_config import read_model_param_dict
-from hydromodel.models.model_dict import MODEL_DICT, rmse43darr
-
-
-def evaluate(individual, x_input, y_true, warmup_length, model):
-    """
-    Calculate fitness for optimization
-
-    Parameters
-    ----------
-    individual
-        individual is the params of XAJ (see details in xaj.py); we initialize all parameters in range [0,1]
-    x_input
-        input of XAJ
-    y_true
-        observation data; we use the part after warmup period
-    warmup_length
-        the length of warmup period
-    model
-        model's config
-
-    Returns
-    -------
-    float
-        fitness
-    """
-    # print("Calculate fitness:")
-    # NOTE: Now only support one basin's calibration for once now
-    params = np.array(individual).reshape(1, -1)
-    # model's output include streamflow and evaporation now,
-    # but now we only calibrate the model with streamflow
-    sim, _ = MODEL_DICT[model["name"]](
-        x_input, params, warmup_length=warmup_length, **model
-    )
-    # Calculate RMSE for multi-dim arrays
-    return rmse43darr(y_true[warmup_length:, :, :], sim)
-
-
-def checkBounds(min, max):
-    """
-    A decorator to set bounds for individuals in a population
-
-    Parameters
-    ----------
-    min
-        the lower bound of individuals
-    max
-        the upper bound of individuals
-
-    Returns
-    -------
-    Function
-        a wrapper for clipping data into a given bound
-    """
-
-    def decorator(func):
-        def wrapper(*args, **kargs):
-            offspring = func(*args, **kargs)
-            for child in offspring:
-                for i in range(len(child)):
-                    if child[i] > max:
-                        child[i] = max
-                    elif child[i] < min:
-                        child[i] = min
-            return offspring
-
-        return wrapper
-
-    return decorator
-
-
-MIN = 0
-MAX = 1
-
-
-def calibrate_by_ga(
-    input_data, observed_output, deap_dir, warmup_length=30, model=None, ga_param=None, **kwargs
-):
-    """
-    Use GA algorithm to find optimal parameters for hydrologic models
-
-    Parameters
-    ----------
-    input_data
-        the input data for model
-    observed_output
-        the "true" values, i.e. observations
-    deap_dir
-        the directory to save the results
-    warmup_length
-        the length of warmup period
-    model
-        the model setting
-    ga_param
-        random_seed: 1234
-        run_counts: int = 40, running counts
-        pop_num: int = 50, the number of individuals in the population
-        cross_prob: float = 0.5, the probability with which two individuals are crossed
-        mut_prob: float=0.5, the probability for mutating an individual
-
-    Returns
-    -------
-    toolbox.population
-        optimal_params
-    """
-    if model is None:
-        model = {
-            "name": "xaj_mz",
-            "source_type": "sources",
-            "source_book": "HF",
-        }
-    if ga_param is None:
-        ga_param = {
-            "random_seed": 1234,
-            "run_counts": 5,
-            "pop_num": 50,
-            "cross_prob": 0.5,
-            "mut_prob": 0.5,
-            "save_freq": 1,
-        }
-    pr_file = kwargs.get("param_range_file", None)
-    model_param_dict = read_model_param_dict(pr_file)
-    np.random.seed(ga_param["random_seed"])
-    param_num = len(model_param_dict[model["name"]]["param_name"])
-    creator.create("FitnessMin", base.Fitness, weights=(-1.0,))
-    creator.create("Individual", list, fitness=creator.FitnessMin)
-    toolbox = base.Toolbox()
-    toolbox.register("attribute", random.random)
-    toolbox.register(
-        "individual",
-        tools.initRepeat,
-        creator.Individual,
-        toolbox.attribute,
-        n=param_num,
-    )
-    toolbox.register("population", tools.initRepeat, list, toolbox.individual)
-
-    toolbox.register("mate", tools.cxTwoPoint)
-    toolbox.register("mutate", tools.mutGaussian, mu=0, sigma=1, indpb=0.1)
-    toolbox.register("select", tools.selTournament, tournsize=3)
-    toolbox.register(
-        "evaluate",
-        evaluate,
-        x_input=input_data,
-        y_true=observed_output,
-        warmup_length=warmup_length,
-        model=model,
-    )
-
-    toolbox.decorate("mate", checkBounds(MIN, MAX))
-    toolbox.decorate("mutate", checkBounds(MIN, MAX))
-
-    pop = toolbox.population(n=ga_param["pop_num"])
-    # cxpb  is the probability with which two individuals are crossed
-    # mutpb is the probability for mutating an individual
-    cxpb, mutpb = ga_param["cross_prob"], ga_param["mut_prob"]
-
-    # save the best individual
-    halloffame = tools.HallOfFame(maxsize=1)
-    logbook = tools.Logbook()
-    stats = tools.Statistics(lambda ind: ind.fitness.values)
-    stats.register("avg", np.mean)
-    stats.register("min", np.min)
-
-    # Evaluate the entire population for the first time
-    print("Initiliazing population...")
-    fitnesses = map(toolbox.evaluate, pop)
-    for ind, fit in zip(pop, fitnesses):
-        ind.fitness.values = fit
-    halloffame.update(pop)
-    record = stats.compile(pop)
-    logbook.record(gen=0, evals=len(pop), **record)
-    cp = dict(
-        population=pop,
-        generation=0,
-        halloffame=halloffame,
-        logbook=logbook,
-        rndstate=random.getstate(),
-    )
-    if not os.path.exists(deap_dir):
-        os.makedirs(deap_dir)
-    with open(os.path.join(deap_dir, "epoch0.pkl"), "wb") as cp_file:
-        pickle.dump(cp, cp_file)
-
-    for gen in tqdm(range(ga_param["run_counts"]), desc="GA calibrating"):
-        # Select the next generation individuals
-        offspring = toolbox.select(pop, len(pop))
-        # Clone the selected individuals
-        offspring = list(map(toolbox.clone, offspring))
-
-        # Apply crossover and mutation on the offspring
-        for child1, child2 in zip(offspring[::2], offspring[1::2]):
-            if random.random() < cxpb:
-                toolbox.mate(child1, child2)
-                del child1.fitness.values
-                del child2.fitness.values
-
-        for mutant in offspring:
-            if random.random() < mutpb:
-                toolbox.mutate(mutant)
-                del mutant.fitness.values
-
-        # Evaluate the individuals with an invalid fitness
-        invalid_ind = [ind for ind in offspring if not ind.fitness.valid]
-        fitnesses = map(toolbox.evaluate, invalid_ind)
-        for ind, fit in tqdm(
-            zip(invalid_ind, fitnesses),
-            desc=f"{str(gen + 1)} generation fitness calculating",
-        ):
-            ind.fitness.values = fit
-
-        halloffame.update(offspring)
-        record = stats.compile(offspring)
-        # +1 means start from 1, 0 means initial generation
-        logbook.record(gen=gen + 1, evals=len(invalid_ind), **record)
-        # The population is entirely replaced by the offspring
-        pop[:] = offspring
-        print(
-            f"Best individual of {str(gen + 1)}"
-            + f" generation is: {halloffame[0]}, {halloffame[0].fitness.values}"
-        )
-        if gen % ga_param["save_freq"] == 0:
-            # Fill the dictionary using the dict(key=value[, ...]) constructor
-            cp = dict(
-                population=pop,
-                generation=gen + 1,
-                halloffame=halloffame,
-                logbook=logbook,
-                rndstate=random.getstate(),
-            )
-
-            with open(
-                os.path.join(deap_dir, f"epoch{str(gen + 1)}.pkl"), "wb"
-            ) as cp_file:
-                pickle.dump(cp, cp_file)
-    top10 = tools.selBest(pop, k=10)
-    return pop
-
-
-def show_ga_result(
-    deap_dir,
-    warmup_length,
-    basin_id,
-    the_data,
-    the_period,
-    basin_area,
-    model_info,
-    result_unit="mm/day",
-    train_mode=True,
-):
-    """
-    show the result of GA
-    """
-    # https://stackoverflow.com/questions/61065222/python-deap-and-multiprocessing-on-windows-attributeerror
-    creator.create("FitnessMin", base.Fitness, weights=(-1.0,))
-    creator.create("Individual", list, fitness=creator.FitnessMin)
-    with open(os.path.join(deap_dir, "epoch2.pkl"), "rb") as cp_file:
-        cp = pickle.load(cp_file)
-    pop = cp["population"]
-    logbook = cp["logbook"]
-    halloffame = cp["halloffame"]
-    print(f"Best individual is: {halloffame[0]}, {halloffame[0].fitness.values}")
-    train_test_flag = "train" if train_mode else "test"
-    best_simulation, _ = MODEL_DICT[model_info["name"]](
-        the_data[:, :, 0:2],
-        np.array(list(halloffame[0])).reshape(1, -1),
-        warmup_length=warmup_length,
-        **model_info,
-    )
-    convert_unit_sim = units.convert_unit(
-        np.array(best_simulation).reshape(1, -1),
-        result_unit,
-        units.unit["streamflow"],
-        basin_area=basin_area,
-    )
-    convert_unit_obs = units.convert_unit(
-        np.array(the_data[warmup_length:, :, -1:]).reshape(1, -1),
-        result_unit,
-        units.unit["streamflow"],
-        basin_area=basin_area,
-    )
-    # save calibrated results of calibration period
-    the_result_file = os.path.join(
-        deap_dir,
-        f"{train_test_flag}_qsim_" + model_info["name"] + "_" + str(basin_id) + ".csv",
-    )
-    pd.DataFrame(convert_unit_sim.reshape(-1, 1)).to_csv(
-        the_result_file,
-        sep=",",
-        index=False,
-        header=False,
-    )
-    # calculation rmse、nashsutcliffe and bias for training period
-    stat_error = hydro_stat.stat_error(
-        convert_unit_obs,
-        convert_unit_sim,
-    )
-    print(f"{train_test_flag}ing metrics:", basin_id, stat_error)
-    hydro_file.serialize_json_np(
-        stat_error, os.path.join(deap_dir, f"{train_test_flag}_metrics.json")
-    )
-    t_range = pd.to_datetime(the_period[warmup_length:]).values.astype("datetime64[D]")
-    save_fig = os.path.join(deap_dir, f"{train_test_flag}_results.png")
-    if train_mode:
-        save_param_file = os.path.join(deap_dir, basin_id + "_calibrate_params.txt")
-        pd.DataFrame(list(halloffame[0])).to_csv(
-            save_param_file, sep=",", index=False, header=True
-        )
-        fit_mins = logbook.select("min")
-        plot_train_iteration(fit_mins, os.path.join(deap_dir, "train_iteration.png"))
-    plot_sim_and_obs(
-        t_range,
-        convert_unit_sim.flatten(),
-        convert_unit_obs.flatten(),
-        save_fig,
-    )
-
-
-if __name__ == "__main__":
-    data_dir = os.path.join(
-        definitions.ROOT_DIR,
-        "hydromodel",
-        "example",
-        "exp004",
-    )
-    deap_dir = os.path.join(
-        data_dir,
-        "Dec25_16-33-56_LAPTOP-DNQOPPMS_fold0_HFsources",
-        "60668",
-    )
-    train_data_info_file = os.path.join(data_dir, "data_info_fold0_train.json")
-    train_data_file = os.path.join(data_dir, "basins_lump_p_pe_q_fold0_train.npy")
-    data_train = hydro_file.unserialize_numpy(train_data_file)
-    data_info_train = hydro_file.unserialize_json_ordered(train_data_info_file)
-    model_info = {
-        "name": "xaj_mz",
-        "source_type": "sources",
-        "source_book": "HF",
-    }
-    train_period = data_info_train["time"]
-    basin_area = data_info_train["area"][0]
-
-    show_ga_result(
-        deap_dir,
-        365,
-        "60668",
-        data_train[:, 0:1, :],
-        train_period,
-        basin_area,
-        model_info,
-        result_unit="mm/day",
-    )
+"""
+Author: Wenyu Ouyang
+Date: 2021-12-10 23:01:02
+LastEditTime: 2024-03-27 15:11:04
+LastEditors: Wenyu Ouyang
+Description: Calibrate XAJ model using DEAP
+FilePath: \hydro-model-xaj\hydromodel\trainers\calibrate_ga.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import pickle
+from deap import base, creator
+import random
+from deap import tools
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+
+from hydroutils import hydro_file, hydro_stat
+
+
+from datasets.data_visualize import plot_sim_and_obs, plot_train_iteration
+from hydromodel.models.model_config import read_model_param_dict
+from hydromodel.models.model_dict import MODEL_DICT, rmse43darr
+
+
+def evaluate(individual, x_input, y_true, warmup_length, model):
+    """
+    Calculate fitness for optimization
+
+    Parameters
+    ----------
+    individual
+        individual is the params of XAJ (see details in xaj.py); we initialize all parameters in range [0,1]
+    x_input
+        input of XAJ
+    y_true
+        observation data; we use the part after warmup period
+    warmup_length
+        the length of warmup period
+    model
+        model's config
+
+    Returns
+    -------
+    float
+        fitness
+    """
+    # print("Calculate fitness:")
+    # NOTE: Now only support one basin's calibration for once now
+    params = np.array(individual).reshape(1, -1)
+    # model's output include streamflow and evaporation now,
+    # but now we only calibrate the model with streamflow
+    sim, _ = MODEL_DICT[model["name"]](
+        x_input, params, warmup_length=warmup_length, **model
+    )
+    # Calculate RMSE for multi-dim arrays
+    return rmse43darr(y_true[warmup_length:, :, :], sim)
+
+
+def checkBounds(min, max):
+    """
+    A decorator to set bounds for individuals in a population
+
+    Parameters
+    ----------
+    min
+        the lower bound of individuals
+    max
+        the upper bound of individuals
+
+    Returns
+    -------
+    Function
+        a wrapper for clipping data into a given bound
+    """
+
+    def decorator(func):
+        def wrapper(*args, **kargs):
+            offspring = func(*args, **kargs)
+            for child in offspring:
+                for i in range(len(child)):
+                    if child[i] > max:
+                        child[i] = max
+                    elif child[i] < min:
+                        child[i] = min
+            return offspring
+
+        return wrapper
+
+    return decorator
+
+
+MIN = 0
+MAX = 1
+
+
+def calibrate_by_ga(
+    input_data, observed_output, deap_dir, warmup_length=30, model=None, ga_param=None, **kwargs
+):
+    """
+    Use GA algorithm to find optimal parameters for hydrologic models
+
+    Parameters
+    ----------
+    input_data
+        the input data for model
+    observed_output
+        the "true" values, i.e. observations
+    deap_dir
+        the directory to save the results
+    warmup_length
+        the length of warmup period
+    model
+        the model setting
+    ga_param
+        random_seed: 1234
+        run_counts: int = 40, running counts
+        pop_num: int = 50, the number of individuals in the population
+        cross_prob: float = 0.5, the probability with which two individuals are crossed
+        mut_prob: float=0.5, the probability for mutating an individual
+
+    Returns
+    -------
+    toolbox.population
+        optimal_params
+    """
+    if model is None:
+        model = {
+            "name": "xaj_mz",
+            "source_type": "sources",
+            "source_book": "HF",
+        }
+    if ga_param is None:
+        ga_param = {
+            "random_seed": 1234,
+            "run_counts": 5,
+            "pop_num": 50,
+            "cross_prob": 0.5,
+            "mut_prob": 0.5,
+            "save_freq": 1,
+        }
+    pr_file = kwargs.get("param_range_file", None)
+    model_param_dict = read_model_param_dict(pr_file)
+    np.random.seed(ga_param["random_seed"])
+    param_num = len(model_param_dict[model["name"]]["param_name"])
+    creator.create("FitnessMin", base.Fitness, weights=(-1.0,))
+    creator.create("Individual", list, fitness=creator.FitnessMin)
+    toolbox = base.Toolbox()
+    toolbox.register("attribute", random.random)
+    toolbox.register(
+        "individual",
+        tools.initRepeat,
+        creator.Individual,
+        toolbox.attribute,
+        n=param_num,
+    )
+    toolbox.register("population", tools.initRepeat, list, toolbox.individual)
+
+    toolbox.register("mate", tools.cxTwoPoint)
+    toolbox.register("mutate", tools.mutGaussian, mu=0, sigma=1, indpb=0.1)
+    toolbox.register("select", tools.selTournament, tournsize=3)
+    toolbox.register(
+        "evaluate",
+        evaluate,
+        x_input=input_data,
+        y_true=observed_output,
+        warmup_length=warmup_length,
+        model=model,
+    )
+
+    toolbox.decorate("mate", checkBounds(MIN, MAX))
+    toolbox.decorate("mutate", checkBounds(MIN, MAX))
+
+    pop = toolbox.population(n=ga_param["pop_num"])
+    # cxpb  is the probability with which two individuals are crossed
+    # mutpb is the probability for mutating an individual
+    cxpb, mutpb = ga_param["cross_prob"], ga_param["mut_prob"]
+
+    # save the best individual
+    halloffame = tools.HallOfFame(maxsize=1)
+    logbook = tools.Logbook()
+    stats = tools.Statistics(lambda ind: ind.fitness.values)
+    stats.register("avg", np.mean)
+    stats.register("min", np.min)
+
+    # Evaluate the entire population for the first time
+    print("Initiliazing population...")
+    fitnesses = map(toolbox.evaluate, pop)
+    for ind, fit in zip(pop, fitnesses):
+        ind.fitness.values = fit
+    halloffame.update(pop)
+    record = stats.compile(pop)
+    logbook.record(gen=0, evals=len(pop), **record)
+    cp = dict(
+        population=pop,
+        generation=0,
+        halloffame=halloffame,
+        logbook=logbook,
+        rndstate=random.getstate(),
+    )
+    if not os.path.exists(deap_dir):
+        os.makedirs(deap_dir)
+    with open(os.path.join(deap_dir, "epoch0.pkl"), "wb") as cp_file:
+        pickle.dump(cp, cp_file)
+
+    for gen in tqdm(range(ga_param["run_counts"]), desc="GA calibrating"):
+        # Select the next generation individuals
+        offspring = toolbox.select(pop, len(pop))
+        # Clone the selected individuals
+        offspring = list(map(toolbox.clone, offspring))
+
+        # Apply crossover and mutation on the offspring
+        for child1, child2 in zip(offspring[::2], offspring[1::2]):
+            if random.random() < cxpb:
+                toolbox.mate(child1, child2)
+                del child1.fitness.values
+                del child2.fitness.values
+
+        for mutant in offspring:
+            if random.random() < mutpb:
+                toolbox.mutate(mutant)
+                del mutant.fitness.values
+
+        # Evaluate the individuals with an invalid fitness
+        invalid_ind = [ind for ind in offspring if not ind.fitness.valid]
+        fitnesses = map(toolbox.evaluate, invalid_ind)
+        for ind, fit in tqdm(
+            zip(invalid_ind, fitnesses),
+            desc=f"{str(gen + 1)} generation fitness calculating",
+        ):
+            ind.fitness.values = fit
+
+        halloffame.update(offspring)
+        record = stats.compile(offspring)
+        # +1 means start from 1, 0 means initial generation
+        logbook.record(gen=gen + 1, evals=len(invalid_ind), **record)
+        # The population is entirely replaced by the offspring
+        pop[:] = offspring
+        print(
+            f"Best individual of {str(gen + 1)}"
+            + f" generation is: {halloffame[0]}, {halloffame[0].fitness.values}"
+        )
+        if gen % ga_param["save_freq"] == 0:
+            # Fill the dictionary using the dict(key=value[, ...]) constructor
+            cp = dict(
+                population=pop,
+                generation=gen + 1,
+                halloffame=halloffame,
+                logbook=logbook,
+                rndstate=random.getstate(),
+            )
+
+            with open(
+                os.path.join(deap_dir, f"epoch{str(gen + 1)}.pkl"), "wb"
+            ) as cp_file:
+                pickle.dump(cp, cp_file)
+    top10 = tools.selBest(pop, k=10)
+    return pop
+
+
+def show_ga_result(
+    deap_dir,
+    warmup_length,
+    basin_id,
+    the_data,
+    the_period,
+    basin_area,
+    model_info,
+    result_unit="mm/day",
+    train_mode=True,
+):
+    """
+    show the result of GA
+    """
+    # https://stackoverflow.com/questions/61065222/python-deap-and-multiprocessing-on-windows-attributeerror
+    creator.create("FitnessMin", base.Fitness, weights=(-1.0,))
+    creator.create("Individual", list, fitness=creator.FitnessMin)
+    with open(os.path.join(deap_dir, "epoch2.pkl"), "rb") as cp_file:
+        cp = pickle.load(cp_file)
+    pop = cp["population"]
+    logbook = cp["logbook"]
+    halloffame = cp["halloffame"]
+    print(f"Best individual is: {halloffame[0]}, {halloffame[0].fitness.values}")
+    train_test_flag = "train" if train_mode else "test"
+    best_simulation, _ = MODEL_DICT[model_info["name"]](
+        the_data[:, :, 0:2],
+        np.array(list(halloffame[0])).reshape(1, -1),
+        warmup_length=warmup_length,
+        **model_info,
+    )
+    convert_unit_sim = units.convert_unit(
+        np.array(best_simulation).reshape(1, -1),
+        result_unit,
+        units.unit["streamflow"],
+        basin_area=basin_area,
+    )
+    convert_unit_obs = units.convert_unit(
+        np.array(the_data[warmup_length:, :, -1:]).reshape(1, -1),
+        result_unit,
+        units.unit["streamflow"],
+        basin_area=basin_area,
+    )
+    # save calibrated results of calibration period
+    the_result_file = os.path.join(
+        deap_dir,
+        f"{train_test_flag}_qsim_" + model_info["name"] + "_" + str(basin_id) + ".csv",
+    )
+    pd.DataFrame(convert_unit_sim.reshape(-1, 1)).to_csv(
+        the_result_file,
+        sep=",",
+        index=False,
+        header=False,
+    )
+    # calculation rmse、nashsutcliffe and bias for training period
+    stat_error = hydro_stat.stat_error(
+        convert_unit_obs,
+        convert_unit_sim,
+    )
+    print(f"{train_test_flag}ing metrics:", basin_id, stat_error)
+    hydro_file.serialize_json_np(
+        stat_error, os.path.join(deap_dir, f"{train_test_flag}_metrics.json")
+    )
+    t_range = pd.to_datetime(the_period[warmup_length:]).values.astype("datetime64[D]")
+    save_fig = os.path.join(deap_dir, f"{train_test_flag}_results.png")
+    if train_mode:
+        save_param_file = os.path.join(deap_dir, basin_id + "_calibrate_params.txt")
+        pd.DataFrame(list(halloffame[0])).to_csv(
+            save_param_file, sep=",", index=False, header=True
+        )
+        fit_mins = logbook.select("min")
+        plot_train_iteration(fit_mins, os.path.join(deap_dir, "train_iteration.png"))
+    plot_sim_and_obs(
+        t_range,
+        convert_unit_sim.flatten(),
+        convert_unit_obs.flatten(),
+        save_fig,
+    )
+
+
+if __name__ == "__main__":
+    data_dir = os.path.join(
+        definitions.ROOT_DIR,
+        "hydromodel",
+        "example",
+        "exp004",
+    )
+    deap_dir = os.path.join(
+        data_dir,
+        "Dec25_16-33-56_LAPTOP-DNQOPPMS_fold0_HFsources",
+        "60668",
+    )
+    train_data_info_file = os.path.join(data_dir, "data_info_fold0_train.json")
+    train_data_file = os.path.join(data_dir, "basins_lump_p_pe_q_fold0_train.npy")
+    data_train = hydro_file.unserialize_numpy(train_data_file)
+    data_info_train = hydro_file.unserialize_json_ordered(train_data_info_file)
+    model_info = {
+        "name": "xaj_mz",
+        "source_type": "sources",
+        "source_book": "HF",
+    }
+    train_period = data_info_train["time"]
+    basin_area = data_info_train["area"][0]
+
+    show_ga_result(
+        deap_dir,
+        365,
+        "60668",
+        data_train[:, 0:1, :],
+        train_period,
+        basin_area,
+        model_info,
+        result_unit="mm/day",
+    )
```

### Comparing `hydromodel-0.2.2/hydromodel/trainers/evaluate.py` & `hydromodel-0.2.3/hydromodel/trainers/evaluate.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-"""
-Author: Wenyu Ouyang
-Date: 2022-10-25 21:16:22
-LastEditTime: 2024-03-28 09:55:58
-LastEditors: Wenyu Ouyang
-Description: Plots for calibration and testing results
-FilePath: \hydromodel\hydromodel\trainers\evaluate.py
-Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
-"""
-
-import pathlib
-import pandas as pd
-import os
-import numpy as np
-import xarray as xr
-import spotpy
-import yaml
-
-from hydroutils import hydro_file, hydro_stat
-from hydrodatasource.utils.utils import streamflow_unit_conv
-
-from hydromodel.datasets import *
-from hydromodel.datasets.data_preprocess import (
-    get_basin_area,
-    _get_pe_q_from_ts,
-)
-from hydromodel.models.model_config import read_model_param_dict
-from hydromodel.models.model_dict import MODEL_DICT
-
-
-class Evaluator:
-    def __init__(self, cali_dir, param_dir=None, eval_dir=None):
-        """_summary_
-
-        Parameters
-        ----------
-        cali_dir : _type_
-            calibration directory
-        param_dir : str
-            parameters directory
-        eval_dir : _type_
-            evaluation directory
-        """
-        if param_dir is None:
-            param_dir = cali_dir
-        if eval_dir is None:
-            eval_dir = cali_dir
-        cali_config = read_yaml_config(os.path.join(cali_dir, "config.yaml"))
-        self.config = cali_config
-        self.data_type = cali_config["data_type"]
-        self.data_dir = cali_config["data_dir"]
-        self.model_info = cali_config["model"]
-        self.save_dir = eval_dir
-        self.params_dir = param_dir
-        self.param_range_file = cali_config["param_range_file"]
-        if not os.path.exists(param_dir):
-            os.makedirs(param_dir)
-        if not os.path.exists(eval_dir):
-            os.makedirs(eval_dir)
-
-    def predict(self, ds):
-        """predict the streamflow of all basins in ds
-
-        Parameters
-        ----------
-        ds : xr.Dataset
-            the input dataset
-
-        Returns
-        -------
-        tuple
-            qsim, qobs
-        """
-        model_info = self.model_info
-        p_and_e, _ = _get_pe_q_from_ts(ds)
-        basins = ds["basin"].data.astype(str)
-        params = _read_all_basin_params(basins, self.params_dir)
-        qsim, _ = MODEL_DICT[model_info["name"]](
-            p_and_e,
-            params,
-            # we set the warmup_length=0 but later we get results from warmup_length to the end to evaluate
-            warmup_length=0,
-            **model_info,
-            **{"param_range_file": self.param_range_file},
-        )
-        qsim, qobs = self._convert_streamflow_units(ds, qsim)
-        return qsim, qobs
-
-    def save_results(self, ds, qsim, qobs):
-        """save the evaluation results
-
-        Parameters
-        ----------
-        ds : _type_
-            input dataset
-        qsim : _type_
-            _description_
-        qobs : _type_
-            _description_
-        """
-        basins = ds["basin"].data.astype(str)
-        self._summarize_parameters(basins)
-        self._renormalize_params(basins)
-        self._save_evaluate_results(qsim, qobs, ds)
-        self._summarize_metrics(basins)
-
-    def _convert_streamflow_units(self, test_data, qsim):
-        data_type = self.data_type
-        data_dir = self.data_dir
-        times = test_data["time"].data
-        basins = test_data["basin"].data
-        flow_name = remove_unit_from_name(FLOW_NAME)
-        flow_dataarray = xr.DataArray(
-            qsim.squeeze(-1),
-            coords=[("time", times), ("basin", basins)],
-            name=flow_name,
-        )
-        flow_dataarray.attrs["units"] = test_data[flow_name].attrs["units"]
-        ds = xr.Dataset()
-        ds[flow_name] = flow_dataarray
-        target_unit = "m^3/s"
-        basin_area = get_basin_area(data_type, data_dir, basins)
-        ds_simflow = streamflow_unit_conv(
-            ds, basin_area, target_unit=target_unit, inverse=True
-        )
-        ds_obsflow = streamflow_unit_conv(
-            test_data[[flow_name]], basin_area, target_unit=target_unit, inverse=True
-        )
-        return ds_simflow, ds_obsflow
-
-    def _summarize_parameters(self, basin_ids):
-        """
-        output parameters of all basins to one file
-
-        Parameters
-        ----------
-        param_dir
-            the directory where we save params
-        model_name
-            the name of the model
-
-        Returns
-        -------
-
-        """
-        param_dir = self.params_dir
-        model_name = self.model_info["name"]
-        params = []
-        model_param_dict = read_model_param_dict(self.param_range_file)
-        for basin_id in basin_ids:
-            columns = model_param_dict[model_name]["param_name"]
-            params_txt = pd.read_csv(
-                os.path.join(param_dir, basin_id + "_calibrate_params.txt")
-            )
-            params_df = pd.DataFrame(params_txt.values.T, columns=columns)
-            params.append(params_df)
-        params_dfs = pd.concat(params, axis=0)
-        params_dfs.index = basin_ids
-        print(params_dfs)
-        params_csv_file = os.path.join(param_dir, "basins_norm_params.csv")
-        params_dfs.to_csv(params_csv_file, sep=",", index=True, header=True)
-
-    def _renormalize_params(self, basin_ids):
-        param_dir = self.params_dir
-        model_name = self.model_info["name"]
-        renormalization_params = []
-        model_param_dict = read_model_param_dict(self.param_range_file)
-        for basin_id in basin_ids:
-            params = np.loadtxt(
-                os.path.join(param_dir, basin_id + "_calibrate_params.txt")
-            )[1:].reshape(1, -1)
-            param_ranges = model_param_dict[model_name]["param_range"]
-            xaj_params = [
-                (value[1] - value[0]) * params[:, i] + value[0]
-                for i, (key, value) in enumerate(param_ranges.items())
-            ]
-            xaj_params_ = np.array([x for j in xaj_params for x in j])
-            params_df = pd.DataFrame(xaj_params_.T)
-            renormalization_params.append(params_df)
-        renormalization_params_dfs = pd.concat(renormalization_params, axis=1)
-        renormalization_params_dfs.index = model_param_dict[model_name]["param_name"]
-        renormalization_params_dfs.columns = basin_ids
-        print(renormalization_params_dfs)
-        params_csv_file = os.path.join(param_dir, "basins_denorm_params.csv")
-        renormalization_params_dfs.transpose().to_csv(
-            params_csv_file, sep=",", index=True, header=True
-        )
-
-    def _summarize_metrics(self, basin_ids):
-        """
-        output all results' metrics of basins to one file
-
-        Parameters
-        ----------
-        basin_ids
-            the ids of basins
-
-        Returns
-        -------
-
-        """
-        result_dir = self.save_dir
-        model_name = self.model_info["name"]
-        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
-        ds = xr.open_dataset(file_path)
-        # for metrics, warmup_length should be considered
-        warmup_length = self.config["warmup"]
-        qobs = ds["qobs"].transpose("basin", "time").to_numpy()[:, warmup_length:]
-        qsim = ds["qsim"].transpose("basin", "time").to_numpy()[:, warmup_length:]
-        test_metrics = hydro_stat.stat_error(
-            qobs,
-            qsim,
-        )
-        metric_dfs_test = pd.DataFrame(test_metrics, index=basin_ids)
-        metric_file_test = os.path.join(result_dir, "basins_metrics.csv")
-        metric_dfs_test.to_csv(metric_file_test, sep=",", index=True, header=True)
-
-    def _save_evaluate_results(self, qsim, qobs, obs_ds):
-        result_dir = self.save_dir
-        model_name = self.model_info["name"]
-        ds = xr.Dataset()
-
-        # 添加 qsim 和 qobs
-        ds["qsim"] = qsim["flow"]
-        ds["qobs"] = qobs["flow"]
-
-        # 添加 prcp 和 pet
-        ds["prcp"] = obs_ds["prcp"]
-        ds["pet"] = obs_ds["pet"]
-
-        # 保存为 .nc 文件
-        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
-        ds.to_netcdf(file_path)
-
-        print(f"Results saved to: {file_path}")
-
-    def load_results(self):
-        result_dir = self.save_dir
-        model_name = self.model_info["name"]
-        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
-        return xr.open_dataset(file_path)
-
-
-def _read_save_sceua_calibrated_params(basin_id, save_dir, sceua_calibrated_file_name):
-    """
-    read the parameters' file generated by spotpy SCE-UA when finishing calibration
-
-    We also save the parameters of the best model run to a file
-
-    Parameters
-    ----------
-    basin_id
-        id of a basin
-    save_dir
-        the directory where we save params
-    sceua_calibrated_file_name
-        the parameters' file generated by spotpy SCE-UA when finishing calibration
-
-    Returns
-    -------
-
-    """
-    results = spotpy.analyser.load_csv_results(sceua_calibrated_file_name)
-    bestindex, bestobjf = spotpy.analyser.get_minlikeindex(
-        results
-    )  # 结果数组中具有最小目标函数的位置的索引
-    best_model_run = results[bestindex]
-    fields = [word for word in best_model_run.dtype.names if word.startswith("par")]
-    best_calibrate_params = pd.DataFrame(list(best_model_run[fields]))
-    save_file = os.path.join(save_dir, basin_id + "_calibrate_params.txt")
-    best_calibrate_params.to_csv(save_file, sep=",", index=False, header=True)
-    return np.array(best_calibrate_params).reshape(1, -1)  # 返回一列最佳的结果
-
-
-def _read_all_basin_params(basins, param_dir):
-    params_list = []
-    for basin_id in basins:
-        db_name = os.path.join(param_dir, basin_id)
-        # 读取每个流域的参数
-        basin_params = _read_save_sceua_calibrated_params(basin_id, param_dir, db_name)
-        # 确保basin_params是一维的
-        basin_params = basin_params.flatten()
-        params_list.append(basin_params)
-    return np.vstack(params_list)
-
-
-def read_and_save_et_ouputs(result_dir, fold: int):
-    # TODO: not finished yet after we refactor the code
-    prameter_file = os.path.join(result_dir, "basins_params.csv")
-    param_values = pd.read_csv(prameter_file, index_col=0)
-    basins_id = param_values.columns.values
-    args_file = os.path.join(result_dir, "args.json")
-    args = hydro_file.unserialize_json(args_file)
-    warmup_length = args["warmup_length"]
-    model_func_param = args["model"]
-    exp_dir = pathlib.Path(result_dir).parent
-    data_info_train = hydro_file.unserialize_json(
-        exp_dir.joinpath(f"data_info_fold{fold}_train.json")
-    )
-    data_info_test = hydro_file.unserialize_json(
-        exp_dir.joinpath(f"data_info_fold{fold}_test.json")
-    )
-    train_period = data_info_train["time"]
-    test_period = data_info_test["time"]
-    # TODO: basins_lump_p_pe_q_fold NAME need to be unified
-    train_np_file = os.path.join(exp_dir, f"data_info_fold{fold}_train.npy")
-    test_np_file = os.path.join(exp_dir, f"data_info_fold{fold}_test.npy")
-    # train_np_file = os.path.join(exp_dir, f"basins_lump_p_pe_q_fold{fold}_train.npy")
-    # test_np_file = os.path.join(exp_dir, f"basins_lump_p_pe_q_fold{fold}_test.npy")
-    train_data = np.load(train_np_file)
-    test_data = np.load(test_np_file)
-    es_test = []
-    es_train = []
-    for i in range(len(basins_id)):
-        _, e_train = xaj(
-            train_data[:, :, 0:2],
-            param_values[basins_id[i]].values.reshape(1, -1),
-            warmup_length=warmup_length,
-            **model_func_param,
-        )
-        _, e_test = xaj(
-            test_data[:, :, 0:2],
-            param_values[basins_id[i]].values.reshape(1, -1),
-            warmup_length=warmup_length,
-            **model_func_param,
-        )
-        es_train.append(e_train.flatten())
-        es_test.append(e_test.flatten())
-    df_e_train = pd.DataFrame(
-        np.array(es_train).T, columns=basins_id, index=train_period[warmup_length:]
-    )
-    df_e_test = pd.DataFrame(
-        np.array(es_test).T, columns=basins_id, index=test_period[warmup_length:]
-    )
-    etsim_train_save_path = os.path.join(result_dir, "basin_etsim_train.csv")
-    etsim_test_save_path = os.path.join(result_dir, "basin_etsim_test.csv")
-    df_e_train.to_csv(etsim_train_save_path)
-    df_e_test.to_csv(etsim_test_save_path)
-
-
-def read_yaml_config(file_path):
-    with open(file_path, "r") as file:
-        config = yaml.safe_load(file)
-    return config
+"""
+Author: Wenyu Ouyang
+Date: 2022-10-25 21:16:22
+LastEditTime: 2024-03-28 09:55:58
+LastEditors: Wenyu Ouyang
+Description: Plots for calibration and testing results
+FilePath: \hydromodel\hydromodel\trainers\evaluate.py
+Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
+"""
+
+import pathlib
+import pandas as pd
+import os
+import numpy as np
+import xarray as xr
+import spotpy
+import yaml
+
+from hydroutils import hydro_file, hydro_stat
+from hydrodatasource.utils.utils import streamflow_unit_conv
+
+from hydromodel.datasets import *
+from hydromodel.datasets.data_preprocess import (
+    get_basin_area,
+    _get_pe_q_from_ts,
+)
+from hydromodel.models.model_config import read_model_param_dict
+from hydromodel.models.model_dict import MODEL_DICT
+
+
+class Evaluator:
+    def __init__(self, cali_dir, param_dir=None, eval_dir=None):
+        """_summary_
+
+        Parameters
+        ----------
+        cali_dir : _type_
+            calibration directory
+        param_dir : str
+            parameters directory
+        eval_dir : _type_
+            evaluation directory
+        """
+        if param_dir is None:
+            param_dir = cali_dir
+        if eval_dir is None:
+            eval_dir = cali_dir
+        cali_config = read_yaml_config(os.path.join(cali_dir, "config.yaml"))
+        self.config = cali_config
+        self.data_type = cali_config["data_type"]
+        self.data_dir = cali_config["data_dir"]
+        self.model_info = cali_config["model"]
+        self.save_dir = eval_dir
+        self.params_dir = param_dir
+        self.param_range_file = cali_config["param_range_file"]
+        if not os.path.exists(param_dir):
+            os.makedirs(param_dir)
+        if not os.path.exists(eval_dir):
+            os.makedirs(eval_dir)
+
+    def predict(self, ds):
+        """predict the streamflow of all basins in ds
+
+        Parameters
+        ----------
+        ds : xr.Dataset
+            the input dataset
+
+        Returns
+        -------
+        tuple
+            qsim, qobs
+        """
+        model_info = self.model_info
+        p_and_e, _ = _get_pe_q_from_ts(ds)
+        basins = ds["basin"].data.astype(str)
+        params = _read_all_basin_params(basins, self.params_dir)
+        qsim, _ = MODEL_DICT[model_info["name"]](
+            p_and_e,
+            params,
+            # we set the warmup_length=0 but later we get results from warmup_length to the end to evaluate
+            warmup_length=0,
+            **model_info,
+            **{"param_range_file": self.param_range_file},
+        )
+        qsim, qobs = self._convert_streamflow_units(ds, qsim)
+        return qsim, qobs
+
+    def save_results(self, ds, qsim, qobs):
+        """save the evaluation results
+
+        Parameters
+        ----------
+        ds : _type_
+            input dataset
+        qsim : _type_
+            _description_
+        qobs : _type_
+            _description_
+        """
+        basins = ds["basin"].data.astype(str)
+        self._summarize_parameters(basins)
+        self._renormalize_params(basins)
+        self._save_evaluate_results(qsim, qobs, ds)
+        self._summarize_metrics(basins)
+
+    def _convert_streamflow_units(self, test_data, qsim):
+        data_type = self.data_type
+        data_dir = self.data_dir
+        times = test_data["time"].data
+        basins = test_data["basin"].data
+        flow_name = remove_unit_from_name(FLOW_NAME)
+        flow_dataarray = xr.DataArray(
+            qsim.squeeze(-1),
+            coords=[("time", times), ("basin", basins)],
+            name=flow_name,
+        )
+        flow_dataarray.attrs["units"] = test_data[flow_name].attrs["units"]
+        ds = xr.Dataset()
+        ds[flow_name] = flow_dataarray
+        target_unit = "m^3/s"
+        basin_area = get_basin_area(data_type, data_dir, basins)
+        ds_simflow = streamflow_unit_conv(
+            ds, basin_area, target_unit=target_unit, inverse=True
+        )
+        ds_obsflow = streamflow_unit_conv(
+            test_data[[flow_name]], basin_area, target_unit=target_unit, inverse=True
+        )
+        return ds_simflow, ds_obsflow
+
+    def _summarize_parameters(self, basin_ids):
+        """
+        output parameters of all basins to one file
+
+        Parameters
+        ----------
+        param_dir
+            the directory where we save params
+        model_name
+            the name of the model
+
+        Returns
+        -------
+
+        """
+        param_dir = self.params_dir
+        model_name = self.model_info["name"]
+        params = []
+        model_param_dict = read_model_param_dict(self.param_range_file)
+        for basin_id in basin_ids:
+            columns = model_param_dict[model_name]["param_name"]
+            params_txt = pd.read_csv(
+                os.path.join(param_dir, basin_id + "_calibrate_params.txt")
+            )
+            params_df = pd.DataFrame(params_txt.values.T, columns=columns)
+            params.append(params_df)
+        params_dfs = pd.concat(params, axis=0)
+        params_dfs.index = basin_ids
+        print(params_dfs)
+        params_csv_file = os.path.join(param_dir, "basins_norm_params.csv")
+        params_dfs.to_csv(params_csv_file, sep=",", index=True, header=True)
+
+    def _renormalize_params(self, basin_ids):
+        param_dir = self.params_dir
+        model_name = self.model_info["name"]
+        renormalization_params = []
+        model_param_dict = read_model_param_dict(self.param_range_file)
+        for basin_id in basin_ids:
+            params = np.loadtxt(
+                os.path.join(param_dir, basin_id + "_calibrate_params.txt")
+            )[1:].reshape(1, -1)
+            param_ranges = model_param_dict[model_name]["param_range"]
+            xaj_params = [
+                (value[1] - value[0]) * params[:, i] + value[0]
+                for i, (key, value) in enumerate(param_ranges.items())
+            ]
+            xaj_params_ = np.array([x for j in xaj_params for x in j])
+            params_df = pd.DataFrame(xaj_params_.T)
+            renormalization_params.append(params_df)
+        renormalization_params_dfs = pd.concat(renormalization_params, axis=1)
+        renormalization_params_dfs.index = model_param_dict[model_name]["param_name"]
+        renormalization_params_dfs.columns = basin_ids
+        print(renormalization_params_dfs)
+        params_csv_file = os.path.join(param_dir, "basins_denorm_params.csv")
+        renormalization_params_dfs.transpose().to_csv(
+            params_csv_file, sep=",", index=True, header=True
+        )
+
+    def _summarize_metrics(self, basin_ids):
+        """
+        output all results' metrics of basins to one file
+
+        Parameters
+        ----------
+        basin_ids
+            the ids of basins
+
+        Returns
+        -------
+
+        """
+        result_dir = self.save_dir
+        model_name = self.model_info["name"]
+        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
+        ds = xr.open_dataset(file_path)
+        # for metrics, warmup_length should be considered
+        warmup_length = self.config["warmup"]
+        qobs = ds["qobs"].transpose("basin", "time").to_numpy()[:, warmup_length:]
+        qsim = ds["qsim"].transpose("basin", "time").to_numpy()[:, warmup_length:]
+        test_metrics = hydro_stat.stat_error(
+            qobs,
+            qsim,
+        )
+        metric_dfs_test = pd.DataFrame(test_metrics, index=basin_ids)
+        metric_file_test = os.path.join(result_dir, "basins_metrics.csv")
+        metric_dfs_test.to_csv(metric_file_test, sep=",", index=True, header=True)
+
+    def _save_evaluate_results(self, qsim, qobs, obs_ds):
+        result_dir = self.save_dir
+        model_name = self.model_info["name"]
+        ds = xr.Dataset()
+
+        # 添加 qsim 和 qobs
+        ds["qsim"] = qsim["flow"]
+        ds["qobs"] = qobs["flow"]
+
+        # 添加 prcp 和 pet
+        ds["prcp"] = obs_ds["prcp"]
+        ds["pet"] = obs_ds["pet"]
+
+        # 保存为 .nc 文件
+        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
+        ds.to_netcdf(file_path)
+
+        print(f"Results saved to: {file_path}")
+
+    def load_results(self):
+        result_dir = self.save_dir
+        model_name = self.model_info["name"]
+        file_path = os.path.join(result_dir, f"{model_name}_evaluation_results.nc")
+        return xr.open_dataset(file_path)
+
+
+def _read_save_sceua_calibrated_params(basin_id, save_dir, sceua_calibrated_file_name):
+    """
+    read the parameters' file generated by spotpy SCE-UA when finishing calibration
+
+    We also save the parameters of the best model run to a file
+
+    Parameters
+    ----------
+    basin_id
+        id of a basin
+    save_dir
+        the directory where we save params
+    sceua_calibrated_file_name
+        the parameters' file generated by spotpy SCE-UA when finishing calibration
+
+    Returns
+    -------
+
+    """
+    results = spotpy.analyser.load_csv_results(sceua_calibrated_file_name)
+    bestindex, bestobjf = spotpy.analyser.get_minlikeindex(
+        results
+    )  # 结果数组中具有最小目标函数的位置的索引
+    best_model_run = results[bestindex]
+    fields = [word for word in best_model_run.dtype.names if word.startswith("par")]
+    best_calibrate_params = pd.DataFrame(list(best_model_run[fields]))
+    save_file = os.path.join(save_dir, basin_id + "_calibrate_params.txt")
+    best_calibrate_params.to_csv(save_file, sep=",", index=False, header=True)
+    return np.array(best_calibrate_params).reshape(1, -1)  # 返回一列最佳的结果
+
+
+def _read_all_basin_params(basins, param_dir):
+    params_list = []
+    for basin_id in basins:
+        db_name = os.path.join(param_dir, basin_id)
+        # 读取每个流域的参数
+        basin_params = _read_save_sceua_calibrated_params(basin_id, param_dir, db_name)
+        # 确保basin_params是一维的
+        basin_params = basin_params.flatten()
+        params_list.append(basin_params)
+    return np.vstack(params_list)
+
+
+def read_and_save_et_ouputs(result_dir, fold: int):
+    # TODO: not finished yet after we refactor the code
+    prameter_file = os.path.join(result_dir, "basins_params.csv")
+    param_values = pd.read_csv(prameter_file, index_col=0)
+    basins_id = param_values.columns.values
+    args_file = os.path.join(result_dir, "args.json")
+    args = hydro_file.unserialize_json(args_file)
+    warmup_length = args["warmup_length"]
+    model_func_param = args["model"]
+    exp_dir = pathlib.Path(result_dir).parent
+    data_info_train = hydro_file.unserialize_json(
+        exp_dir.joinpath(f"data_info_fold{fold}_train.json")
+    )
+    data_info_test = hydro_file.unserialize_json(
+        exp_dir.joinpath(f"data_info_fold{fold}_test.json")
+    )
+    train_period = data_info_train["time"]
+    test_period = data_info_test["time"]
+    # TODO: basins_lump_p_pe_q_fold NAME need to be unified
+    train_np_file = os.path.join(exp_dir, f"data_info_fold{fold}_train.npy")
+    test_np_file = os.path.join(exp_dir, f"data_info_fold{fold}_test.npy")
+    # train_np_file = os.path.join(exp_dir, f"basins_lump_p_pe_q_fold{fold}_train.npy")
+    # test_np_file = os.path.join(exp_dir, f"basins_lump_p_pe_q_fold{fold}_test.npy")
+    train_data = np.load(train_np_file)
+    test_data = np.load(test_np_file)
+    es_test = []
+    es_train = []
+    for i in range(len(basins_id)):
+        _, e_train = xaj(
+            train_data[:, :, 0:2],
+            param_values[basins_id[i]].values.reshape(1, -1),
+            warmup_length=warmup_length,
+            **model_func_param,
+        )
+        _, e_test = xaj(
+            test_data[:, :, 0:2],
+            param_values[basins_id[i]].values.reshape(1, -1),
+            warmup_length=warmup_length,
+            **model_func_param,
+        )
+        es_train.append(e_train.flatten())
+        es_test.append(e_test.flatten())
+    df_e_train = pd.DataFrame(
+        np.array(es_train).T, columns=basins_id, index=train_period[warmup_length:]
+    )
+    df_e_test = pd.DataFrame(
+        np.array(es_test).T, columns=basins_id, index=test_period[warmup_length:]
+    )
+    etsim_train_save_path = os.path.join(result_dir, "basin_etsim_train.csv")
+    etsim_test_save_path = os.path.join(result_dir, "basin_etsim_test.csv")
+    df_e_train.to_csv(etsim_train_save_path)
+    df_e_test.to_csv(etsim_test_save_path)
+
+
+def read_yaml_config(file_path):
+    with open(file_path, "r") as file:
+        config = yaml.safe_load(file)
+    return config
```

### Comparing `hydromodel-0.2.2/hydromodel.egg-info/PKG-INFO` & `hydromodel-0.2.3/hydromodel.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,261 +1,250 @@
-Metadata-Version: 2.1
-Name: hydromodel
-Version: 0.2.2
-Summary: hydrological models starting from XinAnJiang
-Home-page: https://github.com/OuyangWenyu/hydromodel
-Author: Wenyu Ouyang
-Author-email: wenyuouyang@outlook.com
-License: GNU General Public License v3
-Keywords: hydromodel
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: ipykernel
-Requires-Dist: numba
-Requires-Dist: scikit-learn
-Requires-Dist: deap
-Requires-Dist: spotpy
-Requires-Dist: pytest
-Requires-Dist: bmipy
-Requires-Dist: pyyaml
-Requires-Dist: requests
-Requires-Dist: muskingumcunge
-Requires-Dist: hydrodatasource
-
-# hydromodel
-
-[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
-[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
-
-[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
-
--   Free software: GNU General Public License v3
--   Documentation: https://OuyangWenyu.github.io/hydromodel
-
-## What is hydromodel
-
-**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
-
-**Not an official version, just for learning**
-
-This is a Python console program (no graphic interface now). It is **still developing**.
-
-## How to run
-
-### Install
-
-We provided a pip package. You can install it with pip:
-
-
-```Shell
-# create python environment
-$ conda create -n hydromodel python=3.10
-$ conda activate hydromodel
-# install hydromodel
-$ pip install hydromodel
-```
-
-If you want to run the model as a developer, you can clone the repository
-
-```Shell
-# fork hydromodel to your GitHub, and clone it to your computer
-$ git clone <address of hydromodel in your github>
-# move to it
-$ cd hydromodel
-# if updating from upstream, pull the new version to local
-$ git pull
-# create python environment
-$ mamba env create -f env-dev.yml
-# if mamba is not installed:
-# $ conda install -c conda-forge mamba
-# activate it
-$ conda activate hydromodel
-```
-
-### Prepare data
-
-You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
-
-If CAMELS is used, you can skip this step.
-
-To use your own data to run the model, you need prepare the data in the required format.
-
-We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
-
-But you still need to do some manual work before transformation. Here are the steps:
-
-1. Put all data in one directory and check if it is organized as the following format:
-```
-your_data_directory_for_hydromodel/
-# one attribute csv file for all basins
-├─ basin_attributes.csv
-# one timeseries csv file for one basin, xxx and yyy are the basin ids
-├─ basin_xxx.csv
-├─ basin_yyy.csv
-├─ basin_zzz.csv
-├─ ...
-```
-basin_attributes.csv should have the following columns:
-```csv
-id     name  area(km^2)
-xxx  Basin A         100
-yyy  Basin B         200
-zzz  Basin C         300
-```
-basin_xxx.csv should have the following columns:
-```csv
-time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
-2022-01-01 00:00:00            1                 10                 13                 16                 19
-2022-01-02 00:00:00            2                 11                 14                 17                 20
-2022-01-03 00:00:00            3                 12                 15                 18                 21
-```
-The sequence of the columns is not important, but the column names should be the same as the above.
-No more unnecessary columns are allowed.
-For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
-The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
-
-1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
-```Shell
-$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
-```
-
-### Run the model
-
-To run calibration with CAMLES dataset, you can use the following code:
-
-```Shell
-# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
-$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-```
-
-To use your own data, run the following code:
-
-```Shell
-# you can change the algorithm parameters:
-$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
-# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
-```
-
-**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
-
-Then you can evaluate the calibrated model with the following code:
-
-```Shell
-# $ python evaluate_xaj.py --exp expcamels001
-# for your own data
-$ python evaluate_xaj.py --exp expbiliuhe001
-```
-
-### See the results
-
-Run the following code to see the results of the evaluation:
-
-```Shell
-# $ python visualize.py --exp expcamels001
-# for your own data
-$ python visualize.py --exp expbiliuhe001
-```
-
-You will see the results in the `example` directory.
-
-## Why does hydro-model-xaj exist
-
-When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
-models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
-model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
-provided.
-
-Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
-popular now as they are public with great performance and readable documents; as more and more people use them, they
-become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
-and develop it. I think hydro-model-xaj is a good start.
-
-## What are the main features
-
-We basically implement the formula in this book
--- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
-
-Other reference Chinese books：
-
-- ["*Principles of
-  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
-- ["*Hydrologic
-  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
-- ["*Engineering
-  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
-
-More English references could be seen at the end of this README file.
-
-The model mainly includes three parts:
-
-![](docs/img/xaj.jpg)
-
-For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
-evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
-because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
-you use pan evaporation, just treat K as Kc.
-
-For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
-little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
-
-For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
-CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
-from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
-, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
-
-We provide two common calibration methods to optimize XAJ's parameters:
-
-- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
-- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
-  is used, but no completed case is provided yet. We will provide one soon.
-
-Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
-for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
-needed, and it is not implemented yet. The following links may be useful:
-
-- https://github.com/ecoon/watershed-workflow
-- https://github.com/ConnectedSystems/Streamfall.jl
-
-**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
-
-The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
-
-Other implementations for XAJ:
-
-- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
-- Java: https://github.com/wfxr/xaj-hydrological-model
-- R, C++: https://github.com/Sibada/XAJ
-
-## How to contribute
-
-If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
-git branch for your feature and send me a pull request.
-
-If you find any problems in hydro-model-xaj, please post your questions
-on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
-
-## References
-
-- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
-  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
-- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
-  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
-- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
-  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
-  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
-  DOI:https://doi.org/10.1145/2330784.2330799
-- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
-  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
-- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
-  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
-  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
-- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
-  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
-- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
+Metadata-Version: 2.1
+Name: hydromodel
+Version: 0.2.3
+Summary: hydrological models starting from XinAnJiang
+Home-page: https://github.com/OuyangWenyu/hydromodel
+Author: Wenyu Ouyang
+Author-email: wenyuouyang@outlook.com
+License: GNU General Public License v3
+Keywords: hydromodel
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# hydromodel
+
+[![image](https://img.shields.io/pypi/v/hydromodel.svg)](https://pypi.python.org/pypi/hydromodel)
+[![image](https://img.shields.io/conda/vn/conda-forge/hydromodel.svg)](https://anaconda.org/conda-forge/hydromodel)
+
+[![image](https://pyup.io/repos/github/OuyangWenyu/hydromodel/shield.svg)](https://pyup.io/repos/github/OuyangWenyu/hydromodel)
+
+-   Free software: GNU General Public License v3
+-   Documentation: https://OuyangWenyu.github.io/hydromodel
+
+## What is hydromodel
+
+**Hydromodel is a python implementation for common hydrological models such as the XinAnJiang (XAJ) model, which is one of the most famous conceptual hydrological models, especially in Southern China.**
+
+**Not an official version, just for learning**
+
+This is a Python console program (no graphic interface now). It is **still developing**.
+
+## How to run
+
+### Install
+
+We provided a pip package. You can install it with pip:
+
+
+```Shell
+# create python environment
+$ conda create -n hydromodel python=3.10
+$ conda activate hydromodel
+# install hydromodel
+$ pip install hydromodel
+```
+
+If you want to run the model as a developer, you can clone the repository
+
+```Shell
+# fork hydromodel to your GitHub, and clone it to your computer
+$ git clone <address of hydromodel in your github>
+# move to it
+$ cd hydromodel
+# if updating from upstream, pull the new version to local
+$ git pull
+# create python environment
+$ mamba env create -f env-dev.yml
+# if mamba is not installed:
+# $ conda install -c conda-forge mamba
+# activate it
+$ conda activate hydromodel
+```
+
+### Prepare data
+
+You can use the CAMELS dataset (see [here](https://github.com/OuyangWenyu/hydrodataset) to prepare it) to run the model.
+
+If CAMELS is used, you can skip this step.
+
+To use your own data to run the model, you need prepare the data in the required format.
+
+We provide some transformation functions in the "scripts" directory. You can use them to transform your data to the required format.
+
+But you still need to do some manual work before transformation. Here are the steps:
+
+1. Put all data in one directory and check if it is organized as the following format:
+```
+your_data_directory_for_hydromodel/
+# one attribute csv file for all basins
+├─ basin_attributes.csv
+# one timeseries csv file for one basin, xxx and yyy are the basin ids
+├─ basin_xxx.csv
+├─ basin_yyy.csv
+├─ basin_zzz.csv
+├─ ...
+```
+basin_attributes.csv should have the following columns:
+```csv
+id     name  area(km^2)
+xxx  Basin A         100
+yyy  Basin B         200
+zzz  Basin C         300
+```
+basin_xxx.csv should have the following columns:
+```csv
+time  pet(mm/day)  prcp(mm/day)  flow(m^3/s)  et(mm/day)  node1_flow(m^3/s)
+2022-01-01 00:00:00            1                 10                 13                 16                 19
+2022-01-02 00:00:00            2                 11                 14                 17                 20
+2022-01-03 00:00:00            3                 12                 15                 18                 21
+```
+The sequence of the columns is not important, but the column names should be the same as the above.
+No more unnecessary columns are allowed.
+For time series csv files, et and node1_flow are optional. If you don't have them, you can ignore them.
+The units of all variables could be different, but they cannot be missed and should be put in `()` in the column name.
+
+1. Use [prepare_data.py](https://github.com/OuyangWenyu/hydro-model-xaj/tree/master/scripts) -- run the following code to transform the data format to the required format:
+```Shell
+$ python prepare_data.py --origin_data_dir <your_data_directory_for_hydromodel>
+```
+
+### Run the model
+
+To run calibration with CAMLES dataset, you can use the following code:
+
+```Shell
+# just an example the hyper-parameters of the model and the algorithm should be tried by yourself
+$ python calibrate_xaj.py --data_type camels --data_dir camels_us --exp expcamels001 --cv_fold 2 --warmup 365 --period 2007-01-01 2014-01-01 --calibrate_period 2007-01-01 2014-01-01 --test_period 2007-01-01 2014-01-01 --basin_id 01439500 06885500 08104900 09510200 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+```
+
+To use your own data, run the following code:
+
+```Shell
+# you can change the algorithm parameters:
+$ python calibrate_xaj.py --data_type owndata --data_dir "C:/Users/wenyu/OneDrive/data/biliuhe" --exp expbiliuhe001 --cv_fold 1 --warmup 720 --period "2012-06-10 00:00" "2022-08-31 23:00" --calibrate_period "2012-06-10 00:00" "2017-08-31 23:00" --test_period "2017-09-01 00:00" "2022-08-31 23:00" --basin_id 21401550 --model "{\"name\": \"xaj\", \"source_type\": \"sources5mm\", \"source_book\": \"HF\"}" --param_range_file "C:/Users/wenyu/OneDrive/data/biliuhe/param_range.yaml" --algorithm "{\"name\": \"SCE_UA\", \"random_seed\": 1234, \"rep\": 10, \"ngs\": 10, \"kstop\": 5, \"peps\": 0.1, \"pcento\": 0.1}" --loss "{\"type\": \"time_series\", \"obj_func\": \"RMSE\", \"events\": null}"
+# for advices of hyper-parameters of sceua, please see the comment of the function 'calibrate_xaj.py'
+```
+
+**NOTE**: For the parameter range in the `param_range_file` file. You can copy it from "hydromodel/models/param.yaml" of this repo and put it anywhere you want. Then you can modify the parameter range in the file. The parameter range is used to limit the parameter space of the hydromodels. If you don't provide the file, the default parameter range will be used.
+
+Then you can evaluate the calibrated model with the following code:
+
+```Shell
+# $ python evaluate_xaj.py --exp expcamels001
+# for your own data
+$ python evaluate_xaj.py --exp expbiliuhe001
+```
+
+### See the results
+
+Run the following code to see the results of the evaluation:
+
+```Shell
+# $ python visualize.py --exp expcamels001
+# for your own data
+$ python visualize.py --exp expbiliuhe001
+```
+
+You will see the results in the `example` directory.
+
+## Why does hydro-model-xaj exist
+
+When we want to learn about the rainfall-runoff process and make forecasts for floods, etc. We often use classic hydrological
+models such as XAJ as a baseline because it is trusted by many engineers and researchers. However, after searching the website very few repositories could be found. One day I happened to start learning Python, so I decided to implement the
+model with Python. Previous commits for hydro-model-xaj have some errors, but now at least one executable version is
+provided.
+
+Actually open-source science has brought a great impact on hydrological modeling. For example, SWAT and VIC are very
+popular now as they are public with great performance and readable documents; as more and more people use them, they
+become more stable and powerful. XAJ is a nice model used by many engineers for practical production. We need to inherit
+and develop it. I think hydro-model-xaj is a good start.
+
+## What are the main features
+
+We basically implement the formula in this book
+-- [《流域水文模拟》](https://xueshu.baidu.com/usercenter/paper/show?paperid=ad9c545a7baa43321db97f5f16d393bf&site=xueshu_se)
+
+Other reference Chinese books：
+
+- ["*Principles of
+  Hydrology*"/《水文学原理》](https://xueshu.baidu.com/usercenter/paper/show?paperid=5b2d0a40e2d2804f47346ae6ccf2d142&site=xueshu_se)
+- ["*Hydrologic
+  Forecasting*"/《水文预报》](https://xueshu.baidu.com/usercenter/paper/show?paperid=852a9a90a7d26c5fae749169f87b61e0&site=xueshu_se)
+- ["*Engineering
+  Hydrology*"/《工程水文学》](https://xueshu.baidu.com/usercenter/paper/show?paperid=6e2d38726c8e3c0b9f3a14bafb156481&site=xueshu_se)
+
+More English references could be seen at the end of this README file.
+
+The model mainly includes three parts:
+
+![](docs/img/xaj.jpg)
+
+For the first part, we use an evaporation coefficient K (ratio of potential evapotranspiration to reference crop
+evaporation generally from Allen, 1998) rather than Kc (the ratio of potential evapotranspiration to pan evaporation)
+because we often use potential evapotranspiration data from a system like GLDAS, NLDAS, etc. But it doesn't matter, when
+you use pan evaporation, just treat K as Kc.
+
+For the second part, we provide multiple implementations, because, for this module, formulas in different books are a
+little different. One simplest version is chosen as a default setting. More details could be seen in the source code directly now. We provide four versions, two versions from two books.
+
+For the third part -- routing module, we provide different ways: the default is a common way with recession constant (
+CS) and lag time (L) shown in the figure; second (You can set the model's name as "xaj_mz" to use it) is a model
+from [mizuRoute](http://www.geosci-model-dev.net/9/2223/2016/) to generate unit hydrograph for surface runoff (Rs -> Qs)
+, as its parameters are easier to set, and we can optimize all parameters in a uniform way.
+
+We provide two common calibration methods to optimize XAJ's parameters:
+
+- [SCE-UA](https://doi.org/10.1029/91WR02985) from [spotpy](https://github.com/thouska/spotpy)
+- [GA](https://en.wikipedia.org/wiki/Genetic_algorithm) from [DEAP](https://github.com/DEAP/deap): now only the method
+  is used, but no completed case is provided yet. We will provide one soon.
+
+Now the model is only for **one computing element** (typically, a headwater catchment). Soon we will provide calibration
+for multiple headwater catchments. To get a better simulation for large basins, a (semi-)distributed version may be
+needed, and it is not implemented yet. The following links may be useful:
+
+- https://github.com/ecoon/watershed-workflow
+- https://github.com/ConnectedSystems/Streamfall.jl
+
+**NOTE: We also provide a differentiable version of XAJ, which is based on the [PyTorch](https://pytorch.org/) framework.**
+
+The idea comes from this paper: [From calibration to parameter learning: Harnessing the scaling effects of big data in geoscientific modeling](http://dx.doi.org/10.1038/s41467-021-26107-z) by Tsai et al. (2021). We use the same structure as the original XAJ model but replace the original Numpy code with PyTorch. Then we can use the automatic differentiation technique and stochastic gradient descent algorithms to optimize all parameters. The advantage of this method is that we can use the same code to optimize many basins at once and use big data to improve the model performance. Generally, with the native parallel computing ability of PyTorch, the differentiable version is faster than the original version without any parallel processing. The differentiable version is also in the `models` directory.
+
+Other implementations for XAJ:
+
+- Matlab: https://github.com/wknoben/MARRMoT/blob/master/MARRMoT/Models/Model%20files/m_28_xinanjiang_12p_4s.m
+- Java: https://github.com/wfxr/xaj-hydrological-model
+- R, C++: https://github.com/Sibada/XAJ
+
+## How to contribute
+
+If you want to add features for hydro-model-xaj, for example, write a distributed version for XAJ, please create a new
+git branch for your feature and send me a pull request.
+
+If you find any problems in hydro-model-xaj, please post your questions
+on [issues](https://github.com/OuyangWenyu/hydro-model-xaj/issues).
+
+## References
+
+- Allen, R.G., L. Pereira, D. Raes, and M. Smith, 1998. Crop Evapotranspiration, Food and Agriculture Organization of
+  the United Nations, Rome, Italy. FAO publication 56. ISBN 92-5-104219-5. 290p.
+- Duan, Q., Sorooshian, S., and Gupta, V. (1992), Effective and efficient global optimization for conceptual
+  rainfall-runoff models, Water Resour. Res., 28( 4), 1015– 1031, doi:10.1029/91WR02985.
+- François-Michel De Rainville, Félix-Antoine Fortin, Marc-André Gardner, Marc Parizeau, and Christian Gagné. 2012.
+  DEAP: a python framework for evolutionary algorithms. In Proceedings of the 14th annual conference companion on
+  Genetic and evolutionary computation (GECCO '12). Association for Computing Machinery, New York, NY, USA, 85–92.
+  DOI:https://doi.org/10.1145/2330784.2330799
+- Houska T, Kraft P, Chamorro-Chavez A, Breuer L (2015) SPOTting Model Parameters Using a Ready-Made Python Package.
+  PLoS ONE 10(12): e0145180. https://doi.org/10.1371/journal.pone.0145180
+- Mizukami, N., Clark, M. P., Sampson, K., Nijssen, B., Mao, Y., McMillan, H., Viger, R. J., Markstrom, S. L., Hay, L.
+  E., Woods, R., Arnold, J. R., and Brekke, L. D.: mizuRoute version 1: a river network routing tool for a continental
+  domain water resources applications, Geosci. Model Dev., 9, 2223–2238, https://doi.org/10.5194/gmd-9-2223-2016, 2016.
+- Zhao, R.J., Zhuang, Y. L., Fang, L. R., Liu, X. R., Zhang, Q. S. (ed) (1980) The Xinanjiang model, Hydrological
+  Forecasting Proc., Oxford Symp., IAHS Publication, Wallingford, U.K.
+- Zhao, R.J., 1992. The xinanjiang model applied in China. J Hydrol 135 (1–4), 371–381.
```

### Comparing `hydromodel-0.2.2/hydromodel.egg-info/SOURCES.txt` & `hydromodel-0.2.3/hydromodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.2/setup.py` & `hydromodel-0.2.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-28 09:16:46
-LastEditTime: 2024-03-28 12:07:42
-LastEditors: Wenyu Ouyang
-Description: The setup script
-FilePath: \hydromodel\setup.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import io
-import pathlib
-from os import path as op
-from setuptools import setup, find_packages
-
-readme = pathlib.Path("README.md").read_text(encoding='utf-8')
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = []
-
-setup_requirements = [
-    "pytest-runner",
-]
-
-test_requirements = [
-    "pytest>=3",
-]
-
-setup(
-    author="Wenyu Ouyang",
-    author_email="wenyuouyang@outlook.com",
-    python_requires=">=3.10",
-    classifiers=[
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-    description="hydrological models starting from XinAnJiang",
-    entry_points={
-        "console_scripts": [
-            "hydromodel=hydromodel.cli:main",
-        ],
-    },
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="GNU General Public License v3",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    keywords="hydromodel",
-    name="hydromodel",
-    packages=find_packages(include=["hydromodel", "hydromodel.*"]),
-    setup_requires=setup_requirements,
-    test_suite="tests",
-    tests_require=test_requirements,
-    url="https://github.com/OuyangWenyu/hydromodel",
-    version='0.2.2',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-28 09:16:46
+LastEditTime: 2024-03-28 12:07:42
+LastEditors: Wenyu Ouyang
+Description: The setup script
+FilePath: \hydromodel\setup.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import io
+import pathlib
+from os import path as op
+from setuptools import setup, find_packages
+
+readme = pathlib.Path("README.md").read_text(encoding='utf-8')
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = []
+
+setup_requirements = [
+    "pytest-runner",
+]
+
+test_requirements = [
+    "pytest>=3",
+]
+
+setup(
+    author="Wenyu Ouyang",
+    author_email="wenyuouyang@outlook.com",
+    python_requires=">=3.10",
+    classifiers=[
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    description="hydrological models starting from XinAnJiang",
+    entry_points={
+        "console_scripts": [
+            "hydromodel=hydromodel.cli:main",
+        ],
+    },
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="GNU General Public License v3",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    include_package_data=True,
+    keywords="hydromodel",
+    name="hydromodel",
+    packages=find_packages(include=["hydromodel", "hydromodel.*"]),
+    setup_requires=setup_requirements,
+    test_suite="tests",
+    tests_require=test_requirements,
+    url="https://github.com/OuyangWenyu/hydromodel",
+    version='0.2.3',
+    zip_safe=False,
+)
```

### Comparing `hydromodel-0.2.2/test/test_data_preprocess.py` & `hydromodel-0.2.3/test/test_data_preprocess.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-from hydrodataset import Camels
-import numpy as np
-import pytest
-import os
-import pandas as pd
-import xarray as xr
-
-from hydromodel import SETTING
-from hydromodel.datasets import *
-from hydromodel.datasets.data_preprocess import (
-    process_and_save_data_as_nc,
-    split_train_test,
-    check_tsdata_format,
-    check_basin_attr_format,
-    check_folder_contents,
-    cross_valid_data,
-)
-
-
-@pytest.fixture()
-def basin_attrs_file(tmp_path):
-    # Create a temporary CSV file with required columns
-    file_path = tmp_path / "basin_attributes.csv"
-    data = pd.DataFrame(
-        {
-            ID_NAME: [1, 2, 3],
-            NAME_NAME: ["Basin A", "Basin B", "Basin C"],
-            AREA_NAME: [100, 200, 300],
-        }
-    )
-    data.to_csv(file_path, index=False)
-    return str(file_path)
-
-
-@pytest.fixture()
-def all_data_dir(tmp_path):
-    # Create time series data files for basins 1, 2, and 3
-    for basin_id in [1, 2, 3]:
-        file_name = f"basin_{basin_id}.csv"
-        file_path = tmp_path / file_name
-
-        data = pd.DataFrame(
-            {
-                TIME_NAME: [
-                    "2022-01-01 00:00:00",
-                    "2022-01-02 00:00:00",
-                    "2022-01-03 00:00:00",
-                ],
-                PET_NAME: [1, 2, 3],
-                PRCP_NAME: [4, 5, 6],
-                FLOW_NAME: [7, 8, 9],
-                ET_NAME: [10, 11, 12],
-                NODE_FLOW_NAME: [13, 14, 15],
-            }
-        )
-        data.to_csv(file_path, index=False)
-
-    return str(tmp_path)
-
-
-def test_check_basin_attributes_format_with_valid_file(basin_attrs_file):
-    assert check_basin_attr_format(basin_attrs_file) == True
-
-
-def test_check_basin_attributes_format_with_missing_columns(basin_attrs_file):
-    # Remove the 'name' column from the file
-    data = pd.read_csv(basin_attrs_file)
-    data.drop(columns=["name"], inplace=True)
-    data.to_csv(basin_attrs_file, index=False)
-
-    assert check_basin_attr_format(basin_attrs_file) == False
-
-
-def test_check_basin_attributes_format_with_invalid_file(basin_attrs_file):
-    # Write invalid data to the file
-    with open(basin_attrs_file, "w") as f:
-        f.write("Invalid data")
-
-    assert check_basin_attr_format(basin_attrs_file) == False
-
-
-def test_check_your_own_data(all_data_dir):
-    """
-    Test to check the format of hydrological modeling data.
-    """
-    # Define a sample file path
-    file_path = os.path.join(all_data_dir, "basin_1.csv")
-
-    # Check the format of hydrological modeling data
-    result = check_tsdata_format(file_path)
-
-    # Assert that the result is True
-    assert result
-
-    # Clean up the sample file
-    os.remove(file_path)
-
-
-def test_check_your_own_data_missing_required_columns(tmpdir):
-    """
-    Test to check the format of hydrological modeling data with missing required columns.
-    """
-    # Define a sample file path
-    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
-
-    # Create a sample file with missing required columns
-    sample_data = pd.DataFrame(
-        {
-            PRCP_NAME: [4, 5, 6],
-            FLOW_NAME: [7, 8, 9],
-            ET_NAME: [10, 11, 12],
-            NODE_FLOW_NAME: [13, 14, 15],
-        }
-    )
-    sample_data.to_csv(file_path, index=False)
-
-    # Check the format of hydrological modeling data
-    result = check_tsdata_format(file_path)
-
-    # Assert that the result is False
-    assert not result
-
-    # Clean up the sample file
-    os.remove(file_path)
-
-
-def test_check_your_own_data_missing_optional_columns(tmpdir):
-    """
-    Test to check the format of hydrological modeling data with missing optional columns.
-    """
-    # Define a sample file path
-    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
-
-    # Create a sample file with missing optional columns
-    sample_data = pd.DataFrame(
-        {
-            TIME_NAME: [
-                "2022-01-01 00:00:00",
-                "2022-01-02 00:00:00",
-                "2022-01-03 00:00:00",
-            ],
-            PET_NAME: [1, 2, 3],
-            PRCP_NAME: [4, 5, 6],
-            FLOW_NAME: [7, 8, 9],
-        }
-    )
-    sample_data.to_csv(file_path, index=False)
-
-    # Check the format of hydrological modeling data
-    result = check_tsdata_format(file_path)
-
-    # Assert that the result is True
-    assert result
-
-    # Clean up the sample file
-    os.remove(file_path)
-
-
-def test_check_your_own_data_invalid_file(tmpdir):
-    """
-    Test to check the format of an invalid hydrological modeling data file.
-    """
-    # Define a sample file path
-    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
-
-    # Create an invalid file (not a CSV)
-    with open(file_path, "w") as f:
-        f.write("This is not a valid CSV file.")
-
-    # Check the format of hydrological modeling data
-    result = check_tsdata_format(file_path)
-
-    # Assert that the result is False
-    assert not result
-
-    # Clean up the sample file
-    os.remove(file_path)
-
-
-def test_check_folder_contents_with_valid_files(basin_attrs_file, all_data_dir):
-    assert check_folder_contents(all_data_dir, basin_attrs_file) == True
-
-
-def test_check_folder_contents_with_missing_time_series_data_file(
-    basin_attrs_file, tmp_path
-):
-    # 创建一个模拟的时序数据文件，然后删除它，模拟缺失的文件场景
-    file_path = tmp_path / "basin_2.csv"
-    with open(file_path, "w") as f:
-        f.write("Dummy data")
-    os.remove(file_path)
-
-    # 调用检查函数，确保它正确地返回 False
-    assert check_folder_contents(tmp_path, basin_attrs_file) == False
-
-
-def test_check_folder_contents_with_invalid_time_series_data_file(
-    basin_attrs_file, tmp_path
-):
-    # Create an invalid time series data file for basin 1
-    file_path = tmp_path / "basin_1.csv"
-    with open(file_path, "w") as f:
-        f.write("Invalid data")
-
-    assert check_folder_contents(tmp_path, basin_attrs_file) == False
-
-
-def test_check_folder_contents_with_missing_basin_attributes_file(
-    tmp_path, basin_attrs_file
-):
-    # Remove basin attributes file
-    os.remove(basin_attrs_file)
-
-    assert check_folder_contents(tmp_path) == False
-
-
-def test_check_folder_contents_with_missing_basin_attributes_column(
-    basin_attrs_file, all_data_dir
-):
-    # Remove 'name' column from basin attributes file
-    data = pd.read_csv(basin_attrs_file)
-    data.drop(columns=["name"], inplace=True)
-    data.to_csv(basin_attrs_file, index=False)
-
-    assert check_folder_contents(all_data_dir, basin_attrs_file) == False
-
-
-def test_process_and_save_data_as_nc_with_valid_data(all_data_dir, basin_attrs_file):
-    # Create a temporary folder for testing
-    folder_path = os.path.join(all_data_dir, "test_folder")
-    os.makedirs(folder_path)
-
-    # Call the function to process and save the data as NetCDF files
-    result = process_and_save_data_as_nc(all_data_dir, folder_path)
-
-    # Assert that the function returns True
-    assert result
-
-    # Assert that the NetCDF files are created
-    attrs_file = os.path.join(folder_path, "attributes.nc")
-    ts_file = os.path.join(folder_path, "timeseries.nc")
-    assert os.path.exists(attrs_file)
-    assert os.path.exists(ts_file)
-
-    # 使用 xarray 加载 NetCDF 文件
-    ds_attrs = xr.open_dataset(attrs_file)
-    ds_ts = xr.open_dataset(ts_file)
-
-    # 确保加载的数据集不为空
-    assert ds_attrs is not None
-    assert ds_ts is not None
-
-
-def test_load_dataset():
-    dataset_dir = SETTING["local_data_path"]["datasets-origin"]
-    camels = Camels(os.path.join(dataset_dir, "camels", "camels_us"))
-    data = camels.read_ts_xrdataset(
-        ["01013500"], ["2010-01-01", "2014-01-01"], ["streamflow"]
-    )
-    print(data)
-
-
-@pytest.fixture
-def ts_data_tmp(periods=10):
-    basins = ["basin1", "basin2", "basin3"]
-    return xr.Dataset(
-        {
-            "flow": (("time", "basin"), np.random.rand(periods, 3)),
-            "prcp": (("time", "basin"), np.random.rand(periods, 3)),
-        },
-        coords={
-            "time": pd.date_range(start="2022-01-01", periods=periods),
-            "basin": basins,
-        },
-    )
-
-
-def test_cross_valid_data(ts_data_tmp):
-    period = ("2022-01-01", "2022-01-10")
-    warmup = 3
-    cv_fold = 3
-
-    train_test_data = cross_valid_data(ts_data_tmp, period, warmup, cv_fold)
-
-    assert len(train_test_data) == cv_fold
-
-
-def test_split_train_test(ts_data_tmp):
-    # Define the train and test periods
-    train_period = ("2022-01-01", "2022-01-05")
-    test_period = ("2022-01-06", "2022-01-10")
-
-    # Call the function to split the data
-    train_data, test_data = split_train_test(ts_data_tmp, train_period, test_period)
-
-    # Assert that the train and test data have the correct length and shape
-    basins = ["basin1", "basin2", "basin3"]
-    assert len(train_data.time) == 5 and train_data.flow.shape == (5, len(basins))
-    assert len(test_data.time) == 5 and test_data.flow.shape == (5, len(basins))
+from hydrodataset import Camels
+import numpy as np
+import pytest
+import os
+import pandas as pd
+import xarray as xr
+
+from hydromodel import SETTING
+from hydromodel.datasets import *
+from hydromodel.datasets.data_preprocess import (
+    process_and_save_data_as_nc,
+    split_train_test,
+    check_tsdata_format,
+    check_basin_attr_format,
+    check_folder_contents,
+    cross_valid_data,
+)
+
+
+@pytest.fixture()
+def basin_attrs_file(tmp_path):
+    # Create a temporary CSV file with required columns
+    file_path = tmp_path / "basin_attributes.csv"
+    data = pd.DataFrame(
+        {
+            ID_NAME: [1, 2, 3],
+            NAME_NAME: ["Basin A", "Basin B", "Basin C"],
+            AREA_NAME: [100, 200, 300],
+        }
+    )
+    data.to_csv(file_path, index=False)
+    return str(file_path)
+
+
+@pytest.fixture()
+def all_data_dir(tmp_path):
+    # Create time series data files for basins 1, 2, and 3
+    for basin_id in [1, 2, 3]:
+        file_name = f"basin_{basin_id}.csv"
+        file_path = tmp_path / file_name
+
+        data = pd.DataFrame(
+            {
+                TIME_NAME: [
+                    "2022-01-01 00:00:00",
+                    "2022-01-02 00:00:00",
+                    "2022-01-03 00:00:00",
+                ],
+                PET_NAME: [1, 2, 3],
+                PRCP_NAME: [4, 5, 6],
+                FLOW_NAME: [7, 8, 9],
+                ET_NAME: [10, 11, 12],
+                NODE_FLOW_NAME: [13, 14, 15],
+            }
+        )
+        data.to_csv(file_path, index=False)
+
+    return str(tmp_path)
+
+
+def test_check_basin_attributes_format_with_valid_file(basin_attrs_file):
+    assert check_basin_attr_format(basin_attrs_file) == True
+
+
+def test_check_basin_attributes_format_with_missing_columns(basin_attrs_file):
+    # Remove the 'name' column from the file
+    data = pd.read_csv(basin_attrs_file)
+    data.drop(columns=["name"], inplace=True)
+    data.to_csv(basin_attrs_file, index=False)
+
+    assert check_basin_attr_format(basin_attrs_file) == False
+
+
+def test_check_basin_attributes_format_with_invalid_file(basin_attrs_file):
+    # Write invalid data to the file
+    with open(basin_attrs_file, "w") as f:
+        f.write("Invalid data")
+
+    assert check_basin_attr_format(basin_attrs_file) == False
+
+
+def test_check_your_own_data(all_data_dir):
+    """
+    Test to check the format of hydrological modeling data.
+    """
+    # Define a sample file path
+    file_path = os.path.join(all_data_dir, "basin_1.csv")
+
+    # Check the format of hydrological modeling data
+    result = check_tsdata_format(file_path)
+
+    # Assert that the result is True
+    assert result
+
+    # Clean up the sample file
+    os.remove(file_path)
+
+
+def test_check_your_own_data_missing_required_columns(tmpdir):
+    """
+    Test to check the format of hydrological modeling data with missing required columns.
+    """
+    # Define a sample file path
+    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
+
+    # Create a sample file with missing required columns
+    sample_data = pd.DataFrame(
+        {
+            PRCP_NAME: [4, 5, 6],
+            FLOW_NAME: [7, 8, 9],
+            ET_NAME: [10, 11, 12],
+            NODE_FLOW_NAME: [13, 14, 15],
+        }
+    )
+    sample_data.to_csv(file_path, index=False)
+
+    # Check the format of hydrological modeling data
+    result = check_tsdata_format(file_path)
+
+    # Assert that the result is False
+    assert not result
+
+    # Clean up the sample file
+    os.remove(file_path)
+
+
+def test_check_your_own_data_missing_optional_columns(tmpdir):
+    """
+    Test to check the format of hydrological modeling data with missing optional columns.
+    """
+    # Define a sample file path
+    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
+
+    # Create a sample file with missing optional columns
+    sample_data = pd.DataFrame(
+        {
+            TIME_NAME: [
+                "2022-01-01 00:00:00",
+                "2022-01-02 00:00:00",
+                "2022-01-03 00:00:00",
+            ],
+            PET_NAME: [1, 2, 3],
+            PRCP_NAME: [4, 5, 6],
+            FLOW_NAME: [7, 8, 9],
+        }
+    )
+    sample_data.to_csv(file_path, index=False)
+
+    # Check the format of hydrological modeling data
+    result = check_tsdata_format(file_path)
+
+    # Assert that the result is True
+    assert result
+
+    # Clean up the sample file
+    os.remove(file_path)
+
+
+def test_check_your_own_data_invalid_file(tmpdir):
+    """
+    Test to check the format of an invalid hydrological modeling data file.
+    """
+    # Define a sample file path
+    file_path = os.path.join(str(tmpdir), "hydro_data.csv")
+
+    # Create an invalid file (not a CSV)
+    with open(file_path, "w") as f:
+        f.write("This is not a valid CSV file.")
+
+    # Check the format of hydrological modeling data
+    result = check_tsdata_format(file_path)
+
+    # Assert that the result is False
+    assert not result
+
+    # Clean up the sample file
+    os.remove(file_path)
+
+
+def test_check_folder_contents_with_valid_files(basin_attrs_file, all_data_dir):
+    assert check_folder_contents(all_data_dir, basin_attrs_file) == True
+
+
+def test_check_folder_contents_with_missing_time_series_data_file(
+    basin_attrs_file, tmp_path
+):
+    # 创建一个模拟的时序数据文件，然后删除它，模拟缺失的文件场景
+    file_path = tmp_path / "basin_2.csv"
+    with open(file_path, "w") as f:
+        f.write("Dummy data")
+    os.remove(file_path)
+
+    # 调用检查函数，确保它正确地返回 False
+    assert check_folder_contents(tmp_path, basin_attrs_file) == False
+
+
+def test_check_folder_contents_with_invalid_time_series_data_file(
+    basin_attrs_file, tmp_path
+):
+    # Create an invalid time series data file for basin 1
+    file_path = tmp_path / "basin_1.csv"
+    with open(file_path, "w") as f:
+        f.write("Invalid data")
+
+    assert check_folder_contents(tmp_path, basin_attrs_file) == False
+
+
+def test_check_folder_contents_with_missing_basin_attributes_file(
+    tmp_path, basin_attrs_file
+):
+    # Remove basin attributes file
+    os.remove(basin_attrs_file)
+
+    assert check_folder_contents(tmp_path) == False
+
+
+def test_check_folder_contents_with_missing_basin_attributes_column(
+    basin_attrs_file, all_data_dir
+):
+    # Remove 'name' column from basin attributes file
+    data = pd.read_csv(basin_attrs_file)
+    data.drop(columns=["name"], inplace=True)
+    data.to_csv(basin_attrs_file, index=False)
+
+    assert check_folder_contents(all_data_dir, basin_attrs_file) == False
+
+
+def test_process_and_save_data_as_nc_with_valid_data(all_data_dir, basin_attrs_file):
+    # Create a temporary folder for testing
+    folder_path = os.path.join(all_data_dir, "test_folder")
+    os.makedirs(folder_path)
+
+    # Call the function to process and save the data as NetCDF files
+    result = process_and_save_data_as_nc(all_data_dir, folder_path)
+
+    # Assert that the function returns True
+    assert result
+
+    # Assert that the NetCDF files are created
+    attrs_file = os.path.join(folder_path, "attributes.nc")
+    ts_file = os.path.join(folder_path, "timeseries.nc")
+    assert os.path.exists(attrs_file)
+    assert os.path.exists(ts_file)
+
+    # 使用 xarray 加载 NetCDF 文件
+    ds_attrs = xr.open_dataset(attrs_file)
+    ds_ts = xr.open_dataset(ts_file)
+
+    # 确保加载的数据集不为空
+    assert ds_attrs is not None
+    assert ds_ts is not None
+
+
+def test_load_dataset():
+    dataset_dir = SETTING["local_data_path"]["datasets-origin"]
+    camels = Camels(os.path.join(dataset_dir, "camels", "camels_us"))
+    data = camels.read_ts_xrdataset(
+        ["01013500"], ["2010-01-01", "2014-01-01"], ["streamflow"]
+    )
+    print(data)
+
+
+@pytest.fixture
+def ts_data_tmp(periods=10):
+    basins = ["basin1", "basin2", "basin3"]
+    return xr.Dataset(
+        {
+            "flow": (("time", "basin"), np.random.rand(periods, 3)),
+            "prcp": (("time", "basin"), np.random.rand(periods, 3)),
+        },
+        coords={
+            "time": pd.date_range(start="2022-01-01", periods=periods),
+            "basin": basins,
+        },
+    )
+
+
+def test_cross_valid_data(ts_data_tmp):
+    period = ("2022-01-01", "2022-01-10")
+    warmup = 3
+    cv_fold = 3
+
+    train_test_data = cross_valid_data(ts_data_tmp, period, warmup, cv_fold)
+
+    assert len(train_test_data) == cv_fold
+
+
+def test_split_train_test(ts_data_tmp):
+    # Define the train and test periods
+    train_period = ("2022-01-01", "2022-01-05")
+    test_period = ("2022-01-06", "2022-01-10")
+
+    # Call the function to split the data
+    train_data, test_data = split_train_test(ts_data_tmp, train_period, test_period)
+
+    # Assert that the train and test data have the correct length and shape
+    basins = ["basin1", "basin2", "basin3"]
+    assert len(train_data.time) == 5 and train_data.flow.shape == (5, len(basins))
+    assert len(test_data.time) == 5 and test_data.flow.shape == (5, len(basins))
```

### Comparing `hydromodel-0.2.2/test/test_gr4j.py` & `hydromodel-0.2.3/test/test_gr4j.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-06-02 09:30:36
-LastEditTime: 2024-03-22 20:21:30
-LastEditors: Wenyu Ouyang
-Description: Test case for GR4J model
-FilePath: \hydro-model-xaj\test\test_gr4j.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import numpy as np
-import pytest
-
-from hydromodel.models.gr4j import gr4j
-
-
-@pytest.fixture()
-def params():
-    # all parameters are in range [0,1]
-    return np.tile([0.5], (1, 4))
-
-
-def test_gr4j(p_and_e, params, qobs, warmup_length):
-    qsim, _ = gr4j(p_and_e, params, warmup_length=warmup_length)
-    np.testing.assert_array_equal(
-        qsim.shape, (qobs.shape[0] - warmup_length, qobs.shape[1], qobs.shape[2])
-    )
+"""
+Author: Wenyu Ouyang
+Date: 2023-06-02 09:30:36
+LastEditTime: 2024-03-22 20:21:30
+LastEditors: Wenyu Ouyang
+Description: Test case for GR4J model
+FilePath: \hydro-model-xaj\test\test_gr4j.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import numpy as np
+import pytest
+
+from hydromodel.models.gr4j import gr4j
+
+
+@pytest.fixture()
+def params():
+    # all parameters are in range [0,1]
+    return np.tile([0.5], (1, 4))
+
+
+def test_gr4j(p_and_e, params, qobs, warmup_length):
+    qsim, _ = gr4j(p_and_e, params, warmup_length=warmup_length)
+    np.testing.assert_array_equal(
+        qsim.shape, (qobs.shape[0] - warmup_length, qobs.shape[1], qobs.shape[2])
+    )
```

### Comparing `hydromodel-0.2.2/test/test_xaj.py` & `hydromodel-0.2.3/test/test_xaj.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import numpy as np
-import pytest
-
-from hydromodel.models.xaj import xaj, uh_gamma, uh_conv
-
-
-@pytest.fixture()
-def params():
-    # all parameters are in range [0,1]
-    return np.tile([0.5], (1, 15))
-
-
-def test_uh_gamma():
-    # repeat for 20 periods and add one dim as feature: time_seq=20, batch=10, feature=1
-    routa = np.tile(2.5, (20, 10, 1))
-    routb = np.tile(3.5, (20, 10, 1))
-    uh = uh_gamma(routa, routb, len_uh=15)
-    np.testing.assert_almost_equal(
-        uh[:, 0, :],
-        np.array(
-            [
-                [0.0069],
-                [0.0314],
-                [0.0553],
-                [0.0738],
-                [0.0860],
-                [0.0923],
-                [0.0939],
-                [0.0919],
-                [0.0875],
-                [0.0814],
-                [0.0744],
-                [0.0670],
-                [0.0597],
-                [0.0525],
-                [0.0459],
-            ]
-        ),
-        decimal=3,
-    )
-
-
-def test_uh():
-    uh_from_gamma = np.tile(1, (5, 3, 1))
-    # uh_from_gamma = np.arange(15).reshape(5, 3, 1)
-    rf = np.arange(30).reshape(10, 3, 1) / 100
-    qs = uh_conv(rf, uh_from_gamma)
-    np.testing.assert_almost_equal(
-        np.array(
-            [
-                [0.0000, 0.0100, 0.0200],
-                [0.0300, 0.0500, 0.0700],
-                [0.0900, 0.1200, 0.1500],
-                [0.1800, 0.2200, 0.2600],
-                [0.3000, 0.3500, 0.4000],
-                [0.4500, 0.5000, 0.5500],
-                [0.6000, 0.6500, 0.7000],
-                [0.7500, 0.8000, 0.8500],
-                [0.9000, 0.9500, 1.0000],
-                [1.0500, 1.1000, 1.1500],
-            ]
-        ),
-        qs[:, :, 0],
-        decimal=3,
-    )
-
-
-def test_xaj(p_and_e, params, warmup_length):
-    qsim, e = xaj(
-        p_and_e,
-        params,
-        warmup_length=warmup_length,
-        name="xaj",
-        source_book="HF",
-        source_type="sources",
-    )
-    np.testing.assert_array_equal(qsim.shape[0], p_and_e.shape[0] - warmup_length)
-
-
-def test_xaj_mz(p_and_e, params, warmup_length):
-    qsim, e = xaj(
-        p_and_e,
-        np.tile([0.5], (1, 16)),
-        warmup_length=warmup_length,
-        name="xaj_mz",
-        source_book="HF",
-        source_type="sources",
-    )
-    np.testing.assert_array_equal(qsim.shape[0], p_and_e.shape[0] - warmup_length)
+import numpy as np
+import pytest
+
+from hydromodel.models.xaj import xaj, uh_gamma, uh_conv
+
+
+@pytest.fixture()
+def params():
+    # all parameters are in range [0,1]
+    return np.tile([0.5], (1, 15))
+
+
+def test_uh_gamma():
+    # repeat for 20 periods and add one dim as feature: time_seq=20, batch=10, feature=1
+    routa = np.tile(2.5, (20, 10, 1))
+    routb = np.tile(3.5, (20, 10, 1))
+    uh = uh_gamma(routa, routb, len_uh=15)
+    np.testing.assert_almost_equal(
+        uh[:, 0, :],
+        np.array(
+            [
+                [0.0069],
+                [0.0314],
+                [0.0553],
+                [0.0738],
+                [0.0860],
+                [0.0923],
+                [0.0939],
+                [0.0919],
+                [0.0875],
+                [0.0814],
+                [0.0744],
+                [0.0670],
+                [0.0597],
+                [0.0525],
+                [0.0459],
+            ]
+        ),
+        decimal=3,
+    )
+
+
+def test_uh():
+    uh_from_gamma = np.tile(1, (5, 3, 1))
+    # uh_from_gamma = np.arange(15).reshape(5, 3, 1)
+    rf = np.arange(30).reshape(10, 3, 1) / 100
+    qs = uh_conv(rf, uh_from_gamma)
+    np.testing.assert_almost_equal(
+        np.array(
+            [
+                [0.0000, 0.0100, 0.0200],
+                [0.0300, 0.0500, 0.0700],
+                [0.0900, 0.1200, 0.1500],
+                [0.1800, 0.2200, 0.2600],
+                [0.3000, 0.3500, 0.4000],
+                [0.4500, 0.5000, 0.5500],
+                [0.6000, 0.6500, 0.7000],
+                [0.7500, 0.8000, 0.8500],
+                [0.9000, 0.9500, 1.0000],
+                [1.0500, 1.1000, 1.1500],
+            ]
+        ),
+        qs[:, :, 0],
+        decimal=3,
+    )
+
+
+def test_xaj(p_and_e, params, warmup_length):
+    qsim, e = xaj(
+        p_and_e,
+        params,
+        warmup_length=warmup_length,
+        name="xaj",
+        source_book="HF",
+        source_type="sources",
+    )
+    np.testing.assert_array_equal(qsim.shape[0], p_and_e.shape[0] - warmup_length)
+
+
+def test_xaj_mz(p_and_e, params, warmup_length):
+    qsim, e = xaj(
+        p_and_e,
+        np.tile([0.5], (1, 16)),
+        warmup_length=warmup_length,
+        name="xaj_mz",
+        source_book="HF",
+        source_type="sources",
+    )
+    np.testing.assert_array_equal(qsim.shape[0], p_and_e.shape[0] - warmup_length)
```

