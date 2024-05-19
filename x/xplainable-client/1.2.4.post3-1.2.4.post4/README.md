# Comparing `tmp/xplainable_client-1.2.4.post3.tar.gz` & `tmp/xplainable-client-1.2.4.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.4.post3.tar", last modified: Sat May 18 02:38:51 2024, max compression
+gzip compressed data, was "xplainable-client-1.2.4.post4.tar", last modified: Sat May 18 05:53:57 2024, max compression
```

## Comparing `xplainable_client-1.2.4.post3.tar` & `xplainable-client-1.2.4.post4.tar`

### file list

```diff
@@ -1,49 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.571044 xplainable_client-1.2.4.post3/
--rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.4.post3/.gitignore
--rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post3/LICENSE
--rw-rw-rw-   0        0        0    45382 2024-05-18 02:38:51.569544 xplainable_client-1.2.4.post3/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/README.md
--rw-rw-rw-   0        0        0     1494 2024-05-17 23:36:00.000000 xplainable_client-1.2.4.post3/_build.py
--rw-rw-rw-   0        0        0       29 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/_version.py
--rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/config.py
--rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/docker-compose.yaml
--rw-rw-rw-   0        0        0      895 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/pyproject.toml
--rw-rw-rw-   0        0        0      152 2024-05-17 05:49:28.000000 xplainable_client-1.2.4.post3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 02:38:51.571044 xplainable_client-1.2.4.post3/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.532544 xplainable_client-1.2.4.post3/tests/
--rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/nanoid.sql
--rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/prod-db.sql
--rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/test_model.py
--rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/test_test.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.535044 xplainable_client-1.2.4.post3/thebadboycorner/
--rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.4.post3/thebadboycorner/clf_model_test_jason.py
--rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post3/thebadboycorner/test.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.537545 xplainable_client-1.2.4.post3/xplainable_client/
--rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.4.post3/xplainable_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.558044 xplainable_client-1.2.4.post3/xplainable_client/client/
--rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_client_cog_base.py
--rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_collections.py
--rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_datasets.py
--rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_deployments.py
--rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_gpt.py
--rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_inference.py
--rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_misc.py
--rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_models.py
--rw-rw-rw-   0        0        0     9609 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_preprocessing.py
--rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_session.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.566545 xplainable_client-1.2.4.post3/xplainable_client/client/utils/
--rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/encoders.py
--rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/helpers.py
--rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/metrics.py
--rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/model_parsers.py
--rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/scanner.py
--rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/xplainable_client/pytest.ini
-drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.568045 xplainable_client-1.2.4.post3/xplainable_client.egg-info/
--rw-rw-rw-   0        0        0    45382 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/top_level.txt
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.510280 xplainable-client-1.2.4.post4/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    34523 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post4/LICENSE
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44077 2024-05-18 05:53:57.510081 xplainable-client-1.2.4.post4/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3924 2024-02-21 21:39:20.000000 xplainable-client-1.2.4.post4/README.md
+-rw-r--r--   0 jtuppack   (501) staff       (20)      858 2024-05-18 05:49:41.000000 xplainable-client-1.2.4.post4/pyproject.toml
+-rw-r--r--   0 jtuppack   (501) staff       (20)       38 2024-05-18 05:53:57.510326 xplainable-client-1.2.4.post4/setup.cfg
+-rw-r--r--   0 jtuppack   (501) staff       (20)      852 2024-05-18 05:51:31.000000 xplainable-client-1.2.4.post4/setup.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.505405 xplainable-client-1.2.4.post4/tests/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      270 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post4/tests/test_model.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      184 2024-05-18 01:38:20.000000 xplainable-client-1.2.4.post4/tests/test_test.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.505609 xplainable-client-1.2.4.post4/xplainable_client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)       27 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/__init__.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.508308 xplainable-client-1.2.4.post4/xplainable_client/client/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      946 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      123 2024-05-16 09:16:42.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_client_cog_base.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7324 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_collections.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1245 2024-05-16 09:16:42.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_datasets.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    14605 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_deployments.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1218 2024-05-17 03:09:19.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_gpt.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1236 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_inference.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     7982 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_misc.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    20834 2024-05-17 23:17:59.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_models.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     9359 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_preprocessing.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4020 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/_session.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.509413 xplainable-client-1.2.4.post4/xplainable_client/client/utils/
+-rw-r--r--   0 jtuppack   (501) staff       (20)      122 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/__init__.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1291 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/encoders.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)      961 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/helpers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     6416 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/metrics.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)     3042 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/model_parsers.py
+-rw-r--r--   0 jtuppack   (501) staff       (20)    10432 2024-05-17 23:15:50.000000 xplainable-client-1.2.4.post4/xplainable_client/client/utils/scanner.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.509593 xplainable-client-1.2.4.post4/xplainable_client/models/
+-rw-r--r--   0 jtuppack   (501) staff       (20)     4057 2024-03-04 22:40:48.000000 xplainable-client-1.2.4.post4/xplainable_client/models/ebm.py
+drwxr-xr-x   0 jtuppack   (501) staff       (20)        0 2024-05-18 05:53:57.506358 xplainable-client-1.2.4.post4/xplainable_client.egg-info/
+-rw-r--r--   0 jtuppack   (501) staff       (20)    44077 2024-05-18 05:53:57.000000 xplainable-client-1.2.4.post4/xplainable_client.egg-info/PKG-INFO
+-rw-r--r--   0 jtuppack   (501) staff       (20)     1030 2024-05-18 05:53:57.000000 xplainable-client-1.2.4.post4/xplainable_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)        1 2024-05-18 05:53:57.000000 xplainable-client-1.2.4.post4/xplainable_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)      149 2024-05-18 05:53:57.000000 xplainable-client-1.2.4.post4/xplainable_client.egg-info/requires.txt
+-rw-r--r--   0 jtuppack   (501) staff       (20)       18 2024-05-18 05:53:57.000000 xplainable-client-1.2.4.post4/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.4.post3/LICENSE` & `xplainable-client-1.2.4.post4/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
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
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
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
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
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
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
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
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `xplainable_client-1.2.4.post3/PKG-INFO` & `xplainable-client-1.2.4.post4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,804 +1,794 @@
-Metadata-Version: 2.1
-Name: xplainable-client
-Version: 1.2.4.post3
-Summary: The client for persisting and deploying models to Xplainable cloud.
-Author: xplainable pty ltd
-Author-email: xplainable pty ltd <contact@xplainable.io>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.26
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn
-Requires-Dist: setuptools
-Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.4
-
-
-<div align="center">
-<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
-<h1 align="center">xplainable</h1>
-<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
-    
-**Xplainable** makes tabular machine learning transparent, fair, and actionable.
-</div>
-
-## Why Was Xplainable Created?
-In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
-
-To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
-
-
-## Xplainable Cloud
-This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
-
-### Preprocessing with Xplainable Cloud
-Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
-
-
-```python
-import xplainable as xp
-import os
-from xplainable_client import Client
-
-#Initialising the client
-XClient = Client(api_key=os.environ['XP_API_KEY'])
-
-#Creating a Preprocessor ID
-preprocessor_id = XClient.create_preprocessor_id(
-    preprocessor_name="Preprocessor Name",
-    preprocessor_description="Preprocessor Description",
-)
-
-#Creating a Preprocessor Version
-preprocessor_version = XClient.create_preprocessor_version(
-    preprocessor_id, #preprocessor_id,
-    pipeline, # <-- Pass the pipeline
-    df # <-- Pass the raw dataframe
-)
-
-#Loading the Preprocessor Client
-pp_cloud = XClient.load_preprocessor(
-    preprocessor_id,
-    preprocessor_version["version_id"],
-    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
-    )
-```
-
-### Modelling with Xplainable Cloud
-
-After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
-
-```python
-
-#Creating a Model Id
-model_id = XClient.create_model_id(
-    model,
-    model_name="Model Name",
-    model_description='Model Description'
-)
-
-#Creating a Model Version
-version_id = XClient.create_model_version(
-    model,
-    model_id,
-    X_train,
-    y_train
-)
-
-```
-
-### Deployments with Xplainable Cloud
-Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
-
-```python 
-#Creating a Model Deployment
-deployment = XClient.deploy(
-    hostname="https://inference.xplainable.io", 
-    model_id=model_id, 
-    version_id=version_id 
-)
-
-#Activating the Deployment
-XClient.activate_deployment(deployment['deployment_id'])
-
-#Generating an API Key
-deploy_key = XClient.generate_deploy_key(
-    'API Key Name', 
-    deployment['deployment_id'], 
-    7 #-> Days until expiration
-    )
-
-#Hitting the endpoint
-response = requests.post(
-    url="https://inference.xplainable.io/v1/predict",
-    headers={'api_key': deploy_key['deploy_key']},
-    json=body
-)
-
-#Obtaining the value response
-value = response.json()
-```
-
-<div align="center">
-<br></br>
-<br></br>
-Thanks for trying xplainable!
-<br></br>
-<strong>Made with ❤️ in Australia</strong>
-<br></br>
-<hr>
-&copy; copyright xplainable pty ltd
-</div>
-
-
+Metadata-Version: 2.1
+Name: xplainable-client
+Version: 1.2.4.post4
+Summary: The client for persisting and deploying models to Xplainable cloud.
+Home-page: UNKNOWN
+Author: xplainable pty ltd
+Author-email: contact@xplainable.io
+License:                     GNU AFFERO GENERAL PUBLIC LICENSE
+                               Version 3, 19 November 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU Affero General Public License is a free, copyleft license for
+        software and other kinds of works, specifically designed to ensure
+        cooperation with the community in the case of network server software.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        our General Public Licenses are intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          Developers that use our General Public Licenses protect your rights
+        with two steps: (1) assert copyright on the software, and (2) offer
+        you this License which gives you legal permission to copy, distribute
+        and/or modify the software.
+        
+          A secondary benefit of defending all users' freedom is that
+        improvements made in alternate versions of the program, if they
+        receive widespread use, become available for other developers to
+        incorporate.  Many developers of free software are heartened and
+        encouraged by the resulting cooperation.  However, in the case of
+        software used on network servers, this result may fail to come about.
+        The GNU General Public License permits making a modified version and
+        letting the public access it on a server without ever releasing its
+        source code to the public.
+        
+          The GNU Affero General Public License is designed specifically to
+        ensure that, in such cases, the modified source code becomes available
+        to the community.  It requires the operator of a network server to
+        provide the source code of the modified version running there to the
+        users of that server.  Therefore, public use of a modified version, on
+        a publicly accessible server, gives the public access to the source
+        code of the modified version.
+        
+          An older license, called the Affero General Public License and
+        published by Affero, was designed to accomplish similar goals.  This is
+        a different license, not a version of the Affero GPL, but Affero has
+        released a new version of the Affero GPL which permits relicensing under
+        this license.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU Affero General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Remote Network Interaction; Use with the GNU General Public License.
+        
+          Notwithstanding any other provision of this License, if you modify the
+        Program, your modified version must prominently offer all users
+        interacting with it remotely through a computer network (if your version
+        supports such interaction) an opportunity to receive the Corresponding
+        Source of your version by providing access to the Corresponding Source
+        from a network server at no charge, through some standard or customary
+        means of facilitating copying of software.  This Corresponding Source
+        shall include the Corresponding Source for any work covered by version 3
+        of the GNU General Public License that is incorporated pursuant to the
+        following paragraph.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the work with which it is combined will remain governed by version
+        3 of the GNU General Public License.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU Affero General Public License from time to time.  Such new versions
+        will be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU Affero General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU Affero General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU Affero General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU Affero General Public License for more details.
+        
+            You should have received a copy of the GNU Affero General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If your software can interact with users remotely through a computer
+        network, you should also make sure that it provides a way for users to
+        get its source.  For example, if your program is a web application, its
+        interface could display a "Source" link that leads users to an archive
+        of the code.  There are many ways you could offer source, and different
+        solutions will be better for different programs; see section 13 for the
+        specific requirements.
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU AGPL, see
+        <https://www.gnu.org/licenses/>.
+        
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<div align="center">
+<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
+<h1 align="center">xplainable</h1>
+<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
+    
+**Xplainable** makes tabular machine learning transparent, fair, and actionable.
+</div>
+
+## Why Was Xplainable Created?
+In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
+
+To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
+
+
+## Xplainable Cloud
+This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
+
+### Preprocessing with Xplainable Cloud
+Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
+
+
+```python
+import xplainable as xp
+import os
+from xplainable_client import Client
+
+#Initialising the client
+XClient = Client(api_key=os.environ['XP_API_KEY'])
+
+#Creating a Preprocessor ID
+preprocessor_id = XClient.create_preprocessor_id(
+    preprocessor_name="Preprocessor Name",
+    preprocessor_description="Preprocessor Description",
+)
+
+#Creating a Preprocessor Version
+preprocessor_version = XClient.create_preprocessor_version(
+    preprocessor_id, #preprocessor_id,
+    pipeline, # <-- Pass the pipeline
+    df # <-- Pass the raw dataframe
+)
+
+#Loading the Preprocessor Client
+pp_cloud = XClient.load_preprocessor(
+    preprocessor_id,
+    preprocessor_version["version_id"],
+    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
+    )
+```
+
+### Modelling with Xplainable Cloud
+
+After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
+
+```python
+
+#Creating a Model Id
+model_id = XClient.create_model_id(
+    model,
+    model_name="Model Name",
+    model_description='Model Description'
+)
+
+#Creating a Model Version
+version_id = XClient.create_model_version(
+    model,
+    model_id,
+    X_train,
+    y_train
+)
+
+```
+
+### Deployments with Xplainable Cloud
+Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
+
+```python 
+#Creating a Model Deployment
+deployment = XClient.deploy(
+    hostname="https://inference.xplainable.io", 
+    model_id=model_id, 
+    version_id=version_id 
+)
+
+#Activating the Deployment
+XClient.activate_deployment(deployment['deployment_id'])
+
+#Generating an API Key
+deploy_key = XClient.generate_deploy_key(
+    'API Key Name', 
+    deployment['deployment_id'], 
+    7 #-> Days until expiration
+    )
+
+#Hitting the endpoint
+response = requests.post(
+    url="https://inference.xplainable.io/v1/predict",
+    headers={'api_key': deploy_key['deploy_key']},
+    json=body
+)
+
+#Obtaining the value response
+value = response.json()
+```
+
+<div align="center">
+<br></br>
+<br></br>
+Thanks for trying xplainable!
+<br></br>
+<strong>Made with ❤️ in Australia</strong>
+<br></br>
+<hr>
+&copy; copyright xplainable pty ltd
+</div>
+
+
+
+
```

### Comparing `xplainable_client-1.2.4.post3/README.md` & `xplainable-client-1.2.4.post4/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-
-<div align="center">
-<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
-<h1 align="center">xplainable</h1>
-<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
-    
-**Xplainable** makes tabular machine learning transparent, fair, and actionable.
-</div>
-
-## Why Was Xplainable Created?
-In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
-
-To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
-
-
-## Xplainable Cloud
-This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
-
-### Preprocessing with Xplainable Cloud
-Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
-
-
-```python
-import xplainable as xp
-import os
-from xplainable_client import Client
-
-#Initialising the client
-XClient = Client(api_key=os.environ['XP_API_KEY'])
-
-#Creating a Preprocessor ID
-preprocessor_id = XClient.create_preprocessor_id(
-    preprocessor_name="Preprocessor Name",
-    preprocessor_description="Preprocessor Description",
-)
-
-#Creating a Preprocessor Version
-preprocessor_version = XClient.create_preprocessor_version(
-    preprocessor_id, #preprocessor_id,
-    pipeline, # <-- Pass the pipeline
-    df # <-- Pass the raw dataframe
-)
-
-#Loading the Preprocessor Client
-pp_cloud = XClient.load_preprocessor(
-    preprocessor_id,
-    preprocessor_version["version_id"],
-    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
-    )
-```
-
-### Modelling with Xplainable Cloud
-
-After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
-
-```python
-
-#Creating a Model Id
-model_id = XClient.create_model_id(
-    model,
-    model_name="Model Name",
-    model_description='Model Description'
-)
-
-#Creating a Model Version
-version_id = XClient.create_model_version(
-    model,
-    model_id,
-    X_train,
-    y_train
-)
-
-```
-
-### Deployments with Xplainable Cloud
-Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
-
-```python 
-#Creating a Model Deployment
-deployment = XClient.deploy(
-    hostname="https://inference.xplainable.io", 
-    model_id=model_id, 
-    version_id=version_id 
-)
-
-#Activating the Deployment
-XClient.activate_deployment(deployment['deployment_id'])
-
-#Generating an API Key
-deploy_key = XClient.generate_deploy_key(
-    'API Key Name', 
-    deployment['deployment_id'], 
-    7 #-> Days until expiration
-    )
-
-#Hitting the endpoint
-response = requests.post(
-    url="https://inference.xplainable.io/v1/predict",
-    headers={'api_key': deploy_key['deploy_key']},
-    json=body
-)
-
-#Obtaining the value response
-value = response.json()
-```
-
-<div align="center">
-<br></br>
-<br></br>
-Thanks for trying xplainable!
-<br></br>
-<strong>Made with ❤️ in Australia</strong>
-<br></br>
-<hr>
-&copy; copyright xplainable pty ltd
-</div>
-
-
+
+<div align="center">
+<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
+<h1 align="center">xplainable</h1>
+<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
+    
+**Xplainable** makes tabular machine learning transparent, fair, and actionable.
+</div>
+
+## Why Was Xplainable Created?
+In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
+
+To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
+
+
+## Xplainable Cloud
+This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
+
+### Preprocessing with Xplainable Cloud
+Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
+
+
+```python
+import xplainable as xp
+import os
+from xplainable_client import Client
+
+#Initialising the client
+XClient = Client(api_key=os.environ['XP_API_KEY'])
+
+#Creating a Preprocessor ID
+preprocessor_id = XClient.create_preprocessor_id(
+    preprocessor_name="Preprocessor Name",
+    preprocessor_description="Preprocessor Description",
+)
+
+#Creating a Preprocessor Version
+preprocessor_version = XClient.create_preprocessor_version(
+    preprocessor_id, #preprocessor_id,
+    pipeline, # <-- Pass the pipeline
+    df # <-- Pass the raw dataframe
+)
+
+#Loading the Preprocessor Client
+pp_cloud = XClient.load_preprocessor(
+    preprocessor_id,
+    preprocessor_version["version_id"],
+    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
+    )
+```
+
+### Modelling with Xplainable Cloud
+
+After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
+
+```python
+
+#Creating a Model Id
+model_id = XClient.create_model_id(
+    model,
+    model_name="Model Name",
+    model_description='Model Description'
+)
+
+#Creating a Model Version
+version_id = XClient.create_model_version(
+    model,
+    model_id,
+    X_train,
+    y_train
+)
+
+```
+
+### Deployments with Xplainable Cloud
+Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
+
+```python 
+#Creating a Model Deployment
+deployment = XClient.deploy(
+    hostname="https://inference.xplainable.io", 
+    model_id=model_id, 
+    version_id=version_id 
+)
+
+#Activating the Deployment
+XClient.activate_deployment(deployment['deployment_id'])
+
+#Generating an API Key
+deploy_key = XClient.generate_deploy_key(
+    'API Key Name', 
+    deployment['deployment_id'], 
+    7 #-> Days until expiration
+    )
+
+#Hitting the endpoint
+response = requests.post(
+    url="https://inference.xplainable.io/v1/predict",
+    headers={'api_key': deploy_key['deploy_key']},
+    json=body
+)
+
+#Obtaining the value response
+value = response.json()
+```
+
+<div align="center">
+<br></br>
+<br></br>
+Thanks for trying xplainable!
+<br></br>
+<strong>Made with ❤️ in Australia</strong>
+<br></br>
+<hr>
+&copy; copyright xplainable pty ltd
+</div>
+
+
```

### Comparing `xplainable_client-1.2.4.post3/pyproject.toml` & `xplainable-client-1.2.4.post4/pyproject.toml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = ["setuptools>=61.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools.packages]
-find = {} 
-
-[project]
-name = "xplainable-client"
-version = "1.2.4.post3"
-authors = [
-  { name="xplainable pty ltd", email="contact@xplainable.io" },
-]
-description = "The client for persisting and deploying models to Xplainable cloud."
-readme = "README.md"
-license = { file="LICENSE" }
-requires-python = ">=3.8"
-
-classifiers = [
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Operating System :: OS Independent"
-]
-
-dependencies = [
-"ipywidgets==8.0.6",
-"numpy>=1.26",
-"pandas>=1.5.2",
-"pyperclip==1.8.2",
-"Requests==2.31.0",
-"scikit_learn",
-"setuptools",
-"urllib3==2.2.0",
-"xplainable==1.2.4"
-]
+[build-system]
+requires = ["setuptools>=61.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages]
+find = {} 
+
+[project]
+name = "xplainable-client"
+version = "1.2.4.post3"
+authors = [
+  { name="xplainable pty ltd", email="contact@xplainable.io" },
+]
+description = "The client for persisting and deploying models to Xplainable cloud."
+readme = "README.md"
+license = { file="LICENSE" }
+requires-python = ">=3.8"
+
+classifiers = [
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent"
+]
+
+dependencies = [
+"ipywidgets==8.0.6",
+"numpy>=1.26",
+"pandas>=1.5.2",
+"pyperclip==1.8.2",
+"Requests==2.31.0",
+"scikit_learn",
+"setuptools",
+"urllib3==2.2.0",
+"xplainable==1.2.4"
+]
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/__init__.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ._models import *
-from ._misc import *
-from ._session import Session
-from ._misc import Misc
-from ._models import Models
-from ._preprocessing import Preprocessing
-from ._deployments import Deployments
-from ._gpt import GPT
-from ._collections import Collections
-from ._datasets import Datasets
-from ._inference import Inference
-
-
-class Client(Misc, Models, Preprocessing, GPT, Collections, Datasets, Inference, Deployments):
-
-    def __init__(self, api_key=None, hostname='https://api.xplainable.io'):
-        self.session = Session(api_key=api_key, hostname=hostname)
-        Misc.__init__(self, self.session)
-        Models.__init__(self, self.session)
-        Preprocessing.__init__(self, self.session)
-        Deployments.__init__(self, self.session)
-        GPT.__init__(self, self.session)
-        Collections.__init__(self, self.session)
-        Datasets.__init__(self, self.session)
-        Inference.__init__(self, self.session)
-
-
-
-
+from ._models import *
+from ._misc import *
+from ._session import Session
+from ._misc import Misc
+from ._models import Models
+from ._preprocessing import Preprocessing
+from ._deployments import Deployments
+from ._gpt import GPT
+from ._collections import Collections
+from ._datasets import Datasets
+from ._inference import Inference
+
+
+class Client(Misc, Models, Preprocessing, GPT, Collections, Datasets, Inference, Deployments):
+
+    def __init__(self, api_key=None, hostname='https://api.xplainable.io'):
+        self.session = Session(api_key=api_key, hostname=hostname)
+        Misc.__init__(self, self.session)
+        Models.__init__(self, self.session)
+        Preprocessing.__init__(self, self.session)
+        Deployments.__init__(self, self.session)
+        GPT.__init__(self, self.session)
+        Collections.__init__(self, self.session)
+        Datasets.__init__(self, self.session)
+        Inference.__init__(self, self.session)
+
+
+
+
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_datasets.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_datasets.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from ._client_cog_base import *
-
-import requests
-import pandas as pd
-
-
-class Datasets(Client_Cog):
-
-    # upload_dataset
-
-    def list_datasets(self):
-
-        response = requests.get('https://api.xplainable.io/v1/public-datasets')
-        
-        if response.status_code != 200:
-            raise ValueError(f'Unable to list datasets. Check your connection and try again.')
-        
-        return response.json()
-
-    def _get_url_path(self, name):
-        _base = 'xplainablepublic'
-        _type = 'blob.core.windows.net'
-        _loc = 'asset-repository/datasets'
-
-        return f'https://{_base}.{_type}/{_loc}/{name}/data.csv'
-
-    def load_dataset(self, name):
-
-        datasets = self.list_datasets()
-
-        if name not in datasets:
-            raise ValueError(f'{name} is not available. Run xp.list_datasets() to see available datasets.')
-        
-        try:
-            url = self._get_url_path(name)
-            df = pd.read_csv(url)
-
-            return df
-        
-        except Exception as e:
-            raise ValueError(f'Unable to load dataset {name}. Check your connection and try again.')
-        
-    # update_dataset
-
-    # detele_dataset
-
-    # list_dataset_children
-
-    # preview_dataset
-
+from ._client_cog_base import *
+
+import requests
+import pandas as pd
+
+
+class Datasets(Client_Cog):
+
+    # upload_dataset
+
+    def list_datasets(self):
+
+        response = requests.get('https://api.xplainable.io/v1/public-datasets')
+        
+        if response.status_code != 200:
+            raise ValueError(f'Unable to list datasets. Check your connection and try again.')
+        
+        return response.json()
+
+    def _get_url_path(self, name):
+        _base = 'xplainablepublic'
+        _type = 'blob.core.windows.net'
+        _loc = 'asset-repository/datasets'
+
+        return f'https://{_base}.{_type}/{_loc}/{name}/data.csv'
+
+    def load_dataset(self, name):
+
+        datasets = self.list_datasets()
+
+        if name not in datasets:
+            raise ValueError(f'{name} is not available. Run xp.list_datasets() to see available datasets.')
+        
+        try:
+            url = self._get_url_path(name)
+            df = pd.read_csv(url)
+
+            return df
+        
+        except Exception as e:
+            raise ValueError(f'Unable to load dataset {name}. Check your connection and try again.')
+        
+    # update_dataset
+
+    # detele_dataset
+
+    # list_dataset_children
+
+    # preview_dataset
+
     # list_pub_datasets
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_deployments.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_deployments.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,388 +1,388 @@
-import inspect
-from ._client_cog_base import *
-
-
-class Deployments(Client_Cog):
-
-
-    def deploy(
-            self, model_id: str, version_id: str,
-            hostname: str='https://inference.xplainable.io',
-            location: str='syd', raw_output: bool=True) -> dict:
-        """ Deploys a model partition to xplainable cloud.
-        The hostname should be the url of the inference server. For example:
-        https://inference.xplainable.io
-        Args:
-            hostname (str): The host name for the inference server
-            model_id (int): The model id
-            version_id (int): The version id
-            partition_id (int): The partition id
-            raw_output (bool, optional): returns a dictionary
-        Returns:
-            dict: deployment status and details.
-        """
-
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
-            f'{version_id}/deploy'
-        )
-        body = {
-            "location": location
-        }
-        response = self.session._session.put(url, json=body)
-
-        if response.status_code == 200:
-            deployment_id = response.json()['deployment_id']
-            data = {
-                "deployment_id": deployment_id,
-                "status": "inactive",
-                "location": location,
-                "endpoint": f"{hostname}/v1/predict"
-            }
-            return data
-        else:
-            return {
-                "message": f"Failed with status code {response.status_code}"}
-
-    def list_deployments(self):
-        """ Lists all deployments of the active user's team.
-        Returns:
-            dict: Dictionary of deployments.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/deployments'
-            )
-        deployments = self.session.get_response_content(response)
-        return deployments
-    
-    
-    def generate_deploy_key(
-            self, description: str, deployment_id: str,
-            days_until_expiry: float = 90
-            ) -> None:
-        """ Generates a deploy key for a model deployment.
-        Args:
-            description (str): Description of the deploy key use case.
-            deployment_id (str): The deployment id.
-            days_until_expiry (float): The number of days until the key expires.
-        Returns:
-            str: The deploy key.
-        """
-        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/create-deploy-key'
-
-        params = {
-            'description': description,
-            'days_until_expiry': days_until_expiry
-        }
-
-        response = self.session._session.put(
-            url=url,
-            json=params
-            )
-        deploy_key = response.json()
-        if deploy_key:
-            return deploy_key
-        else:
-            raise ConnectionError(
-                f"Falied to generate deploy key. Code: {response.status_code}")
-        
-    def list_deploy_keys(self, deployment_id: str):
-        """ Lists all deploy keys for a deployment.
-        Args:
-            deployment_id (str): The deployment id.
-        Returns:
-            dict: Dictionary of deploy keys.
-        """
-        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys'
-        response = self.session._session.get(url)
-        deploy_keys = self.session.get_response_content(response)
-        return deploy_keys
-
-    def list_active_team_deploy_keys(self, team_id: str):
-        """ Lists all active team deploy keys.
-        Args:
-            team_id (str): The team id.
-        Returns:
-            dict: Dictionary of deploy keys.
-        """
-        url = f'{self.session.hostname}/deployments/active-team-deploy-keys/{team_id}'
-        response = self.session._session.get(url)
-        deploy_keys = self.session.get_response_content(response)
-        return deploy_keys
-
-    def revoke_deploy_key(self, deployment_id: str, deploy_key_id: str):
-        """ Revokes a deploy key for a deployment.
-        Args:
-            deployment_id (str): The deployment id.
-            deploy_key_id (str): The deploy key id.
-        Returns:
-            dict: Dictionary of deploy keys.
-        """
-        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-deploy-key/{deploy_key_id}'
-        response = self.session._session.patch(url)
-        return response.json()
-
-    def delete_deployment(self, deployment_id: str):
-        """ Deletes a model deployment.
-        Args:
-            deployment_id (str): The deployment id
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}'
-        )
-        response = self.session._session.delete(url)
-        return response.json()
-    
-
-    def add_allowed_ip_address(self, deployment_id: str):
-        """ Add allowed ip address to a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            json: The json response if the ip is added.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-allowed-ip'
-
-        )
-        response = self.session._session.put(url)
-        return response.json()
-
-    def list_allowed_ip_addresses(self, deployment_id: str):
-        """ List allowed ip addresses for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            json: The json response of the allowed ip addresses.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall'
-        )
-        response = self.session._session.get(url)
-        firewall = self.session.get_response_content(response)
-        return firewall['allowed_ips']
-
-    def list_allowed_ip_address_and_description(self, deployment_id: str):
-        """ List allowed ip addresses and their descriptions for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            json: The json response of the allowed ip addresses and descriptions.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall-descriptions'
-        )
-        response = self.session._session.get(url)
-        firewall = self.session.get_response_content(response)
-        return firewall
-
-    def delete_allowed_ip_address(self, deployment_id: str, ip_id: str):
-        """ Delete an allowed ip address from a deployment.
-        Args:
-            deployment_id (str): The deployment id
-            ip_id (str): The ip id
-        Return:
-            json: The json response if the ip is deleted.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/ips/{ip_id}'
-        )
-        response = self.session._session.delete(url)
-        message = self.session.get_response_content(response)
-        return message.get('message')
-
-    def activate_deployment(self, deployment_id):
-        """ Activates a model deployment.
-        Args:
-            deployment_id (str): The deployment id
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate'
-        )
-        response = self.session._session.patch(url)
-        if response.status_code == 200:
-            return response.json()
-        else:
-            return {
-                "message": f"Failed with status code {response.status_code}"}
-
-
-    def deactivate_deployment(self, deployment_id):
-        """ Deactivates a model deployment.
-        Args:
-            deployment_id (str): The deployment id
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate'
-        )
-        response = self.session._session.patch(url)
-        if response.status_code == 200:
-            return response.json()
-        else:
-            return {
-                "message": f"Failed with status code {response.status_code}"}
-        
-    def enable_explain(self, deployment_id: str):
-        """ Enables explain for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            str: The message if explain is enabled.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/enable-explain'
-        )
-        response = self.session._session.patch(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"Explain for this deployment could not be enabled. Status code: ", response.status_code}
-
-        
-    def disable_explain(self, deployment_id: str):
-        """ Disables explain for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            str: The message if explain is disabled.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/disable-explain'
-        )
-        response = self.session._session.patch(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"Explain for this deployment could not be disabled. Status code: ", response.status_code}
-
-    def activate_deployment_ip_blocking(self, deployment_id: str):
-        """ Activates ip blocking for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            str: The message if ip blocking is activated.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate-deployment-ip-blocking'
-        )
-        response = self.session._session.patch(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"Ip blocking for this deployment could not be activated. Status code: ", response.status_code}
-
-    def deactivate_deployment_ip_blocking(self, deployment_id: str):
-        """ Deactivates ip blocking for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            str: The message if ip blocking is deactivated.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate-deployment-ip-blocking'
-        )
-        response = self.session._session.patch(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"Ip blocking for this deployment could not be deactivated. Status code: ", response.status_code}
-
-    def revoke_all_deploy_keys(self, deployment_id: str):
-        """ Revokes all deploy keys for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        Return:
-            str: The message if all deploy keys are revoked.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-all-user-deploy-keys'
-        )
-        response = self.session._session.patch(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"All deploy keys for this deployment could not be revoked. Status code: ", response.status_code}
-
-    def delete_deploy_key(self, deployment_id: str, key_id: str):
-        """ Deletes a deploy key for a deployment.
-        Args:
-            deployment_id (str): The deployment id
-            key_id (str): The key id
-        Return:
-            str: The message if the key is deleted.
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys/{key_id}'
-        )
-        response = self.session._session.delete(url)
-        try:
-            message = self.session.get_response_content(response)
-            return message.get('message')
-        except:
-            return {"Deploy key could not be deleted. Status code: ", response.status_code}
-
-
-    def generate_example_deployment_payload(self, deployment_id):
-        """ Generates an example deployment payload for a deployment.
-        Args:
-            deployment_id (str): The deployment id.
-        """
-        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/payload'
-        response = self.session._session.get(url)
-        return response.json()
-    
-
-    def add_deployment_middleware(
-        self, deployment_id, func, name, description=None):
-        """ Adds or replaces a middleware function to a deployment.
-        Args:
-            deployment_id (str): The deployment id
-            func (function): The middleware function
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-middleware'
-        )
-        # Convert function to expected name
-        if func.__name__ != 'middleware':
-            func = self.__parse_function(func)
-            source_code = func.source
-
-        else:
-            source_code = inspect.getsource(func)
-        body = {
-            "code_block": source_code,
-            "name": name,
-            "description": description
-        }
-        response = self.session._session.put(
-            url=url,
-            json=body
-            )
-        return response.json()
-    
-    def get_middleware(self, deployment_id):
-        """ Gets the middleware function from a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
-        )
-        response = self.session._session.get(url)
-        return self.session.get_response_content(response)
-
-    def delete_deployment_middleware(self, deployment_id):
-        """ Deletes a middleware function from a deployment.
-        Args:
-            deployment_id (str): The deployment id
-        """
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
-        )
-        response = self.session._session.delete(url)
-        return {"status_code": response.status_code}
+import inspect
+from ._client_cog_base import *
+
+
+class Deployments(Client_Cog):
+
+
+    def deploy(
+            self, model_id: str, version_id: str,
+            hostname: str='https://inference.xplainable.io',
+            location: str='syd', raw_output: bool=True) -> dict:
+        """ Deploys a model partition to xplainable cloud.
+        The hostname should be the url of the inference server. For example:
+        https://inference.xplainable.io
+        Args:
+            hostname (str): The host name for the inference server
+            model_id (int): The model id
+            version_id (int): The version id
+            partition_id (int): The partition id
+            raw_output (bool, optional): returns a dictionary
+        Returns:
+            dict: deployment status and details.
+        """
+
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
+            f'{version_id}/deploy'
+        )
+        body = {
+            "location": location
+        }
+        response = self.session._session.put(url, json=body)
+
+        if response.status_code == 200:
+            deployment_id = response.json()['deployment_id']
+            data = {
+                "deployment_id": deployment_id,
+                "status": "inactive",
+                "location": location,
+                "endpoint": f"{hostname}/v1/predict"
+            }
+            return data
+        else:
+            return {
+                "message": f"Failed with status code {response.status_code}"}
+
+    def list_deployments(self):
+        """ Lists all deployments of the active user's team.
+        Returns:
+            dict: Dictionary of deployments.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/deployments'
+            )
+        deployments = self.session.get_response_content(response)
+        return deployments
+    
+    
+    def generate_deploy_key(
+            self, description: str, deployment_id: str,
+            days_until_expiry: float = 90
+            ) -> None:
+        """ Generates a deploy key for a model deployment.
+        Args:
+            description (str): Description of the deploy key use case.
+            deployment_id (str): The deployment id.
+            days_until_expiry (float): The number of days until the key expires.
+        Returns:
+            str: The deploy key.
+        """
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/create-deploy-key'
+
+        params = {
+            'description': description,
+            'days_until_expiry': days_until_expiry
+        }
+
+        response = self.session._session.put(
+            url=url,
+            json=params
+            )
+        deploy_key = response.json()
+        if deploy_key:
+            return deploy_key
+        else:
+            raise ConnectionError(
+                f"Falied to generate deploy key. Code: {response.status_code}")
+        
+    def list_deploy_keys(self, deployment_id: str):
+        """ Lists all deploy keys for a deployment.
+        Args:
+            deployment_id (str): The deployment id.
+        Returns:
+            dict: Dictionary of deploy keys.
+        """
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys'
+        response = self.session._session.get(url)
+        deploy_keys = self.session.get_response_content(response)
+        return deploy_keys
+
+    def list_active_team_deploy_keys(self, team_id: str):
+        """ Lists all active team deploy keys.
+        Args:
+            team_id (str): The team id.
+        Returns:
+            dict: Dictionary of deploy keys.
+        """
+        url = f'{self.session.hostname}/deployments/active-team-deploy-keys/{team_id}'
+        response = self.session._session.get(url)
+        deploy_keys = self.session.get_response_content(response)
+        return deploy_keys
+
+    def revoke_deploy_key(self, deployment_id: str, deploy_key_id: str):
+        """ Revokes a deploy key for a deployment.
+        Args:
+            deployment_id (str): The deployment id.
+            deploy_key_id (str): The deploy key id.
+        Returns:
+            dict: Dictionary of deploy keys.
+        """
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-deploy-key/{deploy_key_id}'
+        response = self.session._session.patch(url)
+        return response.json()
+
+    def delete_deployment(self, deployment_id: str):
+        """ Deletes a model deployment.
+        Args:
+            deployment_id (str): The deployment id
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}'
+        )
+        response = self.session._session.delete(url)
+        return response.json()
+    
+
+    def add_allowed_ip_address(self, deployment_id: str):
+        """ Add allowed ip address to a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            json: The json response if the ip is added.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-allowed-ip'
+
+        )
+        response = self.session._session.put(url)
+        return response.json()
+
+    def list_allowed_ip_addresses(self, deployment_id: str):
+        """ List allowed ip addresses for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            json: The json response of the allowed ip addresses.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall'
+        )
+        response = self.session._session.get(url)
+        firewall = self.session.get_response_content(response)
+        return firewall['allowed_ips']
+
+    def list_allowed_ip_address_and_description(self, deployment_id: str):
+        """ List allowed ip addresses and their descriptions for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            json: The json response of the allowed ip addresses and descriptions.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/get-firewall-descriptions'
+        )
+        response = self.session._session.get(url)
+        firewall = self.session.get_response_content(response)
+        return firewall
+
+    def delete_allowed_ip_address(self, deployment_id: str, ip_id: str):
+        """ Delete an allowed ip address from a deployment.
+        Args:
+            deployment_id (str): The deployment id
+            ip_id (str): The ip id
+        Return:
+            json: The json response if the ip is deleted.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/ips/{ip_id}'
+        )
+        response = self.session._session.delete(url)
+        message = self.session.get_response_content(response)
+        return message.get('message')
+
+    def activate_deployment(self, deployment_id):
+        """ Activates a model deployment.
+        Args:
+            deployment_id (str): The deployment id
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate'
+        )
+        response = self.session._session.patch(url)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            return {
+                "message": f"Failed with status code {response.status_code}"}
+
+
+    def deactivate_deployment(self, deployment_id):
+        """ Deactivates a model deployment.
+        Args:
+            deployment_id (str): The deployment id
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate'
+        )
+        response = self.session._session.patch(url)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            return {
+                "message": f"Failed with status code {response.status_code}"}
+        
+    def enable_explain(self, deployment_id: str):
+        """ Enables explain for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            str: The message if explain is enabled.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/enable-explain'
+        )
+        response = self.session._session.patch(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"Explain for this deployment could not be enabled. Status code: ", response.status_code}
+
+        
+    def disable_explain(self, deployment_id: str):
+        """ Disables explain for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            str: The message if explain is disabled.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/disable-explain'
+        )
+        response = self.session._session.patch(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"Explain for this deployment could not be disabled. Status code: ", response.status_code}
+
+    def activate_deployment_ip_blocking(self, deployment_id: str):
+        """ Activates ip blocking for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            str: The message if ip blocking is activated.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/activate-deployment-ip-blocking'
+        )
+        response = self.session._session.patch(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"Ip blocking for this deployment could not be activated. Status code: ", response.status_code}
+
+    def deactivate_deployment_ip_blocking(self, deployment_id: str):
+        """ Deactivates ip blocking for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            str: The message if ip blocking is deactivated.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deactivate-deployment-ip-blocking'
+        )
+        response = self.session._session.patch(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"Ip blocking for this deployment could not be deactivated. Status code: ", response.status_code}
+
+    def revoke_all_deploy_keys(self, deployment_id: str):
+        """ Revokes all deploy keys for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        Return:
+            str: The message if all deploy keys are revoked.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/revoke-all-user-deploy-keys'
+        )
+        response = self.session._session.patch(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"All deploy keys for this deployment could not be revoked. Status code: ", response.status_code}
+
+    def delete_deploy_key(self, deployment_id: str, key_id: str):
+        """ Deletes a deploy key for a deployment.
+        Args:
+            deployment_id (str): The deployment id
+            key_id (str): The key id
+        Return:
+            str: The message if the key is deleted.
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/deploy-keys/{key_id}'
+        )
+        response = self.session._session.delete(url)
+        try:
+            message = self.session.get_response_content(response)
+            return message.get('message')
+        except:
+            return {"Deploy key could not be deleted. Status code: ", response.status_code}
+
+
+    def generate_example_deployment_payload(self, deployment_id):
+        """ Generates an example deployment payload for a deployment.
+        Args:
+            deployment_id (str): The deployment id.
+        """
+        url = f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/payload'
+        response = self.session._session.get(url)
+        return response.json()
+    
+
+    def add_deployment_middleware(
+        self, deployment_id, func, name, description=None):
+        """ Adds or replaces a middleware function to a deployment.
+        Args:
+            deployment_id (str): The deployment id
+            func (function): The middleware function
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/add-middleware'
+        )
+        # Convert function to expected name
+        if func.__name__ != 'middleware':
+            func = self.__parse_function(func)
+            source_code = func.source
+
+        else:
+            source_code = inspect.getsource(func)
+        body = {
+            "code_block": source_code,
+            "name": name,
+            "description": description
+        }
+        response = self.session._session.put(
+            url=url,
+            json=body
+            )
+        return response.json()
+    
+    def get_middleware(self, deployment_id):
+        """ Gets the middleware function from a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
+        )
+        response = self.session._session.get(url)
+        return self.session.get_response_content(response)
+
+    def delete_deployment_middleware(self, deployment_id):
+        """ Deletes a middleware function from a deployment.
+        Args:
+            deployment_id (str): The deployment id
+        """
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/deployments/{deployment_id}/middleware'
+        )
+        response = self.session._session.delete(url)
+        return {"status_code": response.status_code}
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_gpt.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_gpt.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from ._client_cog_base import *
-
-class GPT(Client_Cog):
-
-    def _gpt_report(
-            self, model_id, version_id, target_description='',
-            project_objective='', max_features=15, temperature=0.5):
-        """ Generates a report using Open-AI GPT.
-        Args:
-            model_id (int): The model id
-            version_id (int): The version id
-            target_description (str): The target description
-            project_objective (str): The project objective
-            max_features (int): The maximum number of features
-            temperature (float): The temperature
-        Return:
-            dict: The report
-        """
-
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
-            f'{version_id}/generate-report'
-        )
-        params = {
-            'target_description': target_description,
-            'project_objective': project_objective,
-            'max_features': max_features,
-            'temperature': temperature
-        }
-        response = self.session._session.put(
-            url=url,
-            json=params,
-            )
-
-        content = self.session.get_response_content(response)
-        return content
+from ._client_cog_base import *
+
+class GPT(Client_Cog):
+
+    def _gpt_report(
+            self, model_id, version_id, target_description='',
+            project_objective='', max_features=15, temperature=0.5):
+        """ Generates a report using Open-AI GPT.
+        Args:
+            model_id (int): The model id
+            version_id (int): The version id
+            target_description (str): The target description
+            project_objective (str): The project objective
+            max_features (int): The maximum number of features
+            temperature (float): The temperature
+        Return:
+            dict: The report
+        """
+
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/'
+            f'{version_id}/generate-report'
+        )
+        params = {
+            'target_description': target_description,
+            'project_objective': project_objective,
+            'max_features': max_features,
+            'temperature': temperature
+        }
+        response = self.session._session.put(
+            url=url,
+            json=params,
+            )
+
+        content = self.session.get_response_content(response)
+        return content
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_misc.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_misc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-""" Copyright Xplainable Pty Ltd"""
-import pandas as pd
-import inspect
-import ast
-import xplainable
-from xplainable.utils.model_parsers import *
-from xplainable.quality.scanner import XScan
-
-from xplainable_client.client.utils.encoders import NpEncoder
-from xplainable_client.client.utils.metrics import evaluate_classification, evaluate_regression
-
-from ._client_cog_base import *
-
-
-class Misc(Client_Cog):
-
-    @staticmethod
-    def _get_xplainable_version():
-        """Retrieve the installed xplainable package version."""
-        try:
-            # Access the __version__ attribute from the xplainable package
-            return xplainable.__version__
-        except AttributeError:
-            # Handle the case where __version__ is not defined
-            return "Unknown"
-
-    def ping_server(self, hostname):
-        response = self.session._session.get(
-            f'{hostname}/v1/compute/ping',
-            timeout=1
-            )
-        content = json.loads(response.content)
-        if content == True:
-            return True
-        else:
-            return False
-
-    def ping_gateway(self, hostname):
-        response = self.session._session.get(
-            f'{hostname}/v1/ping',
-            timeout=1
-            )
-        content = json.loads(response.content)
-        if content == True:
-            return True
-        else:
-            return False
-
-
-
-    def load_classifier(self, model_id: int, version_id: int, model=None):
-        """ Loads a binary classification model by model_id
-        Args:
-            model_id (str): A valid model_id
-            version_id (str): A valid version_id
-            model (PartitionedClassifier): An existing model to add partitions
-        Returns:
-            xplainable.PartitionedClassifier: The loaded xplainable classifier
-        """
-        response = self.__get_model__(model_id, version_id)
-        if response['model_type'] != 'binary_classification':
-            raise ValueError(f'Model with ID {model_id}:{version_id} is not a binary classification model')
-        return parse_classifier_response(response, model)
-    
-
-    def load_regressor(self, model_id: int, version_id: int, model=None):
-        """ Loads a regression model by model_id and version_id
-        Args:
-            model_id (str): A valid model_id
-            version_id (str): A valid version_id
-            model (PartitionedRegressor): An existing model to add partitions to
-        Returns:
-            xplainable.PartitionedRegressor: The loaded xplainable regressor
-        """
-        response = self.__get_model__(model_id, version_id)
-        if response['model_type'] != 'regression':
-            raise ValueError(f'Model with ID {model_id}:{version_id} is not a regression model')
-        return parse_regressor_response(response, model)
-    
-
-    def _get_partition_data(
-            self, model, partition_name: str, x: pd.DataFrame,
-            y: pd.Series) -> dict:
-        """ Logs a partition to a model version.
-        Args:
-            model_type (str): The model type
-            partition_name (str): The name of the partition column
-            model (mixed): The model to log
-            model_id (int): The model id
-            version_id (int): The version id
-            evaluation (dict, optional): Model evaluation data and metrics.
-            training_metadata (dict, optional): Model training metadata.
-        """
-        model_type, _ = self._detect_model_type(model)
-        data = {
-            "partition": str(partition_name),
-            "profile": json.dumps(model._profile, cls=NpEncoder),
-            "feature_importances": json.loads(
-                json.dumps(model.feature_importances, cls=NpEncoder)),
-            "id_columns": json.loads(
-                json.dumps(model.id_columns, cls=NpEncoder)),
-            "columns": json.loads(
-                json.dumps(model.columns, cls=NpEncoder)),
-            "parameters": model.params.to_json(),
-            "base_value": json.loads(
-                json.dumps(model.base_value, cls=NpEncoder)),
-            "feature_map": json.loads(
-                json.dumps({k: fm.forward for k, fm in model.feature_map.items()}, cls=NpEncoder)),
-            "target_map": json.loads(
-                json.dumps(model.target_map.reverse, cls=NpEncoder)),
-            "category_meta": json.loads(
-                json.dumps(model.category_meta, cls=NpEncoder)),
-            # "constructs": model.constructs_to_json(),
-            "calibration_map": None,
-            "support_map": None
-        }
-        if model_type == 'binary_classification':
-            data.update({
-                "calibration_map": json.loads(
-                    json.dumps(model._calibration_map, cls=NpEncoder)),
-                "support_map": json.loads(
-                    json.dumps(model._support_map, cls=NpEncoder))
-            })
-            evaluation = model.metadata.get('evaluation', {})
-            if evaluation == {}:
-                y_prob = model.predict_score(x)
-                if model.target_map:
-                    y = y.map(model.target_map)
-                evaluation = {
-                    'train': evaluate_classification(y, y_prob)
-                }
-
-        elif model_type == 'regression':
-            evaluation = model.metadata.get('evaluation', {})
-            if evaluation == {}:
-                y_pred = model.predict(x)
-                evaluation = {
-                            'train': evaluate_regression(y, y_pred)
-                        }
-
-        data["evaluation"] = json.dumps(evaluation, cls=NpEncoder)
-        training_metadata = {
-            i: v for i, v in model.metadata.items() if i != "evaluation"}
-
-        data["training_metadata"] = json.dumps(training_metadata, cls=NpEncoder)
-
-        if x is not None:
-            scanner = XScan()
-            scanner.scan(x)  # Assuming scan method doesn't raise exceptions itself now
-            results = []
-            for i, v in scanner.profile.items():
-                # Check if the column 'i' in dataframe 'x' is completely NA
-                if x[i].isna().all():
-                    # If the column is not all NA, process it
-                    feature_info = {
-                        "feature": i,
-                        "description": '',
-                        "type": "All NA",
-                        "health_info": json.loads(json.dumps({}, cls=NpEncoder))
-                    }
-                # If the column is not all NA, process it
-                feature_info = {
-                    "feature": i,
-                    "description": '',
-                    "type": v['type'],
-                    "health_info": json.loads(json.dumps(v, cls=NpEncoder))
-                }
-                results.append(feature_info)
-            data["health_info"] = json.dumps(results, cls=NpEncoder)
-        return data
-
-    @staticmethod
-    def __parse_function(func):
-        """ Parses a function to a middleware function. """
-        if not callable(func):
-            raise Exception("Function must be callable")
-        sig = inspect.signature(func)
-        params = list(sig.parameters.values())
-        if len(params) != 1:
-            raise Exception("Function must take one parameter")
-        # Parse the source code to an AST
-        source = inspect.getsource(func)
-        parsed_ast = ast.parse(source)
-        # Rename the function in the AST
-        for node in ast.walk(parsed_ast):
-            if isinstance(node, ast.FunctionDef) and node.name == func.__name__:
-                node.name = "middleware"
-                break
-        # Store the modified source
-        modified_source = ast.unparse(parsed_ast)
-        # Compile the AST back to code and execute in a new namespace
-        local_vars = {}
-        exec(compile(
-            parsed_ast, filename="<ast>", mode="exec"),
-            func.__globals__, local_vars)
-        middleware = local_vars['middleware']
-        middleware.source = modified_source
+""" Copyright Xplainable Pty Ltd"""
+import pandas as pd
+import inspect
+import ast
+import xplainable
+from xplainable.utils.model_parsers import *
+from xplainable.quality.scanner import XScan
+
+from xplainable_client.client.utils.encoders import NpEncoder
+from xplainable_client.client.utils.metrics import evaluate_classification, evaluate_regression
+
+from ._client_cog_base import *
+
+
+class Misc(Client_Cog):
+
+    @staticmethod
+    def _get_xplainable_version():
+        """Retrieve the installed xplainable package version."""
+        try:
+            # Access the __version__ attribute from the xplainable package
+            return xplainable.__version__
+        except AttributeError:
+            # Handle the case where __version__ is not defined
+            return "Unknown"
+
+    def ping_server(self, hostname):
+        response = self.session._session.get(
+            f'{hostname}/v1/compute/ping',
+            timeout=1
+            )
+        content = json.loads(response.content)
+        if content == True:
+            return True
+        else:
+            return False
+
+    def ping_gateway(self, hostname):
+        response = self.session._session.get(
+            f'{hostname}/v1/ping',
+            timeout=1
+            )
+        content = json.loads(response.content)
+        if content == True:
+            return True
+        else:
+            return False
+
+
+
+    def load_classifier(self, model_id: int, version_id: int, model=None):
+        """ Loads a binary classification model by model_id
+        Args:
+            model_id (str): A valid model_id
+            version_id (str): A valid version_id
+            model (PartitionedClassifier): An existing model to add partitions
+        Returns:
+            xplainable.PartitionedClassifier: The loaded xplainable classifier
+        """
+        response = self.__get_model__(model_id, version_id)
+        if response['model_type'] != 'binary_classification':
+            raise ValueError(f'Model with ID {model_id}:{version_id} is not a binary classification model')
+        return parse_classifier_response(response, model)
+    
+
+    def load_regressor(self, model_id: int, version_id: int, model=None):
+        """ Loads a regression model by model_id and version_id
+        Args:
+            model_id (str): A valid model_id
+            version_id (str): A valid version_id
+            model (PartitionedRegressor): An existing model to add partitions to
+        Returns:
+            xplainable.PartitionedRegressor: The loaded xplainable regressor
+        """
+        response = self.__get_model__(model_id, version_id)
+        if response['model_type'] != 'regression':
+            raise ValueError(f'Model with ID {model_id}:{version_id} is not a regression model')
+        return parse_regressor_response(response, model)
+    
+
+    def _get_partition_data(
+            self, model, partition_name: str, x: pd.DataFrame,
+            y: pd.Series) -> dict:
+        """ Logs a partition to a model version.
+        Args:
+            model_type (str): The model type
+            partition_name (str): The name of the partition column
+            model (mixed): The model to log
+            model_id (int): The model id
+            version_id (int): The version id
+            evaluation (dict, optional): Model evaluation data and metrics.
+            training_metadata (dict, optional): Model training metadata.
+        """
+        model_type, _ = self._detect_model_type(model)
+        data = {
+            "partition": str(partition_name),
+            "profile": json.dumps(model._profile, cls=NpEncoder),
+            "feature_importances": json.loads(
+                json.dumps(model.feature_importances, cls=NpEncoder)),
+            "id_columns": json.loads(
+                json.dumps(model.id_columns, cls=NpEncoder)),
+            "columns": json.loads(
+                json.dumps(model.columns, cls=NpEncoder)),
+            "parameters": model.params.to_json(),
+            "base_value": json.loads(
+                json.dumps(model.base_value, cls=NpEncoder)),
+            "feature_map": json.loads(
+                json.dumps({k: fm.forward for k, fm in model.feature_map.items()}, cls=NpEncoder)),
+            "target_map": json.loads(
+                json.dumps(model.target_map.reverse, cls=NpEncoder)),
+            "category_meta": json.loads(
+                json.dumps(model.category_meta, cls=NpEncoder)),
+            # "constructs": model.constructs_to_json(),
+            "calibration_map": None,
+            "support_map": None
+        }
+        if model_type == 'binary_classification':
+            data.update({
+                "calibration_map": json.loads(
+                    json.dumps(model._calibration_map, cls=NpEncoder)),
+                "support_map": json.loads(
+                    json.dumps(model._support_map, cls=NpEncoder))
+            })
+            evaluation = model.metadata.get('evaluation', {})
+            if evaluation == {}:
+                y_prob = model.predict_score(x)
+                if model.target_map:
+                    y = y.map(model.target_map)
+                evaluation = {
+                    'train': evaluate_classification(y, y_prob)
+                }
+
+        elif model_type == 'regression':
+            evaluation = model.metadata.get('evaluation', {})
+            if evaluation == {}:
+                y_pred = model.predict(x)
+                evaluation = {
+                            'train': evaluate_regression(y, y_pred)
+                        }
+
+        data["evaluation"] = json.dumps(evaluation, cls=NpEncoder)
+        training_metadata = {
+            i: v for i, v in model.metadata.items() if i != "evaluation"}
+
+        data["training_metadata"] = json.dumps(training_metadata, cls=NpEncoder)
+
+        if x is not None:
+            scanner = XScan()
+            scanner.scan(x)  # Assuming scan method doesn't raise exceptions itself now
+            results = []
+            for i, v in scanner.profile.items():
+                # Check if the column 'i' in dataframe 'x' is completely NA
+                if x[i].isna().all():
+                    # If the column is not all NA, process it
+                    feature_info = {
+                        "feature": i,
+                        "description": '',
+                        "type": "All NA",
+                        "health_info": json.loads(json.dumps({}, cls=NpEncoder))
+                    }
+                # If the column is not all NA, process it
+                feature_info = {
+                    "feature": i,
+                    "description": '',
+                    "type": v['type'],
+                    "health_info": json.loads(json.dumps(v, cls=NpEncoder))
+                }
+                results.append(feature_info)
+            data["health_info"] = json.dumps(results, cls=NpEncoder)
+        return data
+
+    @staticmethod
+    def __parse_function(func):
+        """ Parses a function to a middleware function. """
+        if not callable(func):
+            raise Exception("Function must be callable")
+        sig = inspect.signature(func)
+        params = list(sig.parameters.values())
+        if len(params) != 1:
+            raise Exception("Function must take one parameter")
+        # Parse the source code to an AST
+        source = inspect.getsource(func)
+        parsed_ast = ast.parse(source)
+        # Rename the function in the AST
+        for node in ast.walk(parsed_ast):
+            if isinstance(node, ast.FunctionDef) and node.name == func.__name__:
+                node.name = "middleware"
+                break
+        # Store the modified source
+        modified_source = ast.unparse(parsed_ast)
+        # Compile the AST back to code and execute in a new namespace
+        local_vars = {}
+        exec(compile(
+            parsed_ast, filename="<ast>", mode="exec"),
+            func.__globals__, local_vars)
+        middleware = local_vars['middleware']
+        middleware.source = modified_source
         return middleware
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_models.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,589 +1,589 @@
-import pandas as pd
-from ._client_cog_base import Client_Cog
-from xplainable_client.client.utils.encoders import force_json_compliant
-import json
-from .utils.encoders import NpEncoder
-from .utils.scanner import XScan
-from .utils.metrics import evaluate_classification, evaluate_regression
-
-
-class Models(Client_Cog):
-
-    def create_model(self, model_name: str, model_description: str, model, x: pd.DataFrame, y: pd.Series):
-        """ Creates a new model if the model does not already exist.
-
-        Args:
-            model_name (str): The name of the model
-            model_description (str): The description of the model
-            model (XClassifier | XRegressor): The model to create
-            x (pd.DataFrame): The feature matrix
-            y (pd.Series): The target variable
-
-        Returns:
-            str: The model id
-            str: The version id
-
-        Raises:
-            Exception: If the model creation fails.
-        """
-        model_id = self.create_model_id(model, model_name, model_description)
-        try:
-            version_id = self.create_model_version(model, model_id, x, y)
-        except Exception as e:
-            self.delete_model(model_id)
-            raise e
-        return model_id, version_id
-    
-    def create_model_id(
-            self, model, model_name: str, model_description: str) -> str:
-        """ Creates a new model and returns the model id.
-        Args:
-            model_name (str): The name of the model
-            model_description (str): The description of the model
-            model (XClassifier | XRegressor): The model to create.
-        Returns:
-            int: The model id
-        """
-        model_type, target = self._detect_model_type(model)
-        payoad = {
-            "model_name": model_name,
-            "model_description": model_description,
-            "model_type": model_type,
-            "target_name": target,
-            "algorithm": model.__class__.__name__
-        }
-
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/create-model',
-            json=payoad
-        )
-        model_id = self.session.get_response_content(response)
-
-        return model_id
-
-    
-    #TODO: Refactor this based on notion instructions.
-    def create_model_version(self, model, model_id: str, x: pd.DataFrame, y: pd.Series) -> str:
-        """ Creates a new model version and returns the version id.
-        Args:
-            model_id (int): The model id
-            partition_on (str): The partition column name
-            ruleset (dict | str): The feeature ruleset
-            health_info (dict): Feature health information
-            versions (dict): Versions of current environment
-        Returns:
-            int: The model version id
-        """
-        # Get current versions
-        versions = {
-                "xplainable_version": self.session.xplainable_version,
-                "python_version": self.session.python_version
-            }
-        partition_on = model.partition_on if 'Partitioned' in \
-            model.__class__.__name__ else None
-        payload = {
-            "partition_on": partition_on,
-            "versions": versions,
-            "partitions": []
-            }
-        partitioned_models = ['PartitionedClassifier', 'PartitionedRegressor']
-        independent_models = ['XClassifier', 'XRegressor']
-        # get all partitions
-        if model.__class__.__name__ in partitioned_models:
-            for p, m in model.partitions.items():
-                if p == '__dataset__':
-                    part_x = x
-                    part_y = y
-                else:
-                    part_x = x[x[partition_on].astype(str) == str(p)]
-                    part_y = y[y.index.isin(part_x.index)]
-                pdata = model._get_partition_data(m, p, part_x, part_y)
-                payload['partitions'].append(pdata)
-
-        elif model.__class__.__name__ in independent_models:
-            pdata = self._get_partition_data(model, '__dataset__', x, y)
-            payload['partitions'].append(pdata)
-
-        # Create a new version and fetch id
-        url = f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/add-version'
-        response = self.session._session.post(url=url, json=force_json_compliant(payload))
-        version_id = self.session.get_response_content(response)
-        return version_id
-
-    def _get_partition_data(
-            self, model, partition_name: str, x: pd.DataFrame,
-            y: pd.Series) -> dict:
-        """ Logs a partition to a model version.
-
-        Args:
-            model_type (str): The model type
-            partition_name (str): The name of the partition column
-            model (mixed): The model to log
-            model_id (int): The model id
-            version_id (int): The version id
-            evaluation (dict, optional): Model evaluation data and metrics.
-            training_metadata (dict, optional): Model training metadata.
-
-        """
-
-        model_type, _ = self._detect_model_type(model)
-
-        data = {
-            "partition": str(partition_name),
-            "profile": json.dumps(model._profile, cls=NpEncoder),
-            "feature_importances": json.loads(
-                json.dumps(model.feature_importances, cls=NpEncoder)),
-            "id_columns": json.loads(
-                json.dumps(model.id_columns, cls=NpEncoder)),
-            "columns": json.loads(
-                json.dumps(model.columns, cls=NpEncoder)),
-            "parameters": model.params.to_json(),
-            "base_value": json.loads(
-                json.dumps(model.base_value, cls=NpEncoder)),
-            "feature_map": json.loads(
-                json.dumps({k: fm.forward for k, fm in model.feature_map.items()}, cls=NpEncoder)),
-            "target_map": json.loads(
-                json.dumps(model.target_map.reverse, cls=NpEncoder)),
-            "category_meta": json.loads(
-                json.dumps(model.category_meta, cls=NpEncoder)),
-            # "constructs": model.constructs_to_json(),
-            "calibration_map": None,
-            "support_map": None
-        }
-
-        if model_type == 'binary_classification':
-            data.update({
-                "calibration_map": json.loads(
-                    json.dumps(model._calibration_map, cls=NpEncoder)),
-                "support_map": json.loads(
-                    json.dumps(model._support_map, cls=NpEncoder))
-            })
-
-            evaluation = model.metadata.get('evaluation', {})
-            if evaluation == {}:
-                y_prob = model.predict_score(x)
-
-                if model.target_map:
-                    y = y.map(model.target_map)
-
-                evaluation = {
-                    'train': evaluate_classification(y, y_prob)
-                }
-
-        elif model_type == 'regression':
-            evaluation = model.metadata.get('evaluation', {})
-            if evaluation == {}:
-                y_pred = model.predict(x)
-                evaluation = {
-                    'train': evaluate_regression(y, y_pred)
-                }
-
-        data["evaluation"] = json.dumps(evaluation, cls=NpEncoder)
-
-        training_metadata = {
-            i: v for i, v in model.metadata.items() if i != "evaluation"}
-
-        data["training_metadata"] = json.dumps(training_metadata, cls=NpEncoder)
-
-        if x is not None:
-            scanner = XScan()
-            scanner.scan(x)
-
-            results = []
-            for i, v in scanner.profile.items():
-                feature_info = {
-                    "feature": i,
-                    "description": '',
-                    "type": v['type'],
-                    "health_info": json.loads(json.dumps(v, cls=NpEncoder))
-                }
-                results.append(feature_info)
-
-            data["health_info"] = json.dumps(results, cls=NpEncoder)
-
-        return data
-        
-
-    def list_models(self) -> list:
-        """ Lists all models of the active user's team.
-
-        Returns:
-            dict: Dictionary of saved models.
-        """
-
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models'
-            )
-
-        data = self.session.get_response_content(response)
-
-        # For better readability
-        [i.pop('user') for i in data]
-        [i.pop('contributors') for i in data]
-
-        return data
-    
-
-    def __get_model__(self, model_id: int, version_id: int):
-        """ Gets a model with a specific version.
-
-        Args:
-            model_id (int): The model id
-            version_id (int): The version id
-
-        Returns:
-            dict: The model information
-
-        Raises:
-            ValueError: If the model does not exist.
-        """
-        try:
-            response = self.session._session.get(
-                url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
-            )
-            return self.session.get_response_content(response)
-        except Exception as e:
-            raise ValueError(f'Model with ID {model_id}:{version_id} does not exist')
-
-    #TODO: Refactor this based on notion instructions.
-    def _detect_model_type(self, model):
-        """ Determines the type of model and target.
-        
-        Args:
-            model (XClassifier | XRegressor): The existing model.
-
-        Return:
-            tuple:
-                - model_type (str): The model type, either 'binary_classification' or 'regression'
-                - model.target (str): The model target. 
-        """
-
-
-        if 'Partitioned' in model.__class__.__name__:
-            model = model.partitions['__dataset__']
-        cls_name = model.__class__.__name__
-        if cls_name == "XClassifier":
-            model_type = "binary_classification"
-        elif cls_name == "XRegressor":
-            model_type = "regression"
-        else:
-            raise ValueError(
-                f'Model type {cls_name} is not supported')
-
-        return model_type, model.target
-
-    def list_model_versions(self, model_id: int) -> list:
-        """ Lists all versions of a model.
-        Args:
-            model_id (int): The model id
-        Returns:
-            dict: Dictionary of model versions.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions'
-            )
-        data = self.session.get_response_content(response)
-        [i.pop('user') for i in data]
-        return data
-    
-    def list_model_version_partitions(self, model_id: str, version_id: str):
-        """ Lists all partitions of a model version.
-
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        
-        Return:
-            dict: Dictionary of model partitions.
-
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
-        )
-        partitions = self.session.get_response_content(response)
-        return partitions
-
-
-    def get_model_version_partition(self, model_id: str, version_id: str, partition_id: str):
-        """ Gets a partition of a model version.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-            partition_id (str): The partition id.
-        Returns:
-            json: A json payload.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}'
-        )
-        partition_data = self.session.get_response_content(response)
-        return partition_data
-
-
-    def delete_model_version(self, model_id: str, version_id: str):
-        """ Deletes a model version.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            json: A json payload.
-        """
-        response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
-        )
-        return response
-
-    def restore_model_version(self, model_id: str, version_id: str):
-        """ Restores a model version.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            json: A json payload.
-        """
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/restore'
-        )
-        return response
-
-    def delete_model(self, model_id: str):
-        """ Deletes an existing model.
-        Args:
-            model_id (str): The id of the model to be deleted.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}'
-        )
-        return response
-    
-    def restore_deleted_model(self, model_id: str):
-        """ Restores a deleted model.
-        Args:
-            model_id (str): The id of the model to be restored.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-deleted'
-        )
-        return response
-
-    def activate_model(self, model_id: str):
-        """ Activates a model.
-        Args:
-            model_id (str): The id of the model to be activated.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/activate'
-        )
-        return response
-
-    def deactivate_model(self, model_id: str):
-        """ Deactivates a model.
-        Args:
-            model_id (str): The id of the model to be deactivated.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/deactivate'
-        )
-        return response
-
-    def archive_model(self, model_id: str):
-        """ Archives a model.
-        Args:
-            model_id (str): The id of the model to be archived.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/archive'
-        )
-        return response
-
-    def restore_archived_model(self, model_id: str):
-        """ Restores an archived model.
-        Args:
-            model_id (str): The id of the model to be restored.
-        Return:
-            json: A json payload
-        """
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-archived'
-        )
-        return response
-
-    def publish_model_version(self, model_id: str, version_id: str):
-        """ Publishes a model version.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            json: A json payload.
-        """
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/publish'
-        )
-        return response
-
-
-    def unpublish_model_version(self, model_id: str, version_id: str):
-        """ Unpublishes a model version.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            json: A json payload.
-        """
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/unpublish'
-        )
-        return response
-
-    def update_model_description(self, model_id: str, description: str):
-        """ Updates the description of a model.
-        Args:
-            model_id (str): The model id.
-            description (str): The new description of the model.
-        Return:
-            json: A json payload.
-        """
-        payload = {
-            "description": description
-        }
-
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/description',
-            json=payload
-        )
-        return response
-
-    def update_model_name(self, model_id: str, name: str):
-        """ Updates the name of a model.
-        Args:
-            model_id (str): The model id.
-            name (str): The new name of the model.
-        Return:
-            json: A json payload.
-        """
-        payload = {
-            "name": name
-        }
-
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/name',
-            json=payload
-        )
-        return response
-
-    def get_model_profile(self, model_id: str, version_id: str):
-        """ Gets the profile of a model.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            list: A list of model profiles.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/profile'
-        )
-        profile = self.session.get_response_content(response)
-        return profile
-
-    def get_model_evaluation_data(self, model_id: str, version_id: str, partition_id: str):
-        """ Gets the evaluation data of a model.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-            partition_id (str): The partition id.
-        Return:
-            dict: A dictionary of model evaluation data.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}/evaluation'
-        )
-        evaluation_data = self.session.get_response_content(response)
-        return evaluation_data
-
-    def link_model_preprocessor(self, model_id: str, version_id: str, preprocessor_id: str, preprocessor_version_id: str):
-        """ Links a model to a preprocessor.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-            preprocessor_id (str): The preprocessor id.
-            preprocessor_version_id (str): The preprocessor version id.
-        Return:
-            json: A json payload.
-        """
-        payload = {
-            "preprocessor_id": preprocessor_id,
-            "preprocessor_version_id": preprocessor_version_id
-
-        }
-
-        response = self.session._session.put(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor',
-            json=payload
-        )
-        return response
-
-    def get_model_preprocessor(self, model_id: str, version_id: str):
-        """ Gets the preprocessor of a model.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            dict: A dictionary of model preprocessor.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor'
-        )
-        preprocessor = self.session.get_response_content(response)
-        return preprocessor
-
-    def set_active_version(self, model_id: str, version_id: str):
-        """ Sets the active version of a model.
-        Args:
-            model_id (str): The model id.
-            version_id (str): The version id.
-        Return:
-            json: A json payload.
-        """
-        payload = {
-            "version_id": version_id
-        }
-
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/active-version',
-            json=payload
-        )
-        return response
-
-    def move_model(self, model_id: str, new_team_id: str):
-        """ Moves a model to a new team.
-        Args:
-            model_id (str): The model id.
-            new_team_id (str): The new team id.
-        Return:
-            json: A json payload.
-        """
-        payload = {
-            "new_team_id": new_team_id
-        }
-
-        response = self.session._session.patch(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/move',
-            json=payload
-        )
-        return response
-
-
-
-    
-
-       
+import pandas as pd
+from ._client_cog_base import Client_Cog
+from xplainable_client.client.utils.encoders import force_json_compliant
+import json
+from .utils.encoders import NpEncoder
+from .utils.scanner import XScan
+from .utils.metrics import evaluate_classification, evaluate_regression
+
+
+class Models(Client_Cog):
+
+    def create_model(self, model_name: str, model_description: str, model, x: pd.DataFrame, y: pd.Series):
+        """ Creates a new model if the model does not already exist.
+
+        Args:
+            model_name (str): The name of the model
+            model_description (str): The description of the model
+            model (XClassifier | XRegressor): The model to create
+            x (pd.DataFrame): The feature matrix
+            y (pd.Series): The target variable
+
+        Returns:
+            str: The model id
+            str: The version id
+
+        Raises:
+            Exception: If the model creation fails.
+        """
+        model_id = self.create_model_id(model, model_name, model_description)
+        try:
+            version_id = self.create_model_version(model, model_id, x, y)
+        except Exception as e:
+            self.delete_model(model_id)
+            raise e
+        return model_id, version_id
+    
+    def create_model_id(
+            self, model, model_name: str, model_description: str) -> str:
+        """ Creates a new model and returns the model id.
+        Args:
+            model_name (str): The name of the model
+            model_description (str): The description of the model
+            model (XClassifier | XRegressor): The model to create.
+        Returns:
+            int: The model id
+        """
+        model_type, target = self._detect_model_type(model)
+        payoad = {
+            "model_name": model_name,
+            "model_description": model_description,
+            "model_type": model_type,
+            "target_name": target,
+            "algorithm": model.__class__.__name__
+        }
+
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/create-model',
+            json=payoad
+        )
+        model_id = self.session.get_response_content(response)
+
+        return model_id
+
+    
+    #TODO: Refactor this based on notion instructions.
+    def create_model_version(self, model, model_id: str, x: pd.DataFrame, y: pd.Series) -> str:
+        """ Creates a new model version and returns the version id.
+        Args:
+            model_id (int): The model id
+            partition_on (str): The partition column name
+            ruleset (dict | str): The feeature ruleset
+            health_info (dict): Feature health information
+            versions (dict): Versions of current environment
+        Returns:
+            int: The model version id
+        """
+        # Get current versions
+        versions = {
+                "xplainable_version": self.session.xplainable_version,
+                "python_version": self.session.python_version
+            }
+        partition_on = model.partition_on if 'Partitioned' in \
+            model.__class__.__name__ else None
+        payload = {
+            "partition_on": partition_on,
+            "versions": versions,
+            "partitions": []
+            }
+        partitioned_models = ['PartitionedClassifier', 'PartitionedRegressor']
+        independent_models = ['XClassifier', 'XRegressor']
+        # get all partitions
+        if model.__class__.__name__ in partitioned_models:
+            for p, m in model.partitions.items():
+                if p == '__dataset__':
+                    part_x = x
+                    part_y = y
+                else:
+                    part_x = x[x[partition_on].astype(str) == str(p)]
+                    part_y = y[y.index.isin(part_x.index)]
+                pdata = model._get_partition_data(m, p, part_x, part_y)
+                payload['partitions'].append(pdata)
+
+        elif model.__class__.__name__ in independent_models:
+            pdata = self._get_partition_data(model, '__dataset__', x, y)
+            payload['partitions'].append(pdata)
+
+        # Create a new version and fetch id
+        url = f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/add-version'
+        response = self.session._session.post(url=url, json=force_json_compliant(payload))
+        version_id = self.session.get_response_content(response)
+        return version_id
+
+    def _get_partition_data(
+            self, model, partition_name: str, x: pd.DataFrame,
+            y: pd.Series) -> dict:
+        """ Logs a partition to a model version.
+
+        Args:
+            model_type (str): The model type
+            partition_name (str): The name of the partition column
+            model (mixed): The model to log
+            model_id (int): The model id
+            version_id (int): The version id
+            evaluation (dict, optional): Model evaluation data and metrics.
+            training_metadata (dict, optional): Model training metadata.
+
+        """
+
+        model_type, _ = self._detect_model_type(model)
+
+        data = {
+            "partition": str(partition_name),
+            "profile": json.dumps(model._profile, cls=NpEncoder),
+            "feature_importances": json.loads(
+                json.dumps(model.feature_importances, cls=NpEncoder)),
+            "id_columns": json.loads(
+                json.dumps(model.id_columns, cls=NpEncoder)),
+            "columns": json.loads(
+                json.dumps(model.columns, cls=NpEncoder)),
+            "parameters": model.params.to_json(),
+            "base_value": json.loads(
+                json.dumps(model.base_value, cls=NpEncoder)),
+            "feature_map": json.loads(
+                json.dumps({k: fm.forward for k, fm in model.feature_map.items()}, cls=NpEncoder)),
+            "target_map": json.loads(
+                json.dumps(model.target_map.reverse, cls=NpEncoder)),
+            "category_meta": json.loads(
+                json.dumps(model.category_meta, cls=NpEncoder)),
+            # "constructs": model.constructs_to_json(),
+            "calibration_map": None,
+            "support_map": None
+        }
+
+        if model_type == 'binary_classification':
+            data.update({
+                "calibration_map": json.loads(
+                    json.dumps(model._calibration_map, cls=NpEncoder)),
+                "support_map": json.loads(
+                    json.dumps(model._support_map, cls=NpEncoder))
+            })
+
+            evaluation = model.metadata.get('evaluation', {})
+            if evaluation == {}:
+                y_prob = model.predict_score(x)
+
+                if model.target_map:
+                    y = y.map(model.target_map)
+
+                evaluation = {
+                    'train': evaluate_classification(y, y_prob)
+                }
+
+        elif model_type == 'regression':
+            evaluation = model.metadata.get('evaluation', {})
+            if evaluation == {}:
+                y_pred = model.predict(x)
+                evaluation = {
+                    'train': evaluate_regression(y, y_pred)
+                }
+
+        data["evaluation"] = json.dumps(evaluation, cls=NpEncoder)
+
+        training_metadata = {
+            i: v for i, v in model.metadata.items() if i != "evaluation"}
+
+        data["training_metadata"] = json.dumps(training_metadata, cls=NpEncoder)
+
+        if x is not None:
+            scanner = XScan()
+            scanner.scan(x)
+
+            results = []
+            for i, v in scanner.profile.items():
+                feature_info = {
+                    "feature": i,
+                    "description": '',
+                    "type": v['type'],
+                    "health_info": json.loads(json.dumps(v, cls=NpEncoder))
+                }
+                results.append(feature_info)
+
+            data["health_info"] = json.dumps(results, cls=NpEncoder)
+
+        return data
+        
+
+    def list_models(self) -> list:
+        """ Lists all models of the active user's team.
+
+        Returns:
+            dict: Dictionary of saved models.
+        """
+
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models'
+            )
+
+        data = self.session.get_response_content(response)
+
+        # For better readability
+        [i.pop('user') for i in data]
+        [i.pop('contributors') for i in data]
+
+        return data
+    
+
+    def __get_model__(self, model_id: int, version_id: int):
+        """ Gets a model with a specific version.
+
+        Args:
+            model_id (int): The model id
+            version_id (int): The version id
+
+        Returns:
+            dict: The model information
+
+        Raises:
+            ValueError: If the model does not exist.
+        """
+        try:
+            response = self.session._session.get(
+                url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
+            )
+            return self.session.get_response_content(response)
+        except Exception as e:
+            raise ValueError(f'Model with ID {model_id}:{version_id} does not exist')
+
+    #TODO: Refactor this based on notion instructions.
+    def _detect_model_type(self, model):
+        """ Determines the type of model and target.
+        
+        Args:
+            model (XClassifier | XRegressor): The existing model.
+
+        Return:
+            tuple:
+                - model_type (str): The model type, either 'binary_classification' or 'regression'
+                - model.target (str): The model target. 
+        """
+
+
+        if 'Partitioned' in model.__class__.__name__:
+            model = model.partitions['__dataset__']
+        cls_name = model.__class__.__name__
+        if cls_name == "XClassifier":
+            model_type = "binary_classification"
+        elif cls_name == "XRegressor":
+            model_type = "regression"
+        else:
+            raise ValueError(
+                f'Model type {cls_name} is not supported')
+
+        return model_type, model.target
+
+    def list_model_versions(self, model_id: int) -> list:
+        """ Lists all versions of a model.
+        Args:
+            model_id (int): The model id
+        Returns:
+            dict: Dictionary of model versions.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions'
+            )
+        data = self.session.get_response_content(response)
+        [i.pop('user') for i in data]
+        return data
+    
+    def list_model_version_partitions(self, model_id: str, version_id: str):
+        """ Lists all partitions of a model version.
+
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        
+        Return:
+            dict: Dictionary of model partitions.
+
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
+        )
+        partitions = self.session.get_response_content(response)
+        return partitions
+
+
+    def get_model_version_partition(self, model_id: str, version_id: str, partition_id: str):
+        """ Gets a partition of a model version.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+            partition_id (str): The partition id.
+        Returns:
+            json: A json payload.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}'
+        )
+        partition_data = self.session.get_response_content(response)
+        return partition_data
+
+
+    def delete_model_version(self, model_id: str, version_id: str):
+        """ Deletes a model version.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            json: A json payload.
+        """
+        response = self.session._session.delete(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}'
+        )
+        return response
+
+    def restore_model_version(self, model_id: str, version_id: str):
+        """ Restores a model version.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            json: A json payload.
+        """
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/restore'
+        )
+        return response
+
+    def delete_model(self, model_id: str):
+        """ Deletes an existing model.
+        Args:
+            model_id (str): The id of the model to be deleted.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.delete(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}'
+        )
+        return response
+    
+    def restore_deleted_model(self, model_id: str):
+        """ Restores a deleted model.
+        Args:
+            model_id (str): The id of the model to be restored.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-deleted'
+        )
+        return response
+
+    def activate_model(self, model_id: str):
+        """ Activates a model.
+        Args:
+            model_id (str): The id of the model to be activated.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/activate'
+        )
+        return response
+
+    def deactivate_model(self, model_id: str):
+        """ Deactivates a model.
+        Args:
+            model_id (str): The id of the model to be deactivated.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/deactivate'
+        )
+        return response
+
+    def archive_model(self, model_id: str):
+        """ Archives a model.
+        Args:
+            model_id (str): The id of the model to be archived.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/archive'
+        )
+        return response
+
+    def restore_archived_model(self, model_id: str):
+        """ Restores an archived model.
+        Args:
+            model_id (str): The id of the model to be restored.
+        Return:
+            json: A json payload
+        """
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/restore-archived'
+        )
+        return response
+
+    def publish_model_version(self, model_id: str, version_id: str):
+        """ Publishes a model version.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            json: A json payload.
+        """
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/publish'
+        )
+        return response
+
+
+    def unpublish_model_version(self, model_id: str, version_id: str):
+        """ Unpublishes a model version.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            json: A json payload.
+        """
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/unpublish'
+        )
+        return response
+
+    def update_model_description(self, model_id: str, description: str):
+        """ Updates the description of a model.
+        Args:
+            model_id (str): The model id.
+            description (str): The new description of the model.
+        Return:
+            json: A json payload.
+        """
+        payload = {
+            "description": description
+        }
+
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/description',
+            json=payload
+        )
+        return response
+
+    def update_model_name(self, model_id: str, name: str):
+        """ Updates the name of a model.
+        Args:
+            model_id (str): The model id.
+            name (str): The new name of the model.
+        Return:
+            json: A json payload.
+        """
+        payload = {
+            "name": name
+        }
+
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/name',
+            json=payload
+        )
+        return response
+
+    def get_model_profile(self, model_id: str, version_id: str):
+        """ Gets the profile of a model.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            list: A list of model profiles.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/profile'
+        )
+        profile = self.session.get_response_content(response)
+        return profile
+
+    def get_model_evaluation_data(self, model_id: str, version_id: str, partition_id: str):
+        """ Gets the evaluation data of a model.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+            partition_id (str): The partition id.
+        Return:
+            dict: A dictionary of model evaluation data.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/partitions/{partition_id}/evaluation'
+        )
+        evaluation_data = self.session.get_response_content(response)
+        return evaluation_data
+
+    def link_model_preprocessor(self, model_id: str, version_id: str, preprocessor_id: str, preprocessor_version_id: str):
+        """ Links a model to a preprocessor.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+            preprocessor_id (str): The preprocessor id.
+            preprocessor_version_id (str): The preprocessor version id.
+        Return:
+            json: A json payload.
+        """
+        payload = {
+            "preprocessor_id": preprocessor_id,
+            "preprocessor_version_id": preprocessor_version_id
+
+        }
+
+        response = self.session._session.put(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor',
+            json=payload
+        )
+        return response
+
+    def get_model_preprocessor(self, model_id: str, version_id: str):
+        """ Gets the preprocessor of a model.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            dict: A dictionary of model preprocessor.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/versions/{version_id}/preprocessor'
+        )
+        preprocessor = self.session.get_response_content(response)
+        return preprocessor
+
+    def set_active_version(self, model_id: str, version_id: str):
+        """ Sets the active version of a model.
+        Args:
+            model_id (str): The model id.
+            version_id (str): The version id.
+        Return:
+            json: A json payload.
+        """
+        payload = {
+            "version_id": version_id
+        }
+
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/active-version',
+            json=payload
+        )
+        return response
+
+    def move_model(self, model_id: str, new_team_id: str):
+        """ Moves a model to a new team.
+        Args:
+            model_id (str): The model id.
+            new_team_id (str): The new team id.
+        Return:
+            json: A json payload.
+        """
+        payload = {
+            "new_team_id": new_team_id
+        }
+
+        response = self.session._session.patch(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/models/{model_id}/move',
+            json=payload
+        )
+        return response
+
+
+
+    
+
+
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/_preprocessing.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/_preprocessing.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from ._client_cog_base import *
-import pandas as pd
-import json
-from xplainable_client.client.utils import get_df_delta
-from xplainable.preprocessing.pipeline import XPipeline
-
-
-class Preprocessing(Client_Cog):
-
-    def create_preprocessor_id(
-        self, preprocessor_name: str, preprocessor_description: str) -> str:
-        """ Creates a new preprocessor and returns the preprocessor id.
-        Args:
-            preprocessor_name (str): The name of the preprocessor
-            preprocessor_description (str): The description of the preprocessor
-        Returns:
-            int: The preprocessor id
-        """
-        payoad = {
-            "preprocessor_name": preprocessor_name,
-            "preprocessor_description": preprocessor_description
-        }
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/create-preprocessor',
-            json=payoad
-        )
-
-        preprocessor_id = self.session.get_response_content(response)
-
-        return preprocessor_id
-    
-
-    def create_preprocessor_version(
-        self, preprocessor_id: str, pipeline: list, df: pd.DataFrame = None
-        ) -> str:
-        """ Creates a new preprocessor version and returns the version id.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            pipeline (xplainable.preprocessing.pipeline.Pipeline): pipeline
-        Returns:
-            int: The preprocessor version id
-        """
-        # Structure the stages and deltas
-        stages = []
-        deltas = []
-        if df is not None:
-            before = df.copy()
-            deltas.append({"start": json.loads(before.head(10).to_json(
-                orient='records'))})
-            delta_gen = pipeline.transform_generator(before)
-        for stage in pipeline.stages:
-            step = {
-                'feature': stage['feature'],
-                'name': stage['name'],
-                'params': stage['transformer'].__dict__
-            }
-            stages.append(step)
-            if df is not None:
-                after = delta_gen.__next__()
-                delta = get_df_delta(before.copy(), after.copy())
-                deltas.append(delta)
-                before = after.copy()
-        # Get current versions
-        versions = {
-                "xplainable_version": self.xplainable_version,
-                "python_version": self.python_version
-            }
-        # Create payload
-        payload = {
-            "stages": stages,
-            "deltas": deltas,
-            "versions": versions
-            }
-
-        # Create a new version and fetch id
-        url = (
-            f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/'
-            f'{preprocessor_id}/add-version'
-            )
-
-        response = self.session._session.post(url=url, json=payload)
-        version_id = self.session.get_response_content(response)
-        return version_id
-
-    def list_preprocessors(self) -> list:
-        """ Lists all preprocessors of the active user's team.
-        Returns:
-            dict: Dictionary of preprocessors.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors'
-            )
-        data = self.session.get_response_content(response)
-        [i.pop('user') for i in data]
-        return data
-    
-    # get_preprocessor
-    
-
-
-    def list_preprocessor_versions(self, preprocessor_id: int) -> list:
-        """ Lists all versions of a preprocessor.
-        Args:
-            preprocessor_id (int): The preprocessor id
-        Returns:
-            dict: Dictionary of preprocessor versions.
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions'
-            )
-
-        data = self.session.get_response_content(response)
-        [i.pop('user') for i in data]
-        return data
-
-    def load_preprocessor(
-            self, preprocessor_id: int, version_id: int,
-            gui_object: bool = False, response_only: bool = False):
-        """ Loads a preprocessor by preprocessor_id and version_id.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            version_id (int): The version id
-            response_only (bool, optional): Returns the preprocessor metadata.
-        Returns:
-            xplainable.preprocessing.pipeline.Pipeline: The loaded pipeline
-        """
-        def build_transformer(stage):
-            """Build transformer from metadata"""
-            if not hasattr(xtf, stage["name"]):
-                raise ValueError(f"{stage['name']} does not exist in the transformers module")
-            # Get transformer function
-            func = getattr(xtf, stage["name"])
-            return func(**stage['params'])
-
-        try:
-            preprocessor_response = self.session._session.get(
-                url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
-                )
-            response = self.session.get_response_content(preprocessor_response)
-            if response_only:
-                return response
-        except Exception as e:
-            raise ValueError(
-            f'Preprocessor with ID {preprocessor_id}:{version_id} does not exist')
-
-        stages = response['stages']
-        deltas = response['deltas']
-        pipeline = XPipeline()
-        pipeline.stages = [{"feature": i["feature"], "name": i["name"], \
-                "transformer": build_transformer(i)} for i in stages]
-
-        if not gui_object:
-            return pipeline
-        else:
-            from ..gui.screens.preprocessor import Preprocessor
-            pp = Preprocessor()
-            pp.pipeline = pipeline
-            pp.df_delta = deltas
-            pp.state = len(pipeline.stages)
-            return pp
-
-
-    def get_preprocessor_version_pipeline(self, preprocessor_id: str, version_id: str):
-        """ Returns the pipeline of a preprocessor version.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            version_id (int): The version id
-        Returns:
-            xplainable.preprocessing.pipeline.Pipeline: The pipeline
-        """
-        response = self.session._session.get(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/pipeline'
-            )
-        data = self.session.get_response_content(response)
-        return data
-
-    def delete_preprocessor_version(self, preprocessor_id: str, version_id: str):
-        """ Deletes a preprocessor version.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            version_id (int): The version id
-        Return:
-            json: A json response
-        """
-        response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
-            )
-        return response
-
-    def restore_preprocessor_version(self, preprocessor_id: str, version_id: str):
-        """ Restores a preprocessor version.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            version_id (int): The version id
-        Return:
-            json: A json response. 
-        """
-        response = self.session._session.put(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/restore'
-            )
-        return response
-
-    def delete_preprocessor(self, preprocessor_id: str):
-        """ Deletes a preprocessor.
-        Args:
-            preprocessor_id (int): The preprocessor id
-        Return:
-            json: A json response
-        """
-        response = self.session._session.delete(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}'
-            )
-        return response
-
-    def restore_preprocessor(self, preprocessor_id: str):
-        """ Restores a preprocessor.
-        Args:
-            preprocessor_id (int): The preprocessor id
-        Return:
-            json: A json response
-        """
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/restore'
-            )
-        return response
-
-    def check_signature(self, preprocessor_id: str, preprocessor_version_id: str, model_id: str, model_version_id: str):
-        """ Checks the signature of a preprocessor version.
-        Args:
-            preprocessor_id (int): The preprocessor id
-            preprocessor_version_id (int): The preprocessor version id
-            model_id (int): The model id
-            model_version_id (int): The model version id
-        Return:
-            dict: A json response of signatures_match, pipeline_columns, model_columns.
-        """
-        
-        payload = {
-            'model_id': model_id,
-            'version_id': model_version_id
-        }
-        response = self.session._session.post(
-            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{preprocessor_version_id}/check-signature',
-            json=payload
-        )
-        output = self.session.get_response_content(response)
-        return output
-
-
-    
+from ._client_cog_base import *
+import pandas as pd
+import json
+from xplainable_client.client.utils import get_df_delta
+from xplainable.preprocessing.pipeline import XPipeline
+
+
+class Preprocessing(Client_Cog):
+
+    def create_preprocessor_id(
+        self, preprocessor_name: str, preprocessor_description: str) -> str:
+        """ Creates a new preprocessor and returns the preprocessor id.
+        Args:
+            preprocessor_name (str): The name of the preprocessor
+            preprocessor_description (str): The description of the preprocessor
+        Returns:
+            int: The preprocessor id
+        """
+        payoad = {
+            "preprocessor_name": preprocessor_name,
+            "preprocessor_description": preprocessor_description
+        }
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/create-preprocessor',
+            json=payoad
+        )
+
+        preprocessor_id = self.session.get_response_content(response)
+
+        return preprocessor_id
+    
+
+    def create_preprocessor_version(
+        self, preprocessor_id: str, pipeline: list, df: pd.DataFrame = None
+        ) -> str:
+        """ Creates a new preprocessor version and returns the version id.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            pipeline (xplainable.preprocessing.pipeline.Pipeline): pipeline
+        Returns:
+            int: The preprocessor version id
+        """
+        # Structure the stages and deltas
+        stages = []
+        deltas = []
+        if df is not None:
+            before = df.copy()
+            deltas.append({"start": json.loads(before.head(10).to_json(
+                orient='records'))})
+            delta_gen = pipeline.transform_generator(before)
+        for stage in pipeline.stages:
+            step = {
+                'feature': stage['feature'],
+                'name': stage['name'],
+                'params': stage['transformer'].__dict__
+            }
+            stages.append(step)
+            if df is not None:
+                after = delta_gen.__next__()
+                delta = get_df_delta(before.copy(), after.copy())
+                deltas.append(delta)
+                before = after.copy()
+        # Get current versions
+        versions = {
+                "xplainable_version": self.xplainable_version,
+                "python_version": self.python_version
+            }
+        # Create payload
+        payload = {
+            "stages": stages,
+            "deltas": deltas,
+            "versions": versions
+            }
+
+        # Create a new version and fetch id
+        url = (
+            f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/'
+            f'{preprocessor_id}/add-version'
+            )
+
+        response = self.session._session.post(url=url, json=payload)
+        version_id = self.session.get_response_content(response)
+        return version_id
+
+    def list_preprocessors(self) -> list:
+        """ Lists all preprocessors of the active user's team.
+        Returns:
+            dict: Dictionary of preprocessors.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors'
+            )
+        data = self.session.get_response_content(response)
+        [i.pop('user') for i in data]
+        return data
+    
+    # get_preprocessor
+    
+
+
+    def list_preprocessor_versions(self, preprocessor_id: int) -> list:
+        """ Lists all versions of a preprocessor.
+        Args:
+            preprocessor_id (int): The preprocessor id
+        Returns:
+            dict: Dictionary of preprocessor versions.
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions'
+            )
+
+        data = self.session.get_response_content(response)
+        [i.pop('user') for i in data]
+        return data
+
+    def load_preprocessor(
+            self, preprocessor_id: int, version_id: int,
+            gui_object: bool = False, response_only: bool = False):
+        """ Loads a preprocessor by preprocessor_id and version_id.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            version_id (int): The version id
+            response_only (bool, optional): Returns the preprocessor metadata.
+        Returns:
+            xplainable.preprocessing.pipeline.Pipeline: The loaded pipeline
+        """
+        def build_transformer(stage):
+            """Build transformer from metadata"""
+            if not hasattr(xtf, stage["name"]):
+                raise ValueError(f"{stage['name']} does not exist in the transformers module")
+            # Get transformer function
+            func = getattr(xtf, stage["name"])
+            return func(**stage['params'])
+
+        try:
+            preprocessor_response = self.session._session.get(
+                url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
+                )
+            response = self.session.get_response_content(preprocessor_response)
+            if response_only:
+                return response
+        except Exception as e:
+            raise ValueError(
+            f'Preprocessor with ID {preprocessor_id}:{version_id} does not exist')
+
+        stages = response['stages']
+        deltas = response['deltas']
+        pipeline = XPipeline()
+        pipeline.stages = [{"feature": i["feature"], "name": i["name"], \
+                "transformer": build_transformer(i)} for i in stages]
+
+        if not gui_object:
+            return pipeline
+        else:
+            from ..gui.screens.preprocessor import Preprocessor
+            pp = Preprocessor()
+            pp.pipeline = pipeline
+            pp.df_delta = deltas
+            pp.state = len(pipeline.stages)
+            return pp
+
+
+    def get_preprocessor_version_pipeline(self, preprocessor_id: str, version_id: str):
+        """ Returns the pipeline of a preprocessor version.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            version_id (int): The version id
+        Returns:
+            xplainable.preprocessing.pipeline.Pipeline: The pipeline
+        """
+        response = self.session._session.get(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/pipeline'
+            )
+        data = self.session.get_response_content(response)
+        return data
+
+    def delete_preprocessor_version(self, preprocessor_id: str, version_id: str):
+        """ Deletes a preprocessor version.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            version_id (int): The version id
+        Return:
+            json: A json response
+        """
+        response = self.session._session.delete(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}'
+            )
+        return response
+
+    def restore_preprocessor_version(self, preprocessor_id: str, version_id: str):
+        """ Restores a preprocessor version.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            version_id (int): The version id
+        Return:
+            json: A json response. 
+        """
+        response = self.session._session.put(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{version_id}/restore'
+            )
+        return response
+
+    def delete_preprocessor(self, preprocessor_id: str):
+        """ Deletes a preprocessor.
+        Args:
+            preprocessor_id (int): The preprocessor id
+        Return:
+            json: A json response
+        """
+        response = self.session._session.delete(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}'
+            )
+        return response
+
+    def restore_preprocessor(self, preprocessor_id: str):
+        """ Restores a preprocessor.
+        Args:
+            preprocessor_id (int): The preprocessor id
+        Return:
+            json: A json response
+        """
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/restore'
+            )
+        return response
+
+    def check_signature(self, preprocessor_id: str, preprocessor_version_id: str, model_id: str, model_version_id: str):
+        """ Checks the signature of a preprocessor version.
+        Args:
+            preprocessor_id (int): The preprocessor id
+            preprocessor_version_id (int): The preprocessor version id
+            model_id (int): The model id
+            model_version_id (int): The model version id
+        Return:
+            dict: A json response of signatures_match, pipeline_columns, model_columns.
+        """
+        
+        payload = {
+            'model_id': model_id,
+            'version_id': model_version_id
+        }
+        response = self.session._session.post(
+            url=f'{self.session.hostname}/v1/{self.session._ext}/preprocessors/{preprocessor_id}/versions/{preprocessor_version_id}/check-signature',
+            json=payload
+        )
+        output = self.session.get_response_content(response)
+        return output
+
+
+
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/utils/helpers.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/utils/helpers.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import json
-from .encoders import NpEncoder
-
-
-def get_df_delta(df1, df2):
-    """ Gets the delta between two dataframs"""
-    changed_features = [c for c in df1.columns.intersection(
-        df2.columns) if not df1[c].head(10).equals(df2[c].head(10))]
-
-    rows_changed = {}
-    for c in changed_features:
-        if c in df1.columns and c in df2.columns:
-            rows_changed[c] = (df1[c] != df2[c]).sum()
-        
-    output = {
-        "drop": [col for col in df1.columns if col not in df2.columns],
-        "add": [{"feature": col, "values": json.loads(
-        df2[col].head(10).to_json(orient='records'))} for col in \
-            df2.columns if col not in df1.columns],
-        "update": [{
-            "feature": col,
-            "values": json.loads(df2[col].head(10).to_json(
-                orient='records'))} for col in changed_features],
-        "rows_affected": json.loads(json.dumps(rows_changed, cls=NpEncoder))
-        }
-
+import json
+from .encoders import NpEncoder
+
+
+def get_df_delta(df1, df2):
+    """ Gets the delta between two dataframs"""
+    changed_features = [c for c in df1.columns.intersection(
+        df2.columns) if not df1[c].head(10).equals(df2[c].head(10))]
+
+    rows_changed = {}
+    for c in changed_features:
+        if c in df1.columns and c in df2.columns:
+            rows_changed[c] = (df1[c] != df2[c]).sum()
+        
+    output = {
+        "drop": [col for col in df1.columns if col not in df2.columns],
+        "add": [{"feature": col, "values": json.loads(
+        df2[col].head(10).to_json(orient='records'))} for col in \
+            df2.columns if col not in df1.columns],
+        "update": [{
+            "feature": col,
+            "values": json.loads(df2[col].head(10).to_json(
+                orient='records'))} for col in changed_features],
+        "rows_affected": json.loads(json.dumps(rows_changed, cls=NpEncoder))
+        }
+
     return output
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/utils/metrics.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/utils/metrics.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-""" Copyright Xplainable Pty Ltd, 2023"""
-
-import numpy as np
-from xplainable_client.client.utils.encoders import force_json_compliant
-from sklearn.metrics import (
-    roc_auc_score, matthews_corrcoef, log_loss, auc, mean_absolute_error,
-    mean_squared_error, r2_score, explained_variance_score,
-    mean_squared_log_error, mean_absolute_percentage_error)
-
-
-def calculate_classification_metrics(tp, fp, tn, fn):
-    precision = tp / (tp + fp + 1e-9)
-    recall = tp / (tp + fn + 1e-9)
-    specificity = tn / (tn + fp + 1e-9)
-    accuracy = (tp + tn) / (tp + tn + fp + fn)
-    f1 = 2 * (precision * recall) / (precision + recall + 1e-9)
-    
-    return {
-        "precision": precision,
-        "recall": recall,
-        "specificity": specificity,
-        "accuracy": accuracy,
-        "f1": f1
-        }
-
-def calculate_probability_bins(y_true, y_prob):
-    output_data = []
-
-    for cls in np.unique(y_true):
-        counts = np.bincount((y_prob[y_true == cls]*100).round().astype(int))
-
-        counts = np.concatenate(
-            [counts, np.zeros(101 - len(counts), dtype=int)])
-
-        output_data.append({
-            "class": cls,
-            "values": list(counts)
-        })
-    
-    return output_data
-
-
-def calculate_regression_bins(y_true, y_pred, bin_count):
-
-    # Ensure y_true and y_pred are NumPy arrays
-    y_true = np.array(y_true)
-    y_pred = np.array(y_pred)
-
-    # Calculate the min and max of the predicted values
-    min_val = min(y_pred)
-    max_val = max(y_pred)
-
-    # Define the bins
-    bins = np.linspace(min_val, max_val, bin_count+1)
-
-    # Assign each predicted value to a bin
-    true_bin_indices = np.digitize(y_true, bins)
-    pred_bin_indices = np.digitize(y_pred, bins)
-
-    # For each bin, count the number of true values
-    true_output = []
-    pred_output = []
-    for i in range(1, bin_count+1):
-        true_values_in_bin = y_true[true_bin_indices == i]
-        true_counts = len(true_values_in_bin)
-        true_output.append(true_counts)
-        
-        pred_values_in_bin = y_pred[pred_bin_indices == i]
-        pred_counts = len(pred_values_in_bin)
-        pred_output.append(pred_counts)
-    
-    output = [
-        {
-            "class": "true",
-            "values": true_output
-        },
-        {
-            "class": "pred",
-            "values": pred_output
-        }
-    ]
-    
-    return output
-
-
-def evaluate_classification(y_true, y_pred):
-    results = {}
-    thresholds = np.linspace(0, 1, 101)
-    
-    # TP, FP, TN, FN at each threshold value
-    metrics = []
-    for threshold in thresholds:
-        y_pred_thresholded = np.round(y_pred > threshold)
-        tp = np.sum((y_true == 1) & (y_pred_thresholded == 1))
-        fp = np.sum((y_true == 0) & (y_pred_thresholded == 1))
-        tn = np.sum((y_true == 0) & (y_pred_thresholded == 0))
-        fn = np.sum((y_true == 1) & (y_pred_thresholded == 0))
-        metrics.append({
-            "threshold": threshold,
-            "tp": tp,
-            "fp": fp,
-            "tn": tn,
-            "fn": fn
-            })
-    
-    # Compute other metrics based on TP, FP, TN, and FN
-    scores = []
-    for metric in metrics:
-        scores.append({
-            **metric, **calculate_classification_metrics(metric["tp"],
-            metric["fp"], metric["tn"], metric["fn"])})
-
-    results["scores"] = scores
-    
-    # ROC at each threshold value
-    fpr = [score["fp"] / (score["fp"] + score["tn"] + 1e-9) for score in scores]
-    tpr = [score["tp"] / (score["tp"] + score["fn"] + 1e-9) for score in scores]
-    results["roc"] = {"fpr": fpr, "tpr": tpr}
-    
-    # ROC-AUC
-    try:
-        results["roc_auc"] = roc_auc_score(y_true, y_pred)
-    except:
-        results["roc_auc"] = np.nan
-    
-    # Precision-recall curve
-    precision = [score["precision"] for score in scores]
-    recall = [score["recall"] for score in scores]
-    results["precision_recall_curve"] = {
-        "precision": precision, "recall": recall}
-    
-    # AUC-PR
-    try:
-        results["auc_pr"] = auc(recall, precision)
-    except:
-        results["auc_pr"] = np.nan
-    
-    # Matthews Correlation Coefficient (MCC)
-    try:
-        results["mcc"] = matthews_corrcoef(y_true, np.round(y_pred))
-    except:
-        results["mcc"] = np.nan
-    
-    # Log Loss (Cross-Entropy Loss)
-    try:
-        results["log_loss"] = log_loss(y_true, y_pred)
-    except:
-        results["log_loss"] = np.nan
-
-    # Calculates the number of predictions in each probability bin
-    results["probability_bins"] = calculate_probability_bins(y_true, y_pred)
-
-    return force_json_compliant(results)
-
-
-def evaluate_regression(y_true, y_pred):
-    results = {
-        "charts": {
-            'true': list(y_true.values if len(y_true) < 10000 else y_true[:10000].values),
-            'prediction': list(y_pred if len(y_pred) < 10000 else y_pred[:10000]),
-        }
-    }
-    
-    # Mean Absolute Error (MAE)
-    try:
-        results["mae"] = mean_absolute_error(y_true, y_pred)
-    except:
-        results["mae"] = np.nan
-    
-    # Mean Squared Error (MSE)
-    try:
-        results["mse"] = mean_squared_error(y_true, y_pred)
-    except:
-        results["mse"] = np.nan
-    
-    # Root Mean Squared Error (RMSE)
-    try:
-        results["rmse"] = np.sqrt(mean_squared_error(y_true, y_pred))
-    except:
-        results["rmse"] = np.nan
-
-    # R-squared (R2) Score
-    try:
-        results["r2_score"] = r2_score(y_true, y_pred)
-    except:
-        results["r2_score"] = np.nan
-    
-    # Explained Variance Score
-    try:
-        results["explained_variance_score"] = explained_variance_score(
-            y_true, y_pred)
-    except:
-        results["explained_variance_score"] = np.nan
-    
-    # Mean Squared Logarithmic Error (MSLE)
-    try:
-        results["msle"] = mean_squared_log_error(y_true, y_pred)
-    except:
-        results["msle"] = np.nan
-    
-    # Root Mean Squared Logarithmic Error (RMSLE)
-    try:
-        results["rmsle"] = np.sqrt(mean_squared_log_error(y_true, y_pred))
-    except:
-        results["rmsle"] = np.nan
-    
-    # Mean Absolute Percentage Error (MAPE)
-    try:
-        results["mape"] = mean_absolute_percentage_error(y_true, y_pred)
-    except:
-        results["mape"] = np.nan
-
-    results["prediction_bins"] = calculate_regression_bins(y_true, y_pred, 100)
-    results["observed_min"] = np.nanmin(y_true)
-    results["observed_max"] = np.nanmax(y_true)
-    
-    return force_json_compliant(results)
+""" Copyright Xplainable Pty Ltd, 2023"""
+
+import numpy as np
+from xplainable_client.client.utils.encoders import force_json_compliant
+from sklearn.metrics import (
+    roc_auc_score, matthews_corrcoef, log_loss, auc, mean_absolute_error,
+    mean_squared_error, r2_score, explained_variance_score,
+    mean_squared_log_error, mean_absolute_percentage_error)
+
+
+def calculate_classification_metrics(tp, fp, tn, fn):
+    precision = tp / (tp + fp + 1e-9)
+    recall = tp / (tp + fn + 1e-9)
+    specificity = tn / (tn + fp + 1e-9)
+    accuracy = (tp + tn) / (tp + tn + fp + fn)
+    f1 = 2 * (precision * recall) / (precision + recall + 1e-9)
+    
+    return {
+        "precision": precision,
+        "recall": recall,
+        "specificity": specificity,
+        "accuracy": accuracy,
+        "f1": f1
+        }
+
+def calculate_probability_bins(y_true, y_prob):
+    output_data = []
+
+    for cls in np.unique(y_true):
+        counts = np.bincount((y_prob[y_true == cls]*100).round().astype(int))
+
+        counts = np.concatenate(
+            [counts, np.zeros(101 - len(counts), dtype=int)])
+
+        output_data.append({
+            "class": cls,
+            "values": list(counts)
+        })
+    
+    return output_data
+
+
+def calculate_regression_bins(y_true, y_pred, bin_count):
+
+    # Ensure y_true and y_pred are NumPy arrays
+    y_true = np.array(y_true)
+    y_pred = np.array(y_pred)
+
+    # Calculate the min and max of the predicted values
+    min_val = min(y_pred)
+    max_val = max(y_pred)
+
+    # Define the bins
+    bins = np.linspace(min_val, max_val, bin_count+1)
+
+    # Assign each predicted value to a bin
+    true_bin_indices = np.digitize(y_true, bins)
+    pred_bin_indices = np.digitize(y_pred, bins)
+
+    # For each bin, count the number of true values
+    true_output = []
+    pred_output = []
+    for i in range(1, bin_count+1):
+        true_values_in_bin = y_true[true_bin_indices == i]
+        true_counts = len(true_values_in_bin)
+        true_output.append(true_counts)
+        
+        pred_values_in_bin = y_pred[pred_bin_indices == i]
+        pred_counts = len(pred_values_in_bin)
+        pred_output.append(pred_counts)
+    
+    output = [
+        {
+            "class": "true",
+            "values": true_output
+        },
+        {
+            "class": "pred",
+            "values": pred_output
+        }
+    ]
+    
+    return output
+
+
+def evaluate_classification(y_true, y_pred):
+    results = {}
+    thresholds = np.linspace(0, 1, 101)
+    
+    # TP, FP, TN, FN at each threshold value
+    metrics = []
+    for threshold in thresholds:
+        y_pred_thresholded = np.round(y_pred > threshold)
+        tp = np.sum((y_true == 1) & (y_pred_thresholded == 1))
+        fp = np.sum((y_true == 0) & (y_pred_thresholded == 1))
+        tn = np.sum((y_true == 0) & (y_pred_thresholded == 0))
+        fn = np.sum((y_true == 1) & (y_pred_thresholded == 0))
+        metrics.append({
+            "threshold": threshold,
+            "tp": tp,
+            "fp": fp,
+            "tn": tn,
+            "fn": fn
+            })
+    
+    # Compute other metrics based on TP, FP, TN, and FN
+    scores = []
+    for metric in metrics:
+        scores.append({
+            **metric, **calculate_classification_metrics(metric["tp"],
+            metric["fp"], metric["tn"], metric["fn"])})
+
+    results["scores"] = scores
+    
+    # ROC at each threshold value
+    fpr = [score["fp"] / (score["fp"] + score["tn"] + 1e-9) for score in scores]
+    tpr = [score["tp"] / (score["tp"] + score["fn"] + 1e-9) for score in scores]
+    results["roc"] = {"fpr": fpr, "tpr": tpr}
+    
+    # ROC-AUC
+    try:
+        results["roc_auc"] = roc_auc_score(y_true, y_pred)
+    except:
+        results["roc_auc"] = np.nan
+    
+    # Precision-recall curve
+    precision = [score["precision"] for score in scores]
+    recall = [score["recall"] for score in scores]
+    results["precision_recall_curve"] = {
+        "precision": precision, "recall": recall}
+    
+    # AUC-PR
+    try:
+        results["auc_pr"] = auc(recall, precision)
+    except:
+        results["auc_pr"] = np.nan
+    
+    # Matthews Correlation Coefficient (MCC)
+    try:
+        results["mcc"] = matthews_corrcoef(y_true, np.round(y_pred))
+    except:
+        results["mcc"] = np.nan
+    
+    # Log Loss (Cross-Entropy Loss)
+    try:
+        results["log_loss"] = log_loss(y_true, y_pred)
+    except:
+        results["log_loss"] = np.nan
+
+    # Calculates the number of predictions in each probability bin
+    results["probability_bins"] = calculate_probability_bins(y_true, y_pred)
+
+    return force_json_compliant(results)
+
+
+def evaluate_regression(y_true, y_pred):
+    results = {
+        "charts": {
+            'true': list(y_true.values if len(y_true) < 10000 else y_true[:10000].values),
+            'prediction': list(y_pred if len(y_pred) < 10000 else y_pred[:10000]),
+        }
+    }
+    
+    # Mean Absolute Error (MAE)
+    try:
+        results["mae"] = mean_absolute_error(y_true, y_pred)
+    except:
+        results["mae"] = np.nan
+    
+    # Mean Squared Error (MSE)
+    try:
+        results["mse"] = mean_squared_error(y_true, y_pred)
+    except:
+        results["mse"] = np.nan
+    
+    # Root Mean Squared Error (RMSE)
+    try:
+        results["rmse"] = np.sqrt(mean_squared_error(y_true, y_pred))
+    except:
+        results["rmse"] = np.nan
+
+    # R-squared (R2) Score
+    try:
+        results["r2_score"] = r2_score(y_true, y_pred)
+    except:
+        results["r2_score"] = np.nan
+    
+    # Explained Variance Score
+    try:
+        results["explained_variance_score"] = explained_variance_score(
+            y_true, y_pred)
+    except:
+        results["explained_variance_score"] = np.nan
+    
+    # Mean Squared Logarithmic Error (MSLE)
+    try:
+        results["msle"] = mean_squared_log_error(y_true, y_pred)
+    except:
+        results["msle"] = np.nan
+    
+    # Root Mean Squared Logarithmic Error (RMSLE)
+    try:
+        results["rmsle"] = np.sqrt(mean_squared_log_error(y_true, y_pred))
+    except:
+        results["rmsle"] = np.nan
+    
+    # Mean Absolute Percentage Error (MAPE)
+    try:
+        results["mape"] = mean_absolute_percentage_error(y_true, y_pred)
+    except:
+        results["mape"] = np.nan
+
+    results["prediction_bins"] = calculate_regression_bins(y_true, y_pred, 100)
+    results["observed_min"] = np.nanmin(y_true)
+    results["observed_max"] = np.nanmax(y_true)
+    
+    return force_json_compliant(results)
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/utils/model_parsers.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/utils/model_parsers.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import numpy as np
-from xplainable.utils.dualdict import TargetMap, FeatureMap
-from xplainable.core.ml.classification import PartitionedClassifier, XClassifier
-from xplainable.core.ml.regression import PartitionedRegressor, XRegressor
-from .encoders import profile_parse
-import json
-
-def parse_classifier_response(response, model=None):
-    if response['model_type'] != 'binary_classification':
-        raise ValueError(f'Model is not a binary classification model')
-
-    if model is None:
-        partitioned_model = PartitionedClassifier(response['partition_on'])
-    else:
-        partitioned_model = model
-
-    for p in response['partitions']:
-        model = XClassifier()
-
-        model._profile = np.array([
-            np.array(i) for i in json.loads(p['profile'])], dtype=object)
-
-        model._profile = profile_parse(model._profile)
-
-        model._calibration_map = {
-            int(i): v for i, v in p['calibration_map'].items()}
-
-        model._support_map = {
-            int(i): v for i, v in p['support_map'].items()}
-
-        model.base_value = p['base_value']
-        model.target_map = TargetMap({int(i): v for i, v in p['target_map'].items()}, True)
-        model.feature_map = {k: FeatureMap(v) for k, v in p['feature_map'].items()}
-
-        model.columns = p['columns']
-        model.id_columns = p['id_columns']
-
-        model.categorical_columns = p['feature_map'].keys()
-        model.numeric_columns = [c for c in model.columns if c not in model.categorical_columns]
-
-        if 'constructs' in p:
-            model.constructs_from_json(p['constructs'])
-
-        model.category_meta = {
-            i: {ii: {int(float(k)): v for k, v in vv.items()} for ii, vv \
-                in v.items()} for i, v in p['category_meta'].items()}
-
-        partitioned_model.add_partition(model, p['partition'])
-
-    return partitioned_model
-
-def parse_regressor_response(response, model=None):
-    if model is None:
-        partitioned_model = PartitionedRegressor(response['partition_on'])
-    else:
-        partitioned_model = model
-
-    for p in response['partitions']:
-        model = XRegressor()
-        model._profile = np.array([np.array(i) for i in json.loads(p['profile'])])
-        model._profile = profile_parse(model._profile)
-        model.base_value = p['base_value']
-        model.feature_map = {k: FeatureMap(v) for k, v in p['feature_map'].items()}
-        # model.parameters = ConstructorParams(p['parameters'])
-
-        model.columns = p['columns']
-        model.id_columns = p['id_columns']
-
-        model.categorical_columns = p['feature_map'].keys()
-        model.numeric_columns = [c for c in model.columns if c not in model.categorical_columns]
-
-        if 'constructs' in p:
-            model.constructs_from_json(p['constructs'])
-
-        model.category_meta = {
-            i: {ii: {int(float(k)): v for k, v in vv.items()} for ii, vv \
-                in v.items()} for i, v in p['category_meta'].items()}
-
-        partitioned_model.add_partition(model, p['partition'])
-
+import numpy as np
+from xplainable.utils.dualdict import TargetMap, FeatureMap
+from xplainable.core.ml.classification import PartitionedClassifier, XClassifier
+from xplainable.core.ml.regression import PartitionedRegressor, XRegressor
+from .encoders import profile_parse
+import json
+
+def parse_classifier_response(response, model=None):
+    if response['model_type'] != 'binary_classification':
+        raise ValueError(f'Model is not a binary classification model')
+
+    if model is None:
+        partitioned_model = PartitionedClassifier(response['partition_on'])
+    else:
+        partitioned_model = model
+
+    for p in response['partitions']:
+        model = XClassifier()
+
+        model._profile = np.array([
+            np.array(i) for i in json.loads(p['profile'])], dtype=object)
+
+        model._profile = profile_parse(model._profile)
+
+        model._calibration_map = {
+            int(i): v for i, v in p['calibration_map'].items()}
+
+        model._support_map = {
+            int(i): v for i, v in p['support_map'].items()}
+
+        model.base_value = p['base_value']
+        model.target_map = TargetMap({int(i): v for i, v in p['target_map'].items()}, True)
+        model.feature_map = {k: FeatureMap(v) for k, v in p['feature_map'].items()}
+
+        model.columns = p['columns']
+        model.id_columns = p['id_columns']
+
+        model.categorical_columns = p['feature_map'].keys()
+        model.numeric_columns = [c for c in model.columns if c not in model.categorical_columns]
+
+        if 'constructs' in p:
+            model.constructs_from_json(p['constructs'])
+
+        model.category_meta = {
+            i: {ii: {int(float(k)): v for k, v in vv.items()} for ii, vv \
+                in v.items()} for i, v in p['category_meta'].items()}
+
+        partitioned_model.add_partition(model, p['partition'])
+
+    return partitioned_model
+
+def parse_regressor_response(response, model=None):
+    if model is None:
+        partitioned_model = PartitionedRegressor(response['partition_on'])
+    else:
+        partitioned_model = model
+
+    for p in response['partitions']:
+        model = XRegressor()
+        model._profile = np.array([np.array(i) for i in json.loads(p['profile'])])
+        model._profile = profile_parse(model._profile)
+        model.base_value = p['base_value']
+        model.feature_map = {k: FeatureMap(v) for k, v in p['feature_map'].items()}
+        # model.parameters = ConstructorParams(p['parameters'])
+
+        model.columns = p['columns']
+        model.id_columns = p['id_columns']
+
+        model.categorical_columns = p['feature_map'].keys()
+        model.numeric_columns = [c for c in model.columns if c not in model.categorical_columns]
+
+        if 'constructs' in p:
+            model.constructs_from_json(p['constructs'])
+
+        model.category_meta = {
+            i: {ii: {int(float(k)): v for k, v in vv.items()} for ii, vv \
+                in v.items()} for i, v in p['category_meta'].items()}
+
+        partitioned_model.add_partition(model, p['partition'])
+
     return partitioned_model
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client/client/utils/scanner.py` & `xplainable-client-1.2.4.post4/xplainable_client/client/utils/scanner.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,386 +1,386 @@
-""" Copyright Xplainable Pty Ltd, 2023"""
-
-from pandas.api.types import (is_string_dtype, is_datetime64_dtype,
-                              is_numeric_dtype, is_bool_dtype)
-import pandas as pd
-import numpy as np
-from tqdm.auto import tqdm
-
-
-#Decorator to catch zero division errors
-def catch_zero_division(return_value=0):
-    """
-    A decorator that catches division by zero errors in methods and returns a predefined value.
-
-    Args:
-        return_value: The value to return if a ZeroDivisionError is caught. Defaults to np.nan.
-
-    Returns:
-        The wrapped function's return value, or `return_value` if a ZeroDivisionError is caught.
-    """
-    def decorator(func):
-        def wrapper(*args, **kwargs):
-            try:
-                return func(*args, **kwargs)
-            except ZeroDivisionError:
-                return return_value
-        return wrapper
-    return decorator
-
-
-class XScan:
-    """ Scans a dataframe and returns a profile of each feature."""
-
-    def __init__(self):
-        self.profile = {}
-        self.target = None
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _cardinality(ser):
-        """ Measures the cardinality of a feature.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing a single feature.
-
-        Returns:
-            float: The cardinality score
-        """
-
-        # Drop NA for cardinality calculation
-        ser = ser.dropna()
-
-        # If the series is empty after dropping NA, return 0 or an appropriate value
-        if len(ser) == 0:
-            return 0.0
-
-        return round(ser.nunique() / len(ser), 4)
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _is_mixed_case(ser):
-        """ Percentage of a text feature that contains mixed cases.
-
-        Args:
-            ser (pd.Series): The series to be analysed.
-
-        Returns:
-            bool: True if contains mixed cases else False.
-        """
-
-        def _is_mixed(s):
-            """ Checks if a string contains both numbers and letters.
-
-            Args:
-                s (str): The string to be checked.
-
-            Returns:
-                bool: True if the string is mixed else False.
-            """
-
-            is_mixed = any(char.isupper() for char in str(s).strip()) and \
-                not all(char.isupper() for char in str(s).strip())
-
-            return is_mixed
-
-        # Check if cases are mixed
-        ser = ser.copy().dropna()
-
-        return ser.apply(_is_mixed).mean()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _mixed_char_num(ser):
-        """ Percentage of a text feature that contains numbers and letters.
-
-        Args:
-            ser (pd.Series): The series to be analysed.
-
-        Returns:
-            float: Percentage of feature that contains numbers and letters.
-        """
-
-        def _is_mixed(s):
-            """ Checks if a string contains both numbers and letters.
-
-            Args:
-                s (str): The string to be checked.
-
-            Returns:
-                bool: True if the string is mixed else False.
-            """
-
-            is_mixed = any(char.isdigit() for char in str(s).strip()) and \
-                not all(char.isdigit() for char in str(s).strip())
-
-            return is_mixed
-        
-        ser = ser.copy().dropna()
-
-        return ser.apply(_is_mixed).mean()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _skewness_score(ser):
-        """ Calculates a numeric feature's skewness.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: The skewness score.
-        """
-
-        return ser.skew()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _variance_score(ser):
-        """ Calculates a numeric feature's variance.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: The skewness score.
-        """
-
-        return ser.var()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _kurtosis_score(ser):
-        """ Calculates a numeric feature's kurtosis.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: The kurtosis score.
-        """
-
-        return ser.kurtosis()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _unique_values(ser):
-        """ Counts unique values of feature.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: Number of unique values.
-        """
-
-        return ser.nunique()
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _is_missing(ser):
-        """ Calculates the pct of missing values
-
-        Args:
-            ser (pd.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: pct of missing values
-        """
-        return ser.isna().sum() / len(ser)
-
-    @staticmethod
-    @catch_zero_division(return_value=0)
-    def _category_imbalance(ser):
-        """ Scores a categorical feature's category imbalance.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing the feature.
-
-        Returns:
-            float: The imbalance score.
-        """
-
-        # attain the pct distribution of each category
-        c = ser.value_counts() / len(ser)
-
-        # Calculate the pct of each cat if perfectly imbalanced
-        p = 1 / len(c)
-
-        # Get the mean absolute difference from p
-        mad = (abs(c - p) / p).mean()
-
-        return mad
-
-    def _detect_type(self, ser):
-        """ Detects the machine learning type of a feature.
-
-        Args:
-            ser (Pandas.Series): Pandas Series containing a single feature.
-
-        Returns:
-            str: The feature type.
-        """
-
-        cardinality = self._cardinality(ser)
-        missing_pct = self._is_missing(ser)
-
-        if is_numeric_dtype(ser):
-
-            if cardinality == 1 and missing_pct == 0:
-                return 'id'
-
-            else:
-                return 'numeric'
-
-        elif is_string_dtype(ser):
-            if cardinality == 1:
-
-                if not any(ser.str.contains(" ")):
-                    return 'id'
-
-                else:
-                    return 'nlp'
-
-            elif cardinality > 0.9:
-                return 'nlp'
-
-            else:
-                return 'categorical'
-
-        elif is_datetime64_dtype(ser):
-            return 'date'
-
-        else:
-            return 'categorical'
-
-    def _series_is_empty(self, ser):
-        if len(ser) == 0:
-            return True
-        if ser.isna().sum() / len(ser) == 1:
-            return True
-        else:
-            return False
-
-    def _scan_numeric_feature(self, ser):
-
-        if self._series_is_empty(ser):
-            return {
-                'type': 'empty',
-                'missing_pct': 1
-                }
-
-        ser_type = self._detect_type(ser)
-        if ser_type == 'id':
-            return {
-                'type': ser_type,
-                'missing_pct': 0
-                }
-
-        sub_profile = {
-            'type': ser_type,
-            'missing_pct': self._is_missing(ser),
-            'min': np.nanmin(ser),
-            '25%': ser.quantile(0.25),
-            'mean': np.nanmean(ser),
-            'median': np.nanmedian(ser),
-            '75%': ser.quantile(0.75),
-            'max': np.nanmax(ser),
-            'std': ser.std(),
-            'skewness': self._skewness_score(ser),
-            'kurtosis': self._kurtosis_score(ser),
-            'variance': self._variance_score(ser)
-        }
-
-        return sub_profile
-
-    def _scan_nlp_feature(self, ser):
-
-        sub_profile = {
-            'type': 'nlp',
-            'missing_pct': self._is_missing(ser),
-            'mixed_case': self._is_mixed_case(ser),
-            'mixed_type': self._mixed_char_num(ser)
-        }
-
-        return sub_profile
-
-    def _scan_categorical_feature(self, ser):
-
-        if self._series_is_empty(ser):
-            return {
-                'type': 'empty',
-                'missing_pct': 1
-                }
-
-        ser_type = self._detect_type(ser)
-        if ser_type == 'id':
-            return {
-                'type': ser_type,
-                'missing_pct': 0
-                }
-
-        elif ser_type == 'nlp':
-            return self._scan_nlp_feature(ser)
-
-        sub_profile = {
-            'type': ser_type,
-            'missing_pct': self._is_missing(ser),
-            'nunique': self._unique_values(ser),
-            'mode': ser.mode().values[0] if not ser.mode().empty else np.nan,
-            'cardinality': self._cardinality(ser),
-            'mixed_case': self._is_mixed_case(ser),
-            'mixed_type': self._mixed_char_num(ser),
-            'category_imbalance': self._category_imbalance(ser)
-        }
-
-        return sub_profile
-
-    def _scan_date_feature(self, ser):
-
-        if self._series_is_empty(ser):
-            return {
-                'type': 'empty',
-                'missing_pct': 1
-                }
-
-        sub_profile = {
-            'type': self._detect_type(ser),
-            'missing_pct': self._is_missing(ser)
-        }
-
-        return sub_profile
-
-    def _scan_feature(self, ser):
-
-        if is_bool_dtype(ser):
-            ser = ser.astype(str)
-            sub_profile = self._scan_categorical_feature(ser)
-
-        elif is_numeric_dtype(ser):
-                sub_profile = self._scan_numeric_feature(ser)
-                
-        elif is_string_dtype(ser):
-            sub_profile = self._scan_categorical_feature(ser)
-
-        elif is_datetime64_dtype(ser):
-            sub_profile = self._scan_date_feature(ser)
-
-        else:
-            raise TypeError(f"Feature {ser.name} has unknown type")
-
-        return sub_profile
-
-    def scan(self, df, target=None):
-        if target:
-            if target not in df.columns:
-                raise ValueError(f"{target} not in df")
-            df = df.drop(columns=[target])
-
-        # Iterate over each column and check for non-NaN existence before scanning
-        for col in tqdm(list(df.columns)):
-            if df[col].isna().all():
-                print(f"Skipping column {col} because it is completely NaN.")
-                continue  # Skip this column as it's entirely NaN
-
-            # Proceed with scanning non-NaN columns
-            self.profile[col] = self._scan_feature(df[col])
+""" Copyright Xplainable Pty Ltd, 2023"""
+
+from pandas.api.types import (is_string_dtype, is_datetime64_dtype,
+                              is_numeric_dtype, is_bool_dtype)
+import pandas as pd
+import numpy as np
+from tqdm.auto import tqdm
+
+
+#Decorator to catch zero division errors
+def catch_zero_division(return_value=0):
+    """
+    A decorator that catches division by zero errors in methods and returns a predefined value.
+
+    Args:
+        return_value: The value to return if a ZeroDivisionError is caught. Defaults to np.nan.
+
+    Returns:
+        The wrapped function's return value, or `return_value` if a ZeroDivisionError is caught.
+    """
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except ZeroDivisionError:
+                return return_value
+        return wrapper
+    return decorator
+
+
+class XScan:
+    """ Scans a dataframe and returns a profile of each feature."""
+
+    def __init__(self):
+        self.profile = {}
+        self.target = None
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _cardinality(ser):
+        """ Measures the cardinality of a feature.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing a single feature.
+
+        Returns:
+            float: The cardinality score
+        """
+
+        # Drop NA for cardinality calculation
+        ser = ser.dropna()
+
+        # If the series is empty after dropping NA, return 0 or an appropriate value
+        if len(ser) == 0:
+            return 0.0
+
+        return round(ser.nunique() / len(ser), 4)
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _is_mixed_case(ser):
+        """ Percentage of a text feature that contains mixed cases.
+
+        Args:
+            ser (pd.Series): The series to be analysed.
+
+        Returns:
+            bool: True if contains mixed cases else False.
+        """
+
+        def _is_mixed(s):
+            """ Checks if a string contains both numbers and letters.
+
+            Args:
+                s (str): The string to be checked.
+
+            Returns:
+                bool: True if the string is mixed else False.
+            """
+
+            is_mixed = any(char.isupper() for char in str(s).strip()) and \
+                not all(char.isupper() for char in str(s).strip())
+
+            return is_mixed
+
+        # Check if cases are mixed
+        ser = ser.copy().dropna()
+
+        return ser.apply(_is_mixed).mean()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _mixed_char_num(ser):
+        """ Percentage of a text feature that contains numbers and letters.
+
+        Args:
+            ser (pd.Series): The series to be analysed.
+
+        Returns:
+            float: Percentage of feature that contains numbers and letters.
+        """
+
+        def _is_mixed(s):
+            """ Checks if a string contains both numbers and letters.
+
+            Args:
+                s (str): The string to be checked.
+
+            Returns:
+                bool: True if the string is mixed else False.
+            """
+
+            is_mixed = any(char.isdigit() for char in str(s).strip()) and \
+                not all(char.isdigit() for char in str(s).strip())
+
+            return is_mixed
+        
+        ser = ser.copy().dropna()
+
+        return ser.apply(_is_mixed).mean()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _skewness_score(ser):
+        """ Calculates a numeric feature's skewness.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: The skewness score.
+        """
+
+        return ser.skew()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _variance_score(ser):
+        """ Calculates a numeric feature's variance.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: The skewness score.
+        """
+
+        return ser.var()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _kurtosis_score(ser):
+        """ Calculates a numeric feature's kurtosis.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: The kurtosis score.
+        """
+
+        return ser.kurtosis()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _unique_values(ser):
+        """ Counts unique values of feature.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: Number of unique values.
+        """
+
+        return ser.nunique()
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _is_missing(ser):
+        """ Calculates the pct of missing values
+
+        Args:
+            ser (pd.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: pct of missing values
+        """
+        return ser.isna().sum() / len(ser)
+
+    @staticmethod
+    @catch_zero_division(return_value=0)
+    def _category_imbalance(ser):
+        """ Scores a categorical feature's category imbalance.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing the feature.
+
+        Returns:
+            float: The imbalance score.
+        """
+
+        # attain the pct distribution of each category
+        c = ser.value_counts() / len(ser)
+
+        # Calculate the pct of each cat if perfectly imbalanced
+        p = 1 / len(c)
+
+        # Get the mean absolute difference from p
+        mad = (abs(c - p) / p).mean()
+
+        return mad
+
+    def _detect_type(self, ser):
+        """ Detects the machine learning type of a feature.
+
+        Args:
+            ser (Pandas.Series): Pandas Series containing a single feature.
+
+        Returns:
+            str: The feature type.
+        """
+
+        cardinality = self._cardinality(ser)
+        missing_pct = self._is_missing(ser)
+
+        if is_numeric_dtype(ser):
+
+            if cardinality == 1 and missing_pct == 0:
+                return 'id'
+
+            else:
+                return 'numeric'
+
+        elif is_string_dtype(ser):
+            if cardinality == 1:
+
+                if not any(ser.str.contains(" ")):
+                    return 'id'
+
+                else:
+                    return 'nlp'
+
+            elif cardinality > 0.9:
+                return 'nlp'
+
+            else:
+                return 'categorical'
+
+        elif is_datetime64_dtype(ser):
+            return 'date'
+
+        else:
+            return 'categorical'
+
+    def _series_is_empty(self, ser):
+        if len(ser) == 0:
+            return True
+        if ser.isna().sum() / len(ser) == 1:
+            return True
+        else:
+            return False
+
+    def _scan_numeric_feature(self, ser):
+
+        if self._series_is_empty(ser):
+            return {
+                'type': 'empty',
+                'missing_pct': 1
+                }
+
+        ser_type = self._detect_type(ser)
+        if ser_type == 'id':
+            return {
+                'type': ser_type,
+                'missing_pct': 0
+                }
+
+        sub_profile = {
+            'type': ser_type,
+            'missing_pct': self._is_missing(ser),
+            'min': np.nanmin(ser),
+            '25%': ser.quantile(0.25),
+            'mean': np.nanmean(ser),
+            'median': np.nanmedian(ser),
+            '75%': ser.quantile(0.75),
+            'max': np.nanmax(ser),
+            'std': ser.std(),
+            'skewness': self._skewness_score(ser),
+            'kurtosis': self._kurtosis_score(ser),
+            'variance': self._variance_score(ser)
+        }
+
+        return sub_profile
+
+    def _scan_nlp_feature(self, ser):
+
+        sub_profile = {
+            'type': 'nlp',
+            'missing_pct': self._is_missing(ser),
+            'mixed_case': self._is_mixed_case(ser),
+            'mixed_type': self._mixed_char_num(ser)
+        }
+
+        return sub_profile
+
+    def _scan_categorical_feature(self, ser):
+
+        if self._series_is_empty(ser):
+            return {
+                'type': 'empty',
+                'missing_pct': 1
+                }
+
+        ser_type = self._detect_type(ser)
+        if ser_type == 'id':
+            return {
+                'type': ser_type,
+                'missing_pct': 0
+                }
+
+        elif ser_type == 'nlp':
+            return self._scan_nlp_feature(ser)
+
+        sub_profile = {
+            'type': ser_type,
+            'missing_pct': self._is_missing(ser),
+            'nunique': self._unique_values(ser),
+            'mode': ser.mode().values[0] if not ser.mode().empty else np.nan,
+            'cardinality': self._cardinality(ser),
+            'mixed_case': self._is_mixed_case(ser),
+            'mixed_type': self._mixed_char_num(ser),
+            'category_imbalance': self._category_imbalance(ser)
+        }
+
+        return sub_profile
+
+    def _scan_date_feature(self, ser):
+
+        if self._series_is_empty(ser):
+            return {
+                'type': 'empty',
+                'missing_pct': 1
+                }
+
+        sub_profile = {
+            'type': self._detect_type(ser),
+            'missing_pct': self._is_missing(ser)
+        }
+
+        return sub_profile
+
+    def _scan_feature(self, ser):
+
+        if is_bool_dtype(ser):
+            ser = ser.astype(str)
+            sub_profile = self._scan_categorical_feature(ser)
+
+        elif is_numeric_dtype(ser):
+                sub_profile = self._scan_numeric_feature(ser)
+                
+        elif is_string_dtype(ser):
+            sub_profile = self._scan_categorical_feature(ser)
+
+        elif is_datetime64_dtype(ser):
+            sub_profile = self._scan_date_feature(ser)
+
+        else:
+            raise TypeError(f"Feature {ser.name} has unknown type")
+
+        return sub_profile
+
+    def scan(self, df, target=None):
+        if target:
+            if target not in df.columns:
+                raise ValueError(f"{target} not in df")
+            df = df.drop(columns=[target])
+
+        # Iterate over each column and check for non-NaN existence before scanning
+        for col in tqdm(list(df.columns)):
+            if df[col].isna().all():
+                print(f"Skipping column {col} because it is completely NaN.")
+                continue  # Skip this column as it's entirely NaN
+
+            # Proceed with scanning non-NaN columns
+            self.profile[col] = self._scan_feature(df[col])
```

### Comparing `xplainable_client-1.2.4.post3/xplainable_client.egg-info/PKG-INFO` & `xplainable-client-1.2.4.post4/xplainable_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,804 +1,794 @@
-Metadata-Version: 2.1
-Name: xplainable-client
-Version: 1.2.4.post3
-Summary: The client for persisting and deploying models to Xplainable cloud.
-Author: xplainable pty ltd
-Author-email: xplainable pty ltd <contact@xplainable.io>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ipywidgets==8.0.6
-Requires-Dist: numpy>=1.26
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pyperclip==1.8.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: scikit_learn
-Requires-Dist: setuptools
-Requires-Dist: urllib3==2.2.0
-Requires-Dist: xplainable==1.2.4
-
-
-<div align="center">
-<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
-<h1 align="center">xplainable</h1>
-<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
-    
-**Xplainable** makes tabular machine learning transparent, fair, and actionable.
-</div>
-
-## Why Was Xplainable Created?
-In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
-
-To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
-
-
-## Xplainable Cloud
-This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
-
-### Preprocessing with Xplainable Cloud
-Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
-
-
-```python
-import xplainable as xp
-import os
-from xplainable_client import Client
-
-#Initialising the client
-XClient = Client(api_key=os.environ['XP_API_KEY'])
-
-#Creating a Preprocessor ID
-preprocessor_id = XClient.create_preprocessor_id(
-    preprocessor_name="Preprocessor Name",
-    preprocessor_description="Preprocessor Description",
-)
-
-#Creating a Preprocessor Version
-preprocessor_version = XClient.create_preprocessor_version(
-    preprocessor_id, #preprocessor_id,
-    pipeline, # <-- Pass the pipeline
-    df # <-- Pass the raw dataframe
-)
-
-#Loading the Preprocessor Client
-pp_cloud = XClient.load_preprocessor(
-    preprocessor_id,
-    preprocessor_version["version_id"],
-    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
-    )
-```
-
-### Modelling with Xplainable Cloud
-
-After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
-
-```python
-
-#Creating a Model Id
-model_id = XClient.create_model_id(
-    model,
-    model_name="Model Name",
-    model_description='Model Description'
-)
-
-#Creating a Model Version
-version_id = XClient.create_model_version(
-    model,
-    model_id,
-    X_train,
-    y_train
-)
-
-```
-
-### Deployments with Xplainable Cloud
-Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
-
-```python 
-#Creating a Model Deployment
-deployment = XClient.deploy(
-    hostname="https://inference.xplainable.io", 
-    model_id=model_id, 
-    version_id=version_id 
-)
-
-#Activating the Deployment
-XClient.activate_deployment(deployment['deployment_id'])
-
-#Generating an API Key
-deploy_key = XClient.generate_deploy_key(
-    'API Key Name', 
-    deployment['deployment_id'], 
-    7 #-> Days until expiration
-    )
-
-#Hitting the endpoint
-response = requests.post(
-    url="https://inference.xplainable.io/v1/predict",
-    headers={'api_key': deploy_key['deploy_key']},
-    json=body
-)
-
-#Obtaining the value response
-value = response.json()
-```
-
-<div align="center">
-<br></br>
-<br></br>
-Thanks for trying xplainable!
-<br></br>
-<strong>Made with ❤️ in Australia</strong>
-<br></br>
-<hr>
-&copy; copyright xplainable pty ltd
-</div>
-
-
+Metadata-Version: 2.1
+Name: xplainable-client
+Version: 1.2.4.post4
+Summary: The client for persisting and deploying models to Xplainable cloud.
+Home-page: UNKNOWN
+Author: xplainable pty ltd
+Author-email: contact@xplainable.io
+License:                     GNU AFFERO GENERAL PUBLIC LICENSE
+                               Version 3, 19 November 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU Affero General Public License is a free, copyleft license for
+        software and other kinds of works, specifically designed to ensure
+        cooperation with the community in the case of network server software.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        our General Public Licenses are intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          Developers that use our General Public Licenses protect your rights
+        with two steps: (1) assert copyright on the software, and (2) offer
+        you this License which gives you legal permission to copy, distribute
+        and/or modify the software.
+        
+          A secondary benefit of defending all users' freedom is that
+        improvements made in alternate versions of the program, if they
+        receive widespread use, become available for other developers to
+        incorporate.  Many developers of free software are heartened and
+        encouraged by the resulting cooperation.  However, in the case of
+        software used on network servers, this result may fail to come about.
+        The GNU General Public License permits making a modified version and
+        letting the public access it on a server without ever releasing its
+        source code to the public.
+        
+          The GNU Affero General Public License is designed specifically to
+        ensure that, in such cases, the modified source code becomes available
+        to the community.  It requires the operator of a network server to
+        provide the source code of the modified version running there to the
+        users of that server.  Therefore, public use of a modified version, on
+        a publicly accessible server, gives the public access to the source
+        code of the modified version.
+        
+          An older license, called the Affero General Public License and
+        published by Affero, was designed to accomplish similar goals.  This is
+        a different license, not a version of the Affero GPL, but Affero has
+        released a new version of the Affero GPL which permits relicensing under
+        this license.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU Affero General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Remote Network Interaction; Use with the GNU General Public License.
+        
+          Notwithstanding any other provision of this License, if you modify the
+        Program, your modified version must prominently offer all users
+        interacting with it remotely through a computer network (if your version
+        supports such interaction) an opportunity to receive the Corresponding
+        Source of your version by providing access to the Corresponding Source
+        from a network server at no charge, through some standard or customary
+        means of facilitating copying of software.  This Corresponding Source
+        shall include the Corresponding Source for any work covered by version 3
+        of the GNU General Public License that is incorporated pursuant to the
+        following paragraph.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the work with which it is combined will remain governed by version
+        3 of the GNU General Public License.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU Affero General Public License from time to time.  Such new versions
+        will be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU Affero General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU Affero General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU Affero General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU Affero General Public License for more details.
+        
+            You should have received a copy of the GNU Affero General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If your software can interact with users remotely through a computer
+        network, you should also make sure that it provides a way for users to
+        get its source.  For example, if your program is a web application, its
+        interface could display a "Source" link that leads users to an archive
+        of the code.  There are many ways you could offer source, and different
+        solutions will be better for different programs; see section 13 for the
+        specific requirements.
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU AGPL, see
+        <https://www.gnu.org/licenses/>.
+        
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+<div align="center">
+<img src="https://raw.githubusercontent.com/xplainable/xplainable/main/docs/assets/logo/xplainable-logo.png">
+<h1 align="center">xplainable</h1>
+<h3 align="center">Real-time explainable machine learning for business optimisation</h3>
+    
+**Xplainable** makes tabular machine learning transparent, fair, and actionable.
+</div>
+
+## Why Was Xplainable Created?
+In machine learning, there has long been a trade-off between accuracy and explainability. This drawback has led to the creation of explainable ML libraries such as [Shap](https://github.com/slundberg/shap) and [Lime](https://github.com/marcotcr/lime) which make estimations of model decision processes. These can be incredibly time-expensive and often present steep learning curves making them challenging to implement effectively in production environments.
+
+To solve this problem, we created `xplainable`. **xplainable** presents a suite of novel machine learning algorithms specifically designed to match the performance of popular black box models like [XGBoost](https://github.com/dmlc/xgboost) and [LightGBM](https://github.com/microsoft/LightGBM) while providing complete transparency, all in real-time.
+
+
+## Xplainable Cloud
+This Python package is free and open-source. To add more value to data teams within organisations, we also created Xplainable Cloud that brings your models to a collaborative environment.
+
+### Preprocessing with Xplainable Cloud
+Before modeling, it's essential to preprocess your data. Xplainable Cloud facilitates this process by allowing you to create and manage preprocessors in the cloud.
+
+
+```python
+import xplainable as xp
+import os
+from xplainable_client import Client
+
+#Initialising the client
+XClient = Client(api_key=os.environ['XP_API_KEY'])
+
+#Creating a Preprocessor ID
+preprocessor_id = XClient.create_preprocessor_id(
+    preprocessor_name="Preprocessor Name",
+    preprocessor_description="Preprocessor Description",
+)
+
+#Creating a Preprocessor Version
+preprocessor_version = XClient.create_preprocessor_version(
+    preprocessor_id, #preprocessor_id,
+    pipeline, # <-- Pass the pipeline
+    df # <-- Pass the raw dataframe
+)
+
+#Loading the Preprocessor Client
+pp_cloud = XClient.load_preprocessor(
+    preprocessor_id,
+    preprocessor_version["version_id"],
+    gui_object=False # Set to true to load the GUI object, keep as False for pipeline
+    )
+```
+
+### Modelling with Xplainable Cloud
+
+After preprocessing, the next step is to create and train your model. Xplainable Cloud supports model versioning and ID creation to streamline this process.
+
+```python
+
+#Creating a Model Id
+model_id = XClient.create_model_id(
+    model,
+    model_name="Model Name",
+    model_description='Model Description'
+)
+
+#Creating a Model Version
+version_id = XClient.create_model_version(
+    model,
+    model_id,
+    X_train,
+    y_train
+)
+
+```
+
+### Deployments with Xplainable Cloud
+Once your model is ready, deploying it is straightforward with Xplainable Cloud. You can deploy, activate, and manage API keys for your model deployment keys within your IDE or environment.
+
+```python 
+#Creating a Model Deployment
+deployment = XClient.deploy(
+    hostname="https://inference.xplainable.io", 
+    model_id=model_id, 
+    version_id=version_id 
+)
+
+#Activating the Deployment
+XClient.activate_deployment(deployment['deployment_id'])
+
+#Generating an API Key
+deploy_key = XClient.generate_deploy_key(
+    'API Key Name', 
+    deployment['deployment_id'], 
+    7 #-> Days until expiration
+    )
+
+#Hitting the endpoint
+response = requests.post(
+    url="https://inference.xplainable.io/v1/predict",
+    headers={'api_key': deploy_key['deploy_key']},
+    json=body
+)
+
+#Obtaining the value response
+value = response.json()
+```
+
+<div align="center">
+<br></br>
+<br></br>
+Thanks for trying xplainable!
+<br></br>
+<strong>Made with ❤️ in Australia</strong>
+<br></br>
+<hr>
+&copy; copyright xplainable pty ltd
+</div>
+
+
+
+
```

