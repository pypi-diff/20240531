# Comparing `tmp/ogu-1.52.tar.gz` & `tmp/ogu-1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogu-1.52.tar", last modified: Tue Apr 23 12:03:35 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ogu-1.52.tar` & `ogu-1.54.tar`

### file list

```diff
@@ -1,23 +1,43 @@
--rw-r--r--   0        0        0    35181 2020-03-04 07:53:48.976828 ogu-1.52/LICENSE
--rw-r--r--   0        0        0    34348 2024-02-23 09:41:31.917877 ogu-1.52/README.md
--rw-r--r--   0        0        0     1367 2024-04-23 12:03:35.891722 ogu-1.52/pyproject.toml
--rw-r--r--   0        0        0      496 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/__init__.py
--rw-r--r--   0        0        0      502 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/__main__.py
--rw-r--r--   0        0        0     7906 2024-01-05 09:11:07.894436 ogu-1.52/src/OGU/cli.py
--rw-r--r--   0        0        0    10346 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/animal_orders.csv
--rw-r--r--   0        0        0     2902 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/button1.png
--rw-r--r--   0        0        0     2399 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/button2.png
--rw-r--r--   0        0        0     3139 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/button3.png
--rw-r--r--   0        0        0     1030 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/button4.png
--rw-r--r--   0        0        0     7502 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/classes.csv
--rw-r--r--   0        0        0      154 2024-01-05 08:52:52.080834 ogu-1.52/src/OGU/data/kingdoms.csv
--rw-r--r--   0        0        0        6 2024-01-05 08:52:52.096473 ogu-1.52/src/OGU/data/lineage
--rw-r--r--   0        0        0     6169 2024-01-05 08:52:52.096473 ogu-1.52/src/OGU/data/phyla.csv
--rw-r--r--   0        0        0       34 2024-01-05 08:52:52.096473 ogu-1.52/src/OGU/data/superkingdoms.csv
--rw-r--r--   0        0        0    21189 2024-04-23 11:57:18.961705 ogu-1.52/src/OGU/evaluate.py
--rw-r--r--   0        0        0    32941 2024-01-05 09:10:57.405381 ogu-1.52/src/OGU/gb2fasta.py
--rw-r--r--   0        0        0      502 2024-04-23 11:55:50.842027 ogu-1.52/src/OGU/global_vars.py
--rw-r--r--   0        0        0    31780 2024-02-23 08:10:10.754035 ogu-1.52/src/OGU/primer.py
--rw-r--r--   0        0        0    63204 2024-01-05 09:10:22.924539 ogu-1.52/src/OGU/ui.py
--rw-r--r--   0        0        0    24521 2024-02-23 08:26:57.229822 ogu-1.52/src/OGU/utils.py
--rw-r--r--   0        0        0    34546 1970-01-01 00:00:00.000000 ogu-1.52/PKG-INFO
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ogu-1.54/MANIFEST.in
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 ogu-1.54/TODO
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ogu-1.54/all_test.ps1
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 ogu-1.54/all_test.sh
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ogu-1.54/build.ps1
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ogu-1.54/build_primer3-py.ps1
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ogu-1.54/build_win_package.ps1
+-rw-r--r--   0        0        0    39509 2020-02-02 00:00:00.000000 ogu-1.54/old-README.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ogu-1.54/requirements.txt
+-rwxr-xr-x   0        0        0     1772 2020-02-02 00:00:00.000000 ogu-1.54/setup.py
+-rw-r--r--   0        0        0    80204 2020-02-02 00:00:00.000000 ogu-1.54/ui.tcl
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ogu-1.54/.pdm-build/.gitignore
+-rw-r--r--   0        0        0    34546 2020-02-02 00:00:00.000000 ogu-1.54/.pdm-build/ogu-1.52.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ogu-1.54/.pdm-build/ogu-1.52.dist-info/WHEEL
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ogu-1.54/.pdm-build/ogu-1.52.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    34520 2020-02-02 00:00:00.000000 ogu-1.54/.pdm-build/ogu-1.52.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/__main__.py
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/cli.py
+-rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/evaluate.py
+-rw-r--r--   0        0        0    31989 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/gb2fasta.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/global_vars.py
+-rw-r--r--   0        0        0    30996 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/primer.py
+-rw-r--r--   0        0        0    61731 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/ui.py
+-rw-r--r--   0        0        0    23717 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/utils.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/animal_orders.csv
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/button1.png
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/button2.png
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/button3.png
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/button4.png
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/classes.csv
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/kingdoms.csv
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/lineage
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/phyla.csv
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ogu-1.54/src/OGU/data/superkingdoms.csv
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ogu-1.54/third-party/get_files.py
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 ogu-1.54/visualize/draw_circle_mitochondria.ipynb
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 ogu-1.54/visualize/draw_circle_plastid.ipynb
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 ogu-1.54/.gitignore
+-rw-r--r--   0        0        0    34520 2020-02-02 00:00:00.000000 ogu-1.54/LICENSE
+-rw-r--r--   0        0        0    33405 2020-02-02 00:00:00.000000 ogu-1.54/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ogu-1.54/pyproject.toml
+-rw-r--r--   0        0        0    34568 2020-02-02 00:00:00.000000 ogu-1.54/PKG-INFO
```

### Comparing `ogu-1.52/LICENSE` & `ogu-1.54/.pdm-build/ogu-1.52.dist-info/licenses/LICENSE`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
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
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
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
-<http://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
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
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
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
+<http://www.gnu.org/licenses/>.
```

### Comparing `ogu-1.52/README.md` & `ogu-1.54/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,944 +1,944 @@
-[![PyPI version](https://badge.fury.io/py/OGU.svg)](https://badge.fury.io/py/OGU)
-
-# Quick start
-
-- Install Python 3 (3.9 or newer).
-- Open terminal, run
-
-   ```shell
-   # Install, using pip (recommended)
-   pip3 install OGU --user
-
-   # Initialize with Internet
-   # Windows
-   python -m OGU init
-   # Linux and macOS
-   python3 -m OGU init
-
-   # Run
-   # Windows
-   python -m OGU
-   # Linux and macOS
-   python3 -m OGU
-   ```
-
-# Table of Contents
-
-* [Quick start](#quickstart)
-* [Feature](#feature)
-* [Prerequisite](#prerequisite)
-    * [Hardware](#hardware)
-    * [Software](#software)
-* [Installation](#installation)
-    * [Portable](#portable)
-    * [Install with pip](#Installwithpip)
-    * [Install with conda](#Installwithconda)
-    * [Initialization](#Initialization)
-* [Usage](#usage)
-    * [Quick examples](#quick-examples)
-    * [Sequence ID](#sequence-id)
-    * [Command line](#commandline)
-* [Input](#input)
-* [Output](#output)
-* [Options](#options)
-    * [gb2fasta](#gb2fasta)
-    * [evaluate](#evaluate)
-    * [primer](#primer)
-* [Performance](#performance)
-* [Citation](#citation)
-* [License](#license)
-* [Q&A](q&a)
-
-# Features
-
-:heavy_check_mark: Automatically collect, organize and clean sequence data
-from NCBI GenBank or local: collect data with abundant options; extract CDS,
-intergenic spacer, or any other annotations from original sequence; remove
-redundant sequences according to species information; remove invalid or
-abnormal sequences/fragments; generate clean dataset with uniform sequence id.
-
-:heavy_check_mark: Evaluate variance of sequences by calculating nucleotide
-diversity, observed resolution, Shannon index, tree resolution, phylogenetic
-diversity (original and edited version), gap ratio, and others. Support
-sliding-window scanning.
-
-:heavy_check_mark: Design universal primer for the alignment. Support
-ambiguous bases in primers.
-
-# Prerequisite
-
-## Hardware
-
-`Organelle Genome Utilities (OGU)` requires very few computational resources.
-A normal PC/laptop is enough. For downloading large amount of data, make sure
-the Internet connection is stable and fast enough.
-
-## Software
-
-For the portable version, nothing need to be installed manually.
-
-For installing from pip, [Python](https://www.python.org/downloads/) is
-required. Notice that the python version should be higher than **3.6**.
-
-:white_check_mark: All third-party dependencies will be automatically
-installed with Internet, including `biopython`, `matplotlib`, `coloredlogs`,
-`numpy`, `primer3-py`, (python packages), and
-[MAFFT](https://mafft.cbrc.jp/alignment/software/),
-[IQTREE](http://www.iqtree.org/),
-[BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download).
-
-# Installation
-
-We assume that users have already installed
-[Python3](https://www.python.org/downloads/) (3.9 or above).
-
-## Install with pip
-
-1. Install [Python](https://www.python.org/downloads/). 3.9 or newer is
-   required.
-
-2. Open command line, run
-
-```shell
-pip3 install OGU --user
-```
-
-## Initialization
-
-During the first running, `OGU` will check and initialize the
-running environment. Missing dependencies will be automatically installed.
-
-This step requires Internet connection.
-
-By default, the program will automatically finish initialization, if any error
-occurs, users can choose one of the following methods:
-
-### Automatic
-
-Run the following command.
-
-```shell
-# Windows
-python -m OGU init
-# Linux and macOS
-python3 -m OGU init
-```
-
-### Use prepared package
-According to your system, download related compressed file from [packages](https://github.com/wpwupingwp/OGU/releases).
-
-For Windows users: 
-1. paste `%HOMEDRIVE%%HOMEPATH%/` to explorer's address bar and open.
-2. create `.OGU` folder. Don't miss the dot.
-3. open `.OGU` folder, paste downloaded compressed file and unzip. Make sure after
-decompress there are three folders in `.OGU`.
-
-For Linux and macOS users, please download and unpack files into
-`~/.OGU`.
-
-### Manually install
-
-For Linux users with root privileges, just use the package manager:
-
-```
-# Ubuntu and Debian
-sudo apt install mafft ncbi-blast+ iqtree
-# Fedora (1)
-sudo dnf install mafft ncbi-blast+ iqtree
-# Fedora (2)
-sudo yum install mafft ncbi-blast+ iqtree
-# ArchLinux
-sudo pacman -S mafft ncbi-blast+ iqtree
-# FreeBSD
-sudo pkg install mafft ncbi-blast+ iqtree
-```
-
-For macOS users with root privileges, install `brew` if it has not been
-installed previously:
-
-```
-/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
-```
-
-If any errors occur, install `Xcode-select` and retry.
-
-Then:
-
-```
-brew install blast mafft brewsci/science/iqtree
-```
-
-If using Windows or lacking root privileges, users should follow these
-instructions:
-
-1. BLAST+
-
-    * [Windows](https://www.ncbi.nlm.nih.gov/books/NBK52637/)
-    * [Linux and macOS](https://www.ncbi.nlm.nih.gov/books/NBK52640/)
-2. MAFFT
-
-    * [Windows](https://mafft.cbrc.jp/alignment/software/windows.html)
-
-      Choose "All-in-one version", download and unzip. Then follow the steps
-      in the BLAST+ installation manual to set the `PATH`.
-    * [Linux](https://mafft.cbrc.jp/alignment/software/linux.html)
-
-      Choose "Portable package", download and unzip. Then follow the
-      instructions of BLAST+ to set the `PATH` for `MAFFT`.
-    * [macOS](https://mafft.cbrc.jp/alignment/software/macosx.html)
-
-      Choose "All-in-one version", download and unzip. Then follow the steps
-      in the BLAST+ installation manual to set the `PATH`.
-3. IQ-TREE
-
-    * [Download](http://www.iqtree.org/#download)
-
-      Download the installer according to OS. Unzip and add the path of
-      subfolder `bin` to `PATH`.
-
-# Usage
-
-## Graphical user interface
-Open the command line (Windows) or terminal (Linux and macOS),
-run
-
-```bash
-OGU
-```
-
-or 
-```bash
-# linux and macos
-python3 -m OGU
-# windows
-python -m OGU
-```
-
-## command line
-Once a user opens the command line (Windows) or terminal (Linux and macOS), 
-just type the command:
-
-```
-# Windows
-python -m OGU [input] -[options] -out [out_folder]
-# Linux and macOS
-python3 -m OGU [input] -[options] -out [out_folder]
-```
-
-## Quick examples
-
-1. Download all `rbcL` sequences of species in Poaceae family and do
-   pre-process.
-
-```
-# Windows
-python -m OGU.gb2fasta -gene rbcL -taxon Poaceae -out rbcL_Poaceae
-# Linux and macOS
-python3 -m OGU.gb2fasta -gene rbcL -taxon Poaceae -out rbcL_Poaceae
-```
-
-2. Download all ITS sequences of _Rosa_ genus. Do pre-process and keep redundant
-   sequences:
-
-```
-# Windows
-python -m OGU.gb2fasta -query internal transcribed spacer -taxon Rosa -out Rosa_its -uniq no
-# Linux and macOS
-python3 -m OGU.gb2fasta -query internal transcribed spacer -taxon Rosa -out Rosa_its -uniq no
-```
-
-3. Download all Lamiaceae chloroplast genomic sequences in the RefSeq database.
-   Then do pre-process and evaluation of variance (skip primer designing):
-
-```
-# Windows
-python -m OGU -og cp -refseq yes -taxon Lamiaceae -out Lamiaceae_cp
-# Linux and macOS
-python3 -m OGU -og cp -refseq yes -taxon Lamiaceae -out Lamiaceae_cp
-```
-
-4. Download sequences of _Zea mays_, set length between 100 bp and 3000 bp,
-   and then perform evaluation and primer designing. Note that the space in
-   the species name is replaced with underscore "\_".
-
-```
-# Windows
-python -m OGU -taxon Zea_mays -min_len 100 -max_len 3000 -out Zea_mays -primer
-# Linux and macOS
-python3 -m OGU -taxon Zea_mays -min_len 100 -max_len 3000 -out Zea_mays -primer
-```
-
-5. Download all _Oryza_ mitochondria genomes in RefSeq database, keep the
-   longest sequence for each species and run a full analysis:
-
-```
-# Windows
-python -m OGU -taxon Oryza -og mt -min_len 50000 -max_len 200000 -uniq longest -out Oryza_cp -refseq yes -primer
-# Linux and macOS
-python3 -m OGU -taxon Oryza -og mt -min_len 50000 -max_len 200000 -uniq longest -out Oryza_cp -refseq yes -primer
-```
-
-## Sequence ID
-
-`Organelle Genome Utilities` uses a uniform sequence id format for input fasta files and all output
-sequences.
-
-```
-Locus|Kingdom|Phylum|Class|Order|Family|Genus|Species|Accession|SpecimenID_Isolate|Type
-# example
-rbcL|Viridiplantae|Streptophyta|Magnoliopsida|Poales|Poaceae|Oryza|longistaminata|MF998442|TAN:GB60B-2014|gene
-```
-
-The order of the fields is fixed. The fields are separated by vertical bars
-("|"). The space character (" ") was disallowed and was replaced by an
-underscore ("\_"). Due to missing data, some fields may be empty.
-
-`Locus`: SeqName refers to the name of a sequence. Usually it is the gene
-name. For intergenic spacer, an underscore ("\_") is used to connect two
-gene's names, e.g., "geneA_geneB".
-
-If a valid sequence name cannot be found in the annotations of the GenBank
-file, `Organelle Genome Utilities` will use "Unknown" instead.
-
-For chloroplast genes, if "-rename" option is set, the program will try to use
-regular expressions to fix potential errors in gene names.
-
-`Kingdom`: The kingdom (_Fungi, Viridiplantae, Metazoa_) of a species. For
-convenience, a superkingdom (_Bacteria, Archaea, Eukaryota, Viruses, Viroids_)
-may be used if the kingdom information for a sequence is missing.
-
-`Phylum`: The phylum of the species.
-
-`Class`: The class of the species.
-
-Because some species' classes are empty (for instance, basal angiosperm),
-`Organelle Genome Utilities` will guess the class of the species.
-
-Given the taxonomy information in GenBank file:
-
-```
-Eukaryota; Viridiplantae; Streptophyta; Embryophyta; Tracheophyta;
-    Spermatophyta; Magnoliophyta; basal Magnoliophyta; Amborellales;
-    Amborellaceae; Amborella.
-```
-
-`Organelle Genome Utilities` will use "basal Magnoliophyta" as the class because this
-expression locates before the order name ("Amborellales").
-
-`Order`: The order name of the species.
-
-`Family`: The family name of the species.
-
-`Genus`: The genus name of the species, i.e., the first part of the scientific
-name.
-
-`Species`: The specific epithet of the species, i.e., the second part of the
-scientific name of the species. It may contain the subspecies' name.
-
-`Accession`: The GenBank Accession number for the sequence. It does not
-contain the record's version.
-
-`SpecimenID` and `Isolate`: Specimen ID and Isolate ID of the sequence. May be empty.
-
-`Type`: Type of the sequence. It is usually "gene" or "spacer".
-
-## Command line
-
-:exclamation: In Linux and macOS, Python2 is `python2` and Python3 is
-`python3`. However, in Windows, Python3 is called `python`, too. Please
-notice the difference.
-
-* Show help information of each module
-
- ```shell
- # Windows
- python -m OGU -h
- python -m OGU.gb2fasta -h
- python -m OGU.evaluate -h
- python -m OGU.primer -h
- # Linux and macOS
- python3 -m OGU.gb2fasta -h
- python3 -m OGU.evaluate -h
- python3 -m OGU.primer -h
- ```
-
-* Full process
-
- ```shell
- # Windows
- python -m OGU -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
- # Linux and macOS
- python3 -m OGU -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
- ```
-
-* Collect, convert, and clean GenBank data with gb2fasta module
-
- ```shell
- # Windows
- python -m OGU.GB2fasta -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
- # Linux and macOS
- python3 -m OGU.gb2fasta -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
- ```
-
-* Evaluate variance of given fasta files
-
- ```shell
- # Windows
- python -m OGU.evaluate -fasta [fasta files]
- # Linux and macOS
- python3 -m OGU.evaluate -fasta [input file]
- ```
-
-* Design universal primers of given alignments.
-
- ```shell
- # Windows
- python -m OGU.primer -aln [alignment files]
- # Linux and macOS
- python3 -m OGU.primer -aln [alignment files]
- ```
-
-## Visualize
- 
-Here are to jupyter notebooks for visualize analyze result as detailed circle
-figure:
-  - `Visualize/draw_circle_plastid.ipynb`: for plastid genomes
-  - `Visualize/draw_circle_mitochondria.ipynb`: for mitochondria genomes
-
-Since users may want to customize the figure, we provide jupyter notebooks 
-instead of packaged code. Users can get the result following these steps.
-0. Run `pip install jupyterlab` to install jupyter notebooks
-1. Double click to open in jupyter notebook, Visual Studio Code or other IDEs you prefer.
-2. Edit `filename` to the Evaluation.csv you got
-3. Edit `gb_file` to extended gb file you got. Remember to generate it with 
-`-out_debug` in OGU.gb2fasta
-4. If visualize plastid data, you need provide `LSC, SSC, IRa, IRb` lengths. Or
-you can use default value, which is for *Tobacum*.
-5. Edit color themes as your wish
-6. Run all cells to output pdf figure
- 
-# Input
-
-`Organelle Genome Utilities` accepts:
-
-1. GenBank queries. Users can use "-query" or combine with any other filters;
-2. GenBank-format files.
-3. Unaligned fasta files. Each file is considered as one locus when evaluating
-   the variance;
-4. Alignments (fasta format).
-
-# Output
-
-All results will be put in the output folder. If the user does not set the
-output path via "-out", `Organelle Genome Utilities` will create a folder labelled "Result".
-
-In the output folder, several sub-folders will be created.
-
-* GenBank
-
-  Raw GenBank files.
-
-* Divide
-
-  Fasta files converted from the GenBank file. Each file represents a
-  fragment of the original sequence according to the annotation.
-
-  For instance, a record in a "rbcL.gb" file may also contain atpB gene's
-  sequences. The "rbcL.fasta" file does not contain any upstream/downstream
-  sequences and "atpB_rbcL.fasta" does not have even one base of the atpB or
-  rbcL gene, just the spacer (assuming the annotation is precise).
-
-  User can skip this dividing step with the option "-no_divide".
-* Fasta
-
-  Raw fasta files users provided.
-* Unique
-
-  Fasta files after removing redundant sequences.
-* Expanded_fasta
-
-  To design primers, `Organelle Genome Utilities` extend a sequence to its
-  upstream/downstream. Only used in the primer module.
-* Alignment
-
-  Aligned fasta files.
-
-  `.aln`: The aligned fasta files.
-
-  `.-consensus.fastq`: The fastq format of the consensus sequence of the
-  alignment. Note that it contains alignment gap ("-"). It is NOT
-  RECOMMENDED to be used directly because the consensus-generating algorithm is
-  optimised for primer design.
-* Evaluate
-
-  Including output files from the evaluation module.
-
-  `.pdf`: The PDF format of the figure containing the sliding-window scan
-  result of the alignment.
-
-  `.csv`: The CSV format file of the sliding-window scan result. `"Index"`
-  means the location of the base in the alignment.
-
-* Primer
-
-  Including output files from the primer module.
-
-  `.primer.fastq`: The fastq format file of a primer's sequence. It contains
-  two sequences, and the direction is 5' to 3'. The first is the forward
-  primer, and the second is the reverse primer. The quality of each base is
-  equal to its proportion of the column in the alignment. Note that the
-  sequence may contain ambiguous bases if it was not disabled.
-
-  `.primers.csv`: The list of primer pairs in CSV (comma-separated values
-  text) format.
-
-  `.candidate.fasta`: The candidate primers. This file may contain
-  thousands of records. Do not recommend paying attention to it.
-
-  `.candidate.fastq`: Again, the candidate primers. This time, each file has
-  the quality information that equals to the proportion of the bases in the
-  column of the alignment.
-
-* Temp
-
-  Including temporary files. Could be safely deleted .
-
-In the output folder, there are some other important output files:
-
-* Primers.csv
-
-  The list of primer pairs in CSV (comma-separated values text) format.
-
-  Its title:
-    ```
-    Locus,Samples,Score,AvgProductLength,StdEV,MinProductLength,MaxProductLength,Coverage,Observed_Res,Tree_Res,PD_terminal,Entropy,LeftSeq,LeftTm,LeftAvgBitscore,LeftAvgMismatch,RightSeq,RightTm,RightAvgBitscore,RightAvgMismatch,DeltaTm,AlnStart,AlnEnd,AvgSeqStart,AvgSeqEnd
-    ```
-
-  `Locus`: The name of the locus/fragment.
-
-  `Samples`: The number of sequences used to find this pair of primers.
-
-  `Score`: The score of this pair of primers. Usually the higher, the better.
-
-  `AvgProductLength`: The average length of the DNA fragment amplified by
-  this pair of primers.
-
-  `StdEV`: The standard deviation of the AvgProductLength. A higher number
-  means the primer may amplify different lengths of DNA fragments.
-
-  `MinProductLength`: The minimum length of an amplified fragment.
-
-  `MaxProductLength`: The maximum length of an amplified fragment. Note that
-  all of these fields are calculated using given sequences.
-
-  `Coverage`: The coverage of this pair of primers over the sequences it
-  used. Calculated with the BLAST result. High coverage means that the pair
-  is much more "universal".
-
-  `Observed_Res`: The `observed resolution` of the sub-alignment sliced by
-  the primer pair, which is equal to the number of unique sequences divided
-  by the number of total sequences. The value is between 0 and 1.
-
-    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;R_{o}=\frac{n_{uniq}}{n_{total}}" title="R_{o}=\frac{n_{uniq}}{n_{total}}" />
-
-  `Tree_Res`: The `tree resolution` of the sub-alignment, which is equal to
-  the number of internal nodes on a phylogenetic tree (constructed from the
-  alignment) divided by number of terminal nodes. The value is between 0 and
-    1.
-
-    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;R_{T}=\frac{n_{internal}}{n_{terminal}}" title="R_{T}=\frac{n_{internal}}{n_{terminal}}" />
-
-  `PD_terminal`: The average of the terminal branch's length. It's an edited
-  version of the `Phylogenetic Diversity` for DNA barcoding evaluation.
-
-  `Entropy`: The `Shannon equitability` index of the sub-alignment. The value
-  is between 0 and 1.
-
-    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;E_{H}&space;=&space;\frac{-&space;\sum_{i=1}^{k}{p_{i}&space;\log(p_{i})}}{\log(k)}" title="E_{H} = \frac{- \sum_{i=1}^{k}{p_{i} \log(p_{i})}}{\log(k)}" />
-
-  `LeftSeq`: Sequence of the forward primer. The direction is 5' to 3'.
-
-  `LeftTm`: The melting temperature of the forward primer. The unit is
-  degree Celsius (°C).
-
-  `LeftAvgBitscore`: The average raw bitscore of the forward primer, which
-  is calculated by BLAST.
-
-  `LeftAvgMismatch`: The average number of mismatched bases of the forward
-  primer, as counted by BLAST.
-
-  `RightSeq`: Sequence of reverse primer. The direction is 5' to 3'.
-
-  `RightTm`: The melting temperature of the reverse primer. The unit is
-  degrees Celsius (°C).
-
-  `RightAvgBitscore`: The average raw bitscore of the reverse primer, which
-  is calculated by BLAST.
-
-  `RightAvgMismatch`: The average number of mismatched bases of the reverse
-  primer, as counted by BLAST.
-
-  `DeltaTm`: The difference in the melting temperatures of the forward and
-  reverse primers. A pair of primers with a high DeltaTm may result in
-  failure during the PCR experiment.
-
-  `AlnStart`: The location of the beginning of the forward primer (5',
-  leftmost of primer pairs) in the entire alignment.
-
-  `AlnEnd`: The location of the end of the reverse primer (5', rightmost of
-  primer pairs) in the entire alignment.
-
-  `AvgSeqStart`: The average beginning of the forward primer in the original
-  sequences.  *ONLY USED FOR DEBUG*.
-
-  `AvgSeqEnd`: The average end of the forward primer in the original
-  sequences.  *ONLY USED FOR DEBUG*.
-
-  The primer pairs are sorted by `Score`. Since the score may not fully
-  satisfy the user's specific considerations, it is suggested that primer
-  pairs be chosen manually if the first primer pair fails during the PCR
-  experiment.
-
-* Log.txt
-
-  The log file. Contains all the information printed on the screen.
-
-* Evaluation.csv
-
-  The summary of all loci/fragments, which only contains the variance
-  information for each fragment. One of the new field, `GapRatio`, means the
-  ratio of the gap ("-") in the alignment. `PD` means the original version
-  of the phylogenetic diversity and `PD_stem` means an alternative version
-  of it which only calculate the length of the stem branch in the
-  phylogenetic tree.
-
-# Options
-
-Here are some general options for the program and submodule:
-
-`-h`: Prints help messages of the program or one of the module.
-
-`-gb [filename]`: User-provided GenBank file or files. Could be one or more
-files that separated by space.
-
-For instance,
-
-```
-# one file
--gb sequence.gb
-# multiple files
--gb matK.gb rbcL.gb Oryza.gb Homo_sapiens.gb
-```
-
-`-fasta [filename]`: User-provided unaligned fasta files. Could be one or
-multiple.
-
-`-aln [filename]`: Alignment files that the user provides. Could be one or
-multiple.
-
-It only supports the fasta format. Ambiguous bases and gaps ("-") are supported.
-
-`-out [folder name]`: The output folder's name. All results will be put into
-the output folder. If the user does not set an output path via "-out",
-`Organelle Genome Utilities` will create a folder named "Result".
-
-`OGU` does not overwrite the existing folder with the same name.
-
-It is HIGHLY RECOMMENDED to use only letters, numbers and underscores ("\_") in
-the folder name to avoid mysterious errors caused by other Unicode characters.
-
-Options below are for specific modules.
-
-## gb2fasta
-
-### Query
-
-Options used for querying NCBI GenBank.
-
-`-taxon [taxonomy name]`: The taxonomy name. It could be any taxonomic rank
-from kingdom (same as "-group") to species, as long as the user inputs correct
-name (the scientific name of species or taxonomic group in latin, NOT
-ENGLISH). It will restrict the query to the targeted taxonomy unit. Make sure
-to use quotation marks if `taxonomy` has more than one word or use underscore
-to replace space, for instance `"Zea mays"` or `Zea_mays`.
-
-`-gene [gene name]`: The gene's name which the user wants to query in GenBank.
-If the user wants to use logical expressions like "OR", "AND", "NOT", s/he
-should use "-query" instead. If there is space in the gene's name, make sure
-to use quotation marks.
-
-Note that "ITS" is not a gene name--it is "internal transcribed spacer".
-
-Sometimes "-gene" options may bring in unwanted sequences. For example, if a
-user queries "rbcL[gene]" in GenBank, spacer sequences may contain _rbcL_ or
-_rbcL_'s upstream/downstream gene, such as "atpB_rbcL spacer" or _atpB_.
-
-`-og [ignore|both|no|mt|mitochondrion|cp|chloroplast|pl|plastid]`: Query
-organelle sequences or not. The default value is `ignore`.
-
-    - `ignore`: do not consider organelle type, same as GenBank website's
-      default setting.
-
-    - `both`: only query organelle sequences, including both plastid and
-      mitochondrion.
-
-    - `no`: exclude organelle sequences from the query.
-
-    - `cp` or `chloroplast` or `pl` or `plastid`: only query plastid sequences
-
-    - `mt` or `mitochondrion`: only query mitochondrion sequences.
-
-`-refseq [both|yes|no]`: query in RefSeq database or not. The default value is
-`both`.
-
-    - `both`: query all sequences in or not in RefSeq database, same as NCBI
-      website's default setting.
-
-    - `yes`: only query sequences in RefSeq database.
-
-    - `no`: exclude sequences in RefSeq database.
-
-[RefSeq](https://www.ncbi.nlm.nih.gov/refseq/about/) is considered to have
-higher sequence and annotation quality than GenBank. This option could be used
-for getting nuclear/organelle genomes from NCBI. In this situation (`-refseq
-yes`), the length limit will be removed automatically.
-
-`-count [number]`: Restrict numbers of sequences to be downloaded. The default
-value `0` means no restriction.
-
-`-min_len [length]`: The minimum length of the records downloaded from
-GenBank. The default value is `100` (bp). The number must be an integer.
-
-`-max_len [length]`: The maximum length of the records downloaded from
-GenBank. The default value is `10000` (bp). The number must be an integer.
-
-`-date_start [yyyy/mm/dd]`: The beginning of the release data range of the
-sequences, the format is yyyy/mm/dd.
-
-`-date_end [yyyy/mm/dd]`: The end of the release data range of the sequences,
-the format is yyyy/mm/dd.
-
-`-molecular [all|DNA|RNA]`: The molecular type,
-which could be DNA or RNA. The
-default is `all`--no restriction.
-
-`-email [email address]`: NCBI GenBank database requires users to provide
-an email address in case of abnormal situations that NCBI need to contact
-the user. For convenience, `OGU` will use
-"guest@example.com" if the user does not provide an email address. _However_,
-it is better to provide a real email address for potential contact.
-
-`-query [expression]`: The query string provided by the user. It behaves in
-the same manner as the query the user typed into the Search Box in NCBI
-GenBank's webpage.
-
-Make sure to follow NCBI's grammar for queries. It can contain several words.
-Remember to add quotation marks if an item contains more than one words, for
-instance, `"Homo sapiens"[organism]`, or use underscore to replace space,
-`Homo_sapiens[organism]`.
-
-`-exclude [expression]`: Use this option to use negative option. For instance,
-"-exclude Zea [organism]" (do not include quotation marks) will add " NOT
-(Zea[organism])" to the query.
-
-This option can be useful for excluding a specific taxon.
-
-```
--taxon Zea -exclude "Zea mays"[organism]
-```
-
-This will query all records in genus *Zea* while records of *Zea mays* will be
-excluded.
-
-For much more complex exclude options, please consider to use "Advance search"
-in GenBank website.
-
-`-group [all|animals|plants|fungi|protists|bacteria|archaea|viruses]`: To
-restrict the query in given group. The default value is `all`--no
-restriction.
-
-It is reported that the "group" filter may return abnormal records, for
-instance, return plants' records when the group is "animal" and the
-"organelle" is "chloroplast". Furthermore, it may match a great number of
-records in GenBank. Hence, we strongly recommend using "-taxon" instead.
-
-### Divide
-
-Options used for converting GenBank files to fasta files.
-
-`-out_debug`: If you are going to use visualize pipeline to draw detailed circle
-figure, use this option to generate extended version genbank file.
-
-`-no_divide`: If set, it will analyse the whole sequence instead of the
-divided fragments. By default, `OGU` divides one GenBank record into
-several fragments according to its annotation.
-
-`-rename`: If set, the program will try to rename genes. For instance, "rbcl"
-will be renamed to "rbcL", and "tRNA UAC" will be renamed to "trnVuac", which
-consists of "trn", the amino acid's letter and transcribed codon. This may be
-helpful if the annotation has nonstandard uppercase/lowercase or naming format
-that it can merge the same sequences to one file for the same locus having
-variant names.
-
-If using Windows operating system, consider using this option to avoid
-contradictory filenames.
-
-`-unique [longest|first|no]`: The method used to remove redundant sequences.
-`OGU` will remove redundant sequences to ensure only one sequence per
-species by default. A user can change its behaviour by setting different
-methods.
-
-    - `first`: According to the records' order in the original GenBank file,
-      only the first sequence of the same species' same locus will be kept.
-      Others will be ignored directly. This is the default option due to
-      performance considerations.
-
-    - `longest`: Keep the longest sequence for one species. The program will
-      compare the sequence's length from the same species' same locus.
-
-    - `no`: Skip this step. All sequences will be kept.
-
-`-allow_mosaic_spacer`: If one gene nested with another gene, normally they
-do not have spacers. The default value is `False`.
-
-However, some users want the fragments between two gene's beginnings and ends.
-This option is for this specific purpose (e.g., matK-trnK_UUU). For normal
-usage, *do not recommend*.
-
-`-expand [number]`: The expansion length in upstream/downstream. If set,
-`OGU` will expand the sequence to its upstream/downstream after the
-dividing step to find primer candidates. The default value is `0`.
-
-Note that this option is different with "-max_len". This option limits the
-length of one annotation's sequence. The "-max_len" limits the whole
-sequence's length of one GenBank record.
-
-`-allow_repeat`: If genes repeated in downstream, this option will allow the
-repeat region to be extracted, otherwise any repeated region will be omitted.
-The default value is `False`.
-
-`-allow_invert_repeat`: If two genes invert-repeated in downstream, this
-option will allow spacers of them to be extracted, otherwise the spacer
-will be omitted. The default value is `False`.
-
-For instance, geneA-geneB located in one invert-repeat region (IR) of
-chloroplast genome. In another IR region, there are geneB-geneA. This option
-will extract sequences of two different direction as two unique spacers.
-
-`-max_name_len [number]`: The maximum length of a feature name. Some
-annotation's feature name in GenBank file is too long, and usually, they are
-not the target sequence the user wants. By setting this option, `OGU`
-will truncate the annotation's feature name if it is too long. By default, the
-value is `50`.
-
-`-max_gene_len [value]`: The maximum length of a sequence for one annotation.
-Some annotations' sequences are too long (for instance, one gene has two
-exons, and its intron is longer than 10 Kb). This option will skip those long
-sequences. By default, the value is `20000` (bp).
-
-## Evaluate
-
-`-ig` or `-ignore_gap`: ignore gaps in the alignment.
-
-`-iab` or `-ignore_ambigous`: ignore ambiguous bases in the alignment.
-
-`-quick`: skip sliding-window scan.
-
-`-size [number]`: the window size of the sliding window scan. The default
-value is `500`.
-
-`-step [number]`: the step size of the sliding window scan. The default value
-is `50`.
-
-`-skip_primer`: skip primer designing. The default value is `False`.
-
-## Primer design
-
-`-coverage [value]`: The minimum coverage of the base and primer. The default
-value is `0.5` (50%). It is used to remove primer candidates if its coverage
-among all sequences is smaller than the threshold. The coverage of primers is
-calculated by BLAST.
-
-`-res [value]`: The minimum *observed resolution* of the fragments or primer
-pairs. The default *value* is 0.3 (30%). The value should be in 0.0 to 1.0.
-
-`OGU` uses the *observed resolution* instead of others because of the
-speed. Also, it is considered to be the lower bound of the real resolution
-that a fragment with a low *observed resolution* may not have a satisfactory
-tree resolution/phylogenetic diversity, either.
-
-`-pmin [length]`: The minimal length of the primer. The default *value* is 20.
-
-`-pmax [length]`: The maximal length of the primer. The default *value* is 25.
-
-`-topn [number]`: How many pairs of primers is kept for each input alignment.
-The default value is `1`, i.e., only keep the _best_ primer pair according to
-its `score`. To keep more pairs, set "-t" to more than 1.
-
-`-amin [length]`: The minimum amplified length (include primer). The default
-value is `300` (bp). Note this limits the PCR product's length instead of the
-sub-alignment's length.
-
-`-amax [length]`: The maximum amplified length (include primer). The default
-value is `800` (bp).
-
-The "-amin" and "-amax" are used to screen primer candidates. It uses BLAST
-results to set the location of primers on each template sequence and
-calculates the average lengths of the products. Because of the variance of
-species, the same locus may have different lengths in different species, plus
-with the stretching of the alignment that gaps were added during the aligning,
-please consider adding some *margins* for these two options.
-
-For instance, if a user wants the amplified length to be smaller than 800 and
-greater than 500, s/he could consider setting "-amin" to 550 and "-amax" to
-
-750.
-
-`-ambiguous [number]`: The maximum number of ambiguous bases allowed in one
-primer. The default value is `4`.
-
-`-mismatch [number]`: The maximum number of mismatched bases in a primer. This
-option is used to remove primer candidates if the BLAST results show that
-there is too much mismatch. The default value is `4`.
-
-# Performance
-
-For a taxon that is not very large and includes few fragments, `OGU`
-can finish the task in *minutes*. For a large taxon (such as the Asteraceae
-family or the whole class of the Poales) containing multiple fragments (such
-as the chloroplast genomes), the time to complete may be one hour or more on a
-PC or laptop.
-
-`OGU` requires few memories (usually less than 0.5 GB, although, for a
-large taxon BLAST may require more) and few CPUs (one core is enough). It can
-run very well on a normal PC. Multiple CPU cores may be helpful for the
-alignment and tree construction steps.
-
-For Windows users, MAFFT [may be very slow due to antivirus
-software](https://mafft.cbrc.jp/alignment/software/windows_without_cygwin.html).
-Please consider
-following [this instruction](https://mafft.cbrc.jp/alignment/software/ubuntu_on_windows.html) to
-install
-Ubuntu on Windows to obtain better results.
-
-# Citation
-
-As yet unpublished.
-
-# License
-
-The software itself is licensed under
-[AGPL-3.0](https://github.com/wpwupingwp/OGU/blob/master/LICENSE) (**not include
-third-party
-software**).
-
-# Q&A
-
-Please submit your questions in the
-[Issue](https://github.com/wpwupingwp/OGU/issues) page :smiley:
-* Q: The first-time run is slow.
-
-  A: OGU will automaticlly install third-party software (MAFFT/BLAST/IQTREE)
-  from AWS at first-time running. Microsoft Windows users, especially in some 
-  regions may have slow connection. Please be patient, or you can manually 
+[![PyPI version](https://badge.fury.io/py/OGU.svg)](https://badge.fury.io/py/OGU)
+
+# Quick start
+
+- Install Python 3 (3.9 or newer).
+- Open terminal, run
+
+   ```shell
+   # Install, using pip (recommended)
+   pip3 install OGU --user
+
+   # Initialize with Internet
+   # Windows
+   python -m OGU init
+   # Linux and macOS
+   python3 -m OGU init
+
+   # Run
+   # Windows
+   python -m OGU
+   # Linux and macOS
+   python3 -m OGU
+   ```
+
+# Table of Contents
+
+* [Quick start](#quickstart)
+* [Feature](#feature)
+* [Prerequisite](#prerequisite)
+    * [Hardware](#hardware)
+    * [Software](#software)
+* [Installation](#installation)
+    * [Portable](#portable)
+    * [Install with pip](#Installwithpip)
+    * [Install with conda](#Installwithconda)
+    * [Initialization](#Initialization)
+* [Usage](#usage)
+    * [Quick examples](#quick-examples)
+    * [Sequence ID](#sequence-id)
+    * [Command line](#commandline)
+* [Input](#input)
+* [Output](#output)
+* [Options](#options)
+    * [gb2fasta](#gb2fasta)
+    * [evaluate](#evaluate)
+    * [primer](#primer)
+* [Performance](#performance)
+* [Citation](#citation)
+* [License](#license)
+* [Q&A](q&a)
+
+# Features
+
+:heavy_check_mark: Automatically collect, organize and clean sequence data
+from NCBI GenBank or local: collect data with abundant options; extract CDS,
+intergenic spacer, or any other annotations from original sequence; remove
+redundant sequences according to species information; remove invalid or
+abnormal sequences/fragments; generate clean dataset with uniform sequence id.
+
+:heavy_check_mark: Evaluate variance of sequences by calculating nucleotide
+diversity, observed resolution, Shannon index, tree resolution, phylogenetic
+diversity (original and edited version), gap ratio, and others. Support
+sliding-window scanning.
+
+:heavy_check_mark: Design universal primer for the alignment. Support
+ambiguous bases in primers.
+
+# Prerequisite
+
+## Hardware
+
+`Organelle Genome Utilities (OGU)` requires very few computational resources.
+A normal PC/laptop is enough. For downloading large amount of data, make sure
+the Internet connection is stable and fast enough.
+
+## Software
+
+For the portable version, nothing need to be installed manually.
+
+For installing from pip, [Python](https://www.python.org/downloads/) is
+required. Notice that the python version should be higher than **3.6**.
+
+:white_check_mark: All third-party dependencies will be automatically
+installed with Internet, including `biopython`, `matplotlib`, `coloredlogs`,
+`numpy`, `primer3-py`, (python packages), and
+[MAFFT](https://mafft.cbrc.jp/alignment/software/),
+[IQTREE](http://www.iqtree.org/),
+[BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download).
+
+# Installation
+
+We assume that users have already installed
+[Python3](https://www.python.org/downloads/) (3.9 or above).
+
+## Install with pip
+
+1. Install [Python](https://www.python.org/downloads/). 3.9 or newer is
+   required.
+
+2. Open command line, run
+
+```shell
+pip3 install OGU --user
+```
+
+## Initialization
+
+During the first running, `OGU` will check and initialize the
+running environment. Missing dependencies will be automatically installed.
+
+This step requires Internet connection.
+
+By default, the program will automatically finish initialization, if any error
+occurs, users can choose one of the following methods:
+
+### Automatic
+
+Run the following command.
+
+```shell
+# Windows
+python -m OGU init
+# Linux and macOS
+python3 -m OGU init
+```
+
+### Use prepared package
+According to your system, download related compressed file from [packages](https://github.com/wpwupingwp/OGU/releases).
+
+For Windows users: 
+1. paste `%HOMEDRIVE%%HOMEPATH%/` to explorer's address bar and open.
+2. create `.OGU` folder. Don't miss the dot.
+3. open `.OGU` folder, paste downloaded compressed file and unzip. Make sure after
+decompress there are three folders in `.OGU`.
+
+For Linux and macOS users, please download and unpack files into
+`~/.OGU`.
+
+### Manually install
+
+For Linux users with root privileges, just use the package manager:
+
+```
+# Ubuntu and Debian
+sudo apt install mafft ncbi-blast+ iqtree
+# Fedora (1)
+sudo dnf install mafft ncbi-blast+ iqtree
+# Fedora (2)
+sudo yum install mafft ncbi-blast+ iqtree
+# ArchLinux
+sudo pacman -S mafft ncbi-blast+ iqtree
+# FreeBSD
+sudo pkg install mafft ncbi-blast+ iqtree
+```
+
+For macOS users with root privileges, install `brew` if it has not been
+installed previously:
+
+```
+/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
+```
+
+If any errors occur, install `Xcode-select` and retry.
+
+Then:
+
+```
+brew install blast mafft brewsci/science/iqtree
+```
+
+If using Windows or lacking root privileges, users should follow these
+instructions:
+
+1. BLAST+
+
+    * [Windows](https://www.ncbi.nlm.nih.gov/books/NBK52637/)
+    * [Linux and macOS](https://www.ncbi.nlm.nih.gov/books/NBK52640/)
+2. MAFFT
+
+    * [Windows](https://mafft.cbrc.jp/alignment/software/windows.html)
+
+      Choose "All-in-one version", download and unzip. Then follow the steps
+      in the BLAST+ installation manual to set the `PATH`.
+    * [Linux](https://mafft.cbrc.jp/alignment/software/linux.html)
+
+      Choose "Portable package", download and unzip. Then follow the
+      instructions of BLAST+ to set the `PATH` for `MAFFT`.
+    * [macOS](https://mafft.cbrc.jp/alignment/software/macosx.html)
+
+      Choose "All-in-one version", download and unzip. Then follow the steps
+      in the BLAST+ installation manual to set the `PATH`.
+3. IQ-TREE
+
+    * [Download](http://www.iqtree.org/#download)
+
+      Download the installer according to OS. Unzip and add the path of
+      subfolder `bin` to `PATH`.
+
+# Usage
+
+## Graphical user interface
+Open the command line (Windows) or terminal (Linux and macOS),
+run
+
+```bash
+OGU
+```
+
+or 
+```bash
+# linux and macos
+python3 -m OGU
+# windows
+python -m OGU
+```
+
+## command line
+Once a user opens the command line (Windows) or terminal (Linux and macOS), 
+just type the command:
+
+```
+# Windows
+python -m OGU [input] -[options] -out [out_folder]
+# Linux and macOS
+python3 -m OGU [input] -[options] -out [out_folder]
+```
+
+## Quick examples
+
+1. Download all `rbcL` sequences of species in Poaceae family and do
+   pre-process.
+
+```
+# Windows
+python -m OGU.gb2fasta -gene rbcL -taxon Poaceae -out rbcL_Poaceae
+# Linux and macOS
+python3 -m OGU.gb2fasta -gene rbcL -taxon Poaceae -out rbcL_Poaceae
+```
+
+2. Download all ITS sequences of _Rosa_ genus. Do pre-process and keep redundant
+   sequences:
+
+```
+# Windows
+python -m OGU.gb2fasta -query internal transcribed spacer -taxon Rosa -out Rosa_its -uniq no
+# Linux and macOS
+python3 -m OGU.gb2fasta -query internal transcribed spacer -taxon Rosa -out Rosa_its -uniq no
+```
+
+3. Download all Lamiaceae chloroplast genomic sequences in the RefSeq database.
+   Then do pre-process and evaluation of variance (skip primer designing):
+
+```
+# Windows
+python -m OGU -og cp -refseq yes -taxon Lamiaceae -out Lamiaceae_cp
+# Linux and macOS
+python3 -m OGU -og cp -refseq yes -taxon Lamiaceae -out Lamiaceae_cp
+```
+
+4. Download sequences of _Zea mays_, set length between 100 bp and 3000 bp,
+   and then perform evaluation and primer designing. Note that the space in
+   the species name is replaced with underscore "\_".
+
+```
+# Windows
+python -m OGU -taxon Zea_mays -min_len 100 -max_len 3000 -out Zea_mays -primer
+# Linux and macOS
+python3 -m OGU -taxon Zea_mays -min_len 100 -max_len 3000 -out Zea_mays -primer
+```
+
+5. Download all _Oryza_ mitochondria genomes in RefSeq database, keep the
+   longest sequence for each species and run a full analysis:
+
+```
+# Windows
+python -m OGU -taxon Oryza -og mt -min_len 50000 -max_len 200000 -uniq longest -out Oryza_cp -refseq yes -primer
+# Linux and macOS
+python3 -m OGU -taxon Oryza -og mt -min_len 50000 -max_len 200000 -uniq longest -out Oryza_cp -refseq yes -primer
+```
+
+## Sequence ID
+
+`Organelle Genome Utilities` uses a uniform sequence id format for input fasta files and all output
+sequences.
+
+```
+Locus|Kingdom|Phylum|Class|Order|Family|Genus|Species|Accession|SpecimenID_Isolate|Type
+# example
+rbcL|Viridiplantae|Streptophyta|Magnoliopsida|Poales|Poaceae|Oryza|longistaminata|MF998442|TAN:GB60B-2014|gene
+```
+
+The order of the fields is fixed. The fields are separated by vertical bars
+("|"). The space character (" ") was disallowed and was replaced by an
+underscore ("\_"). Due to missing data, some fields may be empty.
+
+`Locus`: SeqName refers to the name of a sequence. Usually it is the gene
+name. For intergenic spacer, an underscore ("\_") is used to connect two
+gene's names, e.g., "geneA_geneB".
+
+If a valid sequence name cannot be found in the annotations of the GenBank
+file, `Organelle Genome Utilities` will use "Unknown" instead.
+
+For chloroplast genes, if "-rename" option is set, the program will try to use
+regular expressions to fix potential errors in gene names.
+
+`Kingdom`: The kingdom (_Fungi, Viridiplantae, Metazoa_) of a species. For
+convenience, a superkingdom (_Bacteria, Archaea, Eukaryota, Viruses, Viroids_)
+may be used if the kingdom information for a sequence is missing.
+
+`Phylum`: The phylum of the species.
+
+`Class`: The class of the species.
+
+Because some species' classes are empty (for instance, basal angiosperm),
+`Organelle Genome Utilities` will guess the class of the species.
+
+Given the taxonomy information in GenBank file:
+
+```
+Eukaryota; Viridiplantae; Streptophyta; Embryophyta; Tracheophyta;
+    Spermatophyta; Magnoliophyta; basal Magnoliophyta; Amborellales;
+    Amborellaceae; Amborella.
+```
+
+`Organelle Genome Utilities` will use "basal Magnoliophyta" as the class because this
+expression locates before the order name ("Amborellales").
+
+`Order`: The order name of the species.
+
+`Family`: The family name of the species.
+
+`Genus`: The genus name of the species, i.e., the first part of the scientific
+name.
+
+`Species`: The specific epithet of the species, i.e., the second part of the
+scientific name of the species. It may contain the subspecies' name.
+
+`Accession`: The GenBank Accession number for the sequence. It does not
+contain the record's version.
+
+`SpecimenID` and `Isolate`: Specimen ID and Isolate ID of the sequence. May be empty.
+
+`Type`: Type of the sequence. It is usually "gene" or "spacer".
+
+## Command line
+
+:exclamation: In Linux and macOS, Python2 is `python2` and Python3 is
+`python3`. However, in Windows, Python3 is called `python`, too. Please
+notice the difference.
+
+* Show help information of each module
+
+ ```shell
+ # Windows
+ python -m OGU -h
+ python -m OGU.gb2fasta -h
+ python -m OGU.evaluate -h
+ python -m OGU.primer -h
+ # Linux and macOS
+ python3 -m OGU.gb2fasta -h
+ python3 -m OGU.evaluate -h
+ python3 -m OGU.primer -h
+ ```
+
+* Full process
+
+ ```shell
+ # Windows
+ python -m OGU -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
+ # Linux and macOS
+ python3 -m OGU -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
+ ```
+
+* Collect, convert, and clean GenBank data with gb2fasta module
+
+ ```shell
+ # Windows
+ python -m OGU.GB2fasta -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
+ # Linux and macOS
+ python3 -m OGU.gb2fasta -gene [gene name] -taxon [taxon name] -og [organelle type] -out [output name]
+ ```
+
+* Evaluate variance of given fasta files
+
+ ```shell
+ # Windows
+ python -m OGU.evaluate -fasta [fasta files]
+ # Linux and macOS
+ python3 -m OGU.evaluate -fasta [input file]
+ ```
+
+* Design universal primers of given alignments.
+
+ ```shell
+ # Windows
+ python -m OGU.primer -aln [alignment files]
+ # Linux and macOS
+ python3 -m OGU.primer -aln [alignment files]
+ ```
+
+## Visualize
+ 
+Here are to jupyter notebooks for visualize analyze result as detailed circle
+figure:
+  - `Visualize/draw_circle_plastid.ipynb`: for plastid genomes
+  - `Visualize/draw_circle_mitochondria.ipynb`: for mitochondria genomes
+
+Since users may want to customize the figure, we provide jupyter notebooks 
+instead of packaged code. Users can get the result following these steps.
+0. Run `pip install jupyterlab` to install jupyter notebooks
+1. Double click to open in jupyter notebook, Visual Studio Code or other IDEs you prefer.
+2. Edit `filename` to the Evaluation.csv you got
+3. Edit `gb_file` to extended gb file you got. Remember to generate it with 
+`-out_debug` in OGU.gb2fasta
+4. If visualize plastid data, you need provide `LSC, SSC, IRa, IRb` lengths. Or
+you can use default value, which is for *Tobacum*.
+5. Edit color themes as your wish
+6. Run all cells to output pdf figure
+ 
+# Input
+
+`Organelle Genome Utilities` accepts:
+
+1. GenBank queries. Users can use "-query" or combine with any other filters;
+2. GenBank-format files.
+3. Unaligned fasta files. Each file is considered as one locus when evaluating
+   the variance;
+4. Alignments (fasta format).
+
+# Output
+
+All results will be put in the output folder. If the user does not set the
+output path via "-out", `Organelle Genome Utilities` will create a folder labelled "Result".
+
+In the output folder, several sub-folders will be created.
+
+* GenBank
+
+  Raw GenBank files.
+
+* Divide
+
+  Fasta files converted from the GenBank file. Each file represents a
+  fragment of the original sequence according to the annotation.
+
+  For instance, a record in a "rbcL.gb" file may also contain atpB gene's
+  sequences. The "rbcL.fasta" file does not contain any upstream/downstream
+  sequences and "atpB_rbcL.fasta" does not have even one base of the atpB or
+  rbcL gene, just the spacer (assuming the annotation is precise).
+
+  User can skip this dividing step with the option "-no_divide".
+* Fasta
+
+  Raw fasta files users provided.
+* Unique
+
+  Fasta files after removing redundant sequences.
+* Expanded_fasta
+
+  To design primers, `Organelle Genome Utilities` extend a sequence to its
+  upstream/downstream. Only used in the primer module.
+* Alignment
+
+  Aligned fasta files.
+
+  `.aln`: The aligned fasta files.
+
+  `.-consensus.fastq`: The fastq format of the consensus sequence of the
+  alignment. Note that it contains alignment gap ("-"). It is NOT
+  RECOMMENDED to be used directly because the consensus-generating algorithm is
+  optimised for primer design.
+* Evaluate
+
+  Including output files from the evaluation module.
+
+  `.pdf`: The PDF format of the figure containing the sliding-window scan
+  result of the alignment.
+
+  `.csv`: The CSV format file of the sliding-window scan result. `"Index"`
+  means the location of the base in the alignment.
+
+* Primer
+
+  Including output files from the primer module.
+
+  `.primer.fastq`: The fastq format file of a primer's sequence. It contains
+  two sequences, and the direction is 5' to 3'. The first is the forward
+  primer, and the second is the reverse primer. The quality of each base is
+  equal to its proportion of the column in the alignment. Note that the
+  sequence may contain ambiguous bases if it was not disabled.
+
+  `.primers.csv`: The list of primer pairs in CSV (comma-separated values
+  text) format.
+
+  `.candidate.fasta`: The candidate primers. This file may contain
+  thousands of records. Do not recommend paying attention to it.
+
+  `.candidate.fastq`: Again, the candidate primers. This time, each file has
+  the quality information that equals to the proportion of the bases in the
+  column of the alignment.
+
+* Temp
+
+  Including temporary files. Could be safely deleted .
+
+In the output folder, there are some other important output files:
+
+* Primers.csv
+
+  The list of primer pairs in CSV (comma-separated values text) format.
+
+  Its title:
+    ```
+    Locus,Samples,Score,AvgProductLength,StdEV,MinProductLength,MaxProductLength,Coverage,Observed_Res,Tree_Res,PD_terminal,Entropy,LeftSeq,LeftTm,LeftAvgBitscore,LeftAvgMismatch,RightSeq,RightTm,RightAvgBitscore,RightAvgMismatch,DeltaTm,AlnStart,AlnEnd,AvgSeqStart,AvgSeqEnd
+    ```
+
+  `Locus`: The name of the locus/fragment.
+
+  `Samples`: The number of sequences used to find this pair of primers.
+
+  `Score`: The score of this pair of primers. Usually the higher, the better.
+
+  `AvgProductLength`: The average length of the DNA fragment amplified by
+  this pair of primers.
+
+  `StdEV`: The standard deviation of the AvgProductLength. A higher number
+  means the primer may amplify different lengths of DNA fragments.
+
+  `MinProductLength`: The minimum length of an amplified fragment.
+
+  `MaxProductLength`: The maximum length of an amplified fragment. Note that
+  all of these fields are calculated using given sequences.
+
+  `Coverage`: The coverage of this pair of primers over the sequences it
+  used. Calculated with the BLAST result. High coverage means that the pair
+  is much more "universal".
+
+  `Observed_Res`: The `observed resolution` of the sub-alignment sliced by
+  the primer pair, which is equal to the number of unique sequences divided
+  by the number of total sequences. The value is between 0 and 1.
+
+    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;R_{o}=\frac{n_{uniq}}{n_{total}}" title="R_{o}=\frac{n_{uniq}}{n_{total}}" />
+
+  `Tree_Res`: The `tree resolution` of the sub-alignment, which is equal to
+  the number of internal nodes on a phylogenetic tree (constructed from the
+  alignment) divided by number of terminal nodes. The value is between 0 and
+    1.
+
+    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;R_{T}=\frac{n_{internal}}{n_{terminal}}" title="R_{T}=\frac{n_{internal}}{n_{terminal}}" />
+
+  `PD_terminal`: The average of the terminal branch's length. It's an edited
+  version of the `Phylogenetic Diversity` for DNA barcoding evaluation.
+
+  `Entropy`: The `Shannon equitability` index of the sub-alignment. The value
+  is between 0 and 1.
+
+    <img src="https://latex.codecogs.com/svg.latex?\dpi{300}&space;E_{H}&space;=&space;\frac{-&space;\sum_{i=1}^{k}{p_{i}&space;\log(p_{i})}}{\log(k)}" title="E_{H} = \frac{- \sum_{i=1}^{k}{p_{i} \log(p_{i})}}{\log(k)}" />
+
+  `LeftSeq`: Sequence of the forward primer. The direction is 5' to 3'.
+
+  `LeftTm`: The melting temperature of the forward primer. The unit is
+  degree Celsius (°C).
+
+  `LeftAvgBitscore`: The average raw bitscore of the forward primer, which
+  is calculated by BLAST.
+
+  `LeftAvgMismatch`: The average number of mismatched bases of the forward
+  primer, as counted by BLAST.
+
+  `RightSeq`: Sequence of reverse primer. The direction is 5' to 3'.
+
+  `RightTm`: The melting temperature of the reverse primer. The unit is
+  degrees Celsius (°C).
+
+  `RightAvgBitscore`: The average raw bitscore of the reverse primer, which
+  is calculated by BLAST.
+
+  `RightAvgMismatch`: The average number of mismatched bases of the reverse
+  primer, as counted by BLAST.
+
+  `DeltaTm`: The difference in the melting temperatures of the forward and
+  reverse primers. A pair of primers with a high DeltaTm may result in
+  failure during the PCR experiment.
+
+  `AlnStart`: The location of the beginning of the forward primer (5',
+  leftmost of primer pairs) in the entire alignment.
+
+  `AlnEnd`: The location of the end of the reverse primer (5', rightmost of
+  primer pairs) in the entire alignment.
+
+  `AvgSeqStart`: The average beginning of the forward primer in the original
+  sequences.  *ONLY USED FOR DEBUG*.
+
+  `AvgSeqEnd`: The average end of the forward primer in the original
+  sequences.  *ONLY USED FOR DEBUG*.
+
+  The primer pairs are sorted by `Score`. Since the score may not fully
+  satisfy the user's specific considerations, it is suggested that primer
+  pairs be chosen manually if the first primer pair fails during the PCR
+  experiment.
+
+* Log.txt
+
+  The log file. Contains all the information printed on the screen.
+
+* Evaluation.csv
+
+  The summary of all loci/fragments, which only contains the variance
+  information for each fragment. One of the new field, `GapRatio`, means the
+  ratio of the gap ("-") in the alignment. `PD` means the original version
+  of the phylogenetic diversity and `PD_stem` means an alternative version
+  of it which only calculate the length of the stem branch in the
+  phylogenetic tree.
+
+# Options
+
+Here are some general options for the program and submodule:
+
+`-h`: Prints help messages of the program or one of the module.
+
+`-gb [filename]`: User-provided GenBank file or files. Could be one or more
+files that separated by space.
+
+For instance,
+
+```
+# one file
+-gb sequence.gb
+# multiple files
+-gb matK.gb rbcL.gb Oryza.gb Homo_sapiens.gb
+```
+
+`-fasta [filename]`: User-provided unaligned fasta files. Could be one or
+multiple.
+
+`-aln [filename]`: Alignment files that the user provides. Could be one or
+multiple.
+
+It only supports the fasta format. Ambiguous bases and gaps ("-") are supported.
+
+`-out [folder name]`: The output folder's name. All results will be put into
+the output folder. If the user does not set an output path via "-out",
+`Organelle Genome Utilities` will create a folder named "Result".
+
+`OGU` does not overwrite the existing folder with the same name.
+
+It is HIGHLY RECOMMENDED to use only letters, numbers and underscores ("\_") in
+the folder name to avoid mysterious errors caused by other Unicode characters.
+
+Options below are for specific modules.
+
+## gb2fasta
+
+### Query
+
+Options used for querying NCBI GenBank.
+
+`-taxon [taxonomy name]`: The taxonomy name. It could be any taxonomic rank
+from kingdom (same as "-group") to species, as long as the user inputs correct
+name (the scientific name of species or taxonomic group in latin, NOT
+ENGLISH). It will restrict the query to the targeted taxonomy unit. Make sure
+to use quotation marks if `taxonomy` has more than one word or use underscore
+to replace space, for instance `"Zea mays"` or `Zea_mays`.
+
+`-gene [gene name]`: The gene's name which the user wants to query in GenBank.
+If the user wants to use logical expressions like "OR", "AND", "NOT", s/he
+should use "-query" instead. If there is space in the gene's name, make sure
+to use quotation marks.
+
+Note that "ITS" is not a gene name--it is "internal transcribed spacer".
+
+Sometimes "-gene" options may bring in unwanted sequences. For example, if a
+user queries "rbcL[gene]" in GenBank, spacer sequences may contain _rbcL_ or
+_rbcL_'s upstream/downstream gene, such as "atpB_rbcL spacer" or _atpB_.
+
+`-og [ignore|both|no|mt|mitochondrion|cp|chloroplast|pl|plastid]`: Query
+organelle sequences or not. The default value is `ignore`.
+
+    - `ignore`: do not consider organelle type, same as GenBank website's
+      default setting.
+
+    - `both`: only query organelle sequences, including both plastid and
+      mitochondrion.
+
+    - `no`: exclude organelle sequences from the query.
+
+    - `cp` or `chloroplast` or `pl` or `plastid`: only query plastid sequences
+
+    - `mt` or `mitochondrion`: only query mitochondrion sequences.
+
+`-refseq [both|yes|no]`: query in RefSeq database or not. The default value is
+`both`.
+
+    - `both`: query all sequences in or not in RefSeq database, same as NCBI
+      website's default setting.
+
+    - `yes`: only query sequences in RefSeq database.
+
+    - `no`: exclude sequences in RefSeq database.
+
+[RefSeq](https://www.ncbi.nlm.nih.gov/refseq/about/) is considered to have
+higher sequence and annotation quality than GenBank. This option could be used
+for getting nuclear/organelle genomes from NCBI. In this situation (`-refseq
+yes`), the length limit will be removed automatically.
+
+`-count [number]`: Restrict numbers of sequences to be downloaded. The default
+value `0` means no restriction.
+
+`-min_len [length]`: The minimum length of the records downloaded from
+GenBank. The default value is `100` (bp). The number must be an integer.
+
+`-max_len [length]`: The maximum length of the records downloaded from
+GenBank. The default value is `10000` (bp). The number must be an integer.
+
+`-date_start [yyyy/mm/dd]`: The beginning of the release data range of the
+sequences, the format is yyyy/mm/dd.
+
+`-date_end [yyyy/mm/dd]`: The end of the release data range of the sequences,
+the format is yyyy/mm/dd.
+
+`-molecular [all|DNA|RNA]`: The molecular type,
+which could be DNA or RNA. The
+default is `all`--no restriction.
+
+`-email [email address]`: NCBI GenBank database requires users to provide
+an email address in case of abnormal situations that NCBI need to contact
+the user. For convenience, `OGU` will use
+"guest@example.com" if the user does not provide an email address. _However_,
+it is better to provide a real email address for potential contact.
+
+`-query [expression]`: The query string provided by the user. It behaves in
+the same manner as the query the user typed into the Search Box in NCBI
+GenBank's webpage.
+
+Make sure to follow NCBI's grammar for queries. It can contain several words.
+Remember to add quotation marks if an item contains more than one words, for
+instance, `"Homo sapiens"[organism]`, or use underscore to replace space,
+`Homo_sapiens[organism]`.
+
+`-exclude [expression]`: Use this option to use negative option. For instance,
+"-exclude Zea [organism]" (do not include quotation marks) will add " NOT
+(Zea[organism])" to the query.
+
+This option can be useful for excluding a specific taxon.
+
+```
+-taxon Zea -exclude "Zea mays"[organism]
+```
+
+This will query all records in genus *Zea* while records of *Zea mays* will be
+excluded.
+
+For much more complex exclude options, please consider to use "Advance search"
+in GenBank website.
+
+`-group [all|animals|plants|fungi|protists|bacteria|archaea|viruses]`: To
+restrict the query in given group. The default value is `all`--no
+restriction.
+
+It is reported that the "group" filter may return abnormal records, for
+instance, return plants' records when the group is "animal" and the
+"organelle" is "chloroplast". Furthermore, it may match a great number of
+records in GenBank. Hence, we strongly recommend using "-taxon" instead.
+
+### Divide
+
+Options used for converting GenBank files to fasta files.
+
+`-out_debug`: If you are going to use visualize pipeline to draw detailed circle
+figure, use this option to generate extended version genbank file.
+
+`-no_divide`: If set, it will analyse the whole sequence instead of the
+divided fragments. By default, `OGU` divides one GenBank record into
+several fragments according to its annotation.
+
+`-rename`: If set, the program will try to rename genes. For instance, "rbcl"
+will be renamed to "rbcL", and "tRNA UAC" will be renamed to "trnVuac", which
+consists of "trn", the amino acid's letter and transcribed codon. This may be
+helpful if the annotation has nonstandard uppercase/lowercase or naming format
+that it can merge the same sequences to one file for the same locus having
+variant names.
+
+If using Windows operating system, consider using this option to avoid
+contradictory filenames.
+
+`-unique [longest|first|no]`: The method used to remove redundant sequences.
+`OGU` will remove redundant sequences to ensure only one sequence per
+species by default. A user can change its behaviour by setting different
+methods.
+
+    - `first`: According to the records' order in the original GenBank file,
+      only the first sequence of the same species' same locus will be kept.
+      Others will be ignored directly. This is the default option due to
+      performance considerations.
+
+    - `longest`: Keep the longest sequence for one species. The program will
+      compare the sequence's length from the same species' same locus.
+
+    - `no`: Skip this step. All sequences will be kept.
+
+`-allow_mosaic_spacer`: If one gene nested with another gene, normally they
+do not have spacers. The default value is `False`.
+
+However, some users want the fragments between two gene's beginnings and ends.
+This option is for this specific purpose (e.g., matK-trnK_UUU). For normal
+usage, *do not recommend*.
+
+`-expand [number]`: The expansion length in upstream/downstream. If set,
+`OGU` will expand the sequence to its upstream/downstream after the
+dividing step to find primer candidates. The default value is `0`.
+
+Note that this option is different with "-max_len". This option limits the
+length of one annotation's sequence. The "-max_len" limits the whole
+sequence's length of one GenBank record.
+
+`-allow_repeat`: If genes repeated in downstream, this option will allow the
+repeat region to be extracted, otherwise any repeated region will be omitted.
+The default value is `False`.
+
+`-allow_invert_repeat`: If two genes invert-repeated in downstream, this
+option will allow spacers of them to be extracted, otherwise the spacer
+will be omitted. The default value is `False`.
+
+For instance, geneA-geneB located in one invert-repeat region (IR) of
+chloroplast genome. In another IR region, there are geneB-geneA. This option
+will extract sequences of two different direction as two unique spacers.
+
+`-max_name_len [number]`: The maximum length of a feature name. Some
+annotation's feature name in GenBank file is too long, and usually, they are
+not the target sequence the user wants. By setting this option, `OGU`
+will truncate the annotation's feature name if it is too long. By default, the
+value is `50`.
+
+`-max_gene_len [value]`: The maximum length of a sequence for one annotation.
+Some annotations' sequences are too long (for instance, one gene has two
+exons, and its intron is longer than 10 Kb). This option will skip those long
+sequences. By default, the value is `20000` (bp).
+
+## Evaluate
+
+`-ig` or `-ignore_gap`: ignore gaps in the alignment.
+
+`-iab` or `-ignore_ambigous`: ignore ambiguous bases in the alignment.
+
+`-quick`: skip sliding-window scan.
+
+`-size [number]`: the window size of the sliding window scan. The default
+value is `500`.
+
+`-step [number]`: the step size of the sliding window scan. The default value
+is `50`.
+
+`-skip_primer`: skip primer designing. The default value is `False`.
+
+## Primer design
+
+`-coverage [value]`: The minimum coverage of the base and primer. The default
+value is `0.5` (50%). It is used to remove primer candidates if its coverage
+among all sequences is smaller than the threshold. The coverage of primers is
+calculated by BLAST.
+
+`-res [value]`: The minimum *observed resolution* of the fragments or primer
+pairs. The default *value* is 0.3 (30%). The value should be in 0.0 to 1.0.
+
+`OGU` uses the *observed resolution* instead of others because of the
+speed. Also, it is considered to be the lower bound of the real resolution
+that a fragment with a low *observed resolution* may not have a satisfactory
+tree resolution/phylogenetic diversity, either.
+
+`-pmin [length]`: The minimal length of the primer. The default *value* is 20.
+
+`-pmax [length]`: The maximal length of the primer. The default *value* is 25.
+
+`-topn [number]`: How many pairs of primers is kept for each input alignment.
+The default value is `1`, i.e., only keep the _best_ primer pair according to
+its `score`. To keep more pairs, set "-t" to more than 1.
+
+`-amin [length]`: The minimum amplified length (include primer). The default
+value is `300` (bp). Note this limits the PCR product's length instead of the
+sub-alignment's length.
+
+`-amax [length]`: The maximum amplified length (include primer). The default
+value is `800` (bp).
+
+The "-amin" and "-amax" are used to screen primer candidates. It uses BLAST
+results to set the location of primers on each template sequence and
+calculates the average lengths of the products. Because of the variance of
+species, the same locus may have different lengths in different species, plus
+with the stretching of the alignment that gaps were added during the aligning,
+please consider adding some *margins* for these two options.
+
+For instance, if a user wants the amplified length to be smaller than 800 and
+greater than 500, s/he could consider setting "-amin" to 550 and "-amax" to
+
+750.
+
+`-ambiguous [number]`: The maximum number of ambiguous bases allowed in one
+primer. The default value is `4`.
+
+`-mismatch [number]`: The maximum number of mismatched bases in a primer. This
+option is used to remove primer candidates if the BLAST results show that
+there is too much mismatch. The default value is `4`.
+
+# Performance
+
+For a taxon that is not very large and includes few fragments, `OGU`
+can finish the task in *minutes*. For a large taxon (such as the Asteraceae
+family or the whole class of the Poales) containing multiple fragments (such
+as the chloroplast genomes), the time to complete may be one hour or more on a
+PC or laptop.
+
+`OGU` requires few memories (usually less than 0.5 GB, although, for a
+large taxon BLAST may require more) and few CPUs (one core is enough). It can
+run very well on a normal PC. Multiple CPU cores may be helpful for the
+alignment and tree construction steps.
+
+For Windows users, MAFFT [may be very slow due to antivirus
+software](https://mafft.cbrc.jp/alignment/software/windows_without_cygwin.html).
+Please consider
+following [this instruction](https://mafft.cbrc.jp/alignment/software/ubuntu_on_windows.html) to
+install
+Ubuntu on Windows to obtain better results.
+
+# Citation
+
+As yet unpublished.
+
+# License
+
+The software itself is licensed under
+[AGPL-3.0](https://github.com/wpwupingwp/OGU/blob/master/LICENSE) (**not include
+third-party
+software**).
+
+# Q&A
+
+Please submit your questions in the
+[Issue](https://github.com/wpwupingwp/OGU/issues) page :smiley:
+* Q: The first-time run is slow.
+
+  A: OGU will automaticlly install third-party software (MAFFT/BLAST/IQTREE)
+  from AWS at first-time running. Microsoft Windows users, especially in some 
+  regions may have slow connection. Please be patient, or you can manually 
   install them. See [Initialization](#Initialization).
```

### Comparing `ogu-1.52/pyproject.toml` & `ogu-1.54/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,43 @@
 [project]
 name = "OGU"
-version = "1.52"
+version = "1.54"
 description = "Organelle Genome Utilities"
-keywords = [
-    "plastid",
-    "mitochondria",
-    "organelle genome",
-    "analysis",
-    "Bioinformatics",
-]
+keywords = ['plastid', 'mitochondria', 'organelle genome', 'analysis',
+    'Bioinformatics']
 authors = [
     { name = "Ping Wu", email = "wpwupingwp@outlook.com" },
 ]
 maintainers = [
     { name = "Ping Wu", email = "wpwupingwp@outlook.com" },
 ]
 dependencies = [
     "biopython==1.82",
     "certifi>=2023.11.17",
     "coloredlogs>=10.0",
     "matplotlib>=3.0.0",
     "numpy>=1.21.6",
-    "primer3-py==2.0.1",
+    "primer3-py==2.0.2"
 ]
 requires-python = ">=3.9"
 readme = "README.md"
+license = { text = "AGPL-3.0-or-later" }
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Scientific/Engineering :: Bio-Informatics",
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'Intended Audience :: Science/Research',
+    'License :: OSI Approved :: GNU Affero General Public License v3',
+    'Operating System :: MacOS :: MacOS X',
+    'Operating System :: Microsoft :: Windows',
+    'Operating System :: POSIX',
+    'Programming Language :: Python :: 3.10',
+    'Topic :: Scientific/Engineering :: Bio-Informatics'
 ]
-
-[project.license]
-text = "AGPL-3.0-or-later"
-
 [project.scripts]
-ogu = "OGU:main"
-OGU = "OGU:main"
-
+ogu = 'OGU:main'
+OGU = 'OGU:main'
 [project.urls]
-Homepage = "https://github.com/wpwupingwp/OGU"
-"Bug Tracker" = "https://github.com/wpwupingwp/OGU/issues"
-
+'Homepage' = 'https://github.com/wpwupingwp/OGU'
+'Bug Tracker' = 'https://github.com/wpwupingwp/OGU/issues'
 [build-system]
-requires = [
-    "pdm-backend",
-    "setuptools>=69",
-]
-build-backend = "pdm.backend"
-
-[tool.pdm]
-distribution = true
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `ogu-1.52/src/OGU/cli.py` & `ogu-1.54/src/OGU/cli.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/python3
-
-import argparse
-from OGU import utils
-from OGU import gb2fasta, evaluate, primer
-from OGU.global_vars import log, name
-
-
-def parse_args():
-    """
-    Parse args and store some global/temporary values.
-    """
-    arg = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description=cli_main.__doc__)
-    general = arg.add_argument_group('General')
-    general.add_argument('-aln', help='aligned fasta files to analyze')
-    general.add_argument('-fasta', help='unaligned fasta format data to add')
-    general.add_argument('-gb', help='genbank files')
-    general.add_argument('-out', help='output directory')
-    gb2fasta_ = arg.add_argument_group('GB2Fasta')
-    # genes in IR regions
-    gb2fasta_.add_argument('-allow_mosaic_spacer', action='store_true',
-                           help='allow mosaic spacer')
-    gb2fasta_.add_argument('-allow_repeat', action='store_true',
-                           help='allow repeat genes or spacer')
-    gb2fasta_.add_argument('-allow_invert_repeat', action='store_true',
-                           help='allow invert-repeat spacers')
-    # for primer
-    gb2fasta_.add_argument('-expand', type=int, default=0,
-                           help='expand length of upstream/downstream')
-    gb2fasta_.add_argument('-max_name_len', default=100, type=int,
-                           help='maximum length of feature name')
-    # handle rps12
-    gb2fasta_.add_argument('-max_gene_len', default=20000, type=int,
-                           help='maximum length of gene fragments ')
-    gb2fasta_.add_argument('-no_divide', action='store_true',
-                           help='only download')
-    # for plastid genes
-    gb2fasta_.add_argument('-rename', action='store_true',
-                           help='try to rename gene')
-    gb2fasta_.add_argument('-unique', choices=('longest', 'first', 'no'),
-                           default='first',
-                           help='method to remove redundant sequences')
-    gb2fasta_.add_argument('-email', type=str,
-                           help='email address for querying Genbank')
-    gb2fasta_.add_argument('-exclude', type=str, help='exclude option')
-    gb2fasta_.add_argument('-gene', type=str, help='gene name')
-    # in case of same taxonomy name in different group
-    gb2fasta_.add_argument('-group',
-                           choices=('all', 'animals', 'plants', 'fungi',
-                                    'protists', 'bacteria', 'archaea',
-                                    'viruses'),
-                           default='all',
-                           help='Species kind')
-    gb2fasta_.add_argument('-min_len', default=1, type=int,
-                           help='minimum length')
-    gb2fasta_.add_argument('-max_len', default=300000, type=int,
-                           help='maximum length')
-    gb2fasta_.add_argument('-date_start', type=str,
-                           help='release date beginning, (eg. 1970/1/1)')
-    gb2fasta_.add_argument('-date_end', type=str,
-                           help='release date end, (eg. 2020/12/31)')
-    gb2fasta_.add_argument('-molecular', choices=('all', 'DNA', 'RNA'),
-                           default='all', help='molecular type')
-    gb2fasta_.add_argument('-og', '-organelle', dest='organelle',
-                           choices=('ignore', 'both', 'no', 'mt',
-                                    'mitochondrion', 'cp', 'chloroplast',
-                                    'pl', 'plastid'),
-                           default='ignore', help='organelle type')
-    gb2fasta_.add_argument('-query', nargs='*', help='query text')
-    gb2fasta_.add_argument('-refseq', choices=('both', 'yes', 'no'),
-                           default='both', help='include RefSeq or not')
-    gb2fasta_.add_argument('-genome', action='store_true',
-                            help='get complete genome')
-    gb2fasta_.add_argument('-count', default=0, type=int,
-                           help='maximum number of records to download')
-    gb2fasta_.add_argument('-taxon', help='Taxonomy name')
-    evaluate = arg.add_argument_group('Evaluate')
-    evaluate.add_argument('-ig', '-ignore_gap', dest='ignore_gap',
-                          action='store_true',
-                          help='ignore gaps in alignments')
-    evaluate.add_argument('-iab', '-ignore_ambiguous',
-                          dest='ignore_ambiguous_base', action='store_true',
-                          help='ignore ambiguous bases like "M" or "N"')
-    evaluate.add_argument('-quick', action='store_true',
-                          help='skip sliding-window analysis')
-    evaluate.add_argument('-size', type=int, default=500,
-                          help='window size')
-    evaluate.add_argument('-step', default=50, type=int,
-                          help='step length for sliding-window scan')
-    evaluate.add_argument('-primer', action='store_true',
-                          help='design universal primer')
-    primer_ = arg.add_argument_group('Primer')
-    primer_.add_argument('-ambiguous', dest='ambiguous_base_n', default=4,
-                         type=int, help='number of ambiguous bases')
-    primer_.add_argument('-coverage', dest='coverage', default=0.5, type=float,
-                         help='minimal coverage of base and primer')
-    primer_.add_argument('-mismatch', dest='mismatch', default=4, type=int,
-                         help='maximum mismatch bases in primer')
-    primer_.add_argument('-pmin', dest='min_primer', default=20, type=int,
-                         help='minimum primer length')
-    primer_.add_argument('-pmax', dest='max_primer', default=30, type=int,
-                         help='maximum primer length')
-    primer_.add_argument('-res', dest='resolution', type=float, default=0.3,
-                         help='minimal resolution')
-    primer_.add_argument('-topn', dest='top_n', type=int, default=1,
-                         help='keep n primers for each high variant region')
-    primer_.add_argument('-amin', dest='min_product', default=300, type=int,
-                         help='minimum amplified length (include primer)')
-    primer_.add_argument('-amax', dest='max_product', default=800, type=int,
-                         help='maximum amplified length (include primer)')
-    return arg.parse_args()
-
-
-def init_arg(arg):
-    ok1, _ = utils.get_third_party_path()
-    if not ok1:
-        return None
-    ok2 = utils.get_all_third_party()
-    if not ok2:
-        return None
-    arg = utils.init_out(arg)
-    if arg.out is None:
-        return None
-    query = gb2fasta.get_query_string(arg, silence=True)
-    if not any([arg.gb, arg.fasta, arg.aln, arg.query, query]):
-        log.error('Empty input.')
-        return None
-    return arg
-
-
-def cli_main():
-    """
-    Call gb2fasta, evaluate and primer functions.
-    """
-    utils.check_system()
-    log.info('Welcome to {}.'.format(name))
-    arg = parse_args()
-    arg = init_arg(arg)
-    if arg is None:
-        log.error('Quit.')
-        return
-    else:
-        from OGU import global_vars
-        global_vars.global_dict['out_inited'] = True
-    utils.add_file_log(arg)
-    option = utils.arg_to_str(arg)
-    log.debug(f'Options: {option}')
-    arg, other_args, = gb2fasta.gb2fasta_main()
-    log.debug(f'Options 2: {other_args}')
-    arg, other_args2 = evaluate.evaluate_main()
-    # if arg is None:
-    #    global_vars.global_dict['out_inited'] = False
-    log.debug(f'Options 2: {other_args2}')
-    arg, other_args3 = primer.primer_main()
-    if other_args3 is not None and len(other_args3) != 0:
-        log.debug(f'Unrecognized options {" ".join(other_args3)}')
-    log.info('Exit.')
-    return
-
-
-if __name__ == '__main__':
+#!/usr/bin/python3
+
+import argparse
+from OGU import utils
+from OGU import gb2fasta, evaluate, primer
+from OGU.global_vars import log, name
+
+
+def parse_args():
+    """
+    Parse args and store some global/temporary values.
+    """
+    arg = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description=cli_main.__doc__)
+    general = arg.add_argument_group('General')
+    general.add_argument('-aln', help='aligned fasta files to analyze')
+    general.add_argument('-fasta', help='unaligned fasta format data to add')
+    general.add_argument('-gb', help='genbank files')
+    general.add_argument('-out', help='output directory')
+    gb2fasta_ = arg.add_argument_group('GB2Fasta')
+    # genes in IR regions
+    gb2fasta_.add_argument('-allow_mosaic_spacer', action='store_true',
+                           help='allow mosaic spacer')
+    gb2fasta_.add_argument('-allow_repeat', action='store_true',
+                           help='allow repeat genes or spacer')
+    gb2fasta_.add_argument('-allow_invert_repeat', action='store_true',
+                           help='allow invert-repeat spacers')
+    # for primer
+    gb2fasta_.add_argument('-expand', type=int, default=0,
+                           help='expand length of upstream/downstream')
+    gb2fasta_.add_argument('-max_name_len', default=100, type=int,
+                           help='maximum length of feature name')
+    # handle rps12
+    gb2fasta_.add_argument('-max_gene_len', default=20000, type=int,
+                           help='maximum length of gene fragments ')
+    gb2fasta_.add_argument('-no_divide', action='store_true',
+                           help='only download')
+    # for plastid genes
+    gb2fasta_.add_argument('-rename', action='store_true',
+                           help='try to rename gene')
+    gb2fasta_.add_argument('-unique', choices=('longest', 'first', 'no'),
+                           default='first',
+                           help='method to remove redundant sequences')
+    gb2fasta_.add_argument('-email', type=str,
+                           help='email address for querying Genbank')
+    gb2fasta_.add_argument('-exclude', type=str, help='exclude option')
+    gb2fasta_.add_argument('-gene', type=str, help='gene name')
+    # in case of same taxonomy name in different group
+    gb2fasta_.add_argument('-group',
+                           choices=('all', 'animals', 'plants', 'fungi',
+                                    'protists', 'bacteria', 'archaea',
+                                    'viruses'),
+                           default='all',
+                           help='Species kind')
+    gb2fasta_.add_argument('-min_len', default=1, type=int,
+                           help='minimum length')
+    gb2fasta_.add_argument('-max_len', default=300000, type=int,
+                           help='maximum length')
+    gb2fasta_.add_argument('-date_start', type=str,
+                           help='release date beginning, (eg. 1970/1/1)')
+    gb2fasta_.add_argument('-date_end', type=str,
+                           help='release date end, (eg. 2020/12/31)')
+    gb2fasta_.add_argument('-molecular', choices=('all', 'DNA', 'RNA'),
+                           default='all', help='molecular type')
+    gb2fasta_.add_argument('-og', '-organelle', dest='organelle',
+                           choices=('ignore', 'both', 'no', 'mt',
+                                    'mitochondrion', 'cp', 'chloroplast',
+                                    'pl', 'plastid'),
+                           default='ignore', help='organelle type')
+    gb2fasta_.add_argument('-query', nargs='*', help='query text')
+    gb2fasta_.add_argument('-refseq', choices=('both', 'yes', 'no'),
+                           default='both', help='include RefSeq or not')
+    gb2fasta_.add_argument('-genome', action='store_true',
+                            help='get complete genome')
+    gb2fasta_.add_argument('-count', default=0, type=int,
+                           help='maximum number of records to download')
+    gb2fasta_.add_argument('-taxon', help='Taxonomy name')
+    evaluate = arg.add_argument_group('Evaluate')
+    evaluate.add_argument('-ig', '-ignore_gap', dest='ignore_gap',
+                          action='store_true',
+                          help='ignore gaps in alignments')
+    evaluate.add_argument('-iab', '-ignore_ambiguous',
+                          dest='ignore_ambiguous_base', action='store_true',
+                          help='ignore ambiguous bases like "M" or "N"')
+    evaluate.add_argument('-quick', action='store_true',
+                          help='skip sliding-window analysis')
+    evaluate.add_argument('-size', type=int, default=500,
+                          help='window size')
+    evaluate.add_argument('-step', default=50, type=int,
+                          help='step length for sliding-window scan')
+    evaluate.add_argument('-primer', action='store_true',
+                          help='design universal primer')
+    primer_ = arg.add_argument_group('Primer')
+    primer_.add_argument('-ambiguous', dest='ambiguous_base_n', default=4,
+                         type=int, help='number of ambiguous bases')
+    primer_.add_argument('-coverage', dest='coverage', default=0.5, type=float,
+                         help='minimal coverage of base and primer')
+    primer_.add_argument('-mismatch', dest='mismatch', default=4, type=int,
+                         help='maximum mismatch bases in primer')
+    primer_.add_argument('-pmin', dest='min_primer', default=20, type=int,
+                         help='minimum primer length')
+    primer_.add_argument('-pmax', dest='max_primer', default=30, type=int,
+                         help='maximum primer length')
+    primer_.add_argument('-res', dest='resolution', type=float, default=0.3,
+                         help='minimal resolution')
+    primer_.add_argument('-topn', dest='top_n', type=int, default=1,
+                         help='keep n primers for each high variant region')
+    primer_.add_argument('-amin', dest='min_product', default=300, type=int,
+                         help='minimum amplified length (include primer)')
+    primer_.add_argument('-amax', dest='max_product', default=800, type=int,
+                         help='maximum amplified length (include primer)')
+    return arg.parse_args()
+
+
+def init_arg(arg):
+    ok1, _ = utils.get_third_party_path()
+    if not ok1:
+        return None
+    ok2 = utils.get_all_third_party()
+    if not ok2:
+        return None
+    arg = utils.init_out(arg)
+    if arg.out is None:
+        return None
+    query = gb2fasta.get_query_string(arg, silence=True)
+    if not any([arg.gb, arg.fasta, arg.aln, arg.query, query]):
+        log.error('Empty input.')
+        return None
+    return arg
+
+
+def cli_main():
+    """
+    Call gb2fasta, evaluate and primer functions.
+    """
+    utils.check_system()
+    log.info('Welcome to {}.'.format(name))
+    arg = parse_args()
+    arg = init_arg(arg)
+    if arg is None:
+        log.error('Quit.')
+        return
+    else:
+        from OGU import global_vars
+        global_vars.global_dict['out_inited'] = True
+    utils.add_file_log(arg)
+    option = utils.arg_to_str(arg)
+    log.debug(f'Options: {option}')
+    arg, other_args, = gb2fasta.gb2fasta_main()
+    log.debug(f'Options 2: {other_args}')
+    arg, other_args2 = evaluate.evaluate_main()
+    # if arg is None:
+    #    global_vars.global_dict['out_inited'] = False
+    log.debug(f'Options 2: {other_args2}')
+    arg, other_args3 = primer.primer_main()
+    if other_args3 is not None and len(other_args3) != 0:
+        log.debug(f'Unrecognized options {" ".join(other_args3)}')
+    log.info('Exit.')
+    return
+
+
+if __name__ == '__main__':
     cli_main()
```

### Comparing `ogu-1.52/src/OGU/data/animal_orders.csv` & `ogu-1.54/src/OGU/data/animal_orders.csv`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/button1.png` & `ogu-1.54/src/OGU/data/button1.png`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/button2.png` & `ogu-1.54/src/OGU/data/button2.png`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/button3.png` & `ogu-1.54/src/OGU/data/button3.png`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/button4.png` & `ogu-1.54/src/OGU/data/button4.png`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/classes.csv` & `ogu-1.54/src/OGU/data/classes.csv`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/data/phyla.csv` & `ogu-1.54/src/OGU/data/phyla.csv`

 * *Files identical despite different names*

### Comparing `ogu-1.52/src/OGU/evaluate.py` & `ogu-1.54/src/OGU/evaluate.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,580 +1,580 @@
-#!/usr/bin/python3
-
-import argparse
-import sys
-
-from collections import namedtuple
-from os import devnull, cpu_count
-from pathlib import Path
-from subprocess import run
-
-import warnings
-import numpy as np
-from Bio import Phylo
-from matplotlib import use as mpl_use
-
-mpl_use('Agg')
-from matplotlib import pyplot as plt
-from matplotlib import rcParams
-from OGU import utils
-from OGU.global_vars import log
-
-# ignore warnings from numpy
-warnings.filterwarnings('ignore', category=RuntimeWarning)
-# update matplotlib settings
-params = {'axes.labelsize': 12, 'axes.linewidth': 1.5, 'axes.titlesize': 20,
-          'font.size': 12, 'lines.linewidth': 1.5,
-          'legend.fontsize': 10, 'legend.handlelength': 2}
-rcParams.update(params)
-
-
-def parse_args(arg_list=None):
-    arg = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description=evaluate_main.__doc__)
-    arg.add_argument('-fasta', nargs='*', help='unaligned fasta files')
-    arg.add_argument('-fasta_folder', default=None,
-                     help='folder of fasta files')
-    arg.add_argument('-aln', nargs='*', help='aligned files')
-    arg.add_argument('-out', help='output folder')
-    arg.add_argument('-primer', action='store_true',
-                     help='design universal primer')
-    options = arg.add_argument_group('Options')
-    options.add_argument('-ig', '-ignore_gap', dest='ignore_gap',
-                         action='store_true',
-                         help='ignore gaps in alignments')
-    options.add_argument('-iab', '-ignore_ambiguous',
-                         dest='ignore_ambiguous_base',
-                         action='store_true',
-                         help='ignore ambiguous bases like "M" or "N"')
-    sliding_window = arg.add_argument_group('Sliding-window')
-    sliding_window.add_argument('-quick', action='store_true',
-                                help='skip sliding-window analysis')
-    sliding_window.add_argument('-size', type=int, default=500,
-                                help='window size')
-    sliding_window.add_argument('-step', type=int, default=50,
-                                help='step length')
-    if arg_list is None:
-        return arg.parse_known_args()
-    else:
-        return arg.parse_known_args(arg_list)
-
-
-def init_arg(arg):
-    arg = utils.init_out(arg)
-    if all([arg.fasta, arg.fasta_folder]):
-        log.info('Do not recommend to  use "-fasta" and "-fasta_folder" '
-                 'at same time!')
-    if arg.fasta is not None:
-        arg.fasta = [Path(i).absolute() for i in arg.fasta]
-    else:
-        arg.fasta = []
-    if arg.fasta_folder is not None:
-        for i in Path(arg.fasta_folder).glob('*'):
-            arg.fasta.append(i.absolute())
-    log.info('Add fasta from gb2fasta module if possible.')
-    for i in Path(arg._unique).glob('*'):
-        if i.name != 'Unknown.fasta':
-            arg.fasta.append(i.absolute())
-    if arg.fasta:
-        for i in arg.fasta:
-            if not i.exists() or not i.is_file():
-                log.error(f'{i} does not exist or is not a valid file.')
-                return None
-    if arg.aln is not None:
-        arg.aln = [Path(i).absolute() for i in arg.aln]
-        for i in arg.aln:
-            if not i.exists() or not i.is_file():
-                log.error(f'{i} does not exist or is not a valid file.')
-                return None
-    else:
-        arg.aln = []
-    if not any([arg.fasta, arg.aln, arg.fasta_folder]):
-        log.warning('Empty input.')
-        return None
-    if arg.quick:
-        log.info('The "-quick" mode was opened. '
-                 'Skip sliding-window analysis')
-    return arg
-
-
-def align(files: list, folder: Path) -> (list, list):
-    """
-    Align sequences with mafft.
-    Args:
-        files(list): fasta files
-        folder(path): folder for output
-    Returns:
-        aligned(list): aligned fasta
-        unaligned(list): unaligned files
-    """
-    log.info('Align sequences.')
-    aligned = list()
-    unaligned = list()
-    if not files:
-        return aligned, unaligned
-    _, mafft = utils.get_mafft()
-    if not _:
-        log.error('Cannot run MAFFT.')
-        return aligned, unaligned
-    # get available CPU cores
-    cores = max(1, cpu_count() - 1)
-    for fasta in files:
-        log.info('Aligning {}.'.format(fasta))
-        out = folder / fasta.with_suffix('.aln').name
-        with open(devnull, 'w', encoding='utf-8') as f:
-            # if computer is good enough, "--genafpair" is recommended
-            # where is mafft?
-            _ = (f'{mafft} --auto --thread {cores} --reorder --quiet '
-                 f'--adjustdirection {fasta} > {out}')
-            m = run(_, shell=True, stdout=f, stderr=f)
-        if m.returncode == 0:
-            aligned.append(out)
-        else:
-            unaligned.append(fasta)
-            try:
-                out.unlink()
-            except Exception:
-                pass
-    log.info('Alignment finished.')
-    for i in Path().cwd().glob('_order*'):
-        i.unlink()
-    log.info(f'Total {len(files)} files')
-    log.info(f'Aligned {len(aligned)}')
-    log.info(f'Unaligned {len(unaligned)}')
-    return aligned, unaligned
-
-
-def array_to_fasta(alignment: np.array, filename: Path) -> Path:
-    """
-    Convert np.array to fasta.
-    Use index number as sequence id.
-    Args:
-        alignment
-        filename
-    Returns:
-        filename
-    """
-    with open(filename, 'wb') as aln:
-        for index, row in enumerate(alignment):
-            aln.write(b'>' + str(index).encode('utf-8') + b'\n')
-            aln.write(b''.join(row) + b'\n')
-    return filename
-
-
-def fasta_to_array(aln_fasta: Path) -> (np.array, np.array):
-    """
-    Given fasta format alignment filename, return a numpy array for sequence:
-    Faster and use smaller mem.
-    Ensure all bases are capital.
-    Args:
-        aln_fasta(Path): aligned fasta file
-    Returns:
-        name(np.array): name array
-        sequence(np.array): sequence array
-    """
-    data = []
-    record = ['id', 'sequence']
-    with open(aln_fasta, 'r', encoding='utf-8') as raw:
-        for line in raw:
-            if line.startswith('>'):
-                data.append([record[0], ''.join(record[1:])])
-                # remove ">" and CRLF
-                name = line[1:].strip()
-                record = [name, '']
-            else:
-                record.append(line.strip().upper())
-        # add last sequence
-        data.append([record[0], ''.join(record[1:])])
-    # skip head['id', 'seq']
-    data = data[1:]
-    # check sequence length
-    length_check = [len(i[1]) for i in data]
-    if len(set(length_check)) != 1:
-        log.info(f'Invalid alignment file {aln_fasta}')
-        return None, None
-    # Convert List to numpy array.
-    # order 'F' is a bit faster than 'C'
-    # new = np.hstack((name, seq)) -> is slower
-    name_array = np.array([[i[0]] for i in data], dtype=np.bytes_)
-    # fromiter is faster than from list
-    # S1: bytes
-    sequence_array = np.array(
-        [np.fromiter(i[1], dtype=np.dtype('S1')) for i in data],
-        order='F')
-    if name_array is None:
-        log.error('Bad fasta file {}.'.format(aln_fasta))
-    return name_array, sequence_array
-
-
-def remove_gap(alignment: np.array, silence=False) -> (np.array, np.array):
-    """
-    Split alignment into with_gap and without_gap.
-    Args:
-        alignment: raw array
-        silence: if True, don't print log
-    Returns:
-        no_gap_columns: without gap
-        gap_columns: columns having gaps
-    """
-    gap = b'-'
-    # axis 0 for column
-    have_gap = np.any(alignment == gap, axis=0)
-    gap_columns = alignment[:, have_gap]
-    no_gap_columns = alignment[:, ~have_gap]
-    n_columns = alignment.shape[1]
-    n_gap_columns = gap_columns.shape[1]
-    log.info(f'{n_columns} columns, {n_gap_columns} have gaps.')
-    if n_gap_columns / n_columns > 0.5 and not silence:
-        log.warning('Too much columns with gaps.')
-    return no_gap_columns, gap_columns
-
-
-def gc_ratio(alignment: np.array, ignore_ambiguous=True) -> (
-        float, np.array):
-    """
-    Get GC ratio of total alignment and each sequence.
-    Args:
-        alignment: np.array
-        ignore_ambiguous: count ambiguous bases or not
-    Returns:
-        total_gc: gc value
-        gc_array: np.array of gc value for each row(sequence)
-    """
-
-    def get_gc_ratio(row: np.array, ignore: bool):
-        # if True, do not count ambiguous bases as GC, but count them in total
-        # BDVH = 1/3 GC
-        # MSYKRS = 1/2 GC
-        gc = 0
-        count_ = np.unique(row, return_counts=True)
-        count = dict(zip(count_[0], count_[1]))
-        for base in (b'G', b'C'):
-            gc += count.get(base, 0)
-        if not ignore:
-            gc += count.get(b'N', 0) / 4
-            for ambiguous_base in (b'B', b'D', b'V', b'H'):
-                gc += count.get(ambiguous_base, 0) / 3
-            for ambiguous_base in (b'M', b'S', b'Y', b'K', b'R', b'S'):
-                gc += count.get(ambiguous_base, 0) / 2
-        return gc / (rows * columns - count.get(b'-', 0))
-
-    rows, columns = alignment.shape
-    total_gc = get_gc_ratio(alignment, ignore_ambiguous)
-    gc_array = np.fromiter(
-        [get_gc_ratio(row, ignore_ambiguous) for row in alignment],
-        dtype=float)
-    return total_gc, gc_array
-
-
-def normalized_entropy(count: np.array, rows: int) -> float:
-    """
-    Calculate normalized entropy.
-    Args:
-        count: np.unique(axis=0)
-        rows: rows number
-    Returns:
-        entropy(float): normalized entropy
-    """
-    max_h = np.log2(rows)
-    entropy = 0
-    for j in count:
-        p_j = j / rows
-        log2_p_j = np.log2(p_j)
-        entropy += log2_p_j * p_j
-    entropy = -1 * entropy / max_h
-    # entropy should > 0
-    return max(0, entropy)
-
-
-def nucleotide_diversity(alignment: np.array) -> float:
-    """
-    Nucleotide diversity (pi)
-    Args:
-        alignment: np.array
-    Returns:
-        pi: float
-    """
-    rows, columns = alignment.shape
-    m = columns
-    n = rows
-    sum_d_ij = 0
-    for i in range(n):
-        d_ij = np.sum(alignment[i] != alignment[(i + 1):])
-        sum_d_ij += d_ij
-    pi = (2 / (n * (n - 1)) * sum_d_ij) / m
-    # pi should > 0, use max()
-    return max(0, pi)
-
-
-def fix_only_gaps(array: np.array) -> np.array:
-    # for iqtree only
-    tmp = b'A'
-    new = array.copy()
-    n_col = array.shape[1]
-    for row in new:
-        if np.count_nonzero(row == b'-') == n_col:
-            row[0] = tmp
-    return new
-
-
-def phylogenetic_diversity(alignment: np.array, tmp: Path) -> (float, float,
-                                                               float, float):
-    """
-    Calculate the phylogenetic diversity.
-    Use HKY model for saving time.
-    Args:
-        alignment: np.array
-        tmp: tmp folder
-    Returns:
-        pd: phylogenetic diversity
-        pd_stem: only calculate stem branch
-        pd_stem_sd: standard deviation
-        pd_terminal: only calculate terminal
-        pd_terminal_sd: standard deviation
-        tree_res: tree resolution
-    """
-    pd = 0.0
-    pd_stem = 0.0
-    pd_stem_sd = 0.0
-    pd_terminal = 0.0
-    pd_terminal_sd = 0.0
-    tree_res = 0.0
-    rows, columns = alignment.shape
-    if rows < 4:
-        log.debug('Too few sequences.')
-        return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
-    old_max_recursion = sys.getrecursionlimit()
-    sys.setrecursionlimit(max(rows + 10, old_max_recursion))
-    aln_file = tmp / f'{columns}.tmp'
-    fixed_aln = fix_only_gaps(alignment)
-    array_to_fasta(fixed_aln, aln_file)
-    _, iqtree = utils.get_iqtree()
-    if not _:
-        log.critical('Cannot find iqtree.')
-        return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
-    with open(devnull, 'w', encoding='utf-8') as out:
-        t_cmd = f'{iqtree} -s {aln_file} -m HKY -fast -czb -redo'
-        run_ = run(t_cmd, stdout=out, stderr=out, shell=True)
-        # just return 0 if there is error
-    if run_.returncode != 0:
-        log.debug('Found sequence with only gaps.')
-    else:
-        tree = Phylo.read(str(aln_file) + '.treefile', 'newick')
-        try:
-            # skip the first empty node
-            internals = tree.get_nonterminals()[1:]
-            non_zero_internals = [i for i in internals if i.branch_length != 0]
-            terminals = tree.get_terminals()
-            # may be zero
-            n_terminals = max(1, len(terminals))
-            pd = tree.total_branch_length() / n_terminals
-            pd_stem = sum([i.branch_length for i in internals]) / n_terminals
-            pd_stem_sd = np.std(
-                [i.branch_length for i in internals]) / n_terminals
-            pd_terminal = sum(
-                [i.branch_length for i in terminals]) / n_terminals
-            pd_terminal_sd = np.std(
-                [i.branch_length for i in terminals]) / n_terminals
-            tree_res = len(non_zero_internals) / n_terminals
-        except Exception:
-            log.debug('Bad phylogenetic tree.')
-    utils.clean_tmp(aln_file)
-    sys.setrecursionlimit(old_max_recursion)
-    return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
-
-
-class Variance(namedtuple('Variance',
-                          ['Samples', 'Length', 'Gap_Ratio',
-                           'Observed_Res', 'Entropy', 'Pi',
-                           'PD', 'PD_stem', 'PD_stem_SD',
-                           'PD_terminal', 'PD_terminal_SD',
-                           'Tree_Res', 'Total_GC'],
-                          defaults=[0 for i in range(13)])):
-    """
-    For get_resolution()
-    samples: rows
-    length: columns
-    """
-    __slots__ = ()
-
-    def __str__(self):
-        return ('{Samples},{Length},{Gap_Ratio:.4%},'
-                '{Observed_Res:.4%},{Entropy:.8f},{Pi:.8f},'
-                '{PD:.8f},{PD_stem:.8f},{PD_stem_SD:.8f},'
-                '{PD_terminal:.8f},{PD_terminal_SD:.8f},'
-                '{Tree_Res:.4%},{Total_GC:.4%}'.format(**self._asdict()))
-
-
-def get_resolution(alignment: np.array, tmp: Path,
-                   ignore_ambiguous=True) -> tuple:
-    """
-    Given alignment (2d numpy array), location of fragment(start and end, int,
-    start from zero, exclude end),
-    return gap ratio, resolution, entropy, Pi, tree value and average terminal
-    branch length.
-    """
-    gc_array = np.array([0])
-    rows, columns = alignment.shape
-    total = rows * columns
-    # index error
-    if columns == 0:
-        return Variance(), gc_array
-    gap_ratio = len(alignment[alignment == b'-']) / total
-    item, count = np.unique(alignment, return_counts=True, axis=0)
-    observed_res = len(count) / rows
-    # normalized entropy
-    entropy = normalized_entropy(count, rows)
-    pi = nucleotide_diversity(alignment)
-    (pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd,
-     tree_res) = phylogenetic_diversity(alignment, tmp)
-    total_gc, gc_array = gc_ratio(alignment, ignore_ambiguous)
-    variance = Variance(rows, columns, gap_ratio, observed_res, entropy, pi,
-                        pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd,
-                        tree_res, total_gc)
-    return variance, gc_array
-
-
-def output_sliding(sliding: list, name: str, out: Path,
-                   size: int, step: int) -> (Path, Path):
-    if len(sliding) == 0:
-        log.warning('Empty sliding-window result.')
-        return Path(), Path()
-    out_csv = out / (name + '.csv')
-    head = 'Start,End,' + ','.join(Variance._fields) + '\n'
-    handle = open(out_csv, 'w', encoding='utf-8')
-    handle.write(head)
-    index = []
-    # for human reading
-    start = 1
-    for variance in sliding:
-        line = f'{start},{start + size},{variance}\n'
-        index.append(start)
-        handle.write(line)
-        start += step
-    handle.close()
-    # draw
-    out_pdf = out / (name + '.pdf')
-    plt.style.use('seaborn-v0_8-colorblind')
-    # how to find optimized size?
-    fig = plt.figure(figsize=(15 + len(sliding) // 5000, 10))
-    ax1 = plt.subplot(211)
-    ax1.yaxis.set_ticks(np.linspace(0, 1, num=11))
-    ax1.set_title(f'{name} ({sliding[0].Samples} sequences)', pad=30)
-    ax1.set_xlabel('Bases')
-    ax1.set_ylabel('Values')
-    ax1.plot(index, [i.Gap_Ratio for i in sliding], label='Gap Ratio',
-             alpha=0.8)
-    ax1.plot(index, [i.Observed_Res for i in sliding],
-             label='Observed Resolution', alpha=0.8)
-    ax1.plot(index, [i.Entropy for i in sliding],
-             label='Shannon Equitability Index', alpha=0.8)
-    ax1.plot(index, [i.Tree_Res for i in sliding], label='Tree Resolution',
-             alpha=0.8)
-    ax1.plot(index, [i.Total_GC for i in sliding], label='GC Ratio',
-             alpha=0.8)
-    ax1.plot(index, [i.Pi for i in sliding], label=r'$\pi$', alpha=0.8)
-    ax1.legend(loc='upper right', framealpha=0.5)
-    # different ytick
-    ax2 = plt.subplot(212)
-    ax1.set_xlabel('Bases')
-    # ax2..yaxis.set_ticks(np.linspace(0, max_range, 21))
-    ax2.set_ylabel('Values')
-    ax2.plot(index, [i.PD for i in sliding], linestyle='--', label='PD',
-             alpha=0.8)
-    ax2.plot(index, [i.PD_stem for i in sliding], linestyle='--',
-             label='PD_stem', alpha=0.8)
-    ax2.plot(index, [i.PD_terminal for i in sliding], linestyle='--',
-             label='PD_terminal', alpha=0.8)
-    # k--
-    ax2.legend(loc='upper right', framealpha=0.5)
-    plt.savefig(out_pdf)
-    plt.close()
-    return out_csv, out_pdf
-
-
-def evaluate(aln: Path, arg) -> tuple:
-    """
-    Wrapper
-    Args:
-        aln: alignment file
-        arg: args
-    Returns:
-        summary: namedtuple
-        gc_array: for draw
-        sliding: list of Variance
-    """
-    sliding = []
-    name, alignment = fasta_to_array(aln)
-    if name is None:
-        return None, None, None
-    if arg.ignore_gap:
-        no_gap_alignment, gap_alignment = remove_gap(alignment)
-    else:
-        no_gap_alignment = alignment
-        gap_alignment = np.array([[]])
-    rows, columns = alignment.shape
-    log.info(f'Evaluate {aln}')
-    summary, gc_array = get_resolution(no_gap_alignment, arg._tmp,
-                                       arg.ignore_ambiguous_base)
-    if arg.quick:
-        pass
-    else:
-        # sliding window
-        for i in range(0, columns - arg.size, arg.step):
-            # view, not copy
-            subalign = alignment[:, i:i + arg.size]
-            if arg.ignore_gap:
-                subalign, gap_subalign = remove_gap(alignment, silence=True)
-            variance, sub_gc_array = get_resolution(subalign, arg._tmp,
-                                                    arg.ignore_ambiguous_base)
-            sliding.append(variance)
-    return summary, gc_array, sliding
-
-
-def evaluate_main(arg_str=None):
-    """
-    Evaluate variance of alignments.
-    """
-    log.info('Running evaluate module...')
-    if arg_str is None:
-        arg, other_args2 = parse_args()
-    else:
-        arg, other_args2 = parse_args(arg_str.split(' '))
-    arg = init_arg(arg)
-    if arg is None:
-        log.info('Quit evaluate module.')
-        return None, other_args2
-    utils.add_file_log(arg)
-    aligned, unaligned = align(arg.fasta, arg._align)
-    aligned.extend(arg.aln)
-    evaluation_result = arg.out / 'Evaluation.csv'
-    csv_head = 'Loci,' + ','.join(Variance._fields) + '\n'
-    with open(evaluation_result, 'w', encoding='utf-8') as out_csv:
-        out_csv.write(csv_head)
-    for aln in aligned:
-        summary, gc_array, sliding = evaluate(aln, arg)
-        if summary is None:
-            continue
-        log.info(f'\t{aln.stem}')
-        log.info(f'\tSamples:                   {summary.Samples}')
-        log.info(f'\tLength                     {summary.Length} bp')
-        log.info(f'\tGap ratio:                 {summary.Gap_Ratio:.8f}')
-        log.info(f'\tObserved resolution:       {summary.Observed_Res:.8f}')
-        log.info(f'\tNormalized Shannon Index:  {summary.Entropy:.8f}')
-        log.info(f'\tPi:                        {summary.Pi:.8f}')
-        log.info(f'\tPhylogenetic diversity:    {summary.PD:.8f}')
-        log.info(f'\tTree resolution:           {summary.Tree_Res:.8f}')
-        with open(evaluation_result, 'a', encoding='utf-8') as out:
-            out.write(aln.stem + ',' + str(summary) + '\n')
-        if not arg.quick:
-            output_sliding(sliding, aln.stem, arg._evaluate, arg.size, arg.step)
-    log.info(f'Evaluation results could be found in {evaluation_result}')
-    log.info('Evaluate module finished.')
-    # for i in aligned:
-    #     utils.move(i, arg._align/(i.name), copy=True)
-    return arg, other_args2
-
-
-if __name__ == '__main__':
+#!/usr/bin/python3
+
+import argparse
+import sys
+
+from collections import namedtuple
+from os import devnull, cpu_count
+from pathlib import Path
+from subprocess import run
+
+import warnings
+import numpy as np
+from Bio import Phylo
+from matplotlib import use as mpl_use
+
+mpl_use('Agg')
+from matplotlib import pyplot as plt
+from matplotlib import rcParams
+from OGU import utils
+from OGU.global_vars import log
+
+# ignore warnings from numpy
+warnings.filterwarnings('ignore', category=RuntimeWarning)
+# update matplotlib settings
+params = {'axes.labelsize': 12, 'axes.linewidth': 1.5, 'axes.titlesize': 20,
+          'font.size': 12, 'lines.linewidth': 1.5,
+          'legend.fontsize': 10, 'legend.handlelength': 2}
+rcParams.update(params)
+
+
+def parse_args(arg_list=None):
+    arg = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description=evaluate_main.__doc__)
+    arg.add_argument('-fasta', nargs='*', help='unaligned fasta files')
+    arg.add_argument('-fasta_folder', default=None,
+                     help='folder of fasta files')
+    arg.add_argument('-aln', nargs='*', help='aligned files')
+    arg.add_argument('-out', help='output folder')
+    arg.add_argument('-primer', action='store_true',
+                     help='design universal primer')
+    options = arg.add_argument_group('Options')
+    options.add_argument('-ig', '-ignore_gap', dest='ignore_gap',
+                         action='store_true',
+                         help='ignore gaps in alignments')
+    options.add_argument('-iab', '-ignore_ambiguous',
+                         dest='ignore_ambiguous_base',
+                         action='store_true',
+                         help='ignore ambiguous bases like "M" or "N"')
+    sliding_window = arg.add_argument_group('Sliding-window')
+    sliding_window.add_argument('-quick', action='store_true',
+                                help='skip sliding-window analysis')
+    sliding_window.add_argument('-size', type=int, default=500,
+                                help='window size')
+    sliding_window.add_argument('-step', type=int, default=50,
+                                help='step length')
+    if arg_list is None:
+        return arg.parse_known_args()
+    else:
+        return arg.parse_known_args(arg_list)
+
+
+def init_arg(arg):
+    arg = utils.init_out(arg)
+    if all([arg.fasta, arg.fasta_folder]):
+        log.info('Do not recommend to  use "-fasta" and "-fasta_folder" '
+                 'at same time!')
+    if arg.fasta is not None:
+        arg.fasta = [Path(i).absolute() for i in arg.fasta]
+    else:
+        arg.fasta = []
+    if arg.fasta_folder is not None:
+        for i in Path(arg.fasta_folder).glob('*'):
+            arg.fasta.append(i.absolute())
+    log.info('Add fasta from gb2fasta module if possible.')
+    for i in Path(arg._unique).glob('*'):
+        if i.name != 'Unknown.fasta':
+            arg.fasta.append(i.absolute())
+    if arg.fasta:
+        for i in arg.fasta:
+            if not i.exists() or not i.is_file():
+                log.error(f'{i} does not exist or is not a valid file.')
+                return None
+    if arg.aln is not None:
+        arg.aln = [Path(i).absolute() for i in arg.aln]
+        for i in arg.aln:
+            if not i.exists() or not i.is_file():
+                log.error(f'{i} does not exist or is not a valid file.')
+                return None
+    else:
+        arg.aln = []
+    if not any([arg.fasta, arg.aln, arg.fasta_folder]):
+        log.warning('Empty input.')
+        return None
+    if arg.quick:
+        log.info('The "-quick" mode was opened. '
+                 'Skip sliding-window analysis')
+    return arg
+
+
+def align(files: list, folder: Path) -> (list, list):
+    """
+    Align sequences with mafft.
+    Args:
+        files(list): fasta files
+        folder(path): folder for output
+    Returns:
+        aligned(list): aligned fasta
+        unaligned(list): unaligned files
+    """
+    log.info('Align sequences.')
+    aligned = list()
+    unaligned = list()
+    if not files:
+        return aligned, unaligned
+    _, mafft = utils.get_mafft()
+    if not _:
+        log.error('Cannot run MAFFT.')
+        return aligned, unaligned
+    # get available CPU cores
+    cores = max(1, cpu_count() - 1)
+    for fasta in files:
+        log.info('Aligning {}.'.format(fasta))
+        out = folder / fasta.with_suffix('.aln').name
+        with open(devnull, 'w', encoding='utf-8') as f:
+            # if computer is good enough, "--genafpair" is recommended
+            # where is mafft?
+            _ = (f'{mafft} --auto --thread {cores} --reorder --quiet '
+                 f'--adjustdirection {fasta} > {out}')
+            m = run(_, shell=True, stdout=f, stderr=f)
+        if m.returncode == 0:
+            aligned.append(out)
+        else:
+            unaligned.append(fasta)
+            try:
+                out.unlink()
+            except Exception:
+                pass
+    log.info('Alignment finished.')
+    for i in Path().cwd().glob('_order*'):
+        i.unlink()
+    log.info(f'Total {len(files)} files')
+    log.info(f'Aligned {len(aligned)}')
+    log.info(f'Unaligned {len(unaligned)}')
+    return aligned, unaligned
+
+
+def array_to_fasta(alignment: np.array, filename: Path) -> Path:
+    """
+    Convert np.array to fasta.
+    Use index number as sequence id.
+    Args:
+        alignment
+        filename
+    Returns:
+        filename
+    """
+    with open(filename, 'wb') as aln:
+        for index, row in enumerate(alignment):
+            aln.write(b'>' + str(index).encode('utf-8') + b'\n')
+            aln.write(b''.join(row) + b'\n')
+    return filename
+
+
+def fasta_to_array(aln_fasta: Path) -> (np.array, np.array):
+    """
+    Given fasta format alignment filename, return a numpy array for sequence:
+    Faster and use smaller mem.
+    Ensure all bases are capital.
+    Args:
+        aln_fasta(Path): aligned fasta file
+    Returns:
+        name(np.array): name array
+        sequence(np.array): sequence array
+    """
+    data = []
+    record = ['id', 'sequence']
+    with open(aln_fasta, 'r', encoding='utf-8') as raw:
+        for line in raw:
+            if line.startswith('>'):
+                data.append([record[0], ''.join(record[1:])])
+                # remove ">" and CRLF
+                name = line[1:].strip()
+                record = [name, '']
+            else:
+                record.append(line.strip().upper())
+        # add last sequence
+        data.append([record[0], ''.join(record[1:])])
+    # skip head['id', 'seq']
+    data = data[1:]
+    # check sequence length
+    length_check = [len(i[1]) for i in data]
+    if len(set(length_check)) != 1:
+        log.info(f'Invalid alignment file {aln_fasta}')
+        return None, None
+    # Convert List to numpy array.
+    # order 'F' is a bit faster than 'C'
+    # new = np.hstack((name, seq)) -> is slower
+    name_array = np.array([[i[0]] for i in data], dtype=np.bytes_)
+    # fromiter is faster than from list
+    # S1: bytes
+    sequence_array = np.array(
+        [np.fromiter(i[1], dtype=np.dtype('S1')) for i in data],
+        order='F')
+    if name_array is None:
+        log.error('Bad fasta file {}.'.format(aln_fasta))
+    return name_array, sequence_array
+
+
+def remove_gap(alignment: np.array, silence=False) -> (np.array, np.array):
+    """
+    Split alignment into with_gap and without_gap.
+    Args:
+        alignment: raw array
+        silence: if True, don't print log
+    Returns:
+        no_gap_columns: without gap
+        gap_columns: columns having gaps
+    """
+    gap = b'-'
+    # axis 0 for column
+    have_gap = np.any(alignment == gap, axis=0)
+    gap_columns = alignment[:, have_gap]
+    no_gap_columns = alignment[:, ~have_gap]
+    n_columns = alignment.shape[1]
+    n_gap_columns = gap_columns.shape[1]
+    log.info(f'{n_columns} columns, {n_gap_columns} have gaps.')
+    if n_gap_columns / n_columns > 0.5 and not silence:
+        log.warning('Too much columns with gaps.')
+    return no_gap_columns, gap_columns
+
+
+def gc_ratio(alignment: np.array, ignore_ambiguous=True) -> (
+        float, np.array):
+    """
+    Get GC ratio of total alignment and each sequence.
+    Args:
+        alignment: np.array
+        ignore_ambiguous: count ambiguous bases or not
+    Returns:
+        total_gc: gc value
+        gc_array: np.array of gc value for each row(sequence)
+    """
+
+    def get_gc_ratio(row: np.array, ignore: bool):
+        # if True, do not count ambiguous bases as GC, but count them in total
+        # BDVH = 1/3 GC
+        # MSYKRS = 1/2 GC
+        gc = 0
+        count_ = np.unique(row, return_counts=True)
+        count = dict(zip(count_[0], count_[1]))
+        for base in (b'G', b'C'):
+            gc += count.get(base, 0)
+        if not ignore:
+            gc += count.get(b'N', 0) / 4
+            for ambiguous_base in (b'B', b'D', b'V', b'H'):
+                gc += count.get(ambiguous_base, 0) / 3
+            for ambiguous_base in (b'M', b'S', b'Y', b'K', b'R', b'S'):
+                gc += count.get(ambiguous_base, 0) / 2
+        return gc / (rows * columns - count.get(b'-', 0))
+
+    rows, columns = alignment.shape
+    total_gc = get_gc_ratio(alignment, ignore_ambiguous)
+    gc_array = np.fromiter(
+        [get_gc_ratio(row, ignore_ambiguous) for row in alignment],
+        dtype=float)
+    return total_gc, gc_array
+
+
+def normalized_entropy(count: np.array, rows: int) -> float:
+    """
+    Calculate normalized entropy.
+    Args:
+        count: np.unique(axis=0)
+        rows: rows number
+    Returns:
+        entropy(float): normalized entropy
+    """
+    max_h = np.log2(rows)
+    entropy = 0
+    for j in count:
+        p_j = j / rows
+        log2_p_j = np.log2(p_j)
+        entropy += log2_p_j * p_j
+    entropy = -1 * entropy / max_h
+    # entropy should > 0
+    return max(0, entropy)
+
+
+def nucleotide_diversity(alignment: np.array) -> float:
+    """
+    Nucleotide diversity (pi)
+    Args:
+        alignment: np.array
+    Returns:
+        pi: float
+    """
+    rows, columns = alignment.shape
+    m = columns
+    n = rows
+    sum_d_ij = 0
+    for i in range(n):
+        d_ij = np.sum(alignment[i] != alignment[(i + 1):])
+        sum_d_ij += d_ij
+    pi = (2 / (n * (n - 1)) * sum_d_ij) / m
+    # pi should > 0, use max()
+    return max(0, pi)
+
+
+def fix_only_gaps(array: np.array) -> np.array:
+    # for iqtree only
+    tmp = b'A'
+    new = array.copy()
+    n_col = array.shape[1]
+    for row in new:
+        if np.count_nonzero(row == b'-') == n_col:
+            row[0] = tmp
+    return new
+
+
+def phylogenetic_diversity(alignment: np.array, tmp: Path) -> (float, float,
+                                                               float, float):
+    """
+    Calculate the phylogenetic diversity.
+    Use HKY model for saving time.
+    Args:
+        alignment: np.array
+        tmp: tmp folder
+    Returns:
+        pd: phylogenetic diversity
+        pd_stem: only calculate stem branch
+        pd_stem_sd: standard deviation
+        pd_terminal: only calculate terminal
+        pd_terminal_sd: standard deviation
+        tree_res: tree resolution
+    """
+    pd = 0.0
+    pd_stem = 0.0
+    pd_stem_sd = 0.0
+    pd_terminal = 0.0
+    pd_terminal_sd = 0.0
+    tree_res = 0.0
+    rows, columns = alignment.shape
+    if rows < 4:
+        log.debug('Too few sequences.')
+        return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
+    old_max_recursion = sys.getrecursionlimit()
+    sys.setrecursionlimit(max(rows + 10, old_max_recursion))
+    aln_file = tmp / f'{columns}.tmp'
+    fixed_aln = fix_only_gaps(alignment)
+    array_to_fasta(fixed_aln, aln_file)
+    _, iqtree = utils.get_iqtree()
+    if not _:
+        log.critical('Cannot find iqtree.')
+        return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
+    with open(devnull, 'w', encoding='utf-8') as out:
+        t_cmd = f'{iqtree} -s {aln_file} -m HKY -fast -czb -redo'
+        run_ = run(t_cmd, stdout=out, stderr=out, shell=True)
+        # just return 0 if there is error
+    if run_.returncode != 0:
+        log.debug('Found sequence with only gaps.')
+    else:
+        tree = Phylo.read(str(aln_file) + '.treefile', 'newick')
+        try:
+            # skip the first empty node
+            internals = tree.get_nonterminals()[1:]
+            non_zero_internals = [i for i in internals if i.branch_length != 0]
+            terminals = tree.get_terminals()
+            # may be zero
+            n_terminals = max(1, len(terminals))
+            pd = tree.total_branch_length() / n_terminals
+            pd_stem = sum([i.branch_length for i in internals]) / n_terminals
+            pd_stem_sd = np.std(
+                [i.branch_length for i in internals]) / n_terminals
+            pd_terminal = sum(
+                [i.branch_length for i in terminals]) / n_terminals
+            pd_terminal_sd = np.std(
+                [i.branch_length for i in terminals]) / n_terminals
+            tree_res = len(non_zero_internals) / n_terminals
+        except Exception:
+            log.debug('Bad phylogenetic tree.')
+    utils.clean_tmp(aln_file)
+    sys.setrecursionlimit(old_max_recursion)
+    return pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd, tree_res
+
+
+class Variance(namedtuple('Variance',
+                          ['Samples', 'Length', 'Gap_Ratio',
+                           'Observed_Res', 'Entropy', 'Pi',
+                           'PD', 'PD_stem', 'PD_stem_SD',
+                           'PD_terminal', 'PD_terminal_SD',
+                           'Tree_Res', 'Total_GC'],
+                          defaults=[0 for i in range(13)])):
+    """
+    For get_resolution()
+    samples: rows
+    length: columns
+    """
+    __slots__ = ()
+
+    def __str__(self):
+        return ('{Samples},{Length},{Gap_Ratio:.4%},'
+                '{Observed_Res:.4%},{Entropy:.8f},{Pi:.8f},'
+                '{PD:.8f},{PD_stem:.8f},{PD_stem_SD:.8f},'
+                '{PD_terminal:.8f},{PD_terminal_SD:.8f},'
+                '{Tree_Res:.4%},{Total_GC:.4%}'.format(**self._asdict()))
+
+
+def get_resolution(alignment: np.array, tmp: Path,
+                   ignore_ambiguous=True) -> tuple:
+    """
+    Given alignment (2d numpy array), location of fragment(start and end, int,
+    start from zero, exclude end),
+    return gap ratio, resolution, entropy, Pi, tree value and average terminal
+    branch length.
+    """
+    gc_array = np.array([0])
+    rows, columns = alignment.shape
+    total = rows * columns
+    # index error
+    if columns == 0:
+        return Variance(), gc_array
+    gap_ratio = len(alignment[alignment == b'-']) / total
+    item, count = np.unique(alignment, return_counts=True, axis=0)
+    observed_res = len(count) / rows
+    # normalized entropy
+    entropy = normalized_entropy(count, rows)
+    pi = nucleotide_diversity(alignment)
+    (pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd,
+     tree_res) = phylogenetic_diversity(alignment, tmp)
+    total_gc, gc_array = gc_ratio(alignment, ignore_ambiguous)
+    variance = Variance(rows, columns, gap_ratio, observed_res, entropy, pi,
+                        pd, pd_stem, pd_stem_sd, pd_terminal, pd_terminal_sd,
+                        tree_res, total_gc)
+    return variance, gc_array
+
+
+def output_sliding(sliding: list, name: str, out: Path,
+                   size: int, step: int) -> (Path, Path):
+    if len(sliding) == 0:
+        log.warning('Empty sliding-window result.')
+        return Path(), Path()
+    out_csv = out / (name + '.csv')
+    head = 'Start,End,' + ','.join(Variance._fields) + '\n'
+    handle = open(out_csv, 'w', encoding='utf-8')
+    handle.write(head)
+    index = []
+    # for human reading
+    start = 1
+    for variance in sliding:
+        line = f'{start},{start + size},{variance}\n'
+        index.append(start)
+        handle.write(line)
+        start += step
+    handle.close()
+    # draw
+    out_pdf = out / (name + '.pdf')
+    plt.style.use('seaborn-v0_8-colorblind')
+    # how to find optimized size?
+    fig = plt.figure(figsize=(15 + len(sliding) // 5000, 10))
+    ax1 = plt.subplot(211)
+    ax1.yaxis.set_ticks(np.linspace(0, 1, num=11))
+    ax1.set_title(f'{name} ({sliding[0].Samples} sequences)', pad=30)
+    ax1.set_xlabel('Bases')
+    ax1.set_ylabel('Values')
+    ax1.plot(index, [i.Gap_Ratio for i in sliding], label='Gap Ratio',
+             alpha=0.8)
+    ax1.plot(index, [i.Observed_Res for i in sliding],
+             label='Observed Resolution', alpha=0.8)
+    ax1.plot(index, [i.Entropy for i in sliding],
+             label='Shannon Equitability Index', alpha=0.8)
+    ax1.plot(index, [i.Tree_Res for i in sliding], label='Tree Resolution',
+             alpha=0.8)
+    ax1.plot(index, [i.Total_GC for i in sliding], label='GC Ratio',
+             alpha=0.8)
+    ax1.plot(index, [i.Pi for i in sliding], label=r'$\pi$', alpha=0.8)
+    ax1.legend(loc='upper right', framealpha=0.5)
+    # different ytick
+    ax2 = plt.subplot(212)
+    ax1.set_xlabel('Bases')
+    # ax2..yaxis.set_ticks(np.linspace(0, max_range, 21))
+    ax2.set_ylabel('Values')
+    ax2.plot(index, [i.PD for i in sliding], linestyle='--', label='PD',
+             alpha=0.8)
+    ax2.plot(index, [i.PD_stem for i in sliding], linestyle='--',
+             label='PD_stem', alpha=0.8)
+    ax2.plot(index, [i.PD_terminal for i in sliding], linestyle='--',
+             label='PD_terminal', alpha=0.8)
+    # k--
+    ax2.legend(loc='upper right', framealpha=0.5)
+    plt.savefig(out_pdf)
+    plt.close()
+    return out_csv, out_pdf
+
+
+def evaluate(aln: Path, arg) -> tuple:
+    """
+    Wrapper
+    Args:
+        aln: alignment file
+        arg: args
+    Returns:
+        summary: namedtuple
+        gc_array: for draw
+        sliding: list of Variance
+    """
+    sliding = []
+    name, alignment = fasta_to_array(aln)
+    if name is None:
+        return None, None, None
+    if arg.ignore_gap:
+        no_gap_alignment, gap_alignment = remove_gap(alignment)
+    else:
+        no_gap_alignment = alignment
+        gap_alignment = np.array([[]])
+    rows, columns = alignment.shape
+    log.info(f'Evaluate {aln}')
+    summary, gc_array = get_resolution(no_gap_alignment, arg._tmp,
+                                       arg.ignore_ambiguous_base)
+    if arg.quick:
+        pass
+    else:
+        # sliding window
+        for i in range(0, columns - arg.size, arg.step):
+            # view, not copy
+            subalign = alignment[:, i:i + arg.size]
+            if arg.ignore_gap:
+                subalign, gap_subalign = remove_gap(alignment, silence=True)
+            variance, sub_gc_array = get_resolution(subalign, arg._tmp,
+                                                    arg.ignore_ambiguous_base)
+            sliding.append(variance)
+    return summary, gc_array, sliding
+
+
+def evaluate_main(arg_str=None):
+    """
+    Evaluate variance of alignments.
+    """
+    log.info('Running evaluate module...')
+    if arg_str is None:
+        arg, other_args2 = parse_args()
+    else:
+        arg, other_args2 = parse_args(arg_str.split(' '))
+    arg = init_arg(arg)
+    if arg is None:
+        log.info('Quit evaluate module.')
+        return None, other_args2
+    utils.add_file_log(arg)
+    aligned, unaligned = align(arg.fasta, arg._align)
+    aligned.extend(arg.aln)
+    evaluation_result = arg.out / 'Evaluation.csv'
+    csv_head = 'Loci,' + ','.join(Variance._fields) + '\n'
+    with open(evaluation_result, 'w', encoding='utf-8') as out_csv:
+        out_csv.write(csv_head)
+    for aln in aligned:
+        summary, gc_array, sliding = evaluate(aln, arg)
+        if summary is None:
+            continue
+        log.info(f'\t{aln.stem}')
+        log.info(f'\tSamples:                   {summary.Samples}')
+        log.info(f'\tLength                     {summary.Length} bp')
+        log.info(f'\tGap ratio:                 {summary.Gap_Ratio:.8f}')
+        log.info(f'\tObserved resolution:       {summary.Observed_Res:.8f}')
+        log.info(f'\tNormalized Shannon Index:  {summary.Entropy:.8f}')
+        log.info(f'\tPi:                        {summary.Pi:.8f}')
+        log.info(f'\tPhylogenetic diversity:    {summary.PD:.8f}')
+        log.info(f'\tTree resolution:           {summary.Tree_Res:.8f}')
+        with open(evaluation_result, 'a', encoding='utf-8') as out:
+            out.write(aln.stem + ',' + str(summary) + '\n')
+        if not arg.quick:
+            output_sliding(sliding, aln.stem, arg._evaluate, arg.size, arg.step)
+    log.info(f'Evaluation results could be found in {evaluation_result}')
+    log.info('Evaluate module finished.')
+    # for i in aligned:
+    #     utils.move(i, arg._align/(i.name), copy=True)
+    return arg, other_args2
+
+
+if __name__ == '__main__':
     evaluate_main()
```

### Comparing `ogu-1.52/src/OGU/gb2fasta.py` & `ogu-1.54/src/OGU/gb2fasta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,837 +1,834 @@
-#!/usr/bin/python3
-
-import argparse
-import json
-from collections import defaultdict
-from io import StringIO
-from pathlib import Path
-from pkg_resources import resource_filename
-from time import sleep
-
-from Bio import Entrez, SeqIO
-from Bio.SeqFeature import SeqFeature, FeatureLocation, CompoundLocation
-
-from OGU import utils
-from OGU.global_vars import log, name
-
-
-# load data
-with open(resource_filename(name, 'data/superkingdoms.csv'), 'r') as _:
-    SUPERKINGDOMS = set(_.read().split(','))
-with open(resource_filename(name, 'data/kingdoms.csv'),
-          'r') as _:
-    KINGDOMS = set(_.read().split(','))
-with open(resource_filename(name, 'data/phyla.csv'),
-          'r') as _:
-    PHYLA = set(_.read().split(','))
-with open(resource_filename(name, 'data/classes.csv'),
-          'r') as _:
-    CLASSES = set(_.read().split(','))
-with open(resource_filename(name, 'data/animal_orders.csv'),
-          'r') as _:
-    ANIMAL_ORDERS = set(_.read().split(','))
-
-
-def parse_args(arg_list=None):
-    arg = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    arg.add_argument('-gb', nargs='*', help='input filename')
-    arg.add_argument('-out', help='output directory')
-    arg.add_argument('-no_divide', action='store_true', help='only download')
-    # for plastid genes
-    arg.add_argument('-rename', action='store_true', help='try to rename gene')
-    arg.add_argument('-unique', choices=('longest', 'first', 'no'),
-                     default='first',
-                     help='method to remove redundant sequences')
-    adv = arg.add_argument_group('Advance')
-    # trnK-matK
-    adv.add_argument('-allow_mosaic_spacer', action='store_true',
-                     help='allow mosaic spacer')
-    # genes in IR regions
-    adv.add_argument('-allow_repeat', action='store_true',
-                     help='allow repeat genes or spacer')
-    adv.add_argument('-allow_invert_repeat', action='store_true',
-                     help='allow invert-repeat spacers')
-    # for primer
-    adv.add_argument('-expand', type=int, default=0,
-                     help='expand length of upstream/downstream')
-    adv.add_argument('-max_name_len', default=100, type=int,
-                     help='maximum length of feature name')
-    # handle rps12
-    adv.add_argument('-max_gene_len', default=20000, type=int,
-                     help='maximum length of gene sequence')
-    adv.add_argument('-email', type=str,
-                     help='email address for querying Genbank')
-    adv.add_argument('-out_debug', action='store_true',
-                     help='output debug gb')
-    query = arg.add_argument_group('Query')
-    query.add_argument('-exclude', type=str, help='exclude option')
-    query.add_argument('-gene', type=str, help='gene name')
-    # in case of same taxonomy name in different group
-    query.add_argument('-group',
-                       choices=('all', 'animals', 'plants', 'fungi', 'protists',
-                                'bacteria', 'archaea', 'viruses'),
-                       default='all',
-                       help='Kind of species')
-    query.add_argument('-min_len', default=1, type=int,
-                       help='minimum length')
-    query.add_argument('-max_len', default=300000, type=int,
-                       help='maximum length')
-    query.add_argument('-date_start', type=str,
-                       help='release date beginning, (eg. 1970/1/1)')
-    query.add_argument('-date_end', type=str,
-                       help='release date end, (eg. 2020/12/31)')
-    query.add_argument('-molecular', choices=('all', 'DNA', 'RNA'),
-                       default='all', help='molecular type')
-    query.add_argument('-genome', action='store_true',
-                       help='get complete organelle genome')
-    query.add_argument('-og', '-organelle', dest='organelle',
-                       choices=('ignore', 'both', 'no', 'mt',
-                                'mitochondrion', 'cp', 'chloroplast',
-                                'pl', 'plastid'),
-                       default='ignore', help='organelle type')
-    query.add_argument('-query', nargs='*', help='query text')
-    query.add_argument('-refseq', choices=('both', 'yes', 'no'),
-                       default='both', help='include RefSeq or not')
-    query.add_argument('-count', default=0, type=int,
-                       help='maximum number of records to download, '
-                            '0 for unlimited')
-    query.add_argument('-taxon', help='Taxonomy name')
-    if arg_list is None:
-        return arg.parse_known_args()
-    else:
-        return arg.parse_known_args(arg_list)
-
-
-def get_query_string(arg, silence=False):
-    """
-    Based on given options, generate query string from Genbank.
-    """
-    if arg.gb is not None:
-        return
-    if not silence:
-        if arg.allow_repeat:
-            log.info("Repeat genes or spacers will be kept as user's wish.")
-        if arg.allow_invert_repeat:
-            log.info("Invert-repeat spacers will be kept.")
-        if arg.allow_mosaic_spacer:
-            log.info('The "spacers" of overlapped genes will be kept.')
-        if arg.expand != 0:
-            log.info(f'Extend sequences to their upstream/'
-                     f'downstream with {arg.expand} bp')
-        if arg.group is not None and arg.group != 'all':
-            log.warning('The filters "group" was reported to return abnormal '
-                        'records by Genbank. Please consider to use "-taxon" '
-                        'instead.')
-        if arg.rename:
-            log.warning('{} will try to rename genes by regular '
-                        'expression.'.format(name))
-        if arg.genome:
-            log.warning('Conflict options: "-max_len" and "-genome", '
-                        'ignore length limit.')
-    else:
-        pass
-    condition = []
-    # if group is "all", ignore
-    if arg.group != 'all':
-        condition.append(f'{arg.group}[filter]')
-    if arg.gene is not None:
-        if ' ' in arg.gene:
-            condition.append(f'"{arg.gene}"[gene]')
-        else:
-            condition.append(f'{arg.gene}[gene]')
-    if arg.molecular != 'all':
-        d = {'DNA': 'biomol_genomic[PROP]',
-             'RNA': 'biomol_mrna[PROP]'}
-        condition.append(d[arg.molecular])
-    if arg.taxon is not None:
-        if ' ' in arg.taxon:
-            condition.append(f'"{arg.taxon}"[organism]')
-        else:
-            condition.append(f'{arg.taxon}[organism]')
-    if arg.organelle == 'ignore':
-        pass
-    elif arg.organelle == 'both':
-        condition.append('(mitochondrion[filter] OR plastid[filter] '
-                         'OR chloroplast[filter])')
-    elif arg.organelle == 'no':
-        condition.append('NOT mitochondrion[filter] NOT plastid[filter] '
-                         'NOT chloroplast[filter])')
-    elif arg.organelle in ('mt', 'mitochondrion'):
-        condition.append('mitochondrion[filter]')
-    else:
-        condition.append('(plastid[filter] OR chloroplast[filter])')
-    if arg.refseq == 'both':
-        pass
-    elif arg.refseq == 'yes':
-        condition.append('refseq[filter]')
-    else:
-        condition.append('NOT refseq[filter]')
-    # join nargs
-    if arg.query is not None:
-        log.warning('Query string is not empty, make sure the syntax is ok.')
-        condition.append(' '.join(arg.query))
-    if len(condition) > 0:
-        if arg.genome:
-            condition.append(f'("20000"[SLEN] : "{arg.max_len}"[SLEN])')
-        else:
-            condition.append(f'("{arg.min_len}"[SLEN] : "{arg.max_len}"[SLEN])')
-    if arg.exclude is not None:
-        condition.append('NOT ({})'.format(arg.exclude))
-    if arg.date_start is not None and arg.date_end is not None:
-        condition.append(f'"{arg.date_start}"[PDAT] : "{arg.date_end}"[PDAT]')
-    if not condition:
-        return None
-    else:
-        string = ' AND '.join(condition)
-        string = string.replace('AND NOT', 'NOT')
-        return string
-
-
-def init_arg(arg):
-    arg.query = get_query_string(arg)
-    arg = utils.init_out(arg)
-    if arg.gb is None and arg.query is None:
-        log.warning('Empty input.')
-        return None
-    if arg.refseq and arg.gene is None:
-        log.info('Reset the limitation of sequence length for RefSeq.')
-        arg.min_len = None
-        arg.max_len = None
-    if arg.gb is not None:
-        # don't move given gb files?
-        arg.gb = [Path(i).absolute() for i in arg.gb]
-        for i in arg.gb:
-            if not i.exists() or not i.is_file():
-                log.error(f'{i} does not exist or is not a valid file.')
-                return None
-    else:
-        arg.gb = list()
-    if arg.no_divide:
-        log.warning('Only download data because of "-no_divide"')
-    return arg
-
-
-def download(arg):
-    """
-    Download records from Genbank.
-    Because of connection to Genbank website is not stable (especially in
-    Asia), it will retry if failed. Ctrl+C to break.
-    """
-    too_much = 50000
-    # although Bio.Entrez has max_tries, current code could handle error
-    # clearly
-    retry_max = 10
-    if arg.email is None:
-        Entrez.email = 'guest@example.com'
-        log.info(f'\tEmail address for using Entrez missing, '
-                 f'use {Entrez.email} instead.')
-    else:
-        Entrez.email = arg.email
-    query_handle = Entrez.read(Entrez.esearch(db='nuccore', term=arg.query,
-                                              usehistory='y'))
-    count = int(query_handle['Count'])
-
-    if count == 0:
-        log.warning('Got 0 record. Please check the query.')
-        log.info('Abort download.')
-        return None
-    elif count > too_much and arg.count > too_much:
-        log.warning(f'Got {count} records. May cost long time to download.')
-    else:
-        log.info(f'\tGot {count} records.')
-    if arg.count != 0:
-        if count > arg.count:
-            count = arg.count
-            log.info(f'\tDownload {arg.count} records due to "-count".')
-    log.info('\tDownloading...')
-    log.warning('\tMay be slow if connection is unstable. Ctrl+C to quit.')
-    name_words = []
-    for i in (arg.taxon, arg.organelle, arg.gene):
-        if i is not None and i not in ('both', 'ignore', 'no'):
-            name_words.append(i)
-    if len(name_words) != 0:
-        name = utils.safe_path('-'.join(name_words)) + '.gb'
-    else:
-        name = 'sequence.gb'
-    file_name = arg._gb / name
-    output = open(file_name, 'w', encoding='utf-8')
-    ret_start = 0
-    # get ret_max
-    bit = len(str(count)) - 2
-    ret_max = min(1, max(10, 10 ** bit))
-    retry = 0
-    while ret_start < count:
-        log.info('\t{:d}--{:d}'.format(ret_start, ret_start + ret_max))
-        # Entrez accept at most 3 times per second
-        # However, due to slow network, it's fine :)
-        try:
-            data = Entrez.efetch(db='nuccore',
-                                 webenv=query_handle['WebEnv'],
-                                 query_key=query_handle['QueryKey'],
-                                 rettype='gb',
-                                 retmode='text',
-                                 retstart=ret_start,
-                                 retmax=ret_max)
-            output.write(data.read())
-        # just retry if connection failed
-        # IOError could not handle all types of failure
-        except Exception:
-            sleep(1)
-            if retry <= retry_max:
-                log.warning('Failed on download. Retrying...')
-                retry += 1
-                continue
-            else:
-                log.critical(f'Too much failure ({retry_max} times).')
-                log.info('Abort download.')
-                return None
-        ret_start += ret_max
-    log.info('Download finished.')
-    json_file = arg._tmp / 'Query.json'
-    with open(json_file, 'w', encoding='utf-8') as _:
-        json.dump(query_handle, _, indent=4, sort_keys=True)
-    log.info(f'The query info was dumped into {json_file}')
-    return file_name
-
-
-def clean_gb(gbfile):
-    """
-    Records in Genbank may be problematic. Check it before parse and skip
-    abnormal records.
-    """
-    log.info('\tCheck Genbank file to remove abnormal records.')
-
-    def parse_gb(handle):
-        record = []
-        for line in handle:
-            record.append(line)
-            if line.startswith('//'):
-                yield record
-                record = []
-            else:
-                pass
-
-    wrong = 0
-    old_gb = open(gbfile, 'r')
-    tmp_gb = StringIO()
-    for record in parse_gb(old_gb):
-        # StringIO is faster than write tmp file to disk and read
-        tmp_gb = StringIO()
-        for _ in record:
-            tmp_gb.write(_)
-        tmp_gb.seek(0)
-        try:
-            gb_record = SeqIO.read(tmp_gb, 'gb')
-            yield gb_record
-        except Exception as e:
-            log.critical('\tFound problematic record {}: {}'.format(
-                record[0][:25], e.args[0]))
-            wrong += 1
-    tmp_gb.close()
-    old_gb.close()
-    if wrong != 0:
-        log.info('\tRemove {} abnormal records.'.format(wrong))
-
-
-def get_feature_name(feature, arg):
-    """
-    Get feature name and collect genes for extract spacer.
-    Only handle gene, CDS, tRNA, rRNA, misc_feature, misc_RNA.
-    """
-    def _extract_name(feature):
-        if 'gene' in feature.qualifiers:
-            name = feature.qualifiers['gene'][0]
-        elif 'product' in feature.qualifiers:
-            name = feature.qualifiers['product'][0]
-        elif 'locus_tag' in feature.qualifiers:
-            name = feature.qualifiers['locus_tag'][0]
-        elif 'note' in feature.qualifiers:
-            name = feature.qualifiers['note'][0]
-        else:
-            log.debug('Cannot recognize annotation:\n{}'.format(feature))
-            name = None
-        return name
-
-    name = None
-    # ignore exist exon/intron
-    accept_type = {'gene', 'CDS', 'tRNA', 'rRNA', 'misc_feature', 'misc_RNA'}
-    if feature.type not in accept_type:
-        return name
-    name = _extract_name(feature)
-    if name is None:
-        return name
-        # log.warning('Unsupport annotation type {}'.format(feature.type))
-    if feature.type == 'misc_feature':
-        if 'internal transcribed spacer' in name:
-            name = 'ITS'
-        if 'intergenic_spacer' in name or 'IGS' in name:
-            name = name.replace('intergenic_spacer_region', 'IGS')
-    if feature.type == 'misc_RNA':
-        # handle ITS
-        if 'internal transcribed spacer' in name:
-            name = name.replace('internal transcribed spacer', 'ITS')
-    if name is not None:
-        name = utils.safe_path(name)
-    else:
-        return name
-    if arg.rename:
-        name = utils.gene_rename(name)[0]
-    return name
-
-
-def get_spacer(genes):
-    """
-    Given list of genes, extract spacers.
-    genes: [name, feature]
-    """
-    if len(genes) <= 1:
-        return []
-    spacers = list()
-    names = set()
-    # sorted according to sequence starting position
-    genes.sort(key=lambda x: int(x[1].location.start))
-    for i in range(len(genes)-1):
-        b_name, before = genes[i]
-        c_name, current = genes[i+1]
-        invert_repeat = False
-        repeat = False
-        # gene name may contain "_", use "-" instead
-        # sorted_name = '-'.join(sorted([b_name, c_name]))
-        # to be continued
-        name = '-'.join([b_name, c_name])
-        # 1. A.start--A.end--B.start--B.end
-        if before.location.end <= current.location.start:
-            # check invert repeat
-            invert_name = '-'.join([c_name, b_name])
-            if invert_name in names:
-                invert_repeat = True
-            elif name in names:
-                repeat = True
-            else:
-                names.add(name)
-            spacer = SeqFeature(
-                type='spacer',
-                id=name,
-                location=FeatureLocation(before.location.end,
-                                         current.location.start),
-                qualifiers={'upstream': b_name,
-                            'downstream': c_name,
-                            'repeat': str(repeat),
-                            'invert_repeat': str(invert_repeat)})
-            spacers.append(spacer)
-        # 2. A.start--B.start--A.end--B.end
-        elif before.location.end <= current.location.end:
-            # overlap, no spacer
-            pass
-        # 3. A.start--B.start--B.end--A.end
-        else:
-            spacer_up = SeqFeature(
-                type='mosaic_spacer',
-                id=name,
-                location=FeatureLocation(before.location.start,
-                                         current.location.start),
-                qualifiers={'upstream': b_name,
-                            'downstream': c_name,
-                            'repeat': str(repeat),
-                            'invert_repeat': str(invert_repeat)})
-            spacer_down = SeqFeature(
-                type='mosaic_spacer',
-                id='-'.join([c_name, b_name]),
-                location=FeatureLocation(current.location.end,
-                                         before.location.end),
-                qualifiers={'upstream': b_name,
-                            'downstream': c_name,
-                            'repeat': str(repeat),
-                            'invert_repeat': str(invert_repeat)})
-            spacers.extend([spacer_up, spacer_down])
-    spacers = [i for i in spacers if len(i) != 0]
-    return spacers
-
-
-def get_intron(genes):
-    """
-    Given list of genes, extract introns.
-    genes: [name, feature]
-    Return:
-        intron(list): [name, feature]
-    """
-    # exons = []
-    introns = []
-    for gene_name, feature in genes:
-        # for n, part in enumerate(feature.location.parts):
-        #     exon = SeqFeature(
-        #     type='exon',
-        #     id='-'.join([gene_name, n+1]),
-        #     location=part,
-        #     qualifiers={'gene': gene_name,
-        #                 'count': n+1})
-        # exons.append(exon)
-        strand = feature.location.strand
-        # sort by start, no matter which strand
-        parts = sorted(feature.location.parts, key=lambda x: x.start)
-        n_part = len(parts)
-        for i in range(len(parts)-1):
-            before = parts[i]
-            current = parts[i+1]
-            # Z00028
-            if before.end >= current.start:
-                break
-            # complement strand use reversed index
-            # n_intron start with 1 instead of 0
-            if strand != -1:
-                n_intron = i + 1
-            else:
-                n_intron = n_part - i - 1
-            intron = SeqFeature(
-                type='intron',
-                id='{}.{}'.format(gene_name, n_intron),
-                location=FeatureLocation(before.end,
-                                         current.start,
-                                         before.strand),
-                qualifiers={'gene': gene_name,
-                            'count': n_intron})
-            introns.append(intron)
-    return introns
-
-
-def divide(gbfile, arg):
-    """
-    Given genbank file, return divided fasta files.
-    """
-    log.info('Divide {} by annotation.'.format(gbfile))
-
-    def get_taxon(taxon_str):
-        """
-        Get taxon info based on suffix and list from NCBI taxonomy database.
-        """
-        # kingdom|phylum|class|order|family|organims(genus|species)
-        # add my_ prefix to avoid conflict of "class"
-        my_kingdom = ''
-        my_phylum = ''
-        my_class = ''
-        my_order = ''
-        my_family = ''
-        for item in taxon_str:
-            if item in SUPERKINGDOMS:
-                my_kingdom = item
-            # mix superkingdom and kingdom to reduce name length
-            elif item in KINGDOMS:
-                my_kingdom = item
-            elif item in PHYLA:
-                my_phylum = item
-            elif item in CLASSES:
-                my_class = item
-            if item.endswith('ales') or item in ANIMAL_ORDERS:
-                my_order = item
-            elif item.endswith('aceae') or item.endswith('idae'):
-                my_family = item
-        # get fake class for plant
-        if my_phylum == 'Streptophyta' and my_class == '':
-            last_phyta = ''
-            for i in taxon_str:
-                if i.endswith('phyta'):
-                    last_phyta = i
-            try:
-                my_class = taxon_str[taxon_str.index(last_phyta) + 1]
-            except IndexError:
-                my_class = ''
-        return my_kingdom, my_phylum, my_class, my_order, my_family
-
-    raw_fasta = arg._fasta / (gbfile.stem+'.fasta')
-    handle_raw = open(raw_fasta, 'w', encoding='utf-8')
-    for record in clean_gb(gbfile):
-        # only accept gene, product, and spacer in misc_features.note
-        taxon_str = record.annotations.get('taxonomy', None)
-        if taxon_str is None:
-            kingdom, phylum, class_, order, family = '', '', '', '', ''
-        else:
-            kingdom, phylum, class_, order, family = get_taxon(taxon_str)
-        # gb annotation may be empty
-        organism = record.annotations.get('organism', None)
-        if organism is not None:
-            organism = organism.replace(' ', '_')
-            genus, *species = organism.split('_')
-        else:
-            genus, species = '', ''
-        # species name may contain other characters
-        taxon = '{}|{}|{}|{}|{}|{}|{}'.format(kingdom, phylum, class_,
-                                              order, family, genus,
-                                              '_'.join(species))
-        accession = record.annotations.get('accessions', ['', ])[0]
-        specimen = record.features[0].qualifiers.get('specimen_voucher',
-                                                     ['', ])
-        specimen = specimen[0].replace(' ', '_')
-        isolate = record.features[0].qualifiers.get('isolate', ['', ])
-        isolate = isolate[0].replace(' ', '_')
-        # usually the record only has one of them
-        specimen = '_'.join([specimen, isolate]).rstrip('_')
-        seq_info = (taxon, accession, specimen)
-        whole_seq = record.seq
-        feature_name = []
-        have_intron = {}
-        genes = []
-        not_genes = []
-        # get genes
-        for feature in record.features:
-            # skip unsupport feature
-            # support: gene, CDS, tRNA, rRNA, misc_feature, misc_RNA
-            name = get_feature_name(feature, arg)
-            if name is None:
-                continue
-            if len(name) > arg.max_name_len:
-                log.debug(f'Too long name: {name}. Truncated.')
-                name = name[:arg.max_name_len-3] + '...'
-            if feature.type == 'gene':
-                genes.append([name, feature])
-                # only use gene name as sequence id
-                feature_name.append(name)
-            else:
-                not_genes.append([name, feature])
-            if isinstance(feature.location, CompoundLocation):
-                # use dict to remove repeat name of gene/CDS/tRNA/rRNA
-                have_intron[name] = feature
-
-        # write genes
-        write_seq(genes, seq_info, whole_seq, arg)
-        # write non-genes
-        write_seq(not_genes, seq_info, whole_seq, arg)
-        # extract spacer
-        spacers = get_spacer(genes)
-        # write spacer annotations
-        if not arg.allow_mosaic_spacer:
-            spacers = [i for i in spacers if i.type != 'mosaic_spacer']
-        # extract intron
-        introns = get_intron(have_intron.items())
-        if not arg.allow_invert_repeat:
-            spacers = [i for i in spacers if i.qualifiers[
-                'invert_repeat'] == 'False']
-        if arg.out_debug:
-            record.features.extend(spacers)
-            record.features.extend(introns)
-            SeqIO.write(record, arg.out/'extend.gb', 'gb')
-        # write seq
-        spacers_to_write = [[i.id, i] for i in spacers]
-        # write intron or not?
-        introns_to_write = [(i.id, i) for i in introns]
-        write_seq(spacers_to_write, seq_info, whole_seq, arg)
-        write_seq(introns_to_write, seq_info, whole_seq, arg)
-        # write to group_by name, i.e., one gb record one fasta
-        if 'ITS' in feature_name:
-            name_str = 'ITS'
-        elif len(feature_name) >= 4:
-            name_str = '{}-...-{}'.format(feature_name[0], feature_name[-1])
-        elif len(feature_name) == 0:
-            name_str = 'Unknown'
-        else:
-            name_str = '-'.join(feature_name)
-        # directly use genome type as name
-        if arg.organelle not in ('ignore', 'no', 'both'):
-            name_str = '{}_genome'.format(arg.organelle)
-        record.id = '|'.join([name_str, taxon, accession, specimen])
-        record.description = ''
-        filename = arg._fasta / (name_str+'.fasta')
-        try:
-            with open(filename, 'a', encoding='utf-8') as out:
-                SeqIO.write(record, out, 'fasta')
-            # write raw fasta
-            SeqIO.write(record, handle_raw, 'fasta')
-        except Exception:
-            log.warning(f'Invalid sequence {accession}.')
-    # skip analyze of Unknown.fasta
-    # unknown = arg._divide / 'Unknown.fasta'
-    log.info('Divide finished.')
-    return arg._fasta, arg._divide
-
-
-def write_seq(record, seq_info, whole_seq, arg):
-    """
-    Write fasta files to "by-gene" folder only.
-    ID format: >name|taxon|accession|specimen|type
-    Args:
-        record: [name, feature]
-        seq_info: (taxon, accession, specimen)
-        whole_seq: whole sequence
-        arg: arguments
-    Return: {filename}
-    """
-    def careful_extract(name, feature, whole_seq):
-        # illegal annotation may cause extraction failed
-        try:
-            sequence = feature.extract(whole_seq)
-            sequence_str = str(sequence)
-        except Exception as e:
-            sequence_str = ''
-            log.warning('Cannot extract sequence of {} from {} '
-                        'due to "{}".'.format(name, seq_info[1], str(e)))
-        return sequence_str
-
-    seq_len = len(whole_seq)
-    filenames = set()
-    expand_files = set()
-    record_unique = []
-    if not arg.allow_repeat:
-        names = set()
-        for i in record:
-            if i[0] not in names:
-                record_unique.append(i)
-                names.add(i[0])
-    else:
-        record_unique = record
-
-    for i in record_unique:
-        name, feature = i
-        # skip abnormal annotation
-        if len(feature) > arg.max_gene_len:
-            log.debug('The fragment of {} (Accession {}) '
-                      'is too long. Skip.'.format(name, seq_info[1]))
-            continue
-        filename = arg._divide / (feature.type+'-'+name+'.fasta')
-        with open(filename, 'a', encoding='utf-8') as handle:
-            sequence_id = '>' + '|'.join([name, *seq_info, feature.type])
-            sequence = careful_extract(name, feature, whole_seq)
-            handle.write(sequence_id+'\n')
-            handle.write(sequence+'\n')
-        filenames.add(filename)
-        if arg.expand != 0:
-            if feature.location_operator == 'join':
-                loc = feature.location.parts
-                # ensure increasing order
-                # parts do not have sort method
-                loc.sort(key=lambda x: x.start)
-                new_loc = sum([
-                    # avoid IndexError
-                    FeatureLocation(max(0, loc[0].start-arg.expand),
-                                    loc[0].end, loc[0].strand),
-                    *loc[1:-1],
-                    FeatureLocation(loc[-1].start,
-                                    min(seq_len, loc[-1].end+arg.expand),
-                                    loc[-1].strand)])
-                feature.location = new_loc
-            sequence = careful_extract(name, feature, whole_seq)
-            filename2 = arg._expand / (feature.type+'-'+name+'.fasta')
-            with open(filename2, 'a', encoding='utf-8') as handle:
-                handle.write(sequence_id + '\n')
-                handle.write(str(sequence) + '\n')
-            expand_files.add(filename2)
-    # keep = ('gene.fasta', 'misc_feature', 'misc_RNA', 'spacer')
-    # for i in filenames:
-        # if i.endswith(keep):
-            # file_to_analyze.append(i)
-        # else:
-            # log.debug('Skip {}'.format(i))
-    return filenames
-
-
-def count_for_unique(fasta: Path):
-    info = defaultdict(lambda: list())
-    index = 0
-    count = 0
-    for record in SeqIO.parse(fasta, 'fasta'):
-        # gene|kingdom|phylum|class|order|family|genus|species|specimen|type
-        count += 1
-        if '|' in record.id:
-            name = ' '.join(record.id.split('|')[6:8])
-        else:
-            name = record.id
-        length = len(record)
-        # skip empty file
-        if length != 0:
-            info[name].append([index, length])
-        index += 1
-    return info, count
-
-
-def unique(files: list, arg) -> list:
-    """
-    Remove redundant sequences of same species.
-    Files were saved in arg._unique
-    """
-    log.info('Removing redundant records...')
-    unique_files = []
-    # if arg.unique == 'no':
-    #     return unique_files
-    total = 0
-    kept = 0
-    for fasta in files:
-        keep = dict()
-        info, count = count_for_unique(fasta)
-        total += count
-        if arg.unique == 'first':
-            # keep only the first record
-            keep = {info[i][0][0] for i in info}
-        elif arg.unique == 'longest':
-            for i in info:
-                info[i] = sorted(info[i], key=lambda x: x[1], reverse=True)
-            keep = {info[i][0][0] for i in info}
-        else:
-            # ignore "no"
-            pass
-        kept += len(keep)
-        new = arg._unique / fasta.name
-        with open(new, 'w', encoding='utf-8') as out:
-            for idx, record in enumerate(SeqIO.parse(fasta, 'fasta')):
-                if idx in keep:
-                    SeqIO.write(record, out, 'fasta')
-        unique_files.append(new)
-    log.info(f'{kept} of {total} unique records.')
-    return unique_files
-
-
-def gb2fasta_main(arg_str=None):
-    """
-    Collect genbank files and convert them to fasta files.
-    Args:
-        arg_str(str or None): string for parse_arg
-    """
-    log.info('Running gb2fasta module...')
-    if arg_str is None:
-        arg, other_args = parse_args()
-    else:
-        arg, other_args = parse_args(arg_str.split(' '))
-    arg = init_arg(arg)
-    if arg is None:
-        log.info('Quit gb2fasta module.')
-        return None, other_args
-    utils.add_file_log(arg)
-    log.info(f'Input genbank files:\t{arg.gb}')
-    if arg.query is not None:
-        log.info(f'Query: {arg.query}')
-        gb_file = download(arg)
-        if gb_file is not None:
-            arg.gb.append(gb_file)
-    if arg.no_divide:
-        log.info('Download finished. Skip dividing.')
-        log.info('GB2fasta module finished.')
-        return arg, other_args
-    for i in arg.gb:
-        divide(i, arg)
-    if arg.unique == 'no':
-        log.info('Skip removing redundant sequences.')
-        unique_files = arg._divide.glob('*.fasta')
-        unique_files = [i for i in unique_files if i.name != 'Unknown.fasta']
-    else:
-        if arg.no_divide:
-            fasta_files = arg._fasta.glob('*.fasta')
-            fasta_files = [i for i in fasta_files
-                           if i.name != 'Unknown.fasta']
-            unique_files = unique(fasta_files, arg)
-        else:
-            if arg.expand == 0:
-                divided_files = arg._divide.glob('*.fasta')
-                divided_files = [i for i in divided_files
-                                 if i.name != 'Unknown.fasta']
-                unique_files = unique(divided_files, arg)
-            else:
-                expanded_files = arg._expand.glob('*.fasta')
-                expanded_files = [i for i in expanded_files
-                                  if i.name != 'Unknown.fasta']
-                unique_files = unique(expanded_files, arg)
-    # for i in unique_files:
-    #     utils.move(i, arg._unique/(i.name), copy=True)
-    log.info('GB2fasta module finished.')
-    return arg, other_args
-
-
-if __name__ == '__main__':
-    gb2fasta_main()
+#!/usr/bin/python3
+
+import argparse
+import json
+from collections import defaultdict
+from importlib import resources
+from io import StringIO
+from pathlib import Path
+from time import sleep
+
+from Bio import Entrez, SeqIO
+from Bio.SeqFeature import SeqFeature, FeatureLocation, CompoundLocation
+
+from OGU import utils
+from OGU.global_vars import log, name
+
+
+# load data
+data_dir = resources.files(name) / 'data'
+with open(data_dir/'superkingdoms.csv', 'r') as _:
+    SUPERKINGDOMS = set(_.read().split(','))
+with open(data_dir/'kingdoms.csv', 'r') as _:
+    KINGDOMS = set(_.read().split(','))
+with open(data_dir/'phyla.csv', 'r') as _:
+    PHYLA = set(_.read().split(','))
+with open(data_dir/'classes.csv', 'r') as _:
+    CLASSES = set(_.read().split(','))
+with open(data_dir/'animal_orders.csv', 'r') as _:
+    ANIMAL_ORDERS = set(_.read().split(','))
+
+
+def parse_args(arg_list=None):
+    arg = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    arg.add_argument('-gb', nargs='*', help='input filename')
+    arg.add_argument('-out', help='output directory')
+    arg.add_argument('-no_divide', action='store_true', help='only download')
+    # for plastid genes
+    arg.add_argument('-rename', action='store_true', help='try to rename gene')
+    arg.add_argument('-unique', choices=('longest', 'first', 'no'),
+                     default='first',
+                     help='method to remove redundant sequences')
+    adv = arg.add_argument_group('Advance')
+    # trnK-matK
+    adv.add_argument('-allow_mosaic_spacer', action='store_true',
+                     help='allow mosaic spacer')
+    # genes in IR regions
+    adv.add_argument('-allow_repeat', action='store_true',
+                     help='allow repeat genes or spacer')
+    adv.add_argument('-allow_invert_repeat', action='store_true',
+                     help='allow invert-repeat spacers')
+    # for primer
+    adv.add_argument('-expand', type=int, default=0,
+                     help='expand length of upstream/downstream')
+    adv.add_argument('-max_name_len', default=100, type=int,
+                     help='maximum length of feature name')
+    # handle rps12
+    adv.add_argument('-max_gene_len', default=20000, type=int,
+                     help='maximum length of gene sequence')
+    adv.add_argument('-email', type=str,
+                     help='email address for querying Genbank')
+    adv.add_argument('-out_debug', action='store_true',
+                     help='output debug gb')
+    query = arg.add_argument_group('Query')
+    query.add_argument('-exclude', type=str, help='exclude option')
+    query.add_argument('-gene', type=str, help='gene name')
+    # in case of same taxonomy name in different group
+    query.add_argument('-group',
+                       choices=('all', 'animals', 'plants', 'fungi', 'protists',
+                                'bacteria', 'archaea', 'viruses'),
+                       default='all',
+                       help='Kind of species')
+    query.add_argument('-min_len', default=1, type=int,
+                       help='minimum length')
+    query.add_argument('-max_len', default=300000, type=int,
+                       help='maximum length')
+    query.add_argument('-date_start', type=str,
+                       help='release date beginning, (eg. 1970/1/1)')
+    query.add_argument('-date_end', type=str,
+                       help='release date end, (eg. 2020/12/31)')
+    query.add_argument('-molecular', choices=('all', 'DNA', 'RNA'),
+                       default='all', help='molecular type')
+    query.add_argument('-genome', action='store_true',
+                       help='get complete organelle genome')
+    query.add_argument('-og', '-organelle', dest='organelle',
+                       choices=('ignore', 'both', 'no', 'mt',
+                                'mitochondrion', 'cp', 'chloroplast',
+                                'pl', 'plastid'),
+                       default='ignore', help='organelle type')
+    query.add_argument('-query', nargs='*', help='query text')
+    query.add_argument('-refseq', choices=('both', 'yes', 'no'),
+                       default='both', help='include RefSeq or not')
+    query.add_argument('-count', default=0, type=int,
+                       help='maximum number of records to download, '
+                            '0 for unlimited')
+    query.add_argument('-taxon', help='Taxonomy name')
+    if arg_list is None:
+        return arg.parse_known_args()
+    else:
+        return arg.parse_known_args(arg_list)
+
+
+def get_query_string(arg, silence=False):
+    """
+    Based on given options, generate query string from Genbank.
+    """
+    if arg.gb is not None:
+        return
+    if not silence:
+        if arg.allow_repeat:
+            log.info("Repeat genes or spacers will be kept as user's wish.")
+        if arg.allow_invert_repeat:
+            log.info("Invert-repeat spacers will be kept.")
+        if arg.allow_mosaic_spacer:
+            log.info('The "spacers" of overlapped genes will be kept.')
+        if arg.expand != 0:
+            log.info(f'Extend sequences to their upstream/'
+                     f'downstream with {arg.expand} bp')
+        if arg.group is not None and arg.group != 'all':
+            log.warning('The filters "group" was reported to return abnormal '
+                        'records by Genbank. Please consider to use "-taxon" '
+                        'instead.')
+        if arg.rename:
+            log.warning('{} will try to rename genes by regular '
+                        'expression.'.format(name))
+        if arg.genome:
+            log.warning('Conflict options: "-max_len" and "-genome", '
+                        'ignore length limit.')
+    else:
+        pass
+    condition = []
+    # if group is "all", ignore
+    if arg.group != 'all':
+        condition.append(f'{arg.group}[filter]')
+    if arg.gene is not None:
+        if ' ' in arg.gene:
+            condition.append(f'"{arg.gene}"[gene]')
+        else:
+            condition.append(f'{arg.gene}[gene]')
+    if arg.molecular != 'all':
+        d = {'DNA': 'biomol_genomic[PROP]',
+             'RNA': 'biomol_mrna[PROP]'}
+        condition.append(d[arg.molecular])
+    if arg.taxon is not None:
+        if ' ' in arg.taxon:
+            condition.append(f'"{arg.taxon}"[organism]')
+        else:
+            condition.append(f'{arg.taxon}[organism]')
+    if arg.organelle == 'ignore':
+        pass
+    elif arg.organelle == 'both':
+        condition.append('(mitochondrion[filter] OR plastid[filter] '
+                         'OR chloroplast[filter])')
+    elif arg.organelle == 'no':
+        condition.append('NOT mitochondrion[filter] NOT plastid[filter] '
+                         'NOT chloroplast[filter])')
+    elif arg.organelle in ('mt', 'mitochondrion'):
+        condition.append('mitochondrion[filter]')
+    else:
+        condition.append('(plastid[filter] OR chloroplast[filter])')
+    if arg.refseq == 'both':
+        pass
+    elif arg.refseq == 'yes':
+        condition.append('refseq[filter]')
+    else:
+        condition.append('NOT refseq[filter]')
+    # join nargs
+    if arg.query is not None:
+        log.warning('Query string is not empty, make sure the syntax is ok.')
+        condition.append(' '.join(arg.query))
+    if len(condition) > 0:
+        if arg.genome:
+            condition.append(f'("20000"[SLEN] : "{arg.max_len}"[SLEN])')
+        else:
+            condition.append(f'("{arg.min_len}"[SLEN] : "{arg.max_len}"[SLEN])')
+    if arg.exclude is not None:
+        condition.append('NOT ({})'.format(arg.exclude))
+    if arg.date_start is not None and arg.date_end is not None:
+        condition.append(f'"{arg.date_start}"[PDAT] : "{arg.date_end}"[PDAT]')
+    if not condition:
+        return None
+    else:
+        string = ' AND '.join(condition)
+        string = string.replace('AND NOT', 'NOT')
+        return string
+
+
+def init_arg(arg):
+    arg.query = get_query_string(arg)
+    arg = utils.init_out(arg)
+    if arg.gb is None and arg.query is None:
+        log.warning('Empty input.')
+        return None
+    if arg.refseq and arg.gene is None:
+        log.info('Reset the limitation of sequence length for RefSeq.')
+        arg.min_len = None
+        arg.max_len = None
+    if arg.gb is not None:
+        # don't move given gb files?
+        arg.gb = [Path(i).absolute() for i in arg.gb]
+        for i in arg.gb:
+            if not i.exists() or not i.is_file():
+                log.error(f'{i} does not exist or is not a valid file.')
+                return None
+    else:
+        arg.gb = list()
+    if arg.no_divide:
+        log.warning('Only download data because of "-no_divide"')
+    return arg
+
+
+def download(arg):
+    """
+    Download records from Genbank.
+    Because of connection to Genbank website is not stable (especially in
+    Asia), it will retry if failed. Ctrl+C to break.
+    """
+    too_much = 50000
+    # although Bio.Entrez has max_tries, current code could handle error
+    # clearly
+    retry_max = 10
+    if arg.email is None:
+        Entrez.email = 'guest@example.com'
+        log.info(f'\tEmail address for using Entrez missing, '
+                 f'use {Entrez.email} instead.')
+    else:
+        Entrez.email = arg.email
+    query_handle = Entrez.read(Entrez.esearch(db='nuccore', term=arg.query,
+                                              usehistory='y'))
+    count = int(query_handle['Count'])
+
+    if count == 0:
+        log.warning('Got 0 record. Please check the query.')
+        log.info('Abort download.')
+        return None
+    elif count > too_much and arg.count > too_much:
+        log.warning(f'Got {count} records. May cost long time to download.')
+    else:
+        log.info(f'\tGot {count} records.')
+    if arg.count != 0:
+        if count > arg.count:
+            count = arg.count
+            log.info(f'\tDownload {arg.count} records due to "-count".')
+    log.info('\tDownloading...')
+    log.warning('\tMay be slow if connection is unstable. Ctrl+C to quit.')
+    name_words = []
+    for i in (arg.taxon, arg.organelle, arg.gene):
+        if i is not None and i not in ('both', 'ignore', 'no'):
+            name_words.append(i)
+    if len(name_words) != 0:
+        name = utils.safe_path('-'.join(name_words)) + '.gb'
+    else:
+        name = 'sequence.gb'
+    file_name = arg._gb / name
+    output = open(file_name, 'w', encoding='utf-8')
+    ret_start = 0
+    # get ret_max
+    bit = len(str(count)) - 2
+    ret_max = min(1, max(10, 10 ** bit))
+    retry = 0
+    while ret_start < count:
+        log.info('\t{:d}--{:d}'.format(ret_start, ret_start + ret_max))
+        # Entrez accept at most 3 times per second
+        # However, due to slow network, it's fine :)
+        try:
+            data = Entrez.efetch(db='nuccore',
+                                 webenv=query_handle['WebEnv'],
+                                 query_key=query_handle['QueryKey'],
+                                 rettype='gb',
+                                 retmode='text',
+                                 retstart=ret_start,
+                                 retmax=ret_max)
+            output.write(data.read())
+        # just retry if connection failed
+        # IOError could not handle all types of failure
+        except Exception:
+            sleep(1)
+            if retry <= retry_max:
+                log.warning('Failed on download. Retrying...')
+                retry += 1
+                continue
+            else:
+                log.critical(f'Too much failure ({retry_max} times).')
+                log.info('Abort download.')
+                return None
+        ret_start += ret_max
+    log.info('Download finished.')
+    json_file = arg._tmp / 'Query.json'
+    with open(json_file, 'w', encoding='utf-8') as _:
+        json.dump(query_handle, _, indent=4, sort_keys=True)
+    log.info(f'The query info was dumped into {json_file}')
+    return file_name
+
+
+def clean_gb(gbfile):
+    """
+    Records in Genbank may be problematic. Check it before parse and skip
+    abnormal records.
+    """
+    log.info('\tCheck Genbank file to remove abnormal records.')
+
+    def parse_gb(handle):
+        record = []
+        for line in handle:
+            record.append(line)
+            if line.startswith('//'):
+                yield record
+                record = []
+            else:
+                pass
+
+    wrong = 0
+    old_gb = open(gbfile, 'r')
+    tmp_gb = StringIO()
+    for record in parse_gb(old_gb):
+        # StringIO is faster than write tmp file to disk and read
+        tmp_gb = StringIO()
+        for _ in record:
+            tmp_gb.write(_)
+        tmp_gb.seek(0)
+        try:
+            gb_record = SeqIO.read(tmp_gb, 'gb')
+            yield gb_record
+        except Exception as e:
+            log.critical('\tFound problematic record {}: {}'.format(
+                record[0][:25], e.args[0]))
+            wrong += 1
+    tmp_gb.close()
+    old_gb.close()
+    if wrong != 0:
+        log.info('\tRemove {} abnormal records.'.format(wrong))
+
+
+def get_feature_name(feature, arg):
+    """
+    Get feature name and collect genes for extract spacer.
+    Only handle gene, CDS, tRNA, rRNA, misc_feature, misc_RNA.
+    """
+    def _extract_name(feature):
+        if 'gene' in feature.qualifiers:
+            name = feature.qualifiers['gene'][0]
+        elif 'product' in feature.qualifiers:
+            name = feature.qualifiers['product'][0]
+        elif 'locus_tag' in feature.qualifiers:
+            name = feature.qualifiers['locus_tag'][0]
+        elif 'note' in feature.qualifiers:
+            name = feature.qualifiers['note'][0]
+        else:
+            log.debug('Cannot recognize annotation:\n{}'.format(feature))
+            name = None
+        return name
+
+    name = None
+    # ignore exist exon/intron
+    accept_type = {'gene', 'CDS', 'tRNA', 'rRNA', 'misc_feature', 'misc_RNA'}
+    if feature.type not in accept_type:
+        return name
+    name = _extract_name(feature)
+    if name is None:
+        return name
+        # log.warning('Unsupport annotation type {}'.format(feature.type))
+    if feature.type == 'misc_feature':
+        if 'internal transcribed spacer' in name:
+            name = 'ITS'
+        if 'intergenic_spacer' in name or 'IGS' in name:
+            name = name.replace('intergenic_spacer_region', 'IGS')
+    if feature.type == 'misc_RNA':
+        # handle ITS
+        if 'internal transcribed spacer' in name:
+            name = name.replace('internal transcribed spacer', 'ITS')
+    if name is not None:
+        name = utils.safe_path(name)
+    else:
+        return name
+    if arg.rename:
+        name = utils.gene_rename(name)[0]
+    return name
+
+
+def get_spacer(genes):
+    """
+    Given list of genes, extract spacers.
+    genes: [name, feature]
+    """
+    if len(genes) <= 1:
+        return []
+    spacers = list()
+    names = set()
+    # sorted according to sequence starting position
+    genes.sort(key=lambda x: int(x[1].location.start))
+    for i in range(len(genes)-1):
+        b_name, before = genes[i]
+        c_name, current = genes[i+1]
+        invert_repeat = False
+        repeat = False
+        # gene name may contain "_", use "-" instead
+        # sorted_name = '-'.join(sorted([b_name, c_name]))
+        # to be continued
+        name = '-'.join([b_name, c_name])
+        # 1. A.start--A.end--B.start--B.end
+        if before.location.end <= current.location.start:
+            # check invert repeat
+            invert_name = '-'.join([c_name, b_name])
+            if invert_name in names:
+                invert_repeat = True
+            elif name in names:
+                repeat = True
+            else:
+                names.add(name)
+            spacer = SeqFeature(
+                type='spacer',
+                id=name,
+                location=FeatureLocation(before.location.end,
+                                         current.location.start),
+                qualifiers={'upstream': b_name,
+                            'downstream': c_name,
+                            'repeat': str(repeat),
+                            'invert_repeat': str(invert_repeat)})
+            spacers.append(spacer)
+        # 2. A.start--B.start--A.end--B.end
+        elif before.location.end <= current.location.end:
+            # overlap, no spacer
+            pass
+        # 3. A.start--B.start--B.end--A.end
+        else:
+            spacer_up = SeqFeature(
+                type='mosaic_spacer',
+                id=name,
+                location=FeatureLocation(before.location.start,
+                                         current.location.start),
+                qualifiers={'upstream': b_name,
+                            'downstream': c_name,
+                            'repeat': str(repeat),
+                            'invert_repeat': str(invert_repeat)})
+            spacer_down = SeqFeature(
+                type='mosaic_spacer',
+                id='-'.join([c_name, b_name]),
+                location=FeatureLocation(current.location.end,
+                                         before.location.end),
+                qualifiers={'upstream': b_name,
+                            'downstream': c_name,
+                            'repeat': str(repeat),
+                            'invert_repeat': str(invert_repeat)})
+            spacers.extend([spacer_up, spacer_down])
+    spacers = [i for i in spacers if len(i) != 0]
+    return spacers
+
+
+def get_intron(genes):
+    """
+    Given list of genes, extract introns.
+    genes: [name, feature]
+    Return:
+        intron(list): [name, feature]
+    """
+    # exons = []
+    introns = []
+    for gene_name, feature in genes:
+        # for n, part in enumerate(feature.location.parts):
+        #     exon = SeqFeature(
+        #     type='exon',
+        #     id='-'.join([gene_name, n+1]),
+        #     location=part,
+        #     qualifiers={'gene': gene_name,
+        #                 'count': n+1})
+        # exons.append(exon)
+        strand = feature.location.strand
+        # sort by start, no matter which strand
+        parts = sorted(feature.location.parts, key=lambda x: x.start)
+        n_part = len(parts)
+        for i in range(len(parts)-1):
+            before = parts[i]
+            current = parts[i+1]
+            # Z00028
+            if before.end >= current.start:
+                break
+            # complement strand use reversed index
+            # n_intron start with 1 instead of 0
+            if strand != -1:
+                n_intron = i + 1
+            else:
+                n_intron = n_part - i - 1
+            intron = SeqFeature(
+                type='intron',
+                id='{}.{}'.format(gene_name, n_intron),
+                location=FeatureLocation(before.end,
+                                         current.start,
+                                         before.strand),
+                qualifiers={'gene': gene_name,
+                            'count': n_intron})
+            introns.append(intron)
+    return introns
+
+
+def divide(gbfile, arg):
+    """
+    Given genbank file, return divided fasta files.
+    """
+    log.info('Divide {} by annotation.'.format(gbfile))
+
+    def get_taxon(taxon_str):
+        """
+        Get taxon info based on suffix and list from NCBI taxonomy database.
+        """
+        # kingdom|phylum|class|order|family|organims(genus|species)
+        # add my_ prefix to avoid conflict of "class"
+        my_kingdom = ''
+        my_phylum = ''
+        my_class = ''
+        my_order = ''
+        my_family = ''
+        for item in taxon_str:
+            if item in SUPERKINGDOMS:
+                my_kingdom = item
+            # mix superkingdom and kingdom to reduce name length
+            elif item in KINGDOMS:
+                my_kingdom = item
+            elif item in PHYLA:
+                my_phylum = item
+            elif item in CLASSES:
+                my_class = item
+            if item.endswith('ales') or item in ANIMAL_ORDERS:
+                my_order = item
+            elif item.endswith('aceae') or item.endswith('idae'):
+                my_family = item
+        # get fake class for plant
+        if my_phylum == 'Streptophyta' and my_class == '':
+            last_phyta = ''
+            for i in taxon_str:
+                if i.endswith('phyta'):
+                    last_phyta = i
+            try:
+                my_class = taxon_str[taxon_str.index(last_phyta) + 1]
+            except IndexError:
+                my_class = ''
+        return my_kingdom, my_phylum, my_class, my_order, my_family
+
+    raw_fasta = arg._fasta / (gbfile.stem+'.fasta')
+    handle_raw = open(raw_fasta, 'w', encoding='utf-8')
+    for record in clean_gb(gbfile):
+        # only accept gene, product, and spacer in misc_features.note
+        taxon_str = record.annotations.get('taxonomy', None)
+        if taxon_str is None:
+            kingdom, phylum, class_, order, family = '', '', '', '', ''
+        else:
+            kingdom, phylum, class_, order, family = get_taxon(taxon_str)
+        # gb annotation may be empty
+        organism = record.annotations.get('organism', None)
+        if organism is not None:
+            organism = organism.replace(' ', '_')
+            genus, *species = organism.split('_')
+        else:
+            genus, species = '', ''
+        # species name may contain other characters
+        taxon = '{}|{}|{}|{}|{}|{}|{}'.format(kingdom, phylum, class_,
+                                              order, family, genus,
+                                              '_'.join(species))
+        accession = record.annotations.get('accessions', ['', ])[0]
+        specimen = record.features[0].qualifiers.get('specimen_voucher',
+                                                     ['', ])
+        specimen = specimen[0].replace(' ', '_')
+        isolate = record.features[0].qualifiers.get('isolate', ['', ])
+        isolate = isolate[0].replace(' ', '_')
+        # usually the record only has one of them
+        specimen = '_'.join([specimen, isolate]).rstrip('_')
+        seq_info = (taxon, accession, specimen)
+        whole_seq = record.seq
+        feature_name = []
+        have_intron = {}
+        genes = []
+        not_genes = []
+        # get genes
+        for feature in record.features:
+            # skip unsupport feature
+            # support: gene, CDS, tRNA, rRNA, misc_feature, misc_RNA
+            name = get_feature_name(feature, arg)
+            if name is None:
+                continue
+            if len(name) > arg.max_name_len:
+                log.debug(f'Too long name: {name}. Truncated.')
+                name = name[:arg.max_name_len-3] + '...'
+            if feature.type == 'gene':
+                genes.append([name, feature])
+                # only use gene name as sequence id
+                feature_name.append(name)
+            else:
+                not_genes.append([name, feature])
+            if isinstance(feature.location, CompoundLocation):
+                # use dict to remove repeat name of gene/CDS/tRNA/rRNA
+                have_intron[name] = feature
+
+        # write genes
+        write_seq(genes, seq_info, whole_seq, arg)
+        # write non-genes
+        write_seq(not_genes, seq_info, whole_seq, arg)
+        # extract spacer
+        spacers = get_spacer(genes)
+        # write spacer annotations
+        if not arg.allow_mosaic_spacer:
+            spacers = [i for i in spacers if i.type != 'mosaic_spacer']
+        # extract intron
+        introns = get_intron(have_intron.items())
+        if not arg.allow_invert_repeat:
+            spacers = [i for i in spacers if i.qualifiers[
+                'invert_repeat'] == 'False']
+        if arg.out_debug:
+            record.features.extend(spacers)
+            record.features.extend(introns)
+            SeqIO.write(record, arg.out/'extend.gb', 'gb')
+        # write seq
+        spacers_to_write = [[i.id, i] for i in spacers]
+        # write intron or not?
+        introns_to_write = [(i.id, i) for i in introns]
+        write_seq(spacers_to_write, seq_info, whole_seq, arg)
+        write_seq(introns_to_write, seq_info, whole_seq, arg)
+        # write to group_by name, i.e., one gb record one fasta
+        if 'ITS' in feature_name:
+            name_str = 'ITS'
+        elif len(feature_name) >= 4:
+            name_str = '{}-...-{}'.format(feature_name[0], feature_name[-1])
+        elif len(feature_name) == 0:
+            name_str = 'Unknown'
+        else:
+            name_str = '-'.join(feature_name)
+        # directly use genome type as name
+        if arg.organelle not in ('ignore', 'no', 'both'):
+            name_str = '{}_genome'.format(arg.organelle)
+        record.id = '|'.join([name_str, taxon, accession, specimen])
+        record.description = ''
+        filename = arg._fasta / (name_str+'.fasta')
+        try:
+            with open(filename, 'a', encoding='utf-8') as out:
+                SeqIO.write(record, out, 'fasta')
+            # write raw fasta
+            SeqIO.write(record, handle_raw, 'fasta')
+        except Exception:
+            log.warning(f'Invalid sequence {accession}.')
+    # skip analyze of Unknown.fasta
+    # unknown = arg._divide / 'Unknown.fasta'
+    log.info('Divide finished.')
+    return arg._fasta, arg._divide
+
+
+def write_seq(record, seq_info, whole_seq, arg):
+    """
+    Write fasta files to "by-gene" folder only.
+    ID format: >name|taxon|accession|specimen|type
+    Args:
+        record: [name, feature]
+        seq_info: (taxon, accession, specimen)
+        whole_seq: whole sequence
+        arg: arguments
+    Return: {filename}
+    """
+    def careful_extract(name, feature, whole_seq):
+        # illegal annotation may cause extraction failed
+        try:
+            sequence = feature.extract(whole_seq)
+            sequence_str = str(sequence)
+        except Exception as e:
+            sequence_str = ''
+            log.warning('Cannot extract sequence of {} from {} '
+                        'due to "{}".'.format(name, seq_info[1], str(e)))
+        return sequence_str
+
+    seq_len = len(whole_seq)
+    filenames = set()
+    expand_files = set()
+    record_unique = []
+    if not arg.allow_repeat:
+        names = set()
+        for i in record:
+            if i[0] not in names:
+                record_unique.append(i)
+                names.add(i[0])
+    else:
+        record_unique = record
+
+    for i in record_unique:
+        name, feature = i
+        # skip abnormal annotation
+        if len(feature) > arg.max_gene_len:
+            log.debug('The fragment of {} (Accession {}) '
+                      'is too long. Skip.'.format(name, seq_info[1]))
+            continue
+        filename = arg._divide / (feature.type+'-'+name+'.fasta')
+        with open(filename, 'a', encoding='utf-8') as handle:
+            sequence_id = '>' + '|'.join([name, *seq_info, feature.type])
+            sequence = careful_extract(name, feature, whole_seq)
+            handle.write(sequence_id+'\n')
+            handle.write(sequence+'\n')
+        filenames.add(filename)
+        if arg.expand != 0:
+            if feature.location_operator == 'join':
+                loc = feature.location.parts
+                # ensure increasing order
+                # parts do not have sort method
+                loc.sort(key=lambda x: x.start)
+                new_loc = sum([
+                    # avoid IndexError
+                    FeatureLocation(max(0, loc[0].start-arg.expand),
+                                    loc[0].end, loc[0].strand),
+                    *loc[1:-1],
+                    FeatureLocation(loc[-1].start,
+                                    min(seq_len, loc[-1].end+arg.expand),
+                                    loc[-1].strand)])
+                feature.location = new_loc
+            sequence = careful_extract(name, feature, whole_seq)
+            filename2 = arg._expand / (feature.type+'-'+name+'.fasta')
+            with open(filename2, 'a', encoding='utf-8') as handle:
+                handle.write(sequence_id + '\n')
+                handle.write(str(sequence) + '\n')
+            expand_files.add(filename2)
+    # keep = ('gene.fasta', 'misc_feature', 'misc_RNA', 'spacer')
+    # for i in filenames:
+        # if i.endswith(keep):
+            # file_to_analyze.append(i)
+        # else:
+            # log.debug('Skip {}'.format(i))
+    return filenames
+
+
+def count_for_unique(fasta: Path):
+    info = defaultdict(lambda: list())
+    index = 0
+    count = 0
+    for record in SeqIO.parse(fasta, 'fasta'):
+        # gene|kingdom|phylum|class|order|family|genus|species|specimen|type
+        count += 1
+        if '|' in record.id:
+            name = ' '.join(record.id.split('|')[6:8])
+        else:
+            name = record.id
+        length = len(record)
+        # skip empty file
+        if length != 0:
+            info[name].append([index, length])
+        index += 1
+    return info, count
+
+
+def unique(files: list, arg) -> list:
+    """
+    Remove redundant sequences of same species.
+    Files were saved in arg._unique
+    """
+    log.info('Removing redundant records...')
+    unique_files = []
+    # if arg.unique == 'no':
+    #     return unique_files
+    total = 0
+    kept = 0
+    for fasta in files:
+        keep = dict()
+        info, count = count_for_unique(fasta)
+        total += count
+        if arg.unique == 'first':
+            # keep only the first record
+            keep = {info[i][0][0] for i in info}
+        elif arg.unique == 'longest':
+            for i in info:
+                info[i] = sorted(info[i], key=lambda x: x[1], reverse=True)
+            keep = {info[i][0][0] for i in info}
+        else:
+            # ignore "no"
+            pass
+        kept += len(keep)
+        new = arg._unique / fasta.name
+        with open(new, 'w', encoding='utf-8') as out:
+            for idx, record in enumerate(SeqIO.parse(fasta, 'fasta')):
+                if idx in keep:
+                    SeqIO.write(record, out, 'fasta')
+        unique_files.append(new)
+    log.info(f'{kept} of {total} unique records.')
+    return unique_files
+
+
+def gb2fasta_main(arg_str=None):
+    """
+    Collect genbank files and convert them to fasta files.
+    Args:
+        arg_str(str or None): string for parse_arg
+    """
+    log.info('Running gb2fasta module...')
+    if arg_str is None:
+        arg, other_args = parse_args()
+    else:
+        arg, other_args = parse_args(arg_str.split(' '))
+    arg = init_arg(arg)
+    if arg is None:
+        log.info('Quit gb2fasta module.')
+        return None, other_args
+    utils.add_file_log(arg)
+    log.info(f'Input genbank files:\t{arg.gb}')
+    if arg.query is not None:
+        log.info(f'Query: {arg.query}')
+        gb_file = download(arg)
+        if gb_file is not None:
+            arg.gb.append(gb_file)
+    if arg.no_divide:
+        log.info('Download finished. Skip dividing.')
+        log.info('GB2fasta module finished.')
+        return arg, other_args
+    for i in arg.gb:
+        divide(i, arg)
+    if arg.unique == 'no':
+        log.info('Skip removing redundant sequences.')
+        unique_files = arg._divide.glob('*.fasta')
+        unique_files = [i for i in unique_files if i.name != 'Unknown.fasta']
+    else:
+        if arg.no_divide:
+            fasta_files = arg._fasta.glob('*.fasta')
+            fasta_files = [i for i in fasta_files
+                           if i.name != 'Unknown.fasta']
+            unique_files = unique(fasta_files, arg)
+        else:
+            if arg.expand == 0:
+                divided_files = arg._divide.glob('*.fasta')
+                divided_files = [i for i in divided_files
+                                 if i.name != 'Unknown.fasta']
+                unique_files = unique(divided_files, arg)
+            else:
+                expanded_files = arg._expand.glob('*.fasta')
+                expanded_files = [i for i in expanded_files
+                                  if i.name != 'Unknown.fasta']
+                unique_files = unique(expanded_files, arg)
+    # for i in unique_files:
+    #     utils.move(i, arg._unique/(i.name), copy=True)
+    log.info('GB2fasta module finished.')
+    return arg, other_args
+
+
+if __name__ == '__main__':
+    gb2fasta_main()
```

### Comparing `ogu-1.52/src/OGU/primer.py` & `ogu-1.54/src/OGU/primer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,784 +1,784 @@
-#!/usr/bin/python3
-
-import argparse
-import platform
-import re
-import subprocess
-from collections import defaultdict
-from io import StringIO
-from itertools import product as cartesian_product
-from os import cpu_count
-from pathlib import Path
-
-import numpy as np
-from Bio.Seq import Seq
-from Bio.SeqRecord import SeqRecord
-from Bio.SeqFeature import SeqFeature, FeatureLocation
-from Bio.Data.IUPACData import ambiguous_dna_values as ambiguous_data
-from Bio import SeqIO
-from primer3 import (calc_tm, calc_hairpin_tm, calc_homodimer_tm,
-                     calc_heterodimer_tm)
-
-from OGU import utils
-from OGU import evaluate
-from OGU.global_vars import log
-
-
-class Pair:
-    # save memory
-    __slots__ = ['left', 'right', 'delta_tm', 'coverage', 'start', 'end',
-                 'observed_res', 'tree_res', 'pd_terminal', 'entropy',
-                 'have_heterodimer', 'heterodimer_tm', 'pi', 'score',
-                 'length', 'gap_ratio']
-
-    _title = ('Score,AvgProductLength,StdEV,'
-              'MinProductLength,MaxProductLength,'
-              'Coverage,Observed_Res,Tree_Res,PD_terminal,Entropy,'
-              'LeftSeq,LeftTm,LeftAvgBitscore,LeftAvgMismatch,'
-              'RightSeq,RightTm,RightAvgBitscore,RightAvgMismatch,'
-              'DeltaTm,AlnStart,AlnEnd,AvgSeqStart,AvgSeqEnd')
-    _style = ('{:.2f},{:.0f},{:.0f},'
-              '{},{},'
-              '{:.2%},{:.2%},{:.6f},{:.6f},{:.6f},'
-              '{},{:.2f},{:.2f},{:.2f},'
-              '{},{:.2f},{:.2f},{:.2f},'
-              '{:.2f},{},{},{},{}')
-
-    def __init__(self, left, right, alignment):
-        rows, columns = alignment.shape
-        self.left = left
-        self.right = right
-        self.delta_tm = abs(self.left.tm - self.right.tm)
-        # get accurate length
-        a = len(self.left) / 2
-        b = len(self.right) / 2
-        common = left.mid_loc.keys() & right.mid_loc.keys()
-        lengths = [[key, ((right.mid_loc[key] - b) - (left.mid_loc[key] + a))
-                    ] for key in common]
-        lengths = {i[0]: int(i[1]) for i in lengths if i[1] > 0}
-        self.length = lengths
-        self.right.coverage = len(self.right.mid_loc) / rows
-        self.coverage = len(common) / rows
-        # pairs use mid_loc from BLAST as start/end
-        self.start = self.left.avg_mid_loc
-        self.end = self.right.avg_mid_loc
-        self.have_heterodimer = False
-        self.heterodimer_tm = 0.0
-        self.observed_res = 0.0
-        self.tree_res = 0.0
-        self.pd_terminal = 0.0
-        self.entropy = 0.0
-        self.pi = 0.0
-        self.gap_ratio = 0.0
-        self.score = self.get_score()
-
-    def __repr__(self):
-        return (
-            'Pair(score={:.2f}, product={:.0f}, start={}, end={}, left={}, '
-            'right={}, observerd_res={:.2%}, coverage={:.2%},'
-            'delta_tm={:.2f}, have_heterodimer={})'.format(
-                self.score, utils.safe_average(
-                    list(self.length.values())), self.start,
-                self.end, self.left.seq, self.right.seq, self.observed_res,
-                self.coverage, self.delta_tm, self.have_heterodimer))
-
-    def __str__(self):
-        return Pair._style.format(
-            self.score, utils.safe_average(list(self.length.values())),
-            np.std(list(self.length.values())), min(self.length.values()),
-            max(self.length.values()),
-            self.coverage, self.observed_res, self.tree_res,
-            self.pd_terminal, self.entropy,
-            self.left.seq, self.left.tm, self.left.avg_bitscore,
-            self.left.avg_mismatch,
-            self.right.seq, self.right.tm, self.right.avg_bitscore,
-            self.right.avg_mismatch,
-            self.delta_tm, self.left.start, self.right.end, self.start,
-            self.end)
-
-    def get_score(self):
-        # calculate score of given primer pairs. Suggestion only
-        # use score to filter primer pairs
-        return (utils.safe_average(list(self.length.values())) * 0.5
-                + self.coverage * 200
-                + len(self.left) * 10
-                + len(self.right) * 10
-                + self.observed_res * 100
-                + self.tree_res * 100 + self.entropy * 5
-                - int(self.have_heterodimer) * 10
-                - self.delta_tm * 5 - self.left.avg_mismatch * 10
-                - self.right.avg_mismatch * 10)
-
-    def add_info(self, alignment):
-        # put attributes that need heavy computation here for the final primer
-        # pairs in order to save CPU time
-        if not self.right.is_reverse_complement:
-            self.right = self.right.reverse_complement()
-        # include end base, use alignment loc for slice
-        subalign = alignment[:, self.left.start:self.right.end+1]
-        tmp = Path()
-        variance, _ = evaluate.get_resolution(subalign, tmp)
-        (self.gap_ratio, self.observed_res, self.entropy, self.pi,
-         _, _, self.pd_terminal) = variance[2:9]
-        self.heterodimer_tm = calc_ambiguous_seq(
-            calc_heterodimer_tm, self.left.seq, self.right.seq)
-        if max(self.heterodimer_tm, self.left.tm,
-               self.right.tm) == self.heterodimer_tm:
-            self.have_heterodimer = True
-        else:
-            self.have_heterodimer = False
-        self.get_score()
-        self.left.update_id()
-        self.right.update_id()
-        return self
-
-
-class PrimerWithInfo(SeqRecord):
-    # inherit from Bio.SeqRecord.SeqRecord
-    def __init__(self, seq='', quality=None, start=0, coverage=0,
-                 avg_bitscore=0, mid_loc=None, avg_mismatch=0, detail=0,
-                 is_reverse_complement=False):
-        # store str
-        super().__init__(Seq(seq.upper()))
-        self.sequence = str(self.seq)
-
-        # primer3.setGlobals seems have no effect on calcTm, use
-        # calc_ambiguous_seq
-        self.quality = self.letter_annotations['solexa_quality'] = quality
-        self.start = self.annotations['start'] = start
-        self.end = self.annotations['end'] = start + self.__len__() - 1
-        self.coverage = self.annotations['coverage'] = coverage
-        self.avg_bitscore = self.annotations['avg_bitscore'] = avg_bitscore
-        self.mid_loc = self.annotations['mid_loc'] = mid_loc
-        self.avg_mismatch = self.annotations['avg_mismatch'] = avg_mismatch
-        self.detail = self.annotations['detail'] = detail
-        self.is_reverse_complement = self.annotations[
-            'is_reverse_complement'] = False
-        self.description = self.annotations['description'] = ''
-        self.avg_mid_loc = 0
-        self.hairpin_tm = 0
-        self.homodimer_tm = 0
-        self.tm = 0
-        self.update_id()
-
-    def __getitem__(self, i):
-        # part of attribution do not change, others were reset
-        if isinstance(i, int):
-            i = slice(i, i + 1)
-        if isinstance(i, slice):
-            answer = PrimerWithInfo(seq=str(self.seq[i]),
-                                    quality=self.quality[i])
-            answer.annotations = dict(self.annotations.items())
-            return answer
-        else:
-            log.exception('Bad index.')
-            raise
-
-    def reverse_complement(self):
-        table = str.maketrans('ACGTMRWSYKVHDBXN', 'TGCAKYWSRMBDHVXN')
-        new_seq = str.translate(self.sequence, table)[::-1]
-        new_quality = self.quality[::-1]
-        # try to simplify??
-        return PrimerWithInfo(seq=new_seq, quality=new_quality,
-                              start=self.start, coverage=self.coverage,
-                              avg_bitscore=self.avg_bitscore,
-                              mid_loc=self.mid_loc,
-                              is_reverse_complement=True,
-                              detail=self.detail)
-
-    def update_id(self):
-        self.end = self.annotations['end'] = self.start + self.__len__() - 1
-        if self.mid_loc is not None and len(self.mid_loc) != 0:
-            self.avg_mid_loc = int(utils.safe_average(list(
-                self.mid_loc.values())))
-        self.id = ('AvgMidLocation({:.0f})-Tm({:.2f})-Coverage({:.2%})-'
-                   'AvgBitScore({:.2f})-Start({})-End({})'.format(
-            self.avg_mid_loc, self.tm, self.coverage,
-            self.avg_bitscore, self.start, self.end))
-
-
-def parse_args(arg_list=None):
-    arg = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description=primer_main.__doc__)
-    arg.add_argument('-aln', nargs='*', help='alignment files')
-    arg.add_argument('-aln_folder', default=None,
-                     help='folder of aligned files')
-    arg.add_argument('-out', help='output directory')
-    arg.add_argument('-ambiguous', dest='ambiguous_base_n', default=4, type=int,
-                     help='number of ambiguous bases')
-    arg.add_argument('-coverage', dest='coverage', default=0.5, type=float,
-                     help='minimal coverage of base and primer')
-    arg.add_argument('-mismatch', dest='mismatch', default=4, type=int,
-                     help='maximum mismatch bases in primer')
-    arg.add_argument('-pmin', dest='min_primer', default=20, type=int,
-                     help='minimum primer length')
-    arg.add_argument('-pmax', dest='max_primer', default=30, type=int,
-                     help='maximum primer length')
-    arg.add_argument('-res', dest='resolution', type=float, default=0.3,
-                     help='minimal resolution')
-    arg.add_argument('-topn', dest='top_n', type=int, default=1,
-                     help='keep n primers for each high variant region')
-    arg.add_argument('-amin', dest='min_product', default=300, type=int,
-                     help='minimum amplified length (include primer)')
-    arg.add_argument('-amax', dest='max_product', default=800, type=int,
-                     help='maximum amplified length (include primer)')
-    arg.add_argument('-size', type=int, default=500, help='window size for sliding scan')
-    arg.add_argument('-step', type=int, default=50, help='step length for sliding scan')
-    arg.add_argument('-primer', action='store_true', help='design universal primer')
-    if arg_list is None:
-        return arg.parse_known_args()
-    else:
-        return arg.parse_known_args(arg_list)
-
-
-def init_arg(arg):
-    arg = utils.init_out(arg)
-    if all([arg.aln, arg.aln_folder]):
-        log.info('Do not recommend to use "-aln" and "-aln_folder" '
-                 'at same time!')
-    if arg.aln is not None:
-        arg.aln = [Path(i).absolute() for i in arg.aln]
-    else:
-        arg.aln = []
-    if arg.aln_folder is not None:
-        for i in Path(arg.aln_folder).glob('*'):
-            arg.aln.append(i.absolute())
-    log.info('Add aligned files from evaluate module if possible.')
-    for i in Path(arg._align).glob('*'):
-        arg.aln.append(i.absolute())
-    for i in arg.aln:
-        if not i.exists() or not i.is_file():
-            log.error(f'{i} does not exist or is not a valid file.')
-            return None
-    if not any([arg.aln, arg.aln_folder]):
-        log.warning('Empty input.')
-        return None
-    return arg
-
-
-def calc_ambiguous_seq(func, seq, seq2=None):
-    """
-    Expand sequences with ambiguous bases to several clean sequences and apply
-    func to every sequence.
-    Return average value. Return 0 if len(seq) > 60 (from primer3)
-    """
-    # Seems primer3 only accept seqs shorter than 60 bp. Plus, too long seq
-    # will cost too much memory.
-    len_limit = 60
-
-    def _expand(seq):
-        seq_list = []
-        for base in seq:
-            # replace illegal base with 'N'
-            if base not in ambiguous_data:
-                base = 'N'
-            seq_list.append(ambiguous_data[base])
-        seq_product = list(cartesian_product(*seq_list))
-        seq_str = [''.join(i) for i in seq_product]
-        return seq_str
-
-    if len(seq) > len_limit:
-        log.warning('Too many ambiguous bases. Skip')
-        return 0
-    seq_str = _expand(seq)
-    if seq2 is None:
-        values = [func(i) for i in seq_str]
-    else:
-        if len(seq2) > len_limit:
-            log.warning('Too many ambiguous bases. Skip')
-            return 0
-        seq_str2 = _expand(seq2)
-        products = cartesian_product(seq_str, seq_str2)
-        values = [func(i[0], i[1]) for i in products]
-    # primer3 will return negative values sometime
-    values_positive = [max(0, i) for i in values]
-    return utils.safe_average(values_positive)
-
-
-def count_base(alignment: np.array):
-    """
-    Given alignment numpy array, count cumulative frequency of base in each
-    column (consider ambiguous base and "N", "-" and "?", otherwise omit).
-    Return [[float, float, float, float, float, float, float]] for
-    [A, T, C, G, N, GAP, OTHER].
-    """
-    frequency = []
-    rows, columns = alignment.shape
-    for index in range(columns):
-        base, counts = np.unique(alignment[:, [index]], return_counts=True)
-        count_dict = {b'A': 0, b'C': 0, b'G': 0, b'T': 0, b'M': 0, b'R': 0,
-                      b'W': 0, b'S': 0, b'Y': 0, b'K': 0, b'V': 0, b'H': 0,
-                      b'D': 0, b'B': 0, b'X': 0, b'N': 0, b'-': 0, b'?': 0}
-        count_dict.update(dict(zip(base, counts)))
-        a = (count_dict[b'A'] +
-             (count_dict[b'D'] + count_dict[b'H'] + count_dict[b'V']) / 3 +
-             (count_dict[b'M'] + count_dict[b'R'] + count_dict[b'W']) / 2)
-        t = (count_dict[b'T'] +
-             (count_dict[b'B'] + count_dict[b'H'] + count_dict[b'D']) / 3 +
-             (count_dict[b'K'] + count_dict[b'W'] + count_dict[b'Y']) / 2)
-        c = (count_dict[b'C'] +
-             (count_dict[b'B'] + count_dict[b'H'] + count_dict[b'V']) / 3 +
-             (count_dict[b'M'] + count_dict[b'S'] + count_dict[b'Y']) / 2)
-        g = (count_dict[b'G'] +
-             (count_dict[b'B'] + count_dict[b'D'] + count_dict[b'V']) / 3 +
-             (count_dict[b'K'] + count_dict[b'R'] + count_dict[b'S']) / 2)
-        gap = count_dict[b'-']
-        n = count_dict[b'N'] + count_dict[b'X'] + count_dict[b'?']
-        other = rows - a - t - c - g - gap - n
-        frequency.append([a, t, c, g, n, gap, other])
-    return frequency
-
-
-def get_quality(data, rows):
-    """
-    Calculate quality score.
-    """
-    # use fastq-illumina format
-    max_q = 62
-    factor = max_q / rows
-    # use min to avoid KeyError
-    quality_value = [min(max_q, int(i * factor)) - 1 for i in data]
-    return quality_value
-
-
-def get_consensus(base_cumulative_frequency, coverage_percent: float,
-                  rows: int, output: Path):
-    """
-    Given count info of bases, return consensus(PrimerWithInfo).
-    """
-    def get_ambiguous_dict():
-        data = dict(zip(ambiguous_data.values(), ambiguous_data.keys()))
-        # 2:{'AC': 'M',}
-        data_with_len = defaultdict(lambda: dict())
-        for i in data:
-            data_with_len[len(i)][i] = data[i]
-        return data_with_len
-
-    ambiguous_dict = get_ambiguous_dict()
-    most = []
-    coverage = rows * coverage_percent
-
-    limit = coverage / len('ATCG')
-    for location, column in enumerate(base_cumulative_frequency):
-        finish = False
-        # "*" for others
-        value = dict(zip(list('ATCGN-*'), column))
-
-        base = 'N'
-        if value['N'] >= limit:
-            count = value['N']
-            most.append([location, base, count])
-            continue
-        sum_gap = value['-'] + value['*']
-        if sum_gap >= limit:
-            base = '-'
-            count = sum_gap
-            most.append([location, base, count])
-            continue
-        # 1 2 3 4
-        for length in ambiguous_dict:
-            # A T CG CT ACG CTG ATCG
-            for key in ambiguous_dict[length]:
-                count = 0
-                for letter in list(key):
-                    if finish:
-                        break
-                    count += value[letter]
-                    if count >= coverage:
-                        base = ambiguous_dict[length][key]
-                        finish = True
-                        most.append([location, base, count])
-    quality_raw = [i[2] for i in most]
-    consensus = PrimerWithInfo(start=1, seq=''.join([i[1] for i in most]),
-                               quality=get_quality(quality_raw, rows))
-    SeqIO.write(consensus, output, 'fastq')
-    return consensus
-
-
-def get_good_region(index, seq_count, arg):
-    """
-    Return regions marked for finding primers. Because of alignment gap, PCR
-    product may smaller than given length limitation.
-    """
-    n = arg.max_product - arg.min_product
-    good_region = set()
-    for i, j in zip(index, seq_count):
-        if j >= arg.resolution:
-            good_region.update(range(i - arg.max_primer, i - n))
-            good_region.update(range(i + arg.min_product,
-                                     i - arg.max_primer + arg.max_product))
-    return good_region
-
-
-def find_continuous(consensus, good_region, min_len):
-    """
-    Given PrimerWithInfo, good_region, min_len
-    Return consensus with features.
-    """
-    skip = ('N', '-')
-    start = 0
-    for index, base in enumerate(consensus.sequence[:-min_len]):
-        if base in skip or index not in good_region:
-            if (index - start) >= min_len:
-                consensus.features.append(SeqFeature(FeatureLocation(
-                    start, index, strand=1), type='continuous'))
-            start = index + 1
-    return consensus
-
-
-def find_primer(consensus, arg):
-    """
-    Find suitable primer in given consensus with features labeled as candidate
-    primer, return list of PrimerWithInfo, consensus.
-    """
-    # repeat no more than 5 times
-    poly = re.compile(r'([ATCG])\1\1\1\1')
-    tandem = re.compile(r'([ATCG]{2})\1\1\1\1')
-
-    def is_good_primer(primer):
-        # use re and primer3 to check weather it's good primer
-        # ref1. http://www.premierbiosoft.com/tech_notes/PCR_Primer_Design.html
-        ambiguous_base = len(primer)
-        for i in list('ATCG'):
-            ambiguous_base -= primer.seq.count(i)
-        if ambiguous_base > max_ambiguous:
-            return False
-        if re.search(poly, str(primer.seq)) is not None:
-            primer.detail = 'Poly(NNNNN) structure found'
-            return False
-        if re.search(tandem, str(primer.seq)) is not None:
-            primer.detail = 'Tandom(NN*5) exist'
-            return False
-        primer.hairpin_tm = calc_ambiguous_seq(calc_hairpin_tm, primer.seq)
-        primer.tm = primer.annotations['tm'] = calc_ambiguous_seq(calc_tm,
-                                                                  primer.seq)
-        # primer3.calcHairpin or calcHomodimer usually return structure found
-        # with low Tm. Here we compare structure_tm with sequence tm
-        if primer.hairpin_tm >= primer.tm:
-            primer.detail = 'Hairpin found'
-            return False
-        primer.homodimer_tm = calc_ambiguous_seq(calc_homodimer_tm, primer.seq)
-        if primer.homodimer_tm >= primer.tm:
-            primer.detail = 'Homodimer found'
-            return False
-        return True
-
-    primers = []
-    min_len = arg.min_primer
-    max_len = arg.max_primer
-    max_ambiguous = arg.ambiguous_base_n
-    # skip good_region
-    continuous = consensus.features
-    for feature in continuous:
-        fragment = feature.extract(consensus)
-        len_fragment = len(fragment)
-        for begin in range(len_fragment - max_len):
-            for p_len in range(min_len, max_len + 1):
-                start = feature.location.start + begin
-                primer = consensus[start:start + p_len]
-                if is_good_primer(primer):
-                    consensus.features.append(SeqFeature(
-                        FeatureLocation(start, start + p_len, strand=1),
-                        type='primer'))
-                    primer.start = start
-                    primer.update_id()
-                    primers.append(primer)
-    return primers, consensus
-
-
-def old_remove_gap(aln_fasta: Path, new_file: Path) -> Path:
-    # to be removed
-    """
-    old function, for BLAST
-    Args:
-        aln_fasta: fasta with gap
-        new_file: fasta without gap
-    Returns:
-        new_file: fasta without gap
-    """
-    no_gap = StringIO()
-    with open(aln_fasta, 'r', encoding='utf-8') as raw:
-        for line in raw:
-            no_gap.write(line.replace('-', ''))
-    # try to avoid makeblastdb error
-    no_gap.seek(0)
-    SeqIO.convert(no_gap, 'fasta', new_file, 'fasta')
-    no_gap.close()
-    return new_file
-
-
-def validate(primer_candidate: list, aln: Path, n_seqs: int, arg):
-    """
-    Do BLAST. Parse BLAST result. Return list of PrimerWithInfo which passed
-    the validation.
-    """
-    evalue = 1e-2
-    _, blast = utils.get_blast()
-    if not _:
-        log.critical('Cannot find BLAST.')
-        return []
-    locus_name = aln.stem
-    # chmod +x
-    if platform.system() == 'Windows':
-        makeblastdb = Path(blast).parent / 'makeblastdb.exe'
-    else:
-        makeblastdb = Path(blast).parent / 'makeblastdb'
-        makeblastdb.chmod(0o755)
-    query_file = arg._primer / (locus_name+'.candidate.fasta')
-    query_file_fastq = arg._primer / (locus_name+'.candidate.fastq')
-    # SeqIO.write fasta file directly is prohibited. have to write fastq at
-    # first.
-    with open(query_file_fastq, 'w', encoding='utf-8') as _:
-        SeqIO.write(primer_candidate, _, 'fastq')
-    SeqIO.convert(query_file_fastq, 'fastq', query_file, 'fasta')
-    # build blast db
-    db_file = old_remove_gap(aln, arg._tmp/(locus_name+'-db_file.fasta'))
-    # db_file = utils.move(aln, arg._tmp/(locus_name+'-db_file.fasta'), copy=True)
-    _ = subprocess.run(f'{makeblastdb} -in {db_file} -dbtype nucl '
-                       f'-out {db_file}', shell=True,
-                       stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-    if _.returncode != 0:
-        log.critical('Failed to run makeblastdb. Skip BLAST.')
-        return []
-    # BLAST
-    blast_result_file = arg._tmp / (locus_name+'-blast.result.tsv')
-    fmt = '7 qseqid sseqid qseq nident mismatch score qstart qend sstart send'
-    cmd = (f'{blast} -task blastn-short -num_threads {max(1, cpu_count()-1)} '
-           f'-query {query_file} -db {db_file} -evalue {evalue} -max_hsps 1 '
-           f'-outfmt "{fmt}" -out {blast_result_file}')
-    # hide output
-    _ = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL,
-                       stderr=subprocess.DEVNULL)
-    if _.returncode != 0:
-        log.critical('Failed to run BLAST.')
-        return []
-    log.info('BLAST finished.')
-    log.info('Parsing BLAST result.')
-    blast_result = dict()
-    # because SearchIO.parse is slow, use parse_blast_result()
-    for query in utils.parse_blast_tab(blast_result_file):
-        if len(query) == 0:
-            continue
-        sum_bitscore_raw = 0
-        sum_mismatch = 0
-        good_hits = 0
-        mid_loc = dict()
-        hit = query[0]
-        for hit in query:
-            min_positive = len(hit.query_seq) - arg.mismatch
-            hsp_bitscore_raw = hit.bitscore_raw
-            positive = hit.ident_num
-            mismatch = hit.mismatch_num
-            loc = utils.safe_average([hit.hit_start, hit.hit_end])
-            if positive >= min_positive and mismatch <= arg.mismatch:
-                sum_bitscore_raw += hsp_bitscore_raw
-                sum_mismatch += mismatch
-                good_hits += 1
-                # middle location of primer, the difference of two mid_loc
-                # approximately equals to the length of amplified fragment.
-                mid_loc[hit.hit_id] = loc
-        coverage = good_hits / n_seqs
-        if coverage >= arg.coverage:
-            blast_result[hit.query_id] = {
-                'coverage': coverage,
-                'avg_bitscore': sum_bitscore_raw / good_hits,
-                'avg_mismatch': sum_mismatch / good_hits,
-                'mid_loc': mid_loc}
-    primer_verified = []
-    for primer in primer_candidate:
-        i = primer.id
-        if i in blast_result:
-            primer.coverage = blast_result[i]['coverage']
-            primer.avg_bitscore = blast_result[i]['avg_bitscore']
-            primer.mid_loc = blast_result[i]['mid_loc']
-            primer.avg_mismatch = blast_result[i]['avg_mismatch']
-            primer.update_id()
-            primer_verified.append(primer)
-    primer_verified.sort(key=lambda x: x.start)
-    # clean
-    utils.clean_tmp(db_file)
-    blast_result_file.unlink()
-    log.info('Parse finished.')
-    return primer_verified
-
-
-def pick_pair(primers, alignment, arg):
-    """
-    Pick primer pairs passed the validation and its product length fulfill the
-    requirement.
-    """
-    pairs = []
-    for n_left, left in enumerate(primers):
-        # convert mid_loc to 5' location
-        # use int to speedup, comparing of float seems slow
-        location = int(left.avg_mid_loc - len(left) / 2)
-        begin = location + arg.min_product
-        # fragment plus one primer = max_product length
-        end = location + arg.max_product - len(left)
-        # create [] is faster than list()
-        cluster = []
-        for right in primers[(n_left + 1):]:
-            if right.avg_mid_loc < begin:
-                continue
-            if right.avg_mid_loc > end:
-                break
-            pair = Pair(left, right, alignment)
-            if pair.coverage < arg.coverage:
-                continue
-            cluster.append(pair)
-        cluster.sort(key=lambda x: x.score, reverse=True)
-        # only keep top n for each primer cluster
-        pairs.extend(cluster[:arg.top_n])
-    if len(pairs) == 0:
-        return []
-    # remove close located primers
-    less_pairs = []
-    cluster = [pairs[0], ]
-    pairs.sort(key=lambda x: x.start)
-    for index in range(1, len(pairs)):
-        if pairs[index].start - pairs[index - 1].start < arg.min_primer:
-            cluster.append(pairs[index])
-        else:
-            cluster.sort(key=lambda x: x.score, reverse=True)
-            less_pairs.extend(cluster[:arg.top_n])
-            cluster = []
-    cluster.sort(key=lambda x: x.score, reverse=True)
-    less_pairs.extend(cluster[:arg.top_n])
-    log.info('{} pairs of redundant primers were removed.'.format(
-        len(pairs) - len(less_pairs)))
-    good_pairs = []
-    for i in less_pairs:
-        i.add_info(alignment)
-        if i.observed_res >= arg.resolution:
-            good_pairs.append(i)
-    good_pairs.sort(key=lambda x: x.score, reverse=True)
-    log.info('Successfully found validated primers.')
-    return good_pairs[:arg.top_n]
-
-
-def get_observed_res(alignment: np.array, arg):
-    """
-    For primer design.
-    Observed resolution used as lower bound.
-    Args:
-        alignment:
-        arg:
-    Returns:
-        index: list
-        observed_res_list: list
-    """
-    index = []
-    observed_res_list = []
-    rows, columns = alignment.shape
-    for i in range(0, columns, arg.step):
-        subalign = alignment[:, i:i+arg.size]
-        sub_rows, sub_columns = subalign.shape
-        item, count = np.unique(subalign, return_counts=True, axis=0)
-        observed_res = len(count) / sub_rows
-        index.append(i)
-        observed_res_list.append(observed_res)
-    return index, observed_res_list
-
-
-def primer_design(aln: Path, result: Path, arg):
-    locus_name = aln.stem
-    name, alignment, = evaluate.fasta_to_array(aln)
-    if name is None:
-        log.debug(f'Invalid alignment file {aln}.')
-        return False
-    rows, columns = alignment.shape
-    # generate consensus
-    base_cumulative_frequency = count_base(alignment)
-    log.info(f'Generate consensus of {aln}.')
-    consensus = get_consensus(base_cumulative_frequency, arg.coverage, rows,
-                              arg._align/(locus_name+'-consensus.fastq'))
-    log.info(f'Evaluate whole alignment of {aln}.')
-    # a_ : alignment
-    item, count = np.unique(alignment, return_counts=True, axis=0)
-    observed_res = len(count) / rows
-    if observed_res < arg.resolution:
-        log.error('Observed resolution is too low.')
-        return False
-    log.info('Start the sliding-window scan.')
-    index, observed_res_list = get_observed_res(alignment, arg)
-    log.info('Evaluation finished.')
-    log.info('Start finding primers.')
-    log.info('Mark region for finding primer.')
-    good_region = get_good_region(index, observed_res_list, arg)
-    log.info('Finding candidate primers.')
-    consensus = find_continuous(consensus, good_region, arg.min_primer)
-    primer_candidate, consensus = find_primer(consensus, arg)
-    if len(primer_candidate) == 0:
-        log.warning('Cannot find primer candidates. '
-                    'Please consider to loose options.')
-        return True
-    log.info(f'Found {len(primer_candidate)} candidate primers.')
-    log.info('Validate with BLAST. May be slow.')
-    primer_verified = validate(primer_candidate, aln, rows, arg)
-    if len(primer_verified) == 0:
-        log.warning('All candidates failed on validation. '
-                    'Please consider to loose options.')
-        return True
-    log.info('Picking primer pairs.')
-    pairs = pick_pair(primer_verified, alignment, arg)
-    if len(pairs) == 0:
-        log.warning('Cannot find suitable primer pairs. '
-                    'Please consider to loose options.')
-        return True
-    log.info('Output the result.')
-    out1 = open(arg._primer/(locus_name+'.primer.fastq'), 'w', encoding='utf-8')
-    out2 = open(arg._primer/(locus_name+'.primer.csv'), 'w', encoding='utf-8')
-    # write primers to one file
-    out3 = open(result, 'a', encoding='utf-8')
-    csv_title = 'Locus,Samples,' + Pair._title + '\n'
-    out2.write(csv_title)
-    for pair in pairs:
-        line = f'{locus_name},{rows},{str(pair)}\n'
-        out2.write(line)
-        out3.write(line)
-        SeqIO.write(pair.left, out1, 'fastq')
-        SeqIO.write(pair.right, out1, 'fastq')
-    out1.close()
-    out2.close()
-    out3.close()
-    # log.info(f'Primers info were written into {out2}')
-    return True
-
-
-def primer_main(arg_str=None):
-    """
-    Evaluate variance of alignments.
-    """
-    utils.check_system()
-    utils.get_all_third_party(skip_blast=False)
-    if arg_str is None:
-        arg, other_args = parse_args()
-    else:
-        arg, other_args = parse_args(arg_str.split(' '))
-    if not arg.primer and __name__ != '__main__':
-        log.info('Skip primer module.')
-        return None, None
-    log.info('Running primer module...')
-    arg = init_arg(arg)
-    if arg is None:
-        log.info('Quit primer module.')
-        return None, None
-    utils.add_file_log(arg)
-    primer_result = arg.out / 'Primers.csv'
-    csv_title = 'Locus,Samples,' + Pair._title + '\n'
-    with open(primer_result, 'w', encoding='utf-8') as out:
-        out.write(csv_title)
-    if arg is None:
-        log.info('Quit.')
-        return None, None
-    for aln in arg.aln:
-        primer_design(aln, primer_result, arg)
-
-    log.info(f'Primer result could be found in {primer_result}')
-    log.info('Primer module Finished.')
-    return arg, other_args
-
-
-if __name__ == '__main__':
-    primer_main()
+#!/usr/bin/python3
+
+import argparse
+import platform
+import re
+import subprocess
+from collections import defaultdict
+from io import StringIO
+from itertools import product as cartesian_product
+from os import cpu_count
+from pathlib import Path
+
+import numpy as np
+from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
+from Bio.SeqFeature import SeqFeature, FeatureLocation
+from Bio.Data.IUPACData import ambiguous_dna_values as ambiguous_data
+from Bio import SeqIO
+from primer3 import (calc_tm, calc_hairpin_tm, calc_homodimer_tm,
+                     calc_heterodimer_tm)
+
+from OGU import utils
+from OGU import evaluate
+from OGU.global_vars import log
+
+
+class Pair:
+    # save memory
+    __slots__ = ['left', 'right', 'delta_tm', 'coverage', 'start', 'end',
+                 'observed_res', 'tree_res', 'pd_terminal', 'entropy',
+                 'have_heterodimer', 'heterodimer_tm', 'pi', 'score',
+                 'length', 'gap_ratio']
+
+    _title = ('Score,AvgProductLength,StdEV,'
+              'MinProductLength,MaxProductLength,'
+              'Coverage,Observed_Res,Tree_Res,PD_terminal,Entropy,'
+              'LeftSeq,LeftTm,LeftAvgBitscore,LeftAvgMismatch,'
+              'RightSeq,RightTm,RightAvgBitscore,RightAvgMismatch,'
+              'DeltaTm,AlnStart,AlnEnd,AvgSeqStart,AvgSeqEnd')
+    _style = ('{:.2f},{:.0f},{:.0f},'
+              '{},{},'
+              '{:.2%},{:.2%},{:.6f},{:.6f},{:.6f},'
+              '{},{:.2f},{:.2f},{:.2f},'
+              '{},{:.2f},{:.2f},{:.2f},'
+              '{:.2f},{},{},{},{}')
+
+    def __init__(self, left, right, alignment):
+        rows, columns = alignment.shape
+        self.left = left
+        self.right = right
+        self.delta_tm = abs(self.left.tm - self.right.tm)
+        # get accurate length
+        a = len(self.left) / 2
+        b = len(self.right) / 2
+        common = left.mid_loc.keys() & right.mid_loc.keys()
+        lengths = [[key, ((right.mid_loc[key] - b) - (left.mid_loc[key] + a))
+                    ] for key in common]
+        lengths = {i[0]: int(i[1]) for i in lengths if i[1] > 0}
+        self.length = lengths
+        self.right.coverage = len(self.right.mid_loc) / rows
+        self.coverage = len(common) / rows
+        # pairs use mid_loc from BLAST as start/end
+        self.start = self.left.avg_mid_loc
+        self.end = self.right.avg_mid_loc
+        self.have_heterodimer = False
+        self.heterodimer_tm = 0.0
+        self.observed_res = 0.0
+        self.tree_res = 0.0
+        self.pd_terminal = 0.0
+        self.entropy = 0.0
+        self.pi = 0.0
+        self.gap_ratio = 0.0
+        self.score = self.get_score()
+
+    def __repr__(self):
+        return (
+            'Pair(score={:.2f}, product={:.0f}, start={}, end={}, left={}, '
+            'right={}, observerd_res={:.2%}, coverage={:.2%},'
+            'delta_tm={:.2f}, have_heterodimer={})'.format(
+                self.score, utils.safe_average(
+                    list(self.length.values())), self.start,
+                self.end, self.left.seq, self.right.seq, self.observed_res,
+                self.coverage, self.delta_tm, self.have_heterodimer))
+
+    def __str__(self):
+        return Pair._style.format(
+            self.score, utils.safe_average(list(self.length.values())),
+            np.std(list(self.length.values())), min(self.length.values()),
+            max(self.length.values()),
+            self.coverage, self.observed_res, self.tree_res,
+            self.pd_terminal, self.entropy,
+            self.left.seq, self.left.tm, self.left.avg_bitscore,
+            self.left.avg_mismatch,
+            self.right.seq, self.right.tm, self.right.avg_bitscore,
+            self.right.avg_mismatch,
+            self.delta_tm, self.left.start, self.right.end, self.start,
+            self.end)
+
+    def get_score(self):
+        # calculate score of given primer pairs. Suggestion only
+        # use score to filter primer pairs
+        return (utils.safe_average(list(self.length.values())) * 0.5
+                + self.coverage * 200
+                + len(self.left) * 10
+                + len(self.right) * 10
+                + self.observed_res * 100
+                + self.tree_res * 100 + self.entropy * 5
+                - int(self.have_heterodimer) * 10
+                - self.delta_tm * 5 - self.left.avg_mismatch * 10
+                - self.right.avg_mismatch * 10)
+
+    def add_info(self, alignment):
+        # put attributes that need heavy computation here for the final primer
+        # pairs in order to save CPU time
+        if not self.right.is_reverse_complement:
+            self.right = self.right.reverse_complement()
+        # include end base, use alignment loc for slice
+        subalign = alignment[:, self.left.start:self.right.end+1]
+        tmp = Path()
+        variance, _ = evaluate.get_resolution(subalign, tmp)
+        (self.gap_ratio, self.observed_res, self.entropy, self.pi,
+         _, _, self.pd_terminal) = variance[2:9]
+        self.heterodimer_tm = calc_ambiguous_seq(
+            calc_heterodimer_tm, self.left.seq, self.right.seq)
+        if max(self.heterodimer_tm, self.left.tm,
+               self.right.tm) == self.heterodimer_tm:
+            self.have_heterodimer = True
+        else:
+            self.have_heterodimer = False
+        self.get_score()
+        self.left.update_id()
+        self.right.update_id()
+        return self
+
+
+class PrimerWithInfo(SeqRecord):
+    # inherit from Bio.SeqRecord.SeqRecord
+    def __init__(self, seq='', quality=None, start=0, coverage=0,
+                 avg_bitscore=0, mid_loc=None, avg_mismatch=0, detail=0,
+                 is_reverse_complement=False):
+        # store str
+        super().__init__(Seq(seq.upper()))
+        self.sequence = str(self.seq)
+
+        # primer3.setGlobals seems have no effect on calcTm, use
+        # calc_ambiguous_seq
+        self.quality = self.letter_annotations['solexa_quality'] = quality
+        self.start = self.annotations['start'] = start
+        self.end = self.annotations['end'] = start + self.__len__() - 1
+        self.coverage = self.annotations['coverage'] = coverage
+        self.avg_bitscore = self.annotations['avg_bitscore'] = avg_bitscore
+        self.mid_loc = self.annotations['mid_loc'] = mid_loc
+        self.avg_mismatch = self.annotations['avg_mismatch'] = avg_mismatch
+        self.detail = self.annotations['detail'] = detail
+        self.is_reverse_complement = self.annotations[
+            'is_reverse_complement'] = False
+        self.description = self.annotations['description'] = ''
+        self.avg_mid_loc = 0
+        self.hairpin_tm = 0
+        self.homodimer_tm = 0
+        self.tm = 0
+        self.update_id()
+
+    def __getitem__(self, i):
+        # part of attribution do not change, others were reset
+        if isinstance(i, int):
+            i = slice(i, i + 1)
+        if isinstance(i, slice):
+            answer = PrimerWithInfo(seq=str(self.seq[i]),
+                                    quality=self.quality[i])
+            answer.annotations = dict(self.annotations.items())
+            return answer
+        else:
+            log.exception('Bad index.')
+            raise
+
+    def reverse_complement(self):
+        table = str.maketrans('ACGTMRWSYKVHDBXN', 'TGCAKYWSRMBDHVXN')
+        new_seq = str.translate(self.sequence, table)[::-1]
+        new_quality = self.quality[::-1]
+        # try to simplify??
+        return PrimerWithInfo(seq=new_seq, quality=new_quality,
+                              start=self.start, coverage=self.coverage,
+                              avg_bitscore=self.avg_bitscore,
+                              mid_loc=self.mid_loc,
+                              is_reverse_complement=True,
+                              detail=self.detail)
+
+    def update_id(self):
+        self.end = self.annotations['end'] = self.start + self.__len__() - 1
+        if self.mid_loc is not None and len(self.mid_loc) != 0:
+            self.avg_mid_loc = int(utils.safe_average(list(
+                self.mid_loc.values())))
+        self.id = ('AvgMidLocation({:.0f})-Tm({:.2f})-Coverage({:.2%})-'
+                   'AvgBitScore({:.2f})-Start({})-End({})'.format(
+            self.avg_mid_loc, self.tm, self.coverage,
+            self.avg_bitscore, self.start, self.end))
+
+
+def parse_args(arg_list=None):
+    arg = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description=primer_main.__doc__)
+    arg.add_argument('-aln', nargs='*', help='alignment files')
+    arg.add_argument('-aln_folder', default=None,
+                     help='folder of aligned files')
+    arg.add_argument('-out', help='output directory')
+    arg.add_argument('-ambiguous', dest='ambiguous_base_n', default=4, type=int,
+                     help='number of ambiguous bases')
+    arg.add_argument('-coverage', dest='coverage', default=0.5, type=float,
+                     help='minimal coverage of base and primer')
+    arg.add_argument('-mismatch', dest='mismatch', default=4, type=int,
+                     help='maximum mismatch bases in primer')
+    arg.add_argument('-pmin', dest='min_primer', default=20, type=int,
+                     help='minimum primer length')
+    arg.add_argument('-pmax', dest='max_primer', default=30, type=int,
+                     help='maximum primer length')
+    arg.add_argument('-res', dest='resolution', type=float, default=0.3,
+                     help='minimal resolution')
+    arg.add_argument('-topn', dest='top_n', type=int, default=1,
+                     help='keep n primers for each high variant region')
+    arg.add_argument('-amin', dest='min_product', default=300, type=int,
+                     help='minimum amplified length (include primer)')
+    arg.add_argument('-amax', dest='max_product', default=800, type=int,
+                     help='maximum amplified length (include primer)')
+    arg.add_argument('-size', type=int, default=500, help='window size for sliding scan')
+    arg.add_argument('-step', type=int, default=50, help='step length for sliding scan')
+    arg.add_argument('-primer', action='store_true', help='design universal primer')
+    if arg_list is None:
+        return arg.parse_known_args()
+    else:
+        return arg.parse_known_args(arg_list)
+
+
+def init_arg(arg):
+    arg = utils.init_out(arg)
+    if all([arg.aln, arg.aln_folder]):
+        log.info('Do not recommend to use "-aln" and "-aln_folder" '
+                 'at same time!')
+    if arg.aln is not None:
+        arg.aln = [Path(i).absolute() for i in arg.aln]
+    else:
+        arg.aln = []
+    if arg.aln_folder is not None:
+        for i in Path(arg.aln_folder).glob('*'):
+            arg.aln.append(i.absolute())
+    log.info('Add aligned files from evaluate module if possible.')
+    for i in Path(arg._align).glob('*'):
+        arg.aln.append(i.absolute())
+    for i in arg.aln:
+        if not i.exists() or not i.is_file():
+            log.error(f'{i} does not exist or is not a valid file.')
+            return None
+    if not any([arg.aln, arg.aln_folder]):
+        log.warning('Empty input.')
+        return None
+    return arg
+
+
+def calc_ambiguous_seq(func, seq, seq2=None):
+    """
+    Expand sequences with ambiguous bases to several clean sequences and apply
+    func to every sequence.
+    Return average value. Return 0 if len(seq) > 60 (from primer3)
+    """
+    # Seems primer3 only accept seqs shorter than 60 bp. Plus, too long seq
+    # will cost too much memory.
+    len_limit = 60
+
+    def _expand(seq):
+        seq_list = []
+        for base in seq:
+            # replace illegal base with 'N'
+            if base not in ambiguous_data:
+                base = 'N'
+            seq_list.append(ambiguous_data[base])
+        seq_product = list(cartesian_product(*seq_list))
+        seq_str = [''.join(i) for i in seq_product]
+        return seq_str
+
+    if len(seq) > len_limit:
+        log.warning('Too many ambiguous bases. Skip')
+        return 0
+    seq_str = _expand(seq)
+    if seq2 is None:
+        values = [func(i) for i in seq_str]
+    else:
+        if len(seq2) > len_limit:
+            log.warning('Too many ambiguous bases. Skip')
+            return 0
+        seq_str2 = _expand(seq2)
+        products = cartesian_product(seq_str, seq_str2)
+        values = [func(i[0], i[1]) for i in products]
+    # primer3 will return negative values sometime
+    values_positive = [max(0, i) for i in values]
+    return utils.safe_average(values_positive)
+
+
+def count_base(alignment: np.array):
+    """
+    Given alignment numpy array, count cumulative frequency of base in each
+    column (consider ambiguous base and "N", "-" and "?", otherwise omit).
+    Return [[float, float, float, float, float, float, float]] for
+    [A, T, C, G, N, GAP, OTHER].
+    """
+    frequency = []
+    rows, columns = alignment.shape
+    for index in range(columns):
+        base, counts = np.unique(alignment[:, [index]], return_counts=True)
+        count_dict = {b'A': 0, b'C': 0, b'G': 0, b'T': 0, b'M': 0, b'R': 0,
+                      b'W': 0, b'S': 0, b'Y': 0, b'K': 0, b'V': 0, b'H': 0,
+                      b'D': 0, b'B': 0, b'X': 0, b'N': 0, b'-': 0, b'?': 0}
+        count_dict.update(dict(zip(base, counts)))
+        a = (count_dict[b'A'] +
+             (count_dict[b'D'] + count_dict[b'H'] + count_dict[b'V']) / 3 +
+             (count_dict[b'M'] + count_dict[b'R'] + count_dict[b'W']) / 2)
+        t = (count_dict[b'T'] +
+             (count_dict[b'B'] + count_dict[b'H'] + count_dict[b'D']) / 3 +
+             (count_dict[b'K'] + count_dict[b'W'] + count_dict[b'Y']) / 2)
+        c = (count_dict[b'C'] +
+             (count_dict[b'B'] + count_dict[b'H'] + count_dict[b'V']) / 3 +
+             (count_dict[b'M'] + count_dict[b'S'] + count_dict[b'Y']) / 2)
+        g = (count_dict[b'G'] +
+             (count_dict[b'B'] + count_dict[b'D'] + count_dict[b'V']) / 3 +
+             (count_dict[b'K'] + count_dict[b'R'] + count_dict[b'S']) / 2)
+        gap = count_dict[b'-']
+        n = count_dict[b'N'] + count_dict[b'X'] + count_dict[b'?']
+        other = rows - a - t - c - g - gap - n
+        frequency.append([a, t, c, g, n, gap, other])
+    return frequency
+
+
+def get_quality(data, rows):
+    """
+    Calculate quality score.
+    """
+    # use fastq-illumina format
+    max_q = 62
+    factor = max_q / rows
+    # use min to avoid KeyError
+    quality_value = [min(max_q, int(i * factor)) - 1 for i in data]
+    return quality_value
+
+
+def get_consensus(base_cumulative_frequency, coverage_percent: float,
+                  rows: int, output: Path):
+    """
+    Given count info of bases, return consensus(PrimerWithInfo).
+    """
+    def get_ambiguous_dict():
+        data = dict(zip(ambiguous_data.values(), ambiguous_data.keys()))
+        # 2:{'AC': 'M',}
+        data_with_len = defaultdict(lambda: dict())
+        for i in data:
+            data_with_len[len(i)][i] = data[i]
+        return data_with_len
+
+    ambiguous_dict = get_ambiguous_dict()
+    most = []
+    coverage = rows * coverage_percent
+
+    limit = coverage / len('ATCG')
+    for location, column in enumerate(base_cumulative_frequency):
+        finish = False
+        # "*" for others
+        value = dict(zip(list('ATCGN-*'), column))
+
+        base = 'N'
+        if value['N'] >= limit:
+            count = value['N']
+            most.append([location, base, count])
+            continue
+        sum_gap = value['-'] + value['*']
+        if sum_gap >= limit:
+            base = '-'
+            count = sum_gap
+            most.append([location, base, count])
+            continue
+        # 1 2 3 4
+        for length in ambiguous_dict:
+            # A T CG CT ACG CTG ATCG
+            for key in ambiguous_dict[length]:
+                count = 0
+                for letter in list(key):
+                    if finish:
+                        break
+                    count += value[letter]
+                    if count >= coverage:
+                        base = ambiguous_dict[length][key]
+                        finish = True
+                        most.append([location, base, count])
+    quality_raw = [i[2] for i in most]
+    consensus = PrimerWithInfo(start=1, seq=''.join([i[1] for i in most]),
+                               quality=get_quality(quality_raw, rows))
+    SeqIO.write(consensus, output, 'fastq')
+    return consensus
+
+
+def get_good_region(index, seq_count, arg):
+    """
+    Return regions marked for finding primers. Because of alignment gap, PCR
+    product may smaller than given length limitation.
+    """
+    n = arg.max_product - arg.min_product
+    good_region = set()
+    for i, j in zip(index, seq_count):
+        if j >= arg.resolution:
+            good_region.update(range(i - arg.max_primer, i - n))
+            good_region.update(range(i + arg.min_product,
+                                     i - arg.max_primer + arg.max_product))
+    return good_region
+
+
+def find_continuous(consensus, good_region, min_len):
+    """
+    Given PrimerWithInfo, good_region, min_len
+    Return consensus with features.
+    """
+    skip = ('N', '-')
+    start = 0
+    for index, base in enumerate(consensus.sequence[:-min_len]):
+        if base in skip or index not in good_region:
+            if (index - start) >= min_len:
+                consensus.features.append(SeqFeature(FeatureLocation(
+                    start, index, strand=1), type='continuous'))
+            start = index + 1
+    return consensus
+
+
+def find_primer(consensus, arg):
+    """
+    Find suitable primer in given consensus with features labeled as candidate
+    primer, return list of PrimerWithInfo, consensus.
+    """
+    # repeat no more than 5 times
+    poly = re.compile(r'([ATCG])\1\1\1\1')
+    tandem = re.compile(r'([ATCG]{2})\1\1\1\1')
+
+    def is_good_primer(primer):
+        # use re and primer3 to check weather it's good primer
+        # ref1. http://www.premierbiosoft.com/tech_notes/PCR_Primer_Design.html
+        ambiguous_base = len(primer)
+        for i in list('ATCG'):
+            ambiguous_base -= primer.seq.count(i)
+        if ambiguous_base > max_ambiguous:
+            return False
+        if re.search(poly, str(primer.seq)) is not None:
+            primer.detail = 'Poly(NNNNN) structure found'
+            return False
+        if re.search(tandem, str(primer.seq)) is not None:
+            primer.detail = 'Tandom(NN*5) exist'
+            return False
+        primer.hairpin_tm = calc_ambiguous_seq(calc_hairpin_tm, primer.seq)
+        primer.tm = primer.annotations['tm'] = calc_ambiguous_seq(calc_tm,
+                                                                  primer.seq)
+        # primer3.calcHairpin or calcHomodimer usually return structure found
+        # with low Tm. Here we compare structure_tm with sequence tm
+        if primer.hairpin_tm >= primer.tm:
+            primer.detail = 'Hairpin found'
+            return False
+        primer.homodimer_tm = calc_ambiguous_seq(calc_homodimer_tm, primer.seq)
+        if primer.homodimer_tm >= primer.tm:
+            primer.detail = 'Homodimer found'
+            return False
+        return True
+
+    primers = []
+    min_len = arg.min_primer
+    max_len = arg.max_primer
+    max_ambiguous = arg.ambiguous_base_n
+    # skip good_region
+    continuous = consensus.features
+    for feature in continuous:
+        fragment = feature.extract(consensus)
+        len_fragment = len(fragment)
+        for begin in range(len_fragment - max_len):
+            for p_len in range(min_len, max_len + 1):
+                start = feature.location.start + begin
+                primer = consensus[start:start + p_len]
+                if is_good_primer(primer):
+                    consensus.features.append(SeqFeature(
+                        FeatureLocation(start, start + p_len, strand=1),
+                        type='primer'))
+                    primer.start = start
+                    primer.update_id()
+                    primers.append(primer)
+    return primers, consensus
+
+
+def old_remove_gap(aln_fasta: Path, new_file: Path) -> Path:
+    # to be removed
+    """
+    old function, for BLAST
+    Args:
+        aln_fasta: fasta with gap
+        new_file: fasta without gap
+    Returns:
+        new_file: fasta without gap
+    """
+    no_gap = StringIO()
+    with open(aln_fasta, 'r', encoding='utf-8') as raw:
+        for line in raw:
+            no_gap.write(line.replace('-', ''))
+    # try to avoid makeblastdb error
+    no_gap.seek(0)
+    SeqIO.convert(no_gap, 'fasta', new_file, 'fasta')
+    no_gap.close()
+    return new_file
+
+
+def validate(primer_candidate: list, aln: Path, n_seqs: int, arg):
+    """
+    Do BLAST. Parse BLAST result. Return list of PrimerWithInfo which passed
+    the validation.
+    """
+    evalue = 1e-2
+    _, blast = utils.get_blast()
+    if not _:
+        log.critical('Cannot find BLAST.')
+        return []
+    locus_name = aln.stem
+    # chmod +x
+    if platform.system() == 'Windows':
+        makeblastdb = Path(blast).parent / 'makeblastdb.exe'
+    else:
+        makeblastdb = Path(blast).parent / 'makeblastdb'
+        makeblastdb.chmod(0o755)
+    query_file = arg._primer / (locus_name+'.candidate.fasta')
+    query_file_fastq = arg._primer / (locus_name+'.candidate.fastq')
+    # SeqIO.write fasta file directly is prohibited. have to write fastq at
+    # first.
+    with open(query_file_fastq, 'w', encoding='utf-8') as _:
+        SeqIO.write(primer_candidate, _, 'fastq')
+    SeqIO.convert(query_file_fastq, 'fastq', query_file, 'fasta')
+    # build blast db
+    db_file = old_remove_gap(aln, arg._tmp/(locus_name+'-db_file.fasta'))
+    # db_file = utils.move(aln, arg._tmp/(locus_name+'-db_file.fasta'), copy=True)
+    _ = subprocess.run(f'{makeblastdb} -in {db_file} -dbtype nucl '
+                       f'-out {db_file}', shell=True,
+                       stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    if _.returncode != 0:
+        log.critical('Failed to run makeblastdb. Skip BLAST.')
+        return []
+    # BLAST
+    blast_result_file = arg._tmp / (locus_name+'-blast.result.tsv')
+    fmt = '7 qseqid sseqid qseq nident mismatch score qstart qend sstart send'
+    cmd = (f'{blast} -task blastn-short -num_threads {max(1, cpu_count()-1)} '
+           f'-query {query_file} -db {db_file} -evalue {evalue} -max_hsps 1 '
+           f'-outfmt "{fmt}" -out {blast_result_file}')
+    # hide output
+    _ = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL,
+                       stderr=subprocess.DEVNULL)
+    if _.returncode != 0:
+        log.critical('Failed to run BLAST.')
+        return []
+    log.info('BLAST finished.')
+    log.info('Parsing BLAST result.')
+    blast_result = dict()
+    # because SearchIO.parse is slow, use parse_blast_result()
+    for query in utils.parse_blast_tab(blast_result_file):
+        if len(query) == 0:
+            continue
+        sum_bitscore_raw = 0
+        sum_mismatch = 0
+        good_hits = 0
+        mid_loc = dict()
+        hit = query[0]
+        for hit in query:
+            min_positive = len(hit.query_seq) - arg.mismatch
+            hsp_bitscore_raw = hit.bitscore_raw
+            positive = hit.ident_num
+            mismatch = hit.mismatch_num
+            loc = utils.safe_average([hit.hit_start, hit.hit_end])
+            if positive >= min_positive and mismatch <= arg.mismatch:
+                sum_bitscore_raw += hsp_bitscore_raw
+                sum_mismatch += mismatch
+                good_hits += 1
+                # middle location of primer, the difference of two mid_loc
+                # approximately equals to the length of amplified fragment.
+                mid_loc[hit.hit_id] = loc
+        coverage = good_hits / n_seqs
+        if coverage >= arg.coverage:
+            blast_result[hit.query_id] = {
+                'coverage': coverage,
+                'avg_bitscore': sum_bitscore_raw / good_hits,
+                'avg_mismatch': sum_mismatch / good_hits,
+                'mid_loc': mid_loc}
+    primer_verified = []
+    for primer in primer_candidate:
+        i = primer.id
+        if i in blast_result:
+            primer.coverage = blast_result[i]['coverage']
+            primer.avg_bitscore = blast_result[i]['avg_bitscore']
+            primer.mid_loc = blast_result[i]['mid_loc']
+            primer.avg_mismatch = blast_result[i]['avg_mismatch']
+            primer.update_id()
+            primer_verified.append(primer)
+    primer_verified.sort(key=lambda x: x.start)
+    # clean
+    utils.clean_tmp(db_file)
+    blast_result_file.unlink()
+    log.info('Parse finished.')
+    return primer_verified
+
+
+def pick_pair(primers, alignment, arg):
+    """
+    Pick primer pairs passed the validation and its product length fulfill the
+    requirement.
+    """
+    pairs = []
+    for n_left, left in enumerate(primers):
+        # convert mid_loc to 5' location
+        # use int to speedup, comparing of float seems slow
+        location = int(left.avg_mid_loc - len(left) / 2)
+        begin = location + arg.min_product
+        # fragment plus one primer = max_product length
+        end = location + arg.max_product - len(left)
+        # create [] is faster than list()
+        cluster = []
+        for right in primers[(n_left + 1):]:
+            if right.avg_mid_loc < begin:
+                continue
+            if right.avg_mid_loc > end:
+                break
+            pair = Pair(left, right, alignment)
+            if pair.coverage < arg.coverage:
+                continue
+            cluster.append(pair)
+        cluster.sort(key=lambda x: x.score, reverse=True)
+        # only keep top n for each primer cluster
+        pairs.extend(cluster[:arg.top_n])
+    if len(pairs) == 0:
+        return []
+    # remove close located primers
+    less_pairs = []
+    cluster = [pairs[0], ]
+    pairs.sort(key=lambda x: x.start)
+    for index in range(1, len(pairs)):
+        if pairs[index].start - pairs[index - 1].start < arg.min_primer:
+            cluster.append(pairs[index])
+        else:
+            cluster.sort(key=lambda x: x.score, reverse=True)
+            less_pairs.extend(cluster[:arg.top_n])
+            cluster = []
+    cluster.sort(key=lambda x: x.score, reverse=True)
+    less_pairs.extend(cluster[:arg.top_n])
+    log.info('{} pairs of redundant primers were removed.'.format(
+        len(pairs) - len(less_pairs)))
+    good_pairs = []
+    for i in less_pairs:
+        i.add_info(alignment)
+        if i.observed_res >= arg.resolution:
+            good_pairs.append(i)
+    good_pairs.sort(key=lambda x: x.score, reverse=True)
+    log.info('Successfully found validated primers.')
+    return good_pairs[:arg.top_n]
+
+
+def get_observed_res(alignment: np.array, arg):
+    """
+    For primer design.
+    Observed resolution used as lower bound.
+    Args:
+        alignment:
+        arg:
+    Returns:
+        index: list
+        observed_res_list: list
+    """
+    index = []
+    observed_res_list = []
+    rows, columns = alignment.shape
+    for i in range(0, columns, arg.step):
+        subalign = alignment[:, i:i+arg.size]
+        sub_rows, sub_columns = subalign.shape
+        item, count = np.unique(subalign, return_counts=True, axis=0)
+        observed_res = len(count) / sub_rows
+        index.append(i)
+        observed_res_list.append(observed_res)
+    return index, observed_res_list
+
+
+def primer_design(aln: Path, result: Path, arg):
+    locus_name = aln.stem
+    name, alignment, = evaluate.fasta_to_array(aln)
+    if name is None:
+        log.debug(f'Invalid alignment file {aln}.')
+        return False
+    rows, columns = alignment.shape
+    # generate consensus
+    base_cumulative_frequency = count_base(alignment)
+    log.info(f'Generate consensus of {aln}.')
+    consensus = get_consensus(base_cumulative_frequency, arg.coverage, rows,
+                              arg._align/(locus_name+'-consensus.fastq'))
+    log.info(f'Evaluate whole alignment of {aln}.')
+    # a_ : alignment
+    item, count = np.unique(alignment, return_counts=True, axis=0)
+    observed_res = len(count) / rows
+    if observed_res < arg.resolution:
+        log.error('Observed resolution is too low.')
+        return False
+    log.info('Start the sliding-window scan.')
+    index, observed_res_list = get_observed_res(alignment, arg)
+    log.info('Evaluation finished.')
+    log.info('Start finding primers.')
+    log.info('Mark region for finding primer.')
+    good_region = get_good_region(index, observed_res_list, arg)
+    log.info('Finding candidate primers.')
+    consensus = find_continuous(consensus, good_region, arg.min_primer)
+    primer_candidate, consensus = find_primer(consensus, arg)
+    if len(primer_candidate) == 0:
+        log.warning('Cannot find primer candidates. '
+                    'Please consider to loose options.')
+        return True
+    log.info(f'Found {len(primer_candidate)} candidate primers.')
+    log.info('Validate with BLAST. May be slow.')
+    primer_verified = validate(primer_candidate, aln, rows, arg)
+    if len(primer_verified) == 0:
+        log.warning('All candidates failed on validation. '
+                    'Please consider to loose options.')
+        return True
+    log.info('Picking primer pairs.')
+    pairs = pick_pair(primer_verified, alignment, arg)
+    if len(pairs) == 0:
+        log.warning('Cannot find suitable primer pairs. '
+                    'Please consider to loose options.')
+        return True
+    log.info('Output the result.')
+    out1 = open(arg._primer/(locus_name+'.primer.fastq'), 'w', encoding='utf-8')
+    out2 = open(arg._primer/(locus_name+'.primer.csv'), 'w', encoding='utf-8')
+    # write primers to one file
+    out3 = open(result, 'a', encoding='utf-8')
+    csv_title = 'Locus,Samples,' + Pair._title + '\n'
+    out2.write(csv_title)
+    for pair in pairs:
+        line = f'{locus_name},{rows},{str(pair)}\n'
+        out2.write(line)
+        out3.write(line)
+        SeqIO.write(pair.left, out1, 'fastq')
+        SeqIO.write(pair.right, out1, 'fastq')
+    out1.close()
+    out2.close()
+    out3.close()
+    # log.info(f'Primers info were written into {out2}')
+    return True
+
+
+def primer_main(arg_str=None):
+    """
+    Evaluate variance of alignments.
+    """
+    utils.check_system()
+    utils.get_all_third_party(skip_blast=False)
+    if arg_str is None:
+        arg, other_args = parse_args()
+    else:
+        arg, other_args = parse_args(arg_str.split(' '))
+    if not arg.primer and __name__ != '__main__':
+        log.info('Skip primer module.')
+        return None, None
+    log.info('Running primer module...')
+    arg = init_arg(arg)
+    if arg is None:
+        log.info('Quit primer module.')
+        return None, None
+    utils.add_file_log(arg)
+    primer_result = arg.out / 'Primers.csv'
+    csv_title = 'Locus,Samples,' + Pair._title + '\n'
+    with open(primer_result, 'w', encoding='utf-8') as out:
+        out.write(csv_title)
+    if arg is None:
+        log.info('Quit.')
+        return None, None
+    for aln in arg.aln:
+        primer_design(aln, primer_result, arg)
+
+    log.info(f'Primer result could be found in {primer_result}')
+    log.info('Primer module Finished.')
+    return arg, other_args
+
+
+if __name__ == '__main__':
+    primer_main()
```

### Comparing `ogu-1.52/src/OGU/ui.py` & `ogu-1.54/src/OGU/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1426 +1,1427 @@
-#!/usr/bin/env python
-from logging import handlers
-from pkg_resources import resource_filename
-from time import time
-from tkinter import filedialog, messagebox, scrolledtext
-import logging
-import platform
-import queue
-import sys
-import threading
-import tkinter as tk
-import tkinter.ttk as ttk
-import webbrowser
-
-from OGU.evaluate import evaluate_main
-from OGU.gb2fasta import gb2fasta_main
-from OGU.global_vars import log, name, FMT, DATEFMT
-from OGU.primer import primer_main
-from OGU.utils import font_family, get_all_third_party
-
-
-def my_labelframe(parent: tk.LabelFrame) -> tk.LabelFrame:
-    frame = tk.LabelFrame(parent)
-    frame.configure(background="#edf0f3")
-    frame.configure(cursor="fleur")
-    frame.configure(font=f'-family {font_family} -size 14')
-    frame.configure(foreground="#000000")
-    frame.configure(highlightbackground="#edf0f3")
-    frame.configure(highlightcolor="black")
-    frame.configure(relief='groove')
-    return frame
-
-
-def my_label(frame: tk.LabelFrame, fontsize=11) -> tk.Label:
-    label = tk.Label(frame)
-    label.configure(activebackground="#f9f9f9")
-    label.configure(activeforeground="black")
-    label.configure(anchor='w')
-    label.configure(background="#edf0f3")
-    label.configure(compound='left')
-    label.configure(foreground="#000000")
-    label.configure(highlightbackground="#edf0f3")
-    label.configure(highlightcolor="black")
-    label.configure(justify='left')
-    label.configure(font=f'-family {font_family} -size {fontsize}')
-    return label
-
-
-def my_button(frame: tk.LabelFrame, fontsize=12) -> tk.Button:
-    button = tk.Button(frame)
-    button.configure(compound='left')
-    button.configure(activebackground="#ececec")
-    button.configure(activeforeground="#000000")
-    button.configure(background="#edf0f3")
-    button.configure(font=f"-family {font_family} -size {fontsize}")
-    button.configure(foreground="#000000")
-    button.configure(highlightbackground="#edf0f3")
-    button.configure(highlightcolor="black")
-    button.configure(pady="0")
-    button.configure(relief="raised")
-    button.configure(borderwidth=1)
-    return button
-
-
-def my_checkbutton(frame: tk.LabelFrame, fontsize=11) -> tk.Checkbutton:
-    check_b = tk.Checkbutton(frame)
-    check_b.configure(activebackground="#ececec")
-    check_b.configure(activeforeground="#000000")
-    check_b.configure(anchor='w')
-    check_b.configure(background="#edf0f3")
-    check_b.configure(compound='left')
-    check_b.configure(foreground="#000000")
-    check_b.configure(highlightbackground="#edf0f3")
-    check_b.configure(highlightcolor="black")
-    check_b.configure(justify='left')
-    check_b.configure(selectcolor="#ffffff")
-    check_b.configure(font=f'-family {font_family} -size {fontsize}')
-    return check_b
-
-
-def my_entry(frame: tk.LabelFrame, fontsize=11) -> tk.Entry:
-    entry = tk.Entry(frame)
-    entry.configure(font=f'-family {font_family} -size {fontsize}')
-    entry.configure(takefocus="")
-    entry.configure(cursor="fleur")
-    return entry
-
-
-def my_combobox(frame: tk.LabelFrame, fontsize=11) -> ttk.Combobox:
-    style = 'combostyle'
-    combo_style = ttk.Style()
-    if style not in ttk.Style().theme_names():
-        combo_style.theme_create(style, parent='alt', settings={
-            'TCombobox': {'configure': {
-                'selectbackground': 'gray',
-                'fieldbackground': 'white',
-                'background': 'white'}}})
-    combo_style.theme_use(style)
-    combobox = ttk.Combobox(frame, font=(font_family, fontsize))
-    combobox.configure(state='readonly')
-    combobox.configure(takefocus="")
-    return combobox
-
-
-def move_to_center(window: tk.Tk, width: int, height: int) -> None:
-    screen_width = root.winfo_screenwidth()
-    screen_height = root.winfo_screenheight()
-    x = (screen_width - width) // 2
-    y = (screen_height - height) // 2
-    window.geometry(f'{width}x{height}+{x}+{y}')
-    return
-
-
-def after_close(frame):
-    """
-    Deiconify root before destroy.
-    """
-
-    def func():
-        root.deiconify()
-        frame.destroy()
-
-    return func
-
-
-def scroll_text(window):
-    """
-    ScrolledText that shows logs.
-    """
-
-    def poll():
-        while True:
-            try:
-                msg = log_queue.get(block=False)
-                level = msg.levelname
-                msg = formatter.format(msg) + '\n'
-                scroll.insert('end', msg, level)
-                scroll.yview('end')
-            except queue.Empty:
-                break
-        # to avoid orphan poll()
-        if log.hasHandlers():
-            scroll.after(10, poll)
-        else:
-            return
-
-    # clean old handlers
-    for i in log.handlers:
-        log.removeHandler(i)
-    log_queue = queue.Queue()
-    formatter = logging.Formatter(fmt=FMT, datefmt=DATEFMT)
-    # do not add formatter to queuehandler, or msg will be formatted twice
-    queue_handler = handlers.QueueHandler(log_queue)
-    # give poll() time to quit
-    root.after(100, log.addHandler(queue_handler))
-    scroll = scrolledtext.ScrolledText(window)
-    scroll.tag_config('INFO', foreground='black')
-    scroll.tag_config('WARNING', foreground='orange')
-    scroll.tag_config('ERROR', foreground='red')
-    scroll.tag_config('CRITICAL', foreground='red')
-    scroll.tag_config('EXCEPTION', foreground='red')
-    scroll.pack(fill='both')
-    scroll.after(0, poll)
-
-
-def thread_wrap(function, arg_str, window, no_arg=False):
-    """
-    Wrap for callback.
-    Args:
-        function(callable): function to call
-        arg_str(str): string for function's argparse
-        window(Toplevel): window to hide
-        no_arg: function do not need args
-    """
-    try:
-        if not no_arg:
-            result = function(arg_str)
-        else:
-            result = function()
-    except Exception as e:
-        log.exception(str(e))
-        log.exception('Abort.')
-        messagebox.showinfo(message='Abort.')
-        root.deiconify()
-        return
-    if not no_arg:
-        messagebox.showinfo(message=f'Done. See {result[0].out} for details.')
-    else:
-        messagebox.showinfo(message='Install third-party software finished.')
-    window.withdraw()
-    root.deiconify()
-    return
-
-
-def open_file(entry, single=True, type_='file', entry2=None, title=''):
-    """
-    Set title, fill entry 1, empty entry 2.
-    """
-
-    def func():
-        if type_ != 'file':
-            a = filedialog.askdirectory(title=title)
-        else:
-            if single:
-                a = filedialog.askopenfilename(title=title)
-            else:
-                a = filedialog.askopenfilenames(title=title)
-        entry.delete(0, 'end')
-        entry.insert(0, a)
-        if entry2 is not None:
-            entry2.delete(0, 'end')
-
-    return func
-
-
-class Root:
-    def __init__(self, top=None):
-        '''This class configures and populates the toplevel window.
-           top is the toplevel containing window.'''
-        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
-        _fgcolor = '#000000'  # X11 color: 'black'
-        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
-        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
-        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
-        _tabfg1 = 'black'
-        _tabfg2 = 'black'
-        _tabbg1 = 'grey75'
-        _tabbg2 = 'grey89'
-        _bgmode = 'light'
-
-        photo_location1 = resource_filename(name, 'data/button1.png')
-        photo_location2 = resource_filename(name, 'data/button2.png')
-        photo_location3 = resource_filename(name, 'data/button3.png')
-        photo_location4 = resource_filename(name, 'data/button4.png')
-        global _img4
-        _img4 = tk.PhotoImage(file=photo_location4)
-        global _img0
-        _img0 = tk.PhotoImage(file=photo_location1)
-        global _img1
-        _img1 = tk.PhotoImage(file=photo_location2)
-        global _img2
-        _img2 = tk.PhotoImage(file=photo_location3)
-
-        top.geometry("800x450+400+0")
-        move_to_center(top, 800, 450)
-        top.minsize(120, 15)
-        top.resizable(1, 1)
-        top.title(name)
-        top.configure(background="#edf0f3")
-        top.configure(highlightbackground="#edf0f3")
-        top.configure(highlightcolor="black")
-        self.top = top
-
-        self.help_b = my_button(self.top)
-        self.help_b.place(relx=0.913, rely=0.067, height=40, width=40)
-        self.help_b.configure(command=run_help)
-        self.help_b.configure(image=_img4)
-
-        self.gb2fasta_b = my_button(self.top)
-        self.gb2fasta_b.place(relx=0.188, rely=0.288, height=100, width=100)
-        self.gb2fasta_b.configure(command=ui_gb2fasta)
-        self.gb2fasta_b.configure(image=_img0)
-
-        self.evaluate_b = my_button(self.top)
-        self.evaluate_b.place(relx=0.438, rely=0.288, height=100, width=100)
-        self.evaluate_b.configure(command=ui_evaluate)
-        self.evaluate_b.configure(image=_img1)
-
-        self.primer_b = my_button(self.top)
-        self.primer_b.place(relx=0.688, rely=0.288, height=100, width=100)
-        self.primer_b.configure(command=ui_primer)
-        self.primer_b.configure(image=_img2)
-
-        self.install_third_party = my_button(self.top)
-        self.install_third_party.place(relx=0.613, rely=0.865, height=30,
-                                       width=250)
-        self.install_third_party.configure(text='Install third-party software')
-        self.install_third_party.configure(command=run_install(self, self.top))
-
-        self.gb2fasta_label = my_label(self.top, 14)
-        self.gb2fasta_label.place(relx=0.188, rely=0.532, height=30, width=100)
-        self.gb2fasta_label.configure(text='''GB2Fasta''')
-
-        self.evaluate_label = my_label(self.top, 14)
-        self.evaluate_label.place(relx=0.45, rely=0.532, height=30, width=100)
-        self.evaluate_label.configure(text='''Evaluate''')
-
-        self.primer_label = my_label(self.top, 14)
-        self.primer_label.place(relx=0.713, rely=0.532, height=30, width=100)
-        self.primer_label.configure(text='''Primer''')
-
-        self.note_label = my_label(self.top, 14)
-        self.note_label.place(relx=0.35, rely=0.643, height=35, width=300)
-        self.note_label.configure(text='''Click button to run modules''')
-
-
-class GB2Fasta:
-    def __init__(self, top=None):
-        '''This class configures and populates the toplevel window.
-           top is the toplevel containing window.'''
-        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
-        _fgcolor = '#000000'  # X11 color: 'black'
-        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
-        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
-        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
-        _tabfg1 = 'black'
-        _tabfg2 = 'black'
-        _tabbg1 = 'grey75'
-        _tabbg2 = 'grey89'
-        _bgmode = 'light'
-        self.style = ttk.Style()
-        if sys.platform == "win32":
-            self.style.theme_use('winnative')
-        self.style.configure('.', background=_bgcolor)
-        self.style.configure('.', foreground=_fgcolor)
-        self.style.map('.', background=[('selected', _compcolor),
-                                        ('active', _ana2color)])
-        self.tooltip_font = "TkDefaultFont"
-
-        top.geometry("600x800+5+139")
-        move_to_center(top, 600, 800)
-        top.title("GB2Fasta")
-        top.configure(background="#edf0f3")
-        top.configure(highlightbackground="#edf0f3")
-        top.configure(highlightcolor="black")
-
-        self.top = top
-        self.gb = tk.StringVar()
-        self.gene = tk.StringVar()
-        self.molecular = tk.StringVar()
-        self.group = tk.StringVar()
-        self.og = tk.StringVar()
-        self.refseq = tk.StringVar()
-        self.count = tk.StringVar()
-        self.min_len = tk.StringVar()
-        self.max_len = tk.StringVar()
-        self.date_start = tk.StringVar()
-        self.date_end = tk.StringVar()
-        self.exclude = tk.StringVar()
-        self.query = tk.StringVar()
-        self.taxon = tk.StringVar()
-        self.out = tk.StringVar()
-        self.expand = tk.StringVar()
-        self.max_name_len = tk.StringVar()
-        self.max_gene_len = tk.StringVar()
-        self.unique = tk.StringVar()
-        self.allow_repeat = tk.IntVar()
-        self.allow_invert_repeat = tk.IntVar()
-        self.allow_mosaic_repeat = tk.IntVar()
-        self.no_divide = tk.IntVar()
-        self.rename = tk.IntVar()
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.025, rely=0.013, relheight=0.46
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Input''')
-
-        self.TSeparator1 = ttk.Separator(self.Labelframe1)
-        self.TSeparator1.place(relx=0.524, rely=0.19, relheight=0.541
-                               , bordermode='ignore')
-        self.TSeparator1.configure(orient="vertical")
-
-        self.gbfile_label = my_label(self.Labelframe1)
-        self.gbfile_label.place(relx=0.050, rely=0.057, height=35, width=100,
-                                bordermode='ignore')
-        self.gbfile_label.configure(text='''Genbank files''')
-
-        self.gb_entry = my_entry(self.Labelframe1)
-        self.gb_entry.place(relx=0.241, rely=0.057, relheight=0.095,
-                            relwidth=0.562, bordermode='ignore')
-        self.gb_entry.configure(textvariable=self.gb)
-        self.gb_entry_tooltip = ToolTip(self.gb_entry, self.tooltip_font,
-                                        '''gb format files''')
-
-        self.gb_file_b = my_button(self.Labelframe1, 12)
-        self.gb_file_b.place(relx=0.82, rely=0.054, height=35, width=90
-                             , bordermode='ignore')
-        self.gb_file_b.configure(command=open_file(self.gb_entry, single=False))
-        self.gb_file_b.configure(text='''Open''')
-
-        self.gene_label = my_label(self.Labelframe1)
-        self.gene_label.place(relx=0.035, rely=0.217, height=35, width=60,
-                              bordermode='ignore')
-        self.gene_label.configure(text='''Gene''')
-
-        self.gene_entry = my_entry(self.Labelframe1)
-        self.gene_entry.place(relx=0.201, rely=0.217, height=35,
-                              relwidth=0.314, bordermode='ignore')
-        self.gene_entry.configure(textvariable=self.gene)
-        self.gene_entry_tooltip = ToolTip(self.gene_entry, self.tooltip_font,
-                                          'gene name')
-
-        self.taxon_label = my_label(self.Labelframe1)
-        self.taxon_label.place(relx=0.035, rely=0.326, height=35, width=70
-                               , bordermode='ignore')
-        self.taxon_label.configure(text='''Taxonomy''')
-
-        self.molecular_label = my_label(self.Labelframe1)
-        self.molecular_label.place(relx=0.558, rely=0.217, height=35, width=80
-                                   , bordermode='ignore')
-        self.molecular_label.configure(text='''Molecular''')
-
-        self.TCombobox_molecular = my_combobox(self.Labelframe1)
-        self.TCombobox_molecular.place(relx=0.716, rely=0.217, height=35,
-                                       width=150, bordermode='ignore')
-        self.molecular_value_list = ['all', 'DNA', 'RNA', ]
-        self.TCombobox_molecular.configure(values=self.molecular_value_list)
-        self.TCombobox_molecular.configure(textvariable=self.molecular)
-        self.TCombobox_molecular.current(0)
-
-        self.group_label = my_label(self.Labelframe1)
-        self.group_label.place(relx=0.558, rely=0.326, height=35, width=60
-                               , bordermode='ignore')
-        self.group_label.configure(text='''Group''')
-
-        self.TCombobox_group = my_combobox(self.Labelframe1)
-        self.TCombobox_group.place(relx=0.716, rely=0.326, height=35, width=150,
-                                   bordermode='ignore')
-        self.group_value_list = ['all', 'animals', 'plants', 'fungi',
-                                 'protists',
-                                 'bacteria', 'archaea', 'viruses', ]
-        self.TCombobox_group.configure(values=self.group_value_list)
-        self.TCombobox_group.configure(textvariable=self.group)
-        self.TCombobox_group.current(0)
-
-        self.organelle_label = my_label(self.Labelframe1)
-        self.organelle_label.place(relx=0.035, rely=0.435, height=35, width=80
-                                   , bordermode='ignore')
-        self.organelle_label.configure(text='''Organelle''')
-
-        self.TCombobox_og = my_combobox(self.Labelframe1)
-        self.TCombobox_og.place(relx=0.201, rely=0.435, height=35, width=170,
-                                bordermode='ignore')
-        self.og_value_list = ['ignore', 'both', 'no', 'mitochondrion',
-                              'chloroplast', ]
-        self.TCombobox_og.configure(values=self.og_value_list)
-        self.TCombobox_og.configure(textvariable=self.og)
-        self.TCombobox_og.current(0)
-
-        self.refseq_label = my_label(self.Labelframe1)
-        self.refseq_label.place(relx=0.035, rely=0.541, height=35, width=70
-                                , bordermode='ignore')
-        self.refseq_label.configure(text='''RefSeq''')
-
-        self.TCombobox_refseq = my_combobox(self.Labelframe1)
-        self.TCombobox_refseq.place(relx=0.201, rely=0.541, height=35,
-                                    width=150, bordermode='ignore')
-        self.refseq_value_list = ['both', 'yes', 'no', ]
-        self.TCombobox_refseq.configure(values=self.refseq_value_list)
-        self.TCombobox_refseq.configure(textvariable=self.refseq)
-        self.TCombobox_refseq.current(0)
-        self.TCombobox_refseq_tooltip = ToolTip(self.TCombobox_refseq,
-                                                self.tooltip_font,
-                                                'Use RefSeq or not')
-
-        self.count_label = my_label(self.Labelframe1)
-        self.count_label.place(relx=0.035, rely=0.649, height=35, width=60
-                               , bordermode='ignore')
-        self.count_label.configure(text='''Count''')
-
-        self.count_entry = my_entry(self.Labelframe1)
-        self.count_entry.place(relx=0.201, rely=0.649, relheight=0.095
-                               , relwidth=0.314, bordermode='ignore')
-        self.count_entry.configure(textvariable=self.count)
-        self.count_entry_tooltip = ToolTip(
-            self.count_entry, self.tooltip_font,
-            'numbers of sequences to download, 0 for no limit')
-
-        self.len_label = my_label(self.Labelframe1)
-        self.len_label.place(relx=0.558, rely=0.435, height=35, width=60
-                             , bordermode='ignore')
-        self.len_label.configure(text='''Length''')
-
-        self.min_len_entry = my_entry(self.Labelframe1)
-        self.min_len_entry.place(relx=0.686, rely=0.435, relheight=0.095
-                                 , relwidth=0.087, bordermode='ignore')
-        self.min_len_entry.configure(textvariable=self.min_len)
-        self.min_len_entry_tooltip = ToolTip(self.min_len_entry,
-                                             self.tooltip_font,
-                                             'sequence length limit')
-
-        self.to_label = my_label(self.Labelframe1)
-        self.to_label.place(relx=0.785, rely=0.435, height=35, width=36
-                            , bordermode='ignore')
-        self.to_label.configure(text='''to''')
-
-        self.max_len_entry = my_entry(self.Labelframe1)
-        self.max_len_entry.place(relx=0.839, rely=0.435, relheight=0.095
-                                 , relwidth=0.14, bordermode='ignore')
-        self.max_len_entry.configure(textvariable=self.max_len)
-        self.min_len_entry.insert(0, '0')
-        self.max_len_entry.insert(0, '300000')
-
-        self.date_label = my_label(self.Labelframe1)
-        self.date_label.place(relx=0.558, rely=0.541, height=35, width=60
-                              , bordermode='ignore')
-        self.date_label.configure(text='''Date''')
-
-        self.date_start_entry = my_entry(self.Labelframe1)
-        self.date_start_entry.place(relx=0.686, rely=0.541, relheight=0.095
-                                    , relwidth=0.087, bordermode='ignore')
-        self.date_start_entry.configure(textvariable=self.date_start)
-        self.date_start_entry_tooltip = ToolTip(self.date_start_entry,
-                                                self.tooltip_font,
-                                                '''1970/1/1''')
-
-        self.to2_label = my_label(self.Labelframe1)
-        self.to2_label.place(relx=0.789, rely=0.541, height=35, width=36
-                             , bordermode='ignore')
-        self.to2_label.configure(text='''to''')
-
-        self.date_end_entry = my_entry(self.Labelframe1)
-        self.date_end_entry.place(relx=0.839, rely=0.541, relheight=0.095
-                                  , relwidth=0.136, bordermode='ignore')
-        self.date_end_entry.configure(textvariable=self.date_end)
-        self.date_end_entry_tooltip = ToolTip(self.date_end_entry,
-                                              self.tooltip_font,
-                                              '''2022/12/31''')
-
-        self.exclude_label = my_label(self.Labelframe1)
-        self.exclude_label.place(relx=0.558, rely=0.649, height=35, width=60
-                                 , bordermode='ignore')
-        self.exclude_label.configure(text='''Exclude''')
-
-        self.exclude_entry = my_entry(self.Labelframe1)
-        self.exclude_entry.place(relx=0.686, rely=0.649, relheight=0.095
-                                 , relwidth=0.279, bordermode='ignore')
-        self.exclude_entry.configure(textvariable=self.exclude)
-        self.exclude_entry_tooltip = ToolTip(self.exclude_entry,
-                                             self.tooltip_font,
-                                             '''exclude expression''')
-
-        self.query_label = my_label(self.Labelframe1)
-        self.query_label.place(relx=0.035, rely=0.813, height=35, width=60
-                               , bordermode='ignore')
-        self.query_label.configure(text='''Query''')
-
-        self.query_entry = my_entry(self.Labelframe1)
-        self.query_entry.place(relx=0.201, rely=0.813, relheight=0.095
-                               , relwidth=0.785, bordermode='ignore')
-        self.query_entry.configure(textvariable=self.query)
-        self.query_entry_tooltip = ToolTip(self.query_entry, self.tooltip_font,
-                                           '''Entrez query string''')
-
-        self.taxon_entry = my_entry(self.Labelframe1)
-        self.taxon_entry.place(relx=0.201, rely=0.326, relheight=0.095
-                               , relwidth=0.314, bordermode='ignore')
-        self.taxon_entry.configure(textvariable=self.taxon)
-
-        self.out_label = my_label(self.top)
-        self.out_label.place(relx=0.05, rely=0.563, height=36
-                             , width=60)
-        self.out_label.configure(text='''Output''')
-
-        self.out_entry = my_entry(self.top)
-        self.out_entry.place(relx=0.167, rely=0.563, relheight=0.045
-                             , relwidth=0.633)
-        self.out_entry.configure(textvariable=self.out)
-        self.out_entry_tooltip = ToolTip(self.out_entry, self.tooltip_font,
-                                         'output folder')
-        self.out_b = my_button(self.top, 12)
-        self.out_b.place(relx=0.833, rely=0.563, height=35, width=80)
-        self.out_b.configure(command=open_file(self.out_entry, type_='folder'))
-        self.out_b.configure(text='''Open''')
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.025, rely=0.65, relheight=0.176
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Advance''')
-
-        self.expand_label = my_label(self.Labelframe1)
-        self.expand_label.place(relx=0.185, rely=0.142, height=35
-                                , width=60, bordermode='ignore')
-        self.expand_label.configure(text='''Expand''')
-
-        self.expand_entry = my_entry(self.Labelframe1)
-        self.expand_entry.place(relx=0.297, rely=0.142, relheight=0.248
-                                , relwidth=0.187, bordermode='ignore')
-        self.expand_entry.configure(textvariable=self.expand)
-        self.expand_entry_tooltip = ToolTip(self.expand_entry,
-                                            self.tooltip_font,
-                                            '''expand for primer design''')
-
-        self.max_name_len_label = my_label(self.Labelframe1)
-        self.max_name_len_label.place(relx=0.08, rely=0.426, height=35
-                                      , width=130, bordermode='ignore')
-        self.max_name_len_label.configure(text='''Max name length''')
-
-        self.max_frag_len_label = my_label(self.Labelframe1)
-        self.max_frag_len_label.place(relx=0.045, rely=0.709, height=35
-                                      , width=150, bordermode='ignore')
-        self.max_frag_len_label.configure(text='''Max fragment length''')
-
-        self.max_name_len_entry = my_entry(self.Labelframe1)
-        self.max_name_len_entry.place(relx=0.297, rely=0.426, relheight=0.248
-                                      , relwidth=0.187, bordermode='ignore')
-        self.max_name_len_entry.configure(textvariable=self.max_name_len)
-        self.max_name_len_entry_tooltip = ToolTip(self.max_name_len_entry,
-                                                  self.tooltip_font,
-                                                  '''max feature name length''')
-
-        self.max_gene_len_entry = my_entry(self.Labelframe1)
-        self.max_gene_len_entry.place(relx=0.297, rely=0.709, relheight=0.248
-                                      , relwidth=0.187, bordermode='ignore')
-        self.max_gene_len_entry.configure(textvariable=self.max_gene_len)
-        self.max_gene_len_entry_tooltip = ToolTip(self.max_gene_len_entry,
-                                                  self.tooltip_font,
-                                                  '''max fragment sequence length''')
-        self.max_name_len_entry.insert(0, '100')
-        self.max_gene_len_entry.insert(0, '20000')
-
-        self.TSeparator2 = ttk.Separator(self.Labelframe1)
-        self.TSeparator2.place(relx=0.524, rely=0.135, relheight=0.78
-                               , bordermode='ignore')
-        self.TSeparator2.configure(orient="vertical")
-
-        self.allow_repeat_button = my_checkbutton(self.Labelframe1)
-        self.allow_repeat_button.place(relx=0.576, rely=0.142, relheight=0.248
-                                       , relwidth=0.276, bordermode='ignore')
-        self.allow_repeat_button.configure(text='''Allow repeat''')
-        self.allow_repeat_button.configure(variable=self.allow_repeat)
-
-        self.allow_invert_repeat_button = my_checkbutton(self.Labelframe1)
-        self.allow_invert_repeat_button.place(relx=0.576, rely=0.709,
-                                              relheight=0.248
-                                              , relwidth=0.361,
-                                              bordermode='ignore')
-        self.allow_invert_repeat_button.configure(
-            text='''Allow invert repeat''')
-        self.allow_invert_repeat_button.configure(
-            variable=self.allow_invert_repeat)
-
-        self.allow_mosaic_button = my_checkbutton(self.Labelframe1)
-        self.allow_mosaic_button.place(relx=0.576, rely=0.426, relheight=0.248
-                                       , relwidth=0.361, bordermode='ignore')
-        self.allow_mosaic_button.configure(text='''Allow mosaic repeat''')
-        self.allow_mosaic_button.configure(variable=self.allow_mosaic_repeat)
-
-        self.no_divide_b = my_checkbutton(self.top)
-        self.no_divide_b.place(relx=0.733, rely=0.488, relheight=0.044
-                               , relwidth=0.215)
-        self.no_divide_b.configure(text='''No divide''')
-        self.no_divide_b.configure(variable=self.no_divide)
-
-        self.rename_b = my_checkbutton(self.top)
-        self.rename_b.place(relx=0.467, rely=0.488, relheight=0.044
-                            , relwidth=0.243)
-        self.rename_b.configure(text='''Rename gene''')
-        self.rename_b.configure(variable=self.rename)
-
-        self.unique_label = my_label(self.top)
-        self.unique_label.place(relx=0.05, rely=0.488, height=35
-                                , width=69)
-        self.unique_label.configure(text='''Unique''')
-
-        self.TCombobox_unique = my_combobox(self.top)
-        self.TCombobox_unique.place(relx=0.167, rely=0.488, relheight=0.044
-                                    , relwidth=0.245)
-        self.unique_value_list = ['longest', 'first', 'no', ]
-        self.TCombobox_unique.configure(values=self.unique_value_list)
-        self.TCombobox_unique.configure(textvariable=self.unique)
-        self.TCombobox_unique.current(0)
-        self.TCombobox_unique_tooltip = ToolTip(
-            self.TCombobox_unique, self.tooltip_font,
-            'methods to remove redundant records')
-
-        self.run_b = my_button(self.top, 14)
-        self.run_b.place(relx=0.333, rely=0.863, height=40, width=189)
-        self.run_b.configure(command=run_gb2fasta(self, self.top))
-        self.run_b.configure(text='''Run''')
-
-
-class Evaluate:
-    def __init__(self, top=None):
-        '''This class configures and populates the toplevel window.
-           top is the toplevel containing window.'''
-        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
-        _fgcolor = '#000000'  # X11 color: 'black'
-        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
-        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
-        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
-        _tabfg1 = 'black'
-        _tabfg2 = 'black'
-        _tabbg1 = 'grey75'
-        _tabbg2 = 'grey89'
-        _bgmode = 'light'
-        self.style = ttk.Style()
-        if sys.platform == "win32":
-            self.style.theme_use('winnative')
-        self.style.configure('.', background=_bgcolor)
-        self.style.configure('.', foreground=_fgcolor)
-        self.style.map('.', background=[('selected', _compcolor),
-                                        ('active', _ana2color)])
-        self.tooltip_font = "TkDefaultFont"
-
-        top.geometry("600x450+109+248")
-        move_to_center(top, 600, 450)
-        top.title("Evaluate")
-        top.configure(background="#edf0f3")
-        top.configure(highlightbackground="#d9d9d9")
-        top.configure(highlightcolor="black")
-
-        self.top = top
-        self.fasta = tk.StringVar()
-        self.fasta_folder = tk.StringVar()
-        self.aln = tk.StringVar()
-        self.out = tk.StringVar()
-        self.size = tk.StringVar()
-        self.step = tk.StringVar()
-        self.quick = tk.IntVar()
-        self.ig = tk.IntVar()
-        self.iab = tk.IntVar()
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.017, rely=0.0, relheight=0.333
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Input''')
-
-        self.unalign_label = my_label(self.Labelframe1)
-        self.unalign_label.place(relx=0.03, rely=0.133, height=35, width=160
-                                 , bordermode='ignore')
-        self.unalign_label.configure(text='''Unaligned FASTA files''')
-        self.TLabel1_tooltip = ToolTip(self.unalign_label, self.tooltip_font,
-                                       'unaligned')
-
-        self.fasta_entry = my_entry(self.Labelframe1)
-        self.fasta_entry.place(relx=0.314, rely=0.133, relheight=0.233
-                               , relwidth=0.489, bordermode='ignore')
-        self.fasta_entry.configure(textvariable=self.fasta)
-        self.fasta_entry_tooltip = ToolTip(self.fasta_entry, self.tooltip_font,
-                                           '''unaligned fasta files''')
-
-        self.open_btn = my_button(self.Labelframe1)
-        self.open_btn.place(relx=0.82, rely=0.133, height=35, width=90
-                            , bordermode='ignore')
-        self.open_btn.configure(command=open_file(self.fasta_entry,
-                                                  single=False))
-        self.open_btn.configure(text='''Open''')
-
-        self.unalign_label2 = my_label(self.Labelframe1)
-        self.unalign_label2.place(relx=0.03, rely=0.4, height=35, width=160
-                                  , bordermode='ignore')
-        self.unalign_label2.configure(text='''Unaligned FASTA folder''')
-        self.TLabel1_tooltip = ToolTip(self.unalign_label2, self.tooltip_font,
-                                       '''unaligned''')
-
-        self.fasta_folder_entry = my_entry(self.Labelframe1)
-        self.fasta_folder_entry.place(relx=0.314, rely=0.4, relheight=0.233
-                                      , relwidth=0.489, bordermode='ignore')
-        self.fasta_folder_entry.configure(textvariable=self.fasta_folder)
-        self.fasta_folder_entry_tooltip = ToolTip(
-            self.fasta_folder_entry, self.tooltip_font,
-            'unaligned fasta files')
-        self.open1_btn = my_button(self.Labelframe1)
-        self.open1_btn.place(relx=0.82, rely=0.4, height=35, width=90
-                             , bordermode='ignore')
-        self.open1_btn.configure(command=open_file(self.fasta_folder_entry,
-                                                   type_='folder'))
-        self.open1_btn.configure(text='''Open''')
-
-        self.align_label = my_label(self.Labelframe1)
-        self.align_label.place(relx=0.03, rely=0.667, height=35, width=150
-                               , bordermode='ignore')
-        self.align_label.configure(text='''Aligned FASTA files''')
-        self.TLabel1_3_tooltip = ToolTip(self.align_label, self.tooltip_font,
-                                         '''aligned''')
-
-        self.aln_entry = my_entry(self.Labelframe1)
-        self.aln_entry.place(relx=0.314, rely=0.667, relheight=0.233
-                             , relwidth=0.489, bordermode='ignore')
-        self.aln_entry.configure(textvariable=self.aln)
-        self.aln_entry_tooltip = ToolTip(self.aln_entry, self.tooltip_font,
-                                         '''aligned fasta files''')
-        self.open2_btn = my_button(self.Labelframe1)
-        self.open2_btn.place(relx=0.82, rely=0.667, height=35, width=90
-                             , bordermode='ignore')
-        self.open2_btn.configure(command=open_file(self.aln_entry,
-                                                   single=False))
-        self.open2_btn.configure(text='''Open''')
-
-        self.out_label = my_label(self.top)
-        self.out_label.place(relx=0.117, rely=0.356, height=35, width=100)
-        self.out_label.configure(text='''Output folder''')
-        self.TLabel1_3_1_tooltip = ToolTip(self.out_label, self.tooltip_font,
-                                           '''output''')
-
-        self.out_entry = my_entry(self.top)
-        self.out_entry.place(relx=0.317, rely=0.356, relheight=0.078
-                             , relwidth=0.467)
-        self.out_entry.configure(textvariable=self.out)
-        self.out_entry_tooltip = ToolTip(self.out_entry, self.tooltip_font,
-                                         '''unaligned fasta files''')
-
-        self.open3_btn = my_button(self.top)
-        self.open3_btn.place(relx=0.8, rely=0.356, height=35, width=90)
-        self.open3_btn.configure(command=open_file(self.out_entry,
-                                                   type_='folder'))
-        self.open3_btn.configure(text='''Open''')
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.017, rely=0.467, relheight=0.156
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Sliding window''')
-
-        self.Checkbutton1 = my_checkbutton(self.Labelframe1)
-        self.Checkbutton1.place(relx=0.005, rely=0.429, relheight=0.3,
-                                relwidth=0.272, bordermode='ignore')
-        self.Checkbutton1.configure(text='''Skip sliding window''')
-        self.Checkbutton1.configure(variable=self.quick)
-
-        self.window_size_label = my_label(self.Labelframe1)
-        self.window_size_label.place(relx=0.314, rely=0.429, height=22, width=80
-                                     , bordermode='ignore')
-        self.window_size_label.configure(text='Window size')
-
-        self.step_len_label = my_label(self.Labelframe1)
-        self.step_len_label.place(relx=0.681, rely=0.429, height=22, width=80
-                                  , bordermode='ignore')
-        self.step_len_label.configure(text='''Step length''')
-
-        self.size_entry = my_entry(self.Labelframe1)
-        self.size_entry.place(relx=0.489, rely=0.357, relheight=0.5
-                              , relwidth=0.14, bordermode='ignore')
-        self.size_entry.configure(textvariable=self.size)
-
-        self.step_entry = my_entry(self.Labelframe1)
-        self.step_entry.place(relx=0.838, rely=0.357, relheight=0.5
-                              , relwidth=0.14, bordermode='ignore')
-        self.step_entry.configure(textvariable=self.step)
-        self.size_entry.insert(0, '500')
-        self.step_entry.insert(0, '50')
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.017, rely=0.644, relheight=0.156
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Advance''')
-
-        self.Checkbutton1 = my_checkbutton(self.Labelframe1)
-        self.Checkbutton1.place(relx=0.087, rely=0.429, relheight=0.3
-                                , relwidth=0.354, bordermode='ignore')
-        self.Checkbutton1.configure(text='''Ignore gaps in alignment''')
-        self.Checkbutton1.configure(variable=self.ig)
-
-        self.Checkbutton1_2 = my_checkbutton(self.Labelframe1)
-        self.Checkbutton1_2.place(relx=0.593, rely=0.429, relheight=0.3
-                                  , relwidth=0.354, bordermode='ignore')
-        self.Checkbutton1_2.configure(text='''Ignore ambiguous bases''')
-        self.Checkbutton1_2.configure(variable=self.iab)
-
-        self.run_b = my_button(self.top, 14)
-        self.run_b.place(relx=0.333, rely=0.867, height=40, width=189)
-        self.run_b.configure(command=run_evaluate(self, self.top))
-        self.run_b.configure(text='''Run''')
-
-
-class Primer:
-    def __init__(self, top=None):
-        '''This class configures and populates the toplevel window.
-           top is the toplevel containing window.'''
-        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
-        _fgcolor = '#000000'  # X11 color: 'black'
-        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
-        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
-        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
-        _tabfg1 = 'black'
-        _tabfg2 = 'black'
-        _tabbg1 = 'grey75'
-        _tabbg2 = 'grey89'
-        _bgmode = 'light'
-        self.style = ttk.Style()
-        if sys.platform == "win32":
-            self.style.theme_use('winnative')
-        self.style.configure('.', background=_bgcolor)
-        self.style.configure('.', foreground=_fgcolor)
-        self.style.map('.', background=[('selected', _compcolor),
-                                        ('active', _ana2color)])
-        self.tooltip_font = "TkDefaultFont"
-
-        top.geometry("600x500+284+458")
-        move_to_center(top, 600, 600)
-        top.title("Primer")
-        top.configure(background="#edf0f3")
-        top.configure(highlightbackground="#d9d9d9")
-        top.configure(highlightcolor="black")
-
-        self.top = top
-        self.aln = tk.StringVar()
-        self.aln_folder = tk.StringVar()
-        self.out = tk.StringVar()
-        self.coverage = tk.StringVar()
-        self.mismatch = tk.StringVar()
-        self.resolution = tk.StringVar()
-        self.top_n = tk.StringVar()
-        self.pmin = tk.StringVar()
-        self.pmax = tk.StringVar()
-        self.amin = tk.StringVar()
-        self.amax = tk.StringVar()
-        self.size = tk.StringVar()
-        self.step = tk.StringVar()
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.017, rely=0.02, relheight=0.2
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Input''')
-
-        self.aln_fasta_label = my_label(self.Labelframe1)
-        self.aln_fasta_label.place(relx=0.052, rely=0.2, height=35, width=130
-                                   , bordermode='ignore')
-        self.aln_fasta_label.configure(text='''Aligned FASTA files''')
-        self.TLabel1_tooltip = ToolTip(self.aln_fasta_label, self.tooltip_font,
-                                       'unaligned')
-
-        self.aln_entry = my_entry(self.Labelframe1)
-        self.aln_entry.place(relx=0.314, rely=0.2, relheight=0.35,
-                             relwidth=0.489
-                             , bordermode='ignore')
-        self.aln_entry.configure(textvariable=self.aln)
-        self.aln_entry_tooltip = ToolTip(self.aln_entry, self.tooltip_font,
-                                         '''unaligned fasta files''')
-
-        self.out_b = my_button(self.Labelframe1)
-        self.out_b.place(relx=0.82, rely=0.2, height=35, width=90
-                         , bordermode='ignore')
-        self.out_b.configure(command=open_file(self.aln_entry, single=False))
-        self.out_b.configure(text='''Open''')
-
-        self.aln_folder_label = my_label(self.Labelframe1)
-        self.aln_folder_label.place(relx=0.052, rely=0.6, height=35, width=160
-                                    , bordermode='ignore')
-        self.aln_folder_label.configure(text='''Aligned FASTA folder''')
-        self.TLabel1_tooltip = ToolTip(self.aln_folder_label, self.tooltip_font,
-                                       'Folder with aligned fasta files')
-
-        self.aln_folder_entry = my_entry(self.Labelframe1)
-        self.aln_folder_entry.place(relx=0.314, rely=0.6, relheight=0.35
-                                    , relwidth=0.489, bordermode='ignore')
-        self.aln_folder_entry.configure(textvariable=self.aln_folder)
-        self.aln_folder_entry_tooltip = ToolTip(self.aln_folder_entry,
-                                                self.tooltip_font,
-                                                '''unaligned fasta files''')
-
-        self.folder_b = my_button(self.Labelframe1)
-        self.folder_b.place(relx=0.82, rely=0.6, height=35, width=90
-                            , bordermode='ignore')
-        self.folder_b.configure(command=open_file(self.aln_folder_entry,
-                                                  type_='folder'))
-        self.folder_b.configure(text='''Open''')
-
-        self.out_label = my_label(self.top)
-        self.out_label.place(relx=0.07, rely=0.24, height=35, width=150)
-        self.out_label.configure(text='''Output folder''')
-        self.TLabel1_3_1_tooltip = ToolTip(self.out_label, self.tooltip_font,
-                                           'Output')
-
-        self.out_entry = my_entry(self.top)
-        self.out_entry.place(relx=0.317, rely=0.24, relheight=0.07
-                             , relwidth=0.467)
-        self.out_entry.configure(textvariable=self.out)
-
-        self.out_b = my_button(self.top)
-        self.out_b.place(relx=0.8, rely=0.24, height=35, width=90)
-        self.out_b.configure(command=open_file(self.out_entry, type_='folder'))
-        self.out_b.configure(text='''Open''')
-
-        self.Labelframe1 = my_labelframe(self.top)
-        self.Labelframe1.place(relx=0.017, rely=0.34, relheight=0.38
-                               , relwidth=0.955)
-        self.Labelframe1.configure(text='''Advance''')
-
-        self.coverage_label = my_label(self.Labelframe1)
-        self.coverage_label.place(relx=0.07, rely=0.158, height=35
-                                  , width=70, bordermode='ignore')
-        self.coverage_label.configure(text='''Coverage''')
-
-        self.coverage_entry = my_entry(self.Labelframe1)
-        self.coverage_entry.place(relx=0.297, rely=0.142, relheight=0.184
-                                  , relwidth=0.192, bordermode='ignore')
-        self.coverage_entry.configure(textvariable=self.coverage)
-        self.coverage_entry_tooltip = ToolTip(self.coverage_entry,
-                                              self.tooltip_font,
-                                              '''minimal coverage of primer on alignment''')
-        self.coverage_entry.insert(0, '0.5')
-
-        self.mismatch_label = my_label(self.Labelframe1)
-        self.mismatch_label.place(relx=0.07, rely=0.368, height=35
-                                  , width=120, bordermode='ignore')
-        self.mismatch_label.configure(text='''Mismatch''')
-
-        self.res_label = my_label(self.Labelframe1)
-        self.res_label.place(relx=0.07, rely=0.579, height=35
-                             , width=130, bordermode='ignore')
-        self.res_label.configure(text='''Resolution''')
-
-        self.mismatch_entry = my_entry(self.Labelframe1)
-        self.mismatch_entry.place(relx=0.297, rely=0.368, relheight=0.184
-                                  , relwidth=0.192, bordermode='ignore')
-        self.mismatch_entry.configure(textvariable=self.mismatch)
-        self.mismatch_entry_tooltip = ToolTip(
-            self.mismatch_entry, self.tooltip_font,
-            'maximum mismatch bases in primer')
-
-        self.resolution_entry = my_entry(self.Labelframe1)
-        self.resolution_entry.place(relx=0.297, rely=0.579, relheight=0.184
-                                    , relwidth=0.192, bordermode='ignore')
-        self.resolution_entry.configure(textvariable=self.resolution)
-        self.resolution_entry_tooltip = ToolTip(
-            self.resolution_entry, self.tooltip_font,
-            'minimal resolution of amplified fragment''')
-        self.mismatch_entry.insert(0, '4')
-        self.resolution_entry.insert(0, '0.3')
-
-        self.TSeparator2 = ttk.Separator(self.Labelframe1)
-        self.TSeparator2.place(relx=0.524, rely=0.137, relheight=0.779
-                               , bordermode='ignore')
-        self.TSeparator2.configure(orient="vertical")
-
-        self.topn_label = my_label(self.Labelframe1)
-        self.topn_label.place(relx=0.07, rely=0.789, height=35
-                              , width=130, bordermode='ignore')
-        self.topn_label.configure(text='''Top n''')
-
-        self.top_n_entry = my_entry(self.Labelframe1)
-        self.top_n_entry.place(relx=0.297, rely=0.789, relheight=0.184
-                               , relwidth=0.192, bordermode='ignore')
-        self.top_n_entry.configure(textvariable=self.top_n)
-        self.top_n_entry_tooltip = ToolTip(self.top_n_entry, self.tooltip_font,
-                                           '''Only keep top best primers''')
-        self.top_n_entry.insert(0, '1')
-
-        self.primer_len_label = my_label(self.Labelframe1)
-        self.primer_len_label.place(relx=0.541, rely=0.158, height=35
-                                    , width=100, bordermode='ignore')
-        self.primer_len_label.configure(text='''Primer length''')
-
-        self.pmin_entry = my_entry(self.Labelframe1)
-        self.pmin_entry.place(relx=0.716, rely=0.158, relheight=0.184
-                              , relwidth=0.087, bordermode='ignore')
-        self.pmin_entry.configure(textvariable=self.pmin)
-
-        self.to_label1 = my_label(self.Labelframe1)
-        self.to_label1.place(relx=0.803, rely=0.158, height=35, width=36
-                             , bordermode='ignore')
-        self.to_label1.configure(text='''to''')
-
-        self.pmax_entry = my_entry(self.Labelframe1)
-        self.pmax_entry.place(relx=0.855, rely=0.158, relheight=0.184
-                              , relwidth=0.122, bordermode='ignore')
-        self.pmax_entry.configure(textvariable=self.pmax)
-        self.pmin_entry.insert(0, '20')
-        self.pmax_entry.insert(0, '30')
-
-        self.amp_len_label = my_label(self.Labelframe1)
-        self.amp_len_label.place(relx=0.541, rely=0.368, height=35
-                                 , width=120, bordermode='ignore')
-        self.amp_len_label.configure(text='''Amplicon size''')
-
-        self.amin_entry = my_entry(self.Labelframe1)
-        self.amin_entry.place(relx=0.716, rely=0.368, relheight=0.184
-                              , relwidth=0.087, bordermode='ignore')
-        self.amin_entry.configure(textvariable=self.amin)
-        self.amin_entry_tooltip = ToolTip(self.amin_entry, self.tooltip_font,
-                                          'including primer length')
-
-        self.to2_label = my_label(self.Labelframe1)
-        self.to2_label.place(relx=0.803, rely=0.368, height=35, width=36
-                             , bordermode='ignore')
-        self.to2_label.configure(text='''to''')
-
-        self.amax_entry = my_entry(self.Labelframe1)
-        self.amax_entry.place(relx=0.855, rely=0.368, relheight=0.184
-                              , relwidth=0.122, bordermode='ignore')
-        self.amax_entry.configure(textvariable=self.amax)
-        self.amin_entry.insert(0, '300')
-        self.amax_entry.insert(0, '800')
-
-        self.sliding_window_label = my_label(self.Labelframe1)
-        self.sliding_window_label.place(relx=0.541, rely=0.579, height=35,
-                                        width=130
-                                        , bordermode='ignore')
-        self.sliding_window_label.configure(text='''Sliding window size''')
-
-        self.sliding_window2_label = my_label(self.Labelframe1)
-        self.sliding_window2_label.place(relx=0.541, rely=0.789, height=35,
-                                         width=130
-                                         , bordermode='ignore')
-        self.sliding_window2_label.configure(text='''Sliding window step''')
-
-        self.size_entry = my_entry(self.Labelframe1)
-        self.size_entry.place(relx=0.803, rely=0.579, relheight=0.184
-                              , relwidth=0.14, bordermode='ignore')
-        self.size_entry.configure(textvariable=self.size)
-
-        self.step_entry = my_entry(self.Labelframe1)
-        self.step_entry.place(relx=0.803, rely=0.789, relheight=0.184
-                              , relwidth=0.14, bordermode='ignore')
-        self.step_entry.configure(textvariable=self.step)
-        self.size_entry.insert(0, '500')
-        self.step_entry.insert(0, '50')
-
-        self.run_b = my_button(self.top, 14)
-        self.run_b.place(relx=0.367, rely=0.82, height=40, width=180)
-        self.run_b.configure(command=run_primer(self, self.top))
-        self.run_b.configure(text='''Run''')
-
-
-class ToolTip(tk.Toplevel):
-    """ Provides a ToolTip widget for Tkinter. """
-
-    def __init__(self, wdgt, tooltip_font, msg=None, msgFunc=None,
-                 delay=0.5, follow=True):
-        self.wdgt = wdgt
-        self.parent = self.wdgt.master
-        tk.Toplevel.__init__(self, self.parent, bg='black', padx=1, pady=1)
-        self.withdraw()
-        self.overrideredirect(True)
-        self.msgVar = tk.StringVar()
-        if msg is None:
-            self.msgVar.set('No message provided')
-        else:
-            self.msgVar.set(msg)
-        self.msgFunc = msgFunc
-        self.delay = delay
-        self.follow = follow
-        self.visible = 0
-        self.lastMotion = 0
-        tk.Message(self, textvariable=self.msgVar, bg='#FFFFDD',
-                   font=tooltip_font,
-                   aspect=1000).grid()
-        self.wdgt.bind('<Enter>', self.spawn, '+')
-        self.wdgt.bind('<Leave>', self.hide, '+')
-        self.wdgt.bind('<Motion>', self.move, '+')
-
-    def spawn(self, event=None):
-        self.visible = 1
-        self.after(int(self.delay * 1000), self.show)
-
-    def show(self):
-        if self.visible == 1 and time() - self.lastMotion > self.delay:
-            self.visible = 2
-        if self.visible == 2:
-            self.deiconify()
-
-    def move(self, event):
-        self.lastMotion = time()
-        if self.follow is False:
-            self.withdraw()
-            self.visible = 1
-        self.geometry('+%i+%i' % (event.x_root + 20, event.y_root - 10))
-        try:
-            self.msgVar.set(self.msgFunc())
-        except:
-            pass
-        self.after(int(self.delay * 1000), self.show)
-
-    def hide(self, event=None):
-        self.visible = 0
-        self.withdraw()
-
-    def update(self, msg):
-        self.msgVar.set(msg)
-
-
-def _create_container(func):
-    '''Creates a ttk Frame with a given master, and use this new frame to
-    place the scrollbars and the widget.'''
-
-    def wrapped(cls, master, **kw):
-        container = ttk.Frame(master)
-        container.bind('<Enter>', lambda e: _bound_to_mousewheel(e, container))
-        container.bind('<Leave>',
-                       lambda e: _unbound_to_mousewheel(e, container))
-        return func(cls, container, **kw)
-
-    return wrapped
-
-
-def _bound_to_mousewheel(event, widget):
-    child = widget.winfo_children()[0]
-    if platform.system() == 'Windows' or platform.system() == 'Darwin':
-        child.bind_all('<MouseWheel>', lambda e: _on_mousewheel(e, child))
-        child.bind_all('<Shift-MouseWheel>', lambda e: _on_shiftmouse(e, child))
-    else:
-        child.bind_all('<Button-4>', lambda e: _on_mousewheel(e, child))
-        child.bind_all('<Button-5>', lambda e: _on_mousewheel(e, child))
-        child.bind_all('<Shift-Button-4>', lambda e: _on_shiftmouse(e, child))
-        child.bind_all('<Shift-Button-5>', lambda e: _on_shiftmouse(e, child))
-
-
-def _unbound_to_mousewheel(event, widget):
-    if platform.system() == 'Windows' or platform.system() == 'Darwin':
-        widget.unbind_all('<MouseWheel>')
-        widget.unbind_all('<Shift-MouseWheel>')
-    else:
-        widget.unbind_all('<Button-4>')
-        widget.unbind_all('<Button-5>')
-        widget.unbind_all('<Shift-Button-4>')
-        widget.unbind_all('<Shift-Button-5>')
-
-
-def _on_mousewheel(event, widget):
-    if platform.system() == 'Windows':
-        widget.yview_scroll(-1 * int(event.delta / 120), 'units')
-    elif platform.system() == 'Darwin':
-        widget.yview_scroll(-1 * int(event.delta), 'units')
-    else:
-        if event.num == 4:
-            widget.yview_scroll(-1, 'units')
-        elif event.num == 5:
-            widget.yview_scroll(1, 'units')
-
-
-def _on_shiftmouse(event, widget):
-    if platform.system() == 'Windows':
-        widget.xview_scroll(-1 * int(event.delta / 120), 'units')
-    elif platform.system() == 'Darwin':
-        widget.xview_scroll(-1 * int(event.delta), 'units')
-    else:
-        if event.num == 4:
-            widget.xview_scroll(-1, 'units')
-        elif event.num == 5:
-            widget.xview_scroll(1, 'units')
-
-
-def ui_gb2fasta():
-    global _top2, _w2
-    _top2 = tk.Toplevel(root)
-    root.iconify()
-    _top2.protocol('WM_DELETE_WINDOW', after_close(_top2))
-    _w2 = GB2Fasta(_top2)
-
-
-def ui_evaluate():
-    global _top3, _w3
-    _top3 = tk.Toplevel(root)
-    root.iconify()
-    _top3.protocol('WM_DELETE_WINDOW', after_close(_top3))
-    _w3 = Evaluate(_top3)
-
-
-def ui_primer():
-    # Creates a toplevel widget.
-    global _top4, _w4
-    _top4 = tk.Toplevel(root)
-    root.iconify()
-    _top4.protocol('WM_DELETE_WINDOW', after_close(_top4))
-    _w4 = Primer(_top4)
-
-
-def get_arg_str(value: tk.Variable, name: str, arg_str: str,
-                is_bool=False) -> str:
-    value_str = ''
-    if value.get():
-        if is_bool:
-            value_str = f'{name} '
-        else:
-            value_str = f'{name} {value.get()} '
-    arg_str += value_str
-    log.debug(f'{name} {value_str}')
-    return arg_str
-
-
-def run_gb2fasta(win, t: tk.Toplevel):
-    # todo: test options and functions
-    def f():
-        nonlocal win
-        arg_str = ''
-        arg_str = get_arg_str(win.gb, '-gb', arg_str)
-        arg_str = get_arg_str(win.gene, '-gene', arg_str)
-        arg_str = get_arg_str(win.molecular, '-molecular', arg_str)
-        arg_str = get_arg_str(win.group, '-group', arg_str)
-        arg_str = get_arg_str(win.og, '-og', arg_str)
-        arg_str = get_arg_str(win.refseq, '-refseq', arg_str)
-        arg_str = get_arg_str(win.count, '-count', arg_str)
-        arg_str = get_arg_str(win.min_len, '-min_len', arg_str)
-        arg_str = get_arg_str(win.max_len, '-max_len', arg_str)
-        arg_str = get_arg_str(win.date_start, '-date_start', arg_str)
-        arg_str = get_arg_str(win.date_end, '-date_end', arg_str)
-        arg_str = get_arg_str(win.exclude, '-exclude', arg_str)
-        arg_str = get_arg_str(win.query, '-query', arg_str)
-        arg_str = get_arg_str(win.taxon, '-taxon', arg_str)
-        arg_str = get_arg_str(win.out, '-out', arg_str)
-        arg_str = get_arg_str(win.expand, '-expand', arg_str)
-        arg_str = get_arg_str(win.max_name_len, '-max_name_len', arg_str)
-        arg_str = get_arg_str(win.max_gene_len, '-max_gene_len', arg_str)
-        arg_str = get_arg_str(win.unique, '-unique', arg_str)
-        arg_str = get_arg_str(win.allow_repeat, '-allow_repeat', arg_str,
-                              is_bool=True)
-        arg_str = get_arg_str(win.allow_invert_repeat, '-allow_invert_repeat',
-                              arg_str,
-                              is_bool=True)
-        arg_str = get_arg_str(win.allow_mosaic_repeat, '-allow_mosaic_repeat',
-                              arg_str,
-                              is_bool=True)
-        arg_str = get_arg_str(win.no_divide, '-no_divide', arg_str,
-                              is_bool=True)
-        arg_str = get_arg_str(win.rename, '-rename', arg_str, is_bool=True)
-        t.withdraw()
-        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
-        s = min(w, h) // 2
-        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
-        run = tk.Toplevel(root)
-        run.geometry(size)
-        run.title('Running...')
-        run.wm_transient()
-        frame = ttk.Frame(run)
-        frame.pack(fill='both')
-        scroll_text(frame)
-        r = threading.Thread(target=thread_wrap,
-                             args=(gb2fasta_main, arg_str, run),
-                             daemon=True)
-        r.start()
-
-    return f
-
-
-def run_evaluate(win, t: tk.Toplevel):
-    # todo: test options and functions
-    def f():
-        nonlocal win
-        arg_str = ''
-        arg_str = get_arg_str(win.fasta, '-fasta', arg_str)
-        arg_str = get_arg_str(win.fasta_folder, '-fasta_folder', arg_str)
-        arg_str = get_arg_str(win.aln, '-aln', arg_str)
-        arg_str = get_arg_str(win.out, '-out', arg_str)
-        arg_str = get_arg_str(win.size, '-size', arg_str)
-        arg_str = get_arg_str(win.step, '-step', arg_str)
-        arg_str = get_arg_str(win.quick, '-quick', arg_str, is_bool=True)
-        arg_str = get_arg_str(win.ig, '-ig', arg_str, is_bool=True)
-        arg_str = get_arg_str(win.iab, '-iab', arg_str, is_bool=True)
-        t.withdraw()
-        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
-        s = min(w, h) // 2
-        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
-        run = tk.Toplevel(root)
-        run.geometry(size)
-        run.title('Running...')
-        run.wm_transient()
-        frame = ttk.Frame(run)
-        frame.pack(fill='both')
-        scroll_text(frame)
-        r = threading.Thread(target=thread_wrap,
-                             args=(evaluate_main, arg_str, run),
-                             daemon=True)
-        r.start()
-
-    return f
-
-
-def run_primer(win, t: tk.Toplevel):
-    # todo: test options and functions
-    def f():
-        nonlocal win
-        arg_str = ''
-        arg_str = get_arg_str(win.aln, '-aln', arg_str)
-        arg_str = get_arg_str(win.aln_folder, '-aln_folder', arg_str)
-        arg_str = get_arg_str(win.out, '-out', arg_str)
-        arg_str = get_arg_str(win.coverage, '-coverage', arg_str)
-        arg_str = get_arg_str(win.mismatch, '-mismatch', arg_str)
-        arg_str = get_arg_str(win.resolution, '-resolution', arg_str)
-        arg_str = get_arg_str(win.top_n, '-top_n', arg_str)
-        arg_str = get_arg_str(win.pmin, '-pmin', arg_str)
-        arg_str = get_arg_str(win.pmax, '-pmax', arg_str)
-        arg_str = get_arg_str(win.amin, '-amin', arg_str)
-        arg_str = get_arg_str(win.amax, '-amax', arg_str)
-        arg_str = get_arg_str(win.size, '-size', arg_str)
-        arg_str = get_arg_str(win.step, '-step', arg_str)
-        arg_str += '-primer'
-        t.withdraw()
-        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
-        s = min(w, h) // 2
-        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
-        run = tk.Toplevel(root)
-        run.geometry(size)
-        run.title('Running...')
-        run.wm_transient()
-        frame = ttk.Frame(run)
-        frame.pack(fill='both')
-        scroll_text(frame)
-        r = threading.Thread(target=thread_wrap,
-                             args=(primer_main, arg_str, run),
-                             daemon=True)
-        r.start()
-
-    return f
-
-
-def run_help():
-    url = 'https://github.com/wpwupingwp/barcodefinder'
-    webbrowser.open(url, new=2)
-
-
-def run_install(win, t: tk.Toplevel):
-    def f():
-        t.withdraw()
-        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
-        s = min(w, h) // 2
-        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
-        run = tk.Toplevel(root)
-        run.geometry(size)
-        run.title('Running...')
-        run.wm_transient()
-        frame = ttk.Frame(run)
-        frame.pack(fill='both')
-        scroll_text(frame)
-        r = threading.Thread(target=thread_wrap,
-                             args=(get_all_third_party, '', run, True),
-                             daemon=True)
-        r.start()
-
-    return f
-
-
-def ui_main():
-    global root
-    root = tk.Tk()
-    root.protocol('WM_DELETE_WINDOW', root.destroy)
-    root.title('Organelle Genome Utilities')
-    # Creates a toplevel widget.
-    global _top1, _w1
-    _top1 = root
-    _w1 = Root(_top1)
-    root.mainloop()
-
-
-if __name__ == '__main__':
-    ui_main()
+#!/usr/bin/env python
+from importlib import resources
+from logging import handlers
+from time import time
+from tkinter import filedialog, messagebox, scrolledtext
+import logging
+import platform
+import queue
+import sys
+import threading
+import tkinter as tk
+import tkinter.ttk as ttk
+import webbrowser
+
+from OGU.evaluate import evaluate_main
+from OGU.gb2fasta import gb2fasta_main
+from OGU.global_vars import log, name, FMT, DATEFMT
+from OGU.primer import primer_main
+from OGU.utils import font_family, get_all_third_party
+
+
+def my_labelframe(parent: tk.LabelFrame) -> tk.LabelFrame:
+    frame = tk.LabelFrame(parent)
+    frame.configure(background="#edf0f3")
+    frame.configure(cursor="fleur")
+    frame.configure(font=f'-family {font_family} -size 14')
+    frame.configure(foreground="#000000")
+    frame.configure(highlightbackground="#edf0f3")
+    frame.configure(highlightcolor="black")
+    frame.configure(relief='groove')
+    return frame
+
+
+def my_label(frame: tk.LabelFrame, fontsize=11) -> tk.Label:
+    label = tk.Label(frame)
+    label.configure(activebackground="#f9f9f9")
+    label.configure(activeforeground="black")
+    label.configure(anchor='w')
+    label.configure(background="#edf0f3")
+    label.configure(compound='left')
+    label.configure(foreground="#000000")
+    label.configure(highlightbackground="#edf0f3")
+    label.configure(highlightcolor="black")
+    label.configure(justify='left')
+    label.configure(font=f'-family {font_family} -size {fontsize}')
+    return label
+
+
+def my_button(frame: tk.LabelFrame, fontsize=12) -> tk.Button:
+    button = tk.Button(frame)
+    button.configure(compound='left')
+    button.configure(activebackground="#ececec")
+    button.configure(activeforeground="#000000")
+    button.configure(background="#edf0f3")
+    button.configure(font=f"-family {font_family} -size {fontsize}")
+    button.configure(foreground="#000000")
+    button.configure(highlightbackground="#edf0f3")
+    button.configure(highlightcolor="black")
+    button.configure(pady="0")
+    button.configure(relief="raised")
+    button.configure(borderwidth=1)
+    return button
+
+
+def my_checkbutton(frame: tk.LabelFrame, fontsize=11) -> tk.Checkbutton:
+    check_b = tk.Checkbutton(frame)
+    check_b.configure(activebackground="#ececec")
+    check_b.configure(activeforeground="#000000")
+    check_b.configure(anchor='w')
+    check_b.configure(background="#edf0f3")
+    check_b.configure(compound='left')
+    check_b.configure(foreground="#000000")
+    check_b.configure(highlightbackground="#edf0f3")
+    check_b.configure(highlightcolor="black")
+    check_b.configure(justify='left')
+    check_b.configure(selectcolor="#ffffff")
+    check_b.configure(font=f'-family {font_family} -size {fontsize}')
+    return check_b
+
+
+def my_entry(frame: tk.LabelFrame, fontsize=11) -> tk.Entry:
+    entry = tk.Entry(frame)
+    entry.configure(font=f'-family {font_family} -size {fontsize}')
+    entry.configure(takefocus="")
+    entry.configure(cursor="fleur")
+    return entry
+
+
+def my_combobox(frame: tk.LabelFrame, fontsize=11) -> ttk.Combobox:
+    style = 'combostyle'
+    combo_style = ttk.Style()
+    if style not in ttk.Style().theme_names():
+        combo_style.theme_create(style, parent='alt', settings={
+            'TCombobox': {'configure': {
+                'selectbackground': 'gray',
+                'fieldbackground': 'white',
+                'background': 'white'}}})
+    combo_style.theme_use(style)
+    combobox = ttk.Combobox(frame, font=(font_family, fontsize))
+    combobox.configure(state='readonly')
+    combobox.configure(takefocus="")
+    return combobox
+
+
+def move_to_center(window: tk.Tk, width: int, height: int) -> None:
+    screen_width = root.winfo_screenwidth()
+    screen_height = root.winfo_screenheight()
+    x = (screen_width - width) // 2
+    y = (screen_height - height) // 2
+    window.geometry(f'{width}x{height}+{x}+{y}')
+    return
+
+
+def after_close(frame):
+    """
+    Deiconify root before destroy.
+    """
+
+    def func():
+        root.deiconify()
+        frame.destroy()
+
+    return func
+
+
+def scroll_text(window):
+    """
+    ScrolledText that shows logs.
+    """
+
+    def poll():
+        while True:
+            try:
+                msg = log_queue.get(block=False)
+                level = msg.levelname
+                msg = formatter.format(msg) + '\n'
+                scroll.insert('end', msg, level)
+                scroll.yview('end')
+            except queue.Empty:
+                break
+        # to avoid orphan poll()
+        if log.hasHandlers():
+            scroll.after(10, poll)
+        else:
+            return
+
+    # clean old handlers
+    for i in log.handlers:
+        log.removeHandler(i)
+    log_queue = queue.Queue()
+    formatter = logging.Formatter(fmt=FMT, datefmt=DATEFMT)
+    # do not add formatter to queuehandler, or msg will be formatted twice
+    queue_handler = handlers.QueueHandler(log_queue)
+    # give poll() time to quit
+    root.after(100, log.addHandler(queue_handler))
+    scroll = scrolledtext.ScrolledText(window)
+    scroll.tag_config('INFO', foreground='black')
+    scroll.tag_config('WARNING', foreground='orange')
+    scroll.tag_config('ERROR', foreground='red')
+    scroll.tag_config('CRITICAL', foreground='red')
+    scroll.tag_config('EXCEPTION', foreground='red')
+    scroll.pack(fill='both')
+    scroll.after(0, poll)
+
+
+def thread_wrap(function, arg_str, window, no_arg=False):
+    """
+    Wrap for callback.
+    Args:
+        function(callable): function to call
+        arg_str(str): string for function's argparse
+        window(Toplevel): window to hide
+        no_arg: function do not need args
+    """
+    try:
+        if not no_arg:
+            result = function(arg_str)
+        else:
+            result = function()
+    except Exception as e:
+        log.exception(str(e))
+        log.exception('Abort.')
+        messagebox.showinfo(message='Abort.')
+        root.deiconify()
+        return
+    if not no_arg:
+        messagebox.showinfo(message=f'Done. See {result[0].out} for details.')
+    else:
+        messagebox.showinfo(message='Install third-party software finished.')
+    window.withdraw()
+    root.deiconify()
+    return
+
+
+def open_file(entry, single=True, type_='file', entry2=None, title=''):
+    """
+    Set title, fill entry 1, empty entry 2.
+    """
+
+    def func():
+        if type_ != 'file':
+            a = filedialog.askdirectory(title=title)
+        else:
+            if single:
+                a = filedialog.askopenfilename(title=title)
+            else:
+                a = filedialog.askopenfilenames(title=title)
+        entry.delete(0, 'end')
+        entry.insert(0, a)
+        if entry2 is not None:
+            entry2.delete(0, 'end')
+
+    return func
+
+
+class Root:
+    def __init__(self, top=None):
+        '''This class configures and populates the toplevel window.
+           top is the toplevel containing window.'''
+        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
+        _fgcolor = '#000000'  # X11 color: 'black'
+        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
+        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
+        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
+        _tabfg1 = 'black'
+        _tabfg2 = 'black'
+        _tabbg1 = 'grey75'
+        _tabbg2 = 'grey89'
+        _bgmode = 'light'
+
+        img_dir = resources(name) / 'data'
+        photo_location1 = img_dir / 'button1.png'
+        photo_location2 = img_dir / 'button2.png'
+        photo_location3 = img_dir / 'button3.png'
+        photo_location4 = img_dir / 'button4.png'
+        global _img4
+        _img4 = tk.PhotoImage(file=photo_location4)
+        global _img0
+        _img0 = tk.PhotoImage(file=photo_location1)
+        global _img1
+        _img1 = tk.PhotoImage(file=photo_location2)
+        global _img2
+        _img2 = tk.PhotoImage(file=photo_location3)
+
+        top.geometry("800x450+400+0")
+        move_to_center(top, 800, 450)
+        top.minsize(120, 15)
+        top.resizable(1, 1)
+        top.title(name)
+        top.configure(background="#edf0f3")
+        top.configure(highlightbackground="#edf0f3")
+        top.configure(highlightcolor="black")
+        self.top = top
+
+        self.help_b = my_button(self.top)
+        self.help_b.place(relx=0.913, rely=0.067, height=40, width=40)
+        self.help_b.configure(command=run_help)
+        self.help_b.configure(image=_img4)
+
+        self.gb2fasta_b = my_button(self.top)
+        self.gb2fasta_b.place(relx=0.188, rely=0.288, height=100, width=100)
+        self.gb2fasta_b.configure(command=ui_gb2fasta)
+        self.gb2fasta_b.configure(image=_img0)
+
+        self.evaluate_b = my_button(self.top)
+        self.evaluate_b.place(relx=0.438, rely=0.288, height=100, width=100)
+        self.evaluate_b.configure(command=ui_evaluate)
+        self.evaluate_b.configure(image=_img1)
+
+        self.primer_b = my_button(self.top)
+        self.primer_b.place(relx=0.688, rely=0.288, height=100, width=100)
+        self.primer_b.configure(command=ui_primer)
+        self.primer_b.configure(image=_img2)
+
+        self.install_third_party = my_button(self.top)
+        self.install_third_party.place(relx=0.613, rely=0.865, height=30,
+                                       width=250)
+        self.install_third_party.configure(text='Install third-party software')
+        self.install_third_party.configure(command=run_install(self, self.top))
+
+        self.gb2fasta_label = my_label(self.top, 14)
+        self.gb2fasta_label.place(relx=0.188, rely=0.532, height=30, width=100)
+        self.gb2fasta_label.configure(text='''GB2Fasta''')
+
+        self.evaluate_label = my_label(self.top, 14)
+        self.evaluate_label.place(relx=0.45, rely=0.532, height=30, width=100)
+        self.evaluate_label.configure(text='''Evaluate''')
+
+        self.primer_label = my_label(self.top, 14)
+        self.primer_label.place(relx=0.713, rely=0.532, height=30, width=100)
+        self.primer_label.configure(text='''Primer''')
+
+        self.note_label = my_label(self.top, 14)
+        self.note_label.place(relx=0.35, rely=0.643, height=35, width=300)
+        self.note_label.configure(text='''Click button to run modules''')
+
+
+class GB2Fasta:
+    def __init__(self, top=None):
+        '''This class configures and populates the toplevel window.
+           top is the toplevel containing window.'''
+        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
+        _fgcolor = '#000000'  # X11 color: 'black'
+        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
+        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
+        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
+        _tabfg1 = 'black'
+        _tabfg2 = 'black'
+        _tabbg1 = 'grey75'
+        _tabbg2 = 'grey89'
+        _bgmode = 'light'
+        self.style = ttk.Style()
+        if sys.platform == "win32":
+            self.style.theme_use('winnative')
+        self.style.configure('.', background=_bgcolor)
+        self.style.configure('.', foreground=_fgcolor)
+        self.style.map('.', background=[('selected', _compcolor),
+                                        ('active', _ana2color)])
+        self.tooltip_font = "TkDefaultFont"
+
+        top.geometry("600x800+5+139")
+        move_to_center(top, 600, 800)
+        top.title("GB2Fasta")
+        top.configure(background="#edf0f3")
+        top.configure(highlightbackground="#edf0f3")
+        top.configure(highlightcolor="black")
+
+        self.top = top
+        self.gb = tk.StringVar()
+        self.gene = tk.StringVar()
+        self.molecular = tk.StringVar()
+        self.group = tk.StringVar()
+        self.og = tk.StringVar()
+        self.refseq = tk.StringVar()
+        self.count = tk.StringVar()
+        self.min_len = tk.StringVar()
+        self.max_len = tk.StringVar()
+        self.date_start = tk.StringVar()
+        self.date_end = tk.StringVar()
+        self.exclude = tk.StringVar()
+        self.query = tk.StringVar()
+        self.taxon = tk.StringVar()
+        self.out = tk.StringVar()
+        self.expand = tk.StringVar()
+        self.max_name_len = tk.StringVar()
+        self.max_gene_len = tk.StringVar()
+        self.unique = tk.StringVar()
+        self.allow_repeat = tk.IntVar()
+        self.allow_invert_repeat = tk.IntVar()
+        self.allow_mosaic_repeat = tk.IntVar()
+        self.no_divide = tk.IntVar()
+        self.rename = tk.IntVar()
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.025, rely=0.013, relheight=0.46
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Input''')
+
+        self.TSeparator1 = ttk.Separator(self.Labelframe1)
+        self.TSeparator1.place(relx=0.524, rely=0.19, relheight=0.541
+                               , bordermode='ignore')
+        self.TSeparator1.configure(orient="vertical")
+
+        self.gbfile_label = my_label(self.Labelframe1)
+        self.gbfile_label.place(relx=0.050, rely=0.057, height=35, width=100,
+                                bordermode='ignore')
+        self.gbfile_label.configure(text='''Genbank files''')
+
+        self.gb_entry = my_entry(self.Labelframe1)
+        self.gb_entry.place(relx=0.241, rely=0.057, relheight=0.095,
+                            relwidth=0.562, bordermode='ignore')
+        self.gb_entry.configure(textvariable=self.gb)
+        self.gb_entry_tooltip = ToolTip(self.gb_entry, self.tooltip_font,
+                                        '''gb format files''')
+
+        self.gb_file_b = my_button(self.Labelframe1, 12)
+        self.gb_file_b.place(relx=0.82, rely=0.054, height=35, width=90
+                             , bordermode='ignore')
+        self.gb_file_b.configure(command=open_file(self.gb_entry, single=False))
+        self.gb_file_b.configure(text='''Open''')
+
+        self.gene_label = my_label(self.Labelframe1)
+        self.gene_label.place(relx=0.035, rely=0.217, height=35, width=60,
+                              bordermode='ignore')
+        self.gene_label.configure(text='''Gene''')
+
+        self.gene_entry = my_entry(self.Labelframe1)
+        self.gene_entry.place(relx=0.201, rely=0.217, height=35,
+                              relwidth=0.314, bordermode='ignore')
+        self.gene_entry.configure(textvariable=self.gene)
+        self.gene_entry_tooltip = ToolTip(self.gene_entry, self.tooltip_font,
+                                          'gene name')
+
+        self.taxon_label = my_label(self.Labelframe1)
+        self.taxon_label.place(relx=0.035, rely=0.326, height=35, width=70
+                               , bordermode='ignore')
+        self.taxon_label.configure(text='''Taxonomy''')
+
+        self.molecular_label = my_label(self.Labelframe1)
+        self.molecular_label.place(relx=0.558, rely=0.217, height=35, width=80
+                                   , bordermode='ignore')
+        self.molecular_label.configure(text='''Molecular''')
+
+        self.TCombobox_molecular = my_combobox(self.Labelframe1)
+        self.TCombobox_molecular.place(relx=0.716, rely=0.217, height=35,
+                                       width=150, bordermode='ignore')
+        self.molecular_value_list = ['all', 'DNA', 'RNA', ]
+        self.TCombobox_molecular.configure(values=self.molecular_value_list)
+        self.TCombobox_molecular.configure(textvariable=self.molecular)
+        self.TCombobox_molecular.current(0)
+
+        self.group_label = my_label(self.Labelframe1)
+        self.group_label.place(relx=0.558, rely=0.326, height=35, width=60
+                               , bordermode='ignore')
+        self.group_label.configure(text='''Group''')
+
+        self.TCombobox_group = my_combobox(self.Labelframe1)
+        self.TCombobox_group.place(relx=0.716, rely=0.326, height=35, width=150,
+                                   bordermode='ignore')
+        self.group_value_list = ['all', 'animals', 'plants', 'fungi',
+                                 'protists',
+                                 'bacteria', 'archaea', 'viruses', ]
+        self.TCombobox_group.configure(values=self.group_value_list)
+        self.TCombobox_group.configure(textvariable=self.group)
+        self.TCombobox_group.current(0)
+
+        self.organelle_label = my_label(self.Labelframe1)
+        self.organelle_label.place(relx=0.035, rely=0.435, height=35, width=80
+                                   , bordermode='ignore')
+        self.organelle_label.configure(text='''Organelle''')
+
+        self.TCombobox_og = my_combobox(self.Labelframe1)
+        self.TCombobox_og.place(relx=0.201, rely=0.435, height=35, width=170,
+                                bordermode='ignore')
+        self.og_value_list = ['ignore', 'both', 'no', 'mitochondrion',
+                              'chloroplast', ]
+        self.TCombobox_og.configure(values=self.og_value_list)
+        self.TCombobox_og.configure(textvariable=self.og)
+        self.TCombobox_og.current(0)
+
+        self.refseq_label = my_label(self.Labelframe1)
+        self.refseq_label.place(relx=0.035, rely=0.541, height=35, width=70
+                                , bordermode='ignore')
+        self.refseq_label.configure(text='''RefSeq''')
+
+        self.TCombobox_refseq = my_combobox(self.Labelframe1)
+        self.TCombobox_refseq.place(relx=0.201, rely=0.541, height=35,
+                                    width=150, bordermode='ignore')
+        self.refseq_value_list = ['both', 'yes', 'no', ]
+        self.TCombobox_refseq.configure(values=self.refseq_value_list)
+        self.TCombobox_refseq.configure(textvariable=self.refseq)
+        self.TCombobox_refseq.current(0)
+        self.TCombobox_refseq_tooltip = ToolTip(self.TCombobox_refseq,
+                                                self.tooltip_font,
+                                                'Use RefSeq or not')
+
+        self.count_label = my_label(self.Labelframe1)
+        self.count_label.place(relx=0.035, rely=0.649, height=35, width=60
+                               , bordermode='ignore')
+        self.count_label.configure(text='''Count''')
+
+        self.count_entry = my_entry(self.Labelframe1)
+        self.count_entry.place(relx=0.201, rely=0.649, relheight=0.095
+                               , relwidth=0.314, bordermode='ignore')
+        self.count_entry.configure(textvariable=self.count)
+        self.count_entry_tooltip = ToolTip(
+            self.count_entry, self.tooltip_font,
+            'numbers of sequences to download, 0 for no limit')
+
+        self.len_label = my_label(self.Labelframe1)
+        self.len_label.place(relx=0.558, rely=0.435, height=35, width=60
+                             , bordermode='ignore')
+        self.len_label.configure(text='''Length''')
+
+        self.min_len_entry = my_entry(self.Labelframe1)
+        self.min_len_entry.place(relx=0.686, rely=0.435, relheight=0.095
+                                 , relwidth=0.087, bordermode='ignore')
+        self.min_len_entry.configure(textvariable=self.min_len)
+        self.min_len_entry_tooltip = ToolTip(self.min_len_entry,
+                                             self.tooltip_font,
+                                             'sequence length limit')
+
+        self.to_label = my_label(self.Labelframe1)
+        self.to_label.place(relx=0.785, rely=0.435, height=35, width=36
+                            , bordermode='ignore')
+        self.to_label.configure(text='''to''')
+
+        self.max_len_entry = my_entry(self.Labelframe1)
+        self.max_len_entry.place(relx=0.839, rely=0.435, relheight=0.095
+                                 , relwidth=0.14, bordermode='ignore')
+        self.max_len_entry.configure(textvariable=self.max_len)
+        self.min_len_entry.insert(0, '0')
+        self.max_len_entry.insert(0, '300000')
+
+        self.date_label = my_label(self.Labelframe1)
+        self.date_label.place(relx=0.558, rely=0.541, height=35, width=60
+                              , bordermode='ignore')
+        self.date_label.configure(text='''Date''')
+
+        self.date_start_entry = my_entry(self.Labelframe1)
+        self.date_start_entry.place(relx=0.686, rely=0.541, relheight=0.095
+                                    , relwidth=0.087, bordermode='ignore')
+        self.date_start_entry.configure(textvariable=self.date_start)
+        self.date_start_entry_tooltip = ToolTip(self.date_start_entry,
+                                                self.tooltip_font,
+                                                '''1970/1/1''')
+
+        self.to2_label = my_label(self.Labelframe1)
+        self.to2_label.place(relx=0.789, rely=0.541, height=35, width=36
+                             , bordermode='ignore')
+        self.to2_label.configure(text='''to''')
+
+        self.date_end_entry = my_entry(self.Labelframe1)
+        self.date_end_entry.place(relx=0.839, rely=0.541, relheight=0.095
+                                  , relwidth=0.136, bordermode='ignore')
+        self.date_end_entry.configure(textvariable=self.date_end)
+        self.date_end_entry_tooltip = ToolTip(self.date_end_entry,
+                                              self.tooltip_font,
+                                              '''2022/12/31''')
+
+        self.exclude_label = my_label(self.Labelframe1)
+        self.exclude_label.place(relx=0.558, rely=0.649, height=35, width=60
+                                 , bordermode='ignore')
+        self.exclude_label.configure(text='''Exclude''')
+
+        self.exclude_entry = my_entry(self.Labelframe1)
+        self.exclude_entry.place(relx=0.686, rely=0.649, relheight=0.095
+                                 , relwidth=0.279, bordermode='ignore')
+        self.exclude_entry.configure(textvariable=self.exclude)
+        self.exclude_entry_tooltip = ToolTip(self.exclude_entry,
+                                             self.tooltip_font,
+                                             '''exclude expression''')
+
+        self.query_label = my_label(self.Labelframe1)
+        self.query_label.place(relx=0.035, rely=0.813, height=35, width=60
+                               , bordermode='ignore')
+        self.query_label.configure(text='''Query''')
+
+        self.query_entry = my_entry(self.Labelframe1)
+        self.query_entry.place(relx=0.201, rely=0.813, relheight=0.095
+                               , relwidth=0.785, bordermode='ignore')
+        self.query_entry.configure(textvariable=self.query)
+        self.query_entry_tooltip = ToolTip(self.query_entry, self.tooltip_font,
+                                           '''Entrez query string''')
+
+        self.taxon_entry = my_entry(self.Labelframe1)
+        self.taxon_entry.place(relx=0.201, rely=0.326, relheight=0.095
+                               , relwidth=0.314, bordermode='ignore')
+        self.taxon_entry.configure(textvariable=self.taxon)
+
+        self.out_label = my_label(self.top)
+        self.out_label.place(relx=0.05, rely=0.563, height=36
+                             , width=60)
+        self.out_label.configure(text='''Output''')
+
+        self.out_entry = my_entry(self.top)
+        self.out_entry.place(relx=0.167, rely=0.563, relheight=0.045
+                             , relwidth=0.633)
+        self.out_entry.configure(textvariable=self.out)
+        self.out_entry_tooltip = ToolTip(self.out_entry, self.tooltip_font,
+                                         'output folder')
+        self.out_b = my_button(self.top, 12)
+        self.out_b.place(relx=0.833, rely=0.563, height=35, width=80)
+        self.out_b.configure(command=open_file(self.out_entry, type_='folder'))
+        self.out_b.configure(text='''Open''')
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.025, rely=0.65, relheight=0.176
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Advance''')
+
+        self.expand_label = my_label(self.Labelframe1)
+        self.expand_label.place(relx=0.185, rely=0.142, height=35
+                                , width=60, bordermode='ignore')
+        self.expand_label.configure(text='''Expand''')
+
+        self.expand_entry = my_entry(self.Labelframe1)
+        self.expand_entry.place(relx=0.297, rely=0.142, relheight=0.248
+                                , relwidth=0.187, bordermode='ignore')
+        self.expand_entry.configure(textvariable=self.expand)
+        self.expand_entry_tooltip = ToolTip(self.expand_entry,
+                                            self.tooltip_font,
+                                            '''expand for primer design''')
+
+        self.max_name_len_label = my_label(self.Labelframe1)
+        self.max_name_len_label.place(relx=0.08, rely=0.426, height=35
+                                      , width=130, bordermode='ignore')
+        self.max_name_len_label.configure(text='''Max name length''')
+
+        self.max_frag_len_label = my_label(self.Labelframe1)
+        self.max_frag_len_label.place(relx=0.045, rely=0.709, height=35
+                                      , width=150, bordermode='ignore')
+        self.max_frag_len_label.configure(text='''Max fragment length''')
+
+        self.max_name_len_entry = my_entry(self.Labelframe1)
+        self.max_name_len_entry.place(relx=0.297, rely=0.426, relheight=0.248
+                                      , relwidth=0.187, bordermode='ignore')
+        self.max_name_len_entry.configure(textvariable=self.max_name_len)
+        self.max_name_len_entry_tooltip = ToolTip(self.max_name_len_entry,
+                                                  self.tooltip_font,
+                                                  '''max feature name length''')
+
+        self.max_gene_len_entry = my_entry(self.Labelframe1)
+        self.max_gene_len_entry.place(relx=0.297, rely=0.709, relheight=0.248
+                                      , relwidth=0.187, bordermode='ignore')
+        self.max_gene_len_entry.configure(textvariable=self.max_gene_len)
+        self.max_gene_len_entry_tooltip = ToolTip(self.max_gene_len_entry,
+                                                  self.tooltip_font,
+                                                  '''max fragment sequence length''')
+        self.max_name_len_entry.insert(0, '100')
+        self.max_gene_len_entry.insert(0, '20000')
+
+        self.TSeparator2 = ttk.Separator(self.Labelframe1)
+        self.TSeparator2.place(relx=0.524, rely=0.135, relheight=0.78
+                               , bordermode='ignore')
+        self.TSeparator2.configure(orient="vertical")
+
+        self.allow_repeat_button = my_checkbutton(self.Labelframe1)
+        self.allow_repeat_button.place(relx=0.576, rely=0.142, relheight=0.248
+                                       , relwidth=0.276, bordermode='ignore')
+        self.allow_repeat_button.configure(text='''Allow repeat''')
+        self.allow_repeat_button.configure(variable=self.allow_repeat)
+
+        self.allow_invert_repeat_button = my_checkbutton(self.Labelframe1)
+        self.allow_invert_repeat_button.place(relx=0.576, rely=0.709,
+                                              relheight=0.248
+                                              , relwidth=0.361,
+                                              bordermode='ignore')
+        self.allow_invert_repeat_button.configure(
+            text='''Allow invert repeat''')
+        self.allow_invert_repeat_button.configure(
+            variable=self.allow_invert_repeat)
+
+        self.allow_mosaic_button = my_checkbutton(self.Labelframe1)
+        self.allow_mosaic_button.place(relx=0.576, rely=0.426, relheight=0.248
+                                       , relwidth=0.361, bordermode='ignore')
+        self.allow_mosaic_button.configure(text='''Allow mosaic repeat''')
+        self.allow_mosaic_button.configure(variable=self.allow_mosaic_repeat)
+
+        self.no_divide_b = my_checkbutton(self.top)
+        self.no_divide_b.place(relx=0.733, rely=0.488, relheight=0.044
+                               , relwidth=0.215)
+        self.no_divide_b.configure(text='''No divide''')
+        self.no_divide_b.configure(variable=self.no_divide)
+
+        self.rename_b = my_checkbutton(self.top)
+        self.rename_b.place(relx=0.467, rely=0.488, relheight=0.044
+                            , relwidth=0.243)
+        self.rename_b.configure(text='''Rename gene''')
+        self.rename_b.configure(variable=self.rename)
+
+        self.unique_label = my_label(self.top)
+        self.unique_label.place(relx=0.05, rely=0.488, height=35
+                                , width=69)
+        self.unique_label.configure(text='''Unique''')
+
+        self.TCombobox_unique = my_combobox(self.top)
+        self.TCombobox_unique.place(relx=0.167, rely=0.488, relheight=0.044
+                                    , relwidth=0.245)
+        self.unique_value_list = ['longest', 'first', 'no', ]
+        self.TCombobox_unique.configure(values=self.unique_value_list)
+        self.TCombobox_unique.configure(textvariable=self.unique)
+        self.TCombobox_unique.current(0)
+        self.TCombobox_unique_tooltip = ToolTip(
+            self.TCombobox_unique, self.tooltip_font,
+            'methods to remove redundant records')
+
+        self.run_b = my_button(self.top, 14)
+        self.run_b.place(relx=0.333, rely=0.863, height=40, width=189)
+        self.run_b.configure(command=run_gb2fasta(self, self.top))
+        self.run_b.configure(text='''Run''')
+
+
+class Evaluate:
+    def __init__(self, top=None):
+        '''This class configures and populates the toplevel window.
+           top is the toplevel containing window.'''
+        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
+        _fgcolor = '#000000'  # X11 color: 'black'
+        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
+        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
+        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
+        _tabfg1 = 'black'
+        _tabfg2 = 'black'
+        _tabbg1 = 'grey75'
+        _tabbg2 = 'grey89'
+        _bgmode = 'light'
+        self.style = ttk.Style()
+        if sys.platform == "win32":
+            self.style.theme_use('winnative')
+        self.style.configure('.', background=_bgcolor)
+        self.style.configure('.', foreground=_fgcolor)
+        self.style.map('.', background=[('selected', _compcolor),
+                                        ('active', _ana2color)])
+        self.tooltip_font = "TkDefaultFont"
+
+        top.geometry("600x450+109+248")
+        move_to_center(top, 600, 450)
+        top.title("Evaluate")
+        top.configure(background="#edf0f3")
+        top.configure(highlightbackground="#d9d9d9")
+        top.configure(highlightcolor="black")
+
+        self.top = top
+        self.fasta = tk.StringVar()
+        self.fasta_folder = tk.StringVar()
+        self.aln = tk.StringVar()
+        self.out = tk.StringVar()
+        self.size = tk.StringVar()
+        self.step = tk.StringVar()
+        self.quick = tk.IntVar()
+        self.ig = tk.IntVar()
+        self.iab = tk.IntVar()
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.017, rely=0.0, relheight=0.333
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Input''')
+
+        self.unalign_label = my_label(self.Labelframe1)
+        self.unalign_label.place(relx=0.03, rely=0.133, height=35, width=160
+                                 , bordermode='ignore')
+        self.unalign_label.configure(text='''Unaligned FASTA files''')
+        self.TLabel1_tooltip = ToolTip(self.unalign_label, self.tooltip_font,
+                                       'unaligned')
+
+        self.fasta_entry = my_entry(self.Labelframe1)
+        self.fasta_entry.place(relx=0.314, rely=0.133, relheight=0.233
+                               , relwidth=0.489, bordermode='ignore')
+        self.fasta_entry.configure(textvariable=self.fasta)
+        self.fasta_entry_tooltip = ToolTip(self.fasta_entry, self.tooltip_font,
+                                           '''unaligned fasta files''')
+
+        self.open_btn = my_button(self.Labelframe1)
+        self.open_btn.place(relx=0.82, rely=0.133, height=35, width=90
+                            , bordermode='ignore')
+        self.open_btn.configure(command=open_file(self.fasta_entry,
+                                                  single=False))
+        self.open_btn.configure(text='''Open''')
+
+        self.unalign_label2 = my_label(self.Labelframe1)
+        self.unalign_label2.place(relx=0.03, rely=0.4, height=35, width=160
+                                  , bordermode='ignore')
+        self.unalign_label2.configure(text='''Unaligned FASTA folder''')
+        self.TLabel1_tooltip = ToolTip(self.unalign_label2, self.tooltip_font,
+                                       '''unaligned''')
+
+        self.fasta_folder_entry = my_entry(self.Labelframe1)
+        self.fasta_folder_entry.place(relx=0.314, rely=0.4, relheight=0.233
+                                      , relwidth=0.489, bordermode='ignore')
+        self.fasta_folder_entry.configure(textvariable=self.fasta_folder)
+        self.fasta_folder_entry_tooltip = ToolTip(
+            self.fasta_folder_entry, self.tooltip_font,
+            'unaligned fasta files')
+        self.open1_btn = my_button(self.Labelframe1)
+        self.open1_btn.place(relx=0.82, rely=0.4, height=35, width=90
+                             , bordermode='ignore')
+        self.open1_btn.configure(command=open_file(self.fasta_folder_entry,
+                                                   type_='folder'))
+        self.open1_btn.configure(text='''Open''')
+
+        self.align_label = my_label(self.Labelframe1)
+        self.align_label.place(relx=0.03, rely=0.667, height=35, width=150
+                               , bordermode='ignore')
+        self.align_label.configure(text='''Aligned FASTA files''')
+        self.TLabel1_3_tooltip = ToolTip(self.align_label, self.tooltip_font,
+                                         '''aligned''')
+
+        self.aln_entry = my_entry(self.Labelframe1)
+        self.aln_entry.place(relx=0.314, rely=0.667, relheight=0.233
+                             , relwidth=0.489, bordermode='ignore')
+        self.aln_entry.configure(textvariable=self.aln)
+        self.aln_entry_tooltip = ToolTip(self.aln_entry, self.tooltip_font,
+                                         '''aligned fasta files''')
+        self.open2_btn = my_button(self.Labelframe1)
+        self.open2_btn.place(relx=0.82, rely=0.667, height=35, width=90
+                             , bordermode='ignore')
+        self.open2_btn.configure(command=open_file(self.aln_entry,
+                                                   single=False))
+        self.open2_btn.configure(text='''Open''')
+
+        self.out_label = my_label(self.top)
+        self.out_label.place(relx=0.117, rely=0.356, height=35, width=100)
+        self.out_label.configure(text='''Output folder''')
+        self.TLabel1_3_1_tooltip = ToolTip(self.out_label, self.tooltip_font,
+                                           '''output''')
+
+        self.out_entry = my_entry(self.top)
+        self.out_entry.place(relx=0.317, rely=0.356, relheight=0.078
+                             , relwidth=0.467)
+        self.out_entry.configure(textvariable=self.out)
+        self.out_entry_tooltip = ToolTip(self.out_entry, self.tooltip_font,
+                                         '''unaligned fasta files''')
+
+        self.open3_btn = my_button(self.top)
+        self.open3_btn.place(relx=0.8, rely=0.356, height=35, width=90)
+        self.open3_btn.configure(command=open_file(self.out_entry,
+                                                   type_='folder'))
+        self.open3_btn.configure(text='''Open''')
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.017, rely=0.467, relheight=0.156
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Sliding window''')
+
+        self.Checkbutton1 = my_checkbutton(self.Labelframe1)
+        self.Checkbutton1.place(relx=0.005, rely=0.429, relheight=0.3,
+                                relwidth=0.272, bordermode='ignore')
+        self.Checkbutton1.configure(text='''Skip sliding window''')
+        self.Checkbutton1.configure(variable=self.quick)
+
+        self.window_size_label = my_label(self.Labelframe1)
+        self.window_size_label.place(relx=0.314, rely=0.429, height=22, width=80
+                                     , bordermode='ignore')
+        self.window_size_label.configure(text='Window size')
+
+        self.step_len_label = my_label(self.Labelframe1)
+        self.step_len_label.place(relx=0.681, rely=0.429, height=22, width=80
+                                  , bordermode='ignore')
+        self.step_len_label.configure(text='''Step length''')
+
+        self.size_entry = my_entry(self.Labelframe1)
+        self.size_entry.place(relx=0.489, rely=0.357, relheight=0.5
+                              , relwidth=0.14, bordermode='ignore')
+        self.size_entry.configure(textvariable=self.size)
+
+        self.step_entry = my_entry(self.Labelframe1)
+        self.step_entry.place(relx=0.838, rely=0.357, relheight=0.5
+                              , relwidth=0.14, bordermode='ignore')
+        self.step_entry.configure(textvariable=self.step)
+        self.size_entry.insert(0, '500')
+        self.step_entry.insert(0, '50')
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.017, rely=0.644, relheight=0.156
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Advance''')
+
+        self.Checkbutton1 = my_checkbutton(self.Labelframe1)
+        self.Checkbutton1.place(relx=0.087, rely=0.429, relheight=0.3
+                                , relwidth=0.354, bordermode='ignore')
+        self.Checkbutton1.configure(text='''Ignore gaps in alignment''')
+        self.Checkbutton1.configure(variable=self.ig)
+
+        self.Checkbutton1_2 = my_checkbutton(self.Labelframe1)
+        self.Checkbutton1_2.place(relx=0.593, rely=0.429, relheight=0.3
+                                  , relwidth=0.354, bordermode='ignore')
+        self.Checkbutton1_2.configure(text='''Ignore ambiguous bases''')
+        self.Checkbutton1_2.configure(variable=self.iab)
+
+        self.run_b = my_button(self.top, 14)
+        self.run_b.place(relx=0.333, rely=0.867, height=40, width=189)
+        self.run_b.configure(command=run_evaluate(self, self.top))
+        self.run_b.configure(text='''Run''')
+
+
+class Primer:
+    def __init__(self, top=None):
+        '''This class configures and populates the toplevel window.
+           top is the toplevel containing window.'''
+        _bgcolor = '#edf0f3'  # Closest X11 color: 'gray94'
+        _fgcolor = '#000000'  # X11 color: 'black'
+        _compcolor = '#d9d9d9'  # X11 color: 'gray85'
+        _ana1color = '#d9d9d9'  # X11 color: 'gray85'
+        _ana2color = '#ececec'  # Closest X11 color: 'gray92'
+        _tabfg1 = 'black'
+        _tabfg2 = 'black'
+        _tabbg1 = 'grey75'
+        _tabbg2 = 'grey89'
+        _bgmode = 'light'
+        self.style = ttk.Style()
+        if sys.platform == "win32":
+            self.style.theme_use('winnative')
+        self.style.configure('.', background=_bgcolor)
+        self.style.configure('.', foreground=_fgcolor)
+        self.style.map('.', background=[('selected', _compcolor),
+                                        ('active', _ana2color)])
+        self.tooltip_font = "TkDefaultFont"
+
+        top.geometry("600x500+284+458")
+        move_to_center(top, 600, 600)
+        top.title("Primer")
+        top.configure(background="#edf0f3")
+        top.configure(highlightbackground="#d9d9d9")
+        top.configure(highlightcolor="black")
+
+        self.top = top
+        self.aln = tk.StringVar()
+        self.aln_folder = tk.StringVar()
+        self.out = tk.StringVar()
+        self.coverage = tk.StringVar()
+        self.mismatch = tk.StringVar()
+        self.resolution = tk.StringVar()
+        self.top_n = tk.StringVar()
+        self.pmin = tk.StringVar()
+        self.pmax = tk.StringVar()
+        self.amin = tk.StringVar()
+        self.amax = tk.StringVar()
+        self.size = tk.StringVar()
+        self.step = tk.StringVar()
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.017, rely=0.02, relheight=0.2
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Input''')
+
+        self.aln_fasta_label = my_label(self.Labelframe1)
+        self.aln_fasta_label.place(relx=0.052, rely=0.2, height=35, width=130
+                                   , bordermode='ignore')
+        self.aln_fasta_label.configure(text='''Aligned FASTA files''')
+        self.TLabel1_tooltip = ToolTip(self.aln_fasta_label, self.tooltip_font,
+                                       'unaligned')
+
+        self.aln_entry = my_entry(self.Labelframe1)
+        self.aln_entry.place(relx=0.314, rely=0.2, relheight=0.35,
+                             relwidth=0.489
+                             , bordermode='ignore')
+        self.aln_entry.configure(textvariable=self.aln)
+        self.aln_entry_tooltip = ToolTip(self.aln_entry, self.tooltip_font,
+                                         '''unaligned fasta files''')
+
+        self.out_b = my_button(self.Labelframe1)
+        self.out_b.place(relx=0.82, rely=0.2, height=35, width=90
+                         , bordermode='ignore')
+        self.out_b.configure(command=open_file(self.aln_entry, single=False))
+        self.out_b.configure(text='''Open''')
+
+        self.aln_folder_label = my_label(self.Labelframe1)
+        self.aln_folder_label.place(relx=0.052, rely=0.6, height=35, width=160
+                                    , bordermode='ignore')
+        self.aln_folder_label.configure(text='''Aligned FASTA folder''')
+        self.TLabel1_tooltip = ToolTip(self.aln_folder_label, self.tooltip_font,
+                                       'Folder with aligned fasta files')
+
+        self.aln_folder_entry = my_entry(self.Labelframe1)
+        self.aln_folder_entry.place(relx=0.314, rely=0.6, relheight=0.35
+                                    , relwidth=0.489, bordermode='ignore')
+        self.aln_folder_entry.configure(textvariable=self.aln_folder)
+        self.aln_folder_entry_tooltip = ToolTip(self.aln_folder_entry,
+                                                self.tooltip_font,
+                                                '''unaligned fasta files''')
+
+        self.folder_b = my_button(self.Labelframe1)
+        self.folder_b.place(relx=0.82, rely=0.6, height=35, width=90
+                            , bordermode='ignore')
+        self.folder_b.configure(command=open_file(self.aln_folder_entry,
+                                                  type_='folder'))
+        self.folder_b.configure(text='''Open''')
+
+        self.out_label = my_label(self.top)
+        self.out_label.place(relx=0.07, rely=0.24, height=35, width=150)
+        self.out_label.configure(text='''Output folder''')
+        self.TLabel1_3_1_tooltip = ToolTip(self.out_label, self.tooltip_font,
+                                           'Output')
+
+        self.out_entry = my_entry(self.top)
+        self.out_entry.place(relx=0.317, rely=0.24, relheight=0.07
+                             , relwidth=0.467)
+        self.out_entry.configure(textvariable=self.out)
+
+        self.out_b = my_button(self.top)
+        self.out_b.place(relx=0.8, rely=0.24, height=35, width=90)
+        self.out_b.configure(command=open_file(self.out_entry, type_='folder'))
+        self.out_b.configure(text='''Open''')
+
+        self.Labelframe1 = my_labelframe(self.top)
+        self.Labelframe1.place(relx=0.017, rely=0.34, relheight=0.38
+                               , relwidth=0.955)
+        self.Labelframe1.configure(text='''Advance''')
+
+        self.coverage_label = my_label(self.Labelframe1)
+        self.coverage_label.place(relx=0.07, rely=0.158, height=35
+                                  , width=70, bordermode='ignore')
+        self.coverage_label.configure(text='''Coverage''')
+
+        self.coverage_entry = my_entry(self.Labelframe1)
+        self.coverage_entry.place(relx=0.297, rely=0.142, relheight=0.184
+                                  , relwidth=0.192, bordermode='ignore')
+        self.coverage_entry.configure(textvariable=self.coverage)
+        self.coverage_entry_tooltip = ToolTip(self.coverage_entry,
+                                              self.tooltip_font,
+                                              '''minimal coverage of primer on alignment''')
+        self.coverage_entry.insert(0, '0.5')
+
+        self.mismatch_label = my_label(self.Labelframe1)
+        self.mismatch_label.place(relx=0.07, rely=0.368, height=35
+                                  , width=120, bordermode='ignore')
+        self.mismatch_label.configure(text='''Mismatch''')
+
+        self.res_label = my_label(self.Labelframe1)
+        self.res_label.place(relx=0.07, rely=0.579, height=35
+                             , width=130, bordermode='ignore')
+        self.res_label.configure(text='''Resolution''')
+
+        self.mismatch_entry = my_entry(self.Labelframe1)
+        self.mismatch_entry.place(relx=0.297, rely=0.368, relheight=0.184
+                                  , relwidth=0.192, bordermode='ignore')
+        self.mismatch_entry.configure(textvariable=self.mismatch)
+        self.mismatch_entry_tooltip = ToolTip(
+            self.mismatch_entry, self.tooltip_font,
+            'maximum mismatch bases in primer')
+
+        self.resolution_entry = my_entry(self.Labelframe1)
+        self.resolution_entry.place(relx=0.297, rely=0.579, relheight=0.184
+                                    , relwidth=0.192, bordermode='ignore')
+        self.resolution_entry.configure(textvariable=self.resolution)
+        self.resolution_entry_tooltip = ToolTip(
+            self.resolution_entry, self.tooltip_font,
+            'minimal resolution of amplified fragment''')
+        self.mismatch_entry.insert(0, '4')
+        self.resolution_entry.insert(0, '0.3')
+
+        self.TSeparator2 = ttk.Separator(self.Labelframe1)
+        self.TSeparator2.place(relx=0.524, rely=0.137, relheight=0.779
+                               , bordermode='ignore')
+        self.TSeparator2.configure(orient="vertical")
+
+        self.topn_label = my_label(self.Labelframe1)
+        self.topn_label.place(relx=0.07, rely=0.789, height=35
+                              , width=130, bordermode='ignore')
+        self.topn_label.configure(text='''Top n''')
+
+        self.top_n_entry = my_entry(self.Labelframe1)
+        self.top_n_entry.place(relx=0.297, rely=0.789, relheight=0.184
+                               , relwidth=0.192, bordermode='ignore')
+        self.top_n_entry.configure(textvariable=self.top_n)
+        self.top_n_entry_tooltip = ToolTip(self.top_n_entry, self.tooltip_font,
+                                           '''Only keep top best primers''')
+        self.top_n_entry.insert(0, '1')
+
+        self.primer_len_label = my_label(self.Labelframe1)
+        self.primer_len_label.place(relx=0.541, rely=0.158, height=35
+                                    , width=100, bordermode='ignore')
+        self.primer_len_label.configure(text='''Primer length''')
+
+        self.pmin_entry = my_entry(self.Labelframe1)
+        self.pmin_entry.place(relx=0.716, rely=0.158, relheight=0.184
+                              , relwidth=0.087, bordermode='ignore')
+        self.pmin_entry.configure(textvariable=self.pmin)
+
+        self.to_label1 = my_label(self.Labelframe1)
+        self.to_label1.place(relx=0.803, rely=0.158, height=35, width=36
+                             , bordermode='ignore')
+        self.to_label1.configure(text='''to''')
+
+        self.pmax_entry = my_entry(self.Labelframe1)
+        self.pmax_entry.place(relx=0.855, rely=0.158, relheight=0.184
+                              , relwidth=0.122, bordermode='ignore')
+        self.pmax_entry.configure(textvariable=self.pmax)
+        self.pmin_entry.insert(0, '20')
+        self.pmax_entry.insert(0, '30')
+
+        self.amp_len_label = my_label(self.Labelframe1)
+        self.amp_len_label.place(relx=0.541, rely=0.368, height=35
+                                 , width=120, bordermode='ignore')
+        self.amp_len_label.configure(text='''Amplicon size''')
+
+        self.amin_entry = my_entry(self.Labelframe1)
+        self.amin_entry.place(relx=0.716, rely=0.368, relheight=0.184
+                              , relwidth=0.087, bordermode='ignore')
+        self.amin_entry.configure(textvariable=self.amin)
+        self.amin_entry_tooltip = ToolTip(self.amin_entry, self.tooltip_font,
+                                          'including primer length')
+
+        self.to2_label = my_label(self.Labelframe1)
+        self.to2_label.place(relx=0.803, rely=0.368, height=35, width=36
+                             , bordermode='ignore')
+        self.to2_label.configure(text='''to''')
+
+        self.amax_entry = my_entry(self.Labelframe1)
+        self.amax_entry.place(relx=0.855, rely=0.368, relheight=0.184
+                              , relwidth=0.122, bordermode='ignore')
+        self.amax_entry.configure(textvariable=self.amax)
+        self.amin_entry.insert(0, '300')
+        self.amax_entry.insert(0, '800')
+
+        self.sliding_window_label = my_label(self.Labelframe1)
+        self.sliding_window_label.place(relx=0.541, rely=0.579, height=35,
+                                        width=130
+                                        , bordermode='ignore')
+        self.sliding_window_label.configure(text='''Sliding window size''')
+
+        self.sliding_window2_label = my_label(self.Labelframe1)
+        self.sliding_window2_label.place(relx=0.541, rely=0.789, height=35,
+                                         width=130
+                                         , bordermode='ignore')
+        self.sliding_window2_label.configure(text='''Sliding window step''')
+
+        self.size_entry = my_entry(self.Labelframe1)
+        self.size_entry.place(relx=0.803, rely=0.579, relheight=0.184
+                              , relwidth=0.14, bordermode='ignore')
+        self.size_entry.configure(textvariable=self.size)
+
+        self.step_entry = my_entry(self.Labelframe1)
+        self.step_entry.place(relx=0.803, rely=0.789, relheight=0.184
+                              , relwidth=0.14, bordermode='ignore')
+        self.step_entry.configure(textvariable=self.step)
+        self.size_entry.insert(0, '500')
+        self.step_entry.insert(0, '50')
+
+        self.run_b = my_button(self.top, 14)
+        self.run_b.place(relx=0.367, rely=0.82, height=40, width=180)
+        self.run_b.configure(command=run_primer(self, self.top))
+        self.run_b.configure(text='''Run''')
+
+
+class ToolTip(tk.Toplevel):
+    """ Provides a ToolTip widget for Tkinter. """
+
+    def __init__(self, wdgt, tooltip_font, msg=None, msgFunc=None,
+                 delay=0.5, follow=True):
+        self.wdgt = wdgt
+        self.parent = self.wdgt.master
+        tk.Toplevel.__init__(self, self.parent, bg='black', padx=1, pady=1)
+        self.withdraw()
+        self.overrideredirect(True)
+        self.msgVar = tk.StringVar()
+        if msg is None:
+            self.msgVar.set('No message provided')
+        else:
+            self.msgVar.set(msg)
+        self.msgFunc = msgFunc
+        self.delay = delay
+        self.follow = follow
+        self.visible = 0
+        self.lastMotion = 0
+        tk.Message(self, textvariable=self.msgVar, bg='#FFFFDD',
+                   font=tooltip_font,
+                   aspect=1000).grid()
+        self.wdgt.bind('<Enter>', self.spawn, '+')
+        self.wdgt.bind('<Leave>', self.hide, '+')
+        self.wdgt.bind('<Motion>', self.move, '+')
+
+    def spawn(self, event=None):
+        self.visible = 1
+        self.after(int(self.delay * 1000), self.show)
+
+    def show(self):
+        if self.visible == 1 and time() - self.lastMotion > self.delay:
+            self.visible = 2
+        if self.visible == 2:
+            self.deiconify()
+
+    def move(self, event):
+        self.lastMotion = time()
+        if self.follow is False:
+            self.withdraw()
+            self.visible = 1
+        self.geometry('+%i+%i' % (event.x_root + 20, event.y_root - 10))
+        try:
+            self.msgVar.set(self.msgFunc())
+        except:
+            pass
+        self.after(int(self.delay * 1000), self.show)
+
+    def hide(self, event=None):
+        self.visible = 0
+        self.withdraw()
+
+    def update(self, msg):
+        self.msgVar.set(msg)
+
+
+def _create_container(func):
+    '''Creates a ttk Frame with a given master, and use this new frame to
+    place the scrollbars and the widget.'''
+
+    def wrapped(cls, master, **kw):
+        container = ttk.Frame(master)
+        container.bind('<Enter>', lambda e: _bound_to_mousewheel(e, container))
+        container.bind('<Leave>',
+                       lambda e: _unbound_to_mousewheel(e, container))
+        return func(cls, container, **kw)
+
+    return wrapped
+
+
+def _bound_to_mousewheel(event, widget):
+    child = widget.winfo_children()[0]
+    if platform.system() == 'Windows' or platform.system() == 'Darwin':
+        child.bind_all('<MouseWheel>', lambda e: _on_mousewheel(e, child))
+        child.bind_all('<Shift-MouseWheel>', lambda e: _on_shiftmouse(e, child))
+    else:
+        child.bind_all('<Button-4>', lambda e: _on_mousewheel(e, child))
+        child.bind_all('<Button-5>', lambda e: _on_mousewheel(e, child))
+        child.bind_all('<Shift-Button-4>', lambda e: _on_shiftmouse(e, child))
+        child.bind_all('<Shift-Button-5>', lambda e: _on_shiftmouse(e, child))
+
+
+def _unbound_to_mousewheel(event, widget):
+    if platform.system() == 'Windows' or platform.system() == 'Darwin':
+        widget.unbind_all('<MouseWheel>')
+        widget.unbind_all('<Shift-MouseWheel>')
+    else:
+        widget.unbind_all('<Button-4>')
+        widget.unbind_all('<Button-5>')
+        widget.unbind_all('<Shift-Button-4>')
+        widget.unbind_all('<Shift-Button-5>')
+
+
+def _on_mousewheel(event, widget):
+    if platform.system() == 'Windows':
+        widget.yview_scroll(-1 * int(event.delta / 120), 'units')
+    elif platform.system() == 'Darwin':
+        widget.yview_scroll(-1 * int(event.delta), 'units')
+    else:
+        if event.num == 4:
+            widget.yview_scroll(-1, 'units')
+        elif event.num == 5:
+            widget.yview_scroll(1, 'units')
+
+
+def _on_shiftmouse(event, widget):
+    if platform.system() == 'Windows':
+        widget.xview_scroll(-1 * int(event.delta / 120), 'units')
+    elif platform.system() == 'Darwin':
+        widget.xview_scroll(-1 * int(event.delta), 'units')
+    else:
+        if event.num == 4:
+            widget.xview_scroll(-1, 'units')
+        elif event.num == 5:
+            widget.xview_scroll(1, 'units')
+
+
+def ui_gb2fasta():
+    global _top2, _w2
+    _top2 = tk.Toplevel(root)
+    root.iconify()
+    _top2.protocol('WM_DELETE_WINDOW', after_close(_top2))
+    _w2 = GB2Fasta(_top2)
+
+
+def ui_evaluate():
+    global _top3, _w3
+    _top3 = tk.Toplevel(root)
+    root.iconify()
+    _top3.protocol('WM_DELETE_WINDOW', after_close(_top3))
+    _w3 = Evaluate(_top3)
+
+
+def ui_primer():
+    # Creates a toplevel widget.
+    global _top4, _w4
+    _top4 = tk.Toplevel(root)
+    root.iconify()
+    _top4.protocol('WM_DELETE_WINDOW', after_close(_top4))
+    _w4 = Primer(_top4)
+
+
+def get_arg_str(value: tk.Variable, name: str, arg_str: str,
+                is_bool=False) -> str:
+    value_str = ''
+    if value.get():
+        if is_bool:
+            value_str = f'{name} '
+        else:
+            value_str = f'{name} {value.get()} '
+    arg_str += value_str
+    log.debug(f'{name} {value_str}')
+    return arg_str
+
+
+def run_gb2fasta(win, t: tk.Toplevel):
+    # todo: test options and functions
+    def f():
+        nonlocal win
+        arg_str = ''
+        arg_str = get_arg_str(win.gb, '-gb', arg_str)
+        arg_str = get_arg_str(win.gene, '-gene', arg_str)
+        arg_str = get_arg_str(win.molecular, '-molecular', arg_str)
+        arg_str = get_arg_str(win.group, '-group', arg_str)
+        arg_str = get_arg_str(win.og, '-og', arg_str)
+        arg_str = get_arg_str(win.refseq, '-refseq', arg_str)
+        arg_str = get_arg_str(win.count, '-count', arg_str)
+        arg_str = get_arg_str(win.min_len, '-min_len', arg_str)
+        arg_str = get_arg_str(win.max_len, '-max_len', arg_str)
+        arg_str = get_arg_str(win.date_start, '-date_start', arg_str)
+        arg_str = get_arg_str(win.date_end, '-date_end', arg_str)
+        arg_str = get_arg_str(win.exclude, '-exclude', arg_str)
+        arg_str = get_arg_str(win.query, '-query', arg_str)
+        arg_str = get_arg_str(win.taxon, '-taxon', arg_str)
+        arg_str = get_arg_str(win.out, '-out', arg_str)
+        arg_str = get_arg_str(win.expand, '-expand', arg_str)
+        arg_str = get_arg_str(win.max_name_len, '-max_name_len', arg_str)
+        arg_str = get_arg_str(win.max_gene_len, '-max_gene_len', arg_str)
+        arg_str = get_arg_str(win.unique, '-unique', arg_str)
+        arg_str = get_arg_str(win.allow_repeat, '-allow_repeat', arg_str,
+                              is_bool=True)
+        arg_str = get_arg_str(win.allow_invert_repeat, '-allow_invert_repeat',
+                              arg_str,
+                              is_bool=True)
+        arg_str = get_arg_str(win.allow_mosaic_repeat, '-allow_mosaic_repeat',
+                              arg_str,
+                              is_bool=True)
+        arg_str = get_arg_str(win.no_divide, '-no_divide', arg_str,
+                              is_bool=True)
+        arg_str = get_arg_str(win.rename, '-rename', arg_str, is_bool=True)
+        t.withdraw()
+        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
+        s = min(w, h) // 2
+        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
+        run = tk.Toplevel(root)
+        run.geometry(size)
+        run.title('Running...')
+        run.wm_transient()
+        frame = ttk.Frame(run)
+        frame.pack(fill='both')
+        scroll_text(frame)
+        r = threading.Thread(target=thread_wrap,
+                             args=(gb2fasta_main, arg_str, run),
+                             daemon=True)
+        r.start()
+
+    return f
+
+
+def run_evaluate(win, t: tk.Toplevel):
+    # todo: test options and functions
+    def f():
+        nonlocal win
+        arg_str = ''
+        arg_str = get_arg_str(win.fasta, '-fasta', arg_str)
+        arg_str = get_arg_str(win.fasta_folder, '-fasta_folder', arg_str)
+        arg_str = get_arg_str(win.aln, '-aln', arg_str)
+        arg_str = get_arg_str(win.out, '-out', arg_str)
+        arg_str = get_arg_str(win.size, '-size', arg_str)
+        arg_str = get_arg_str(win.step, '-step', arg_str)
+        arg_str = get_arg_str(win.quick, '-quick', arg_str, is_bool=True)
+        arg_str = get_arg_str(win.ig, '-ig', arg_str, is_bool=True)
+        arg_str = get_arg_str(win.iab, '-iab', arg_str, is_bool=True)
+        t.withdraw()
+        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
+        s = min(w, h) // 2
+        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
+        run = tk.Toplevel(root)
+        run.geometry(size)
+        run.title('Running...')
+        run.wm_transient()
+        frame = ttk.Frame(run)
+        frame.pack(fill='both')
+        scroll_text(frame)
+        r = threading.Thread(target=thread_wrap,
+                             args=(evaluate_main, arg_str, run),
+                             daemon=True)
+        r.start()
+
+    return f
+
+
+def run_primer(win, t: tk.Toplevel):
+    # todo: test options and functions
+    def f():
+        nonlocal win
+        arg_str = ''
+        arg_str = get_arg_str(win.aln, '-aln', arg_str)
+        arg_str = get_arg_str(win.aln_folder, '-aln_folder', arg_str)
+        arg_str = get_arg_str(win.out, '-out', arg_str)
+        arg_str = get_arg_str(win.coverage, '-coverage', arg_str)
+        arg_str = get_arg_str(win.mismatch, '-mismatch', arg_str)
+        arg_str = get_arg_str(win.resolution, '-resolution', arg_str)
+        arg_str = get_arg_str(win.top_n, '-top_n', arg_str)
+        arg_str = get_arg_str(win.pmin, '-pmin', arg_str)
+        arg_str = get_arg_str(win.pmax, '-pmax', arg_str)
+        arg_str = get_arg_str(win.amin, '-amin', arg_str)
+        arg_str = get_arg_str(win.amax, '-amax', arg_str)
+        arg_str = get_arg_str(win.size, '-size', arg_str)
+        arg_str = get_arg_str(win.step, '-step', arg_str)
+        arg_str += '-primer'
+        t.withdraw()
+        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
+        s = min(w, h) // 2
+        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
+        run = tk.Toplevel(root)
+        run.geometry(size)
+        run.title('Running...')
+        run.wm_transient()
+        frame = ttk.Frame(run)
+        frame.pack(fill='both')
+        scroll_text(frame)
+        r = threading.Thread(target=thread_wrap,
+                             args=(primer_main, arg_str, run),
+                             daemon=True)
+        r.start()
+
+    return f
+
+
+def run_help():
+    url = 'https://github.com/wpwupingwp/barcodefinder'
+    webbrowser.open(url, new=2)
+
+
+def run_install(win, t: tk.Toplevel):
+    def f():
+        t.withdraw()
+        w, h = root.winfo_screenwidth(), root.winfo_screenheight()
+        s = min(w, h) // 2
+        size = f'{s}x{int(s * 0.618)}+{w // 3}+{h // 3}'
+        run = tk.Toplevel(root)
+        run.geometry(size)
+        run.title('Running...')
+        run.wm_transient()
+        frame = ttk.Frame(run)
+        frame.pack(fill='both')
+        scroll_text(frame)
+        r = threading.Thread(target=thread_wrap,
+                             args=(get_all_third_party, '', run, True),
+                             daemon=True)
+        r.start()
+
+    return f
+
+
+def ui_main():
+    global root
+    root = tk.Tk()
+    root.protocol('WM_DELETE_WINDOW', root.destroy)
+    root.title('Organelle Genome Utilities')
+    # Creates a toplevel widget.
+    global _top1, _w1
+    _top1 = root
+    _w1 = Root(_top1)
+    root.mainloop()
+
+
+if __name__ == '__main__':
+    ui_main()
```

### Comparing `ogu-1.52/src/OGU/utils.py` & `ogu-1.54/src/OGU/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,740 +1,739 @@
-#!/usr/bin/python3
-import re
-import logging
-import platform
-import subprocess
-try:
-    from collections import Iterable
-except ImportError:
-    from collections.abc import Iterable
-from functools import lru_cache
-from pathlib import Path
-from queue import Queue
-from shutil import unpack_archive
-from sys import argv, version_info
-from threading import Thread
-from urllib.parse import quote
-from urllib.request import urlopen
-from zipfile import ZipFile
-from pkg_resources import resource_filename
-
-from Bio.Seq import Seq
-from OGU.global_vars import log, name, FMT, DATEFMT
-
-
-# hosting in non-free AWS S3 server
-aws_url = 'https://ogu2023.s3.ap-east-1.amazonaws.com/'
-test_url = 'https://s3.ap-east-1.amazonaws.com'
-# font family
-if platform.system() == 'Windows':
-    font_family = 'Arial'
-else:
-    font_family = 'Helvetica'
-
-
-class BlastResult:
-    # slightly faster than namedtuple
-    __slots = ('query_id', 'hit_id', 'query_seq', 'ident_num', 'mismatch_num',
-               'bitscore_raw', 'query_start', 'query_end', 'hit_start',
-               'hit_end')
-
-    def __init__(self, line):
-        record = line.strip().split('\t')
-        self.query_id, self.hit_id, self.query_seq = record[0:3]
-        (self.ident_num, self.mismatch_num, self.bitscore_raw,
-         self.query_start, self.query_end, self.hit_start,
-         self.hit_end) = [int(i) for i in record[3:]]
-
-    def __repr__(self):
-        fmt = ('query_id: {}\thit_id: {}\tbitscore_raw: {}\tquery_start:{}\t'
-               'query_end: {}\thit_start: {}\thit_end: {}')
-        return fmt.format(self.query_id, self.hit_id, self.bitscore_raw,
-                          self.query_start, self.query_end, self.hit_start,
-                          self.hit_end)
-
-
-def check_system():
-    """
-    # primer3-py is currently unavailable on Windows with Python 3.9/3.10
-    # 2023.1 solved.
-    f-strings are not available on Python 3.5 or older.
-    """
-    if version_info.minor < 9:
-        raise RuntimeError('Python 3.9 or newer is required.')
-    if platform.system() == 'Windows':
-        if version_info.minor > 11:
-            # raise RuntimeError('Python 3.7 or 3.8 is required.')
-            raise RuntimeError('Do not support python 3.12 or higher.')
-    return
-
-
-def arg_to_str(arg) -> str:
-    s = ''
-    arg_dict = vars(arg)
-    for key, value in arg_dict.items():
-        if isinstance(value, str):
-            pass
-        elif isinstance(value, Iterable):
-            value = ' '.join(value)
-        elif value is None:
-            continue
-        elif isinstance(value, bool):
-            if value:
-                value = ''
-            else:
-                # Assume all bool option using action='store_true'
-                continue
-        s += f' -{key} {value}'
-    return s
-
-
-def add_file_log(arg):
-    """
-    Add file handler if not exist.
-    Note that "log" is a global variable.
-    """
-    has_file_hdl = any([type(i)==logging.FileHandler for i in log.handlers])
-    if has_file_hdl:
-        pass
-    else:
-        log_file = arg.out / 'Log.txt'
-        log_file_handler = logging.FileHandler(log_file, mode='a')
-        log_file_handler.setLevel(logging.DEBUG)
-        log_file_handler.setFormatter(
-            logging.Formatter(fmt=FMT, datefmt=DATEFMT))
-        log.addHandler(log_file_handler)
-        log.debug('Add file handler.')
-        log.debug('Arguments:')
-        log.debug(' '.join(argv))
-    return
-
-
-def move(source: Path, dest, copy=False):
-    """
-    Move source to dest and return dest.
-    If set "copy", copy source to dest instead of move.
-    Because Path.rename could not move file across different filesystem or
-    drive, have to use copy and delete to implement "move".
-    Warning:
-        This function does not check whether dest exists or not.
-    Args:
-        source(Path): old path
-        dest(Path or str): new path
-        copy(bool): copy or move
-    Return:
-        dest(Path): new path
-    """
-    source = Path(source).absolute()
-    dest = Path(dest).absolute()
-    # avoid useless copy
-    # Path.samefile may raise FileNotFoundError
-    if source == dest:
-        log.debug(f'{source} and {dest} are same.')
-    else:
-        # read_bytes/write_bytes includes open, read/write and close steps
-        dest.write_bytes(source.read_bytes())
-        if not copy:
-            source.unlink()
-    return dest
-
-
-def init_out(arg):
-    """
-    Initilize output folder.
-    Args:
-        arg(NameSpace): arguments
-    Returns:
-        arg(NameSpace): arguments
-    """
-    if not hasattr(arg, 'out') or arg.out is None:
-        log.warning('Output folder was not set.')
-        log.info('\tUse "Result" instead.')
-        arg.out = Path().cwd().absolute() / 'Result'
-    else:
-        arg.out = Path(arg.out).absolute()
-    if arg.out.exists() and len(list(arg.out.iterdir())) == 0:
-        from OGU import global_vars
-        if not global_vars.global_dict.get('out_inited', False):
-            log.warning(f'Output folder {arg.out} exists.')
-            arg.out = arg.out / (arg.out.name+'_')
-            log.info(f'Use {arg.out} instead.')
-            if arg.out.exists():
-                log.error(f'{arg.out} exists, too!')
-                raise SystemExit(-1)
-        else:
-            pass
-    arg._gb = arg.out / 'GenBank'
-    arg._fasta = arg.out / 'Fasta'
-    arg._divide = arg.out / 'Divide'
-    arg._expand = arg.out / 'Expanded_fasta'
-    arg._unique = arg.out / 'Unique'
-    arg._align = arg.out / 'Alignment'
-    arg._evaluate = arg.out / 'Evaluate'
-    arg._primer = arg.out / 'Primer'
-    arg._tmp = arg.out / 'Temp'
-    try:
-        arg.out.mkdir()
-        arg._gb.mkdir()
-        arg._fasta.mkdir()
-        arg._divide.mkdir()
-        arg._expand.mkdir()
-        arg._unique.mkdir()
-        arg._align.mkdir()
-        arg._evaluate.mkdir()
-        arg._primer.mkdir()
-        arg._tmp.mkdir()
-    except Exception:
-        log.debug('Folder exists.')
-    out_inited = True
-    return arg
-
-
-def clean_tmp(filename: Path):
-    if filename.is_dir():
-        for i in filename.glob('*'):
-            i.unlink()
-    elif filename.is_file():
-        for i in filename.parent.glob(f'{filename.name}*'):
-            i.unlink()
-    return
-
-
-@lru_cache(maxsize=None)
-def gene_rename(old_name: str, genbank_format=False) -> (str, str):
-    """
-    Old doc:
-        Different name of same gene will cause data to be split to numerous
-        files instead of one and some data may be dropped.
-
-        For chloroplast genes, the author summarized various kinds of
-        annotation error of gene name or synonyms and try to use regular
-        expression to fix it.
-
-        Ideally, use BLAST to re-annotate sequence is the best(and slow) way to
-        find the correct name. This function only offers a "hotfix" which is
-        enough.
-    Rename plastid genes.
-    May be dangerous.
-    Will cache results.
-    Args:
-        old_name: old gene name
-        genbank_format: use style like "trnH-GUG" or "trnHgug"
-    Returns:
-        new_name(str): new name, if fail, return old name
-        gene_type(str): gene types, guessed from name
-    """
-    lower = old_name.lower()
-    # (trna|trn(?=[b-z]))
-    s = re.compile(r'(\d+\.?\d?)(s|rrn|rdna)')
-    if lower.startswith('trn'):
-        pattern = re.compile(r'([atcgu]{3})')
-        prefix = 'trn'
-        aa_letter = 'X'
-        try:
-            anticodon = Seq(re.search(pattern, lower[3:]).group(1))
-        except Exception:
-            return old_name, 'bad_name'
-        # rna editing? trnI-CAU
-        if anticodon == 'cau' and lower.startswith('trni'):
-            aa_letter = 'I'
-        # for trnfM-CAU
-        elif lower.startswith('trnfm'):
-            prefix = 'trnf'
-            aa_letter = 'M'
-        else:
-            try:
-                aa_letter = anticodon.reverse_complement_rna().translate().upper()
-                if aa_letter == '*':
-                    aa_letter = 'UNKNOWN'
-            except Exception:
-                return old_name, 'bad_name'
-            # anticodon = anticodon.transcribe()
-        if genbank_format:
-            new_name = f'{prefix}{aa_letter}-{anticodon.upper()}'
-        else:
-            new_name = f'{prefix}{aa_letter}_{anticodon.upper()}'
-        gene_type = 'tRNA'
-    elif lower.startswith('rrn'):
-        pattern = re.compile(r'(\d+\.?\d?)')
-        try:
-            number = re.search(pattern, lower).group(1)
-        except Exception:
-            return old_name, 'bad_name'
-        new_name = 'rrn{}'.format(number)
-        gene_type = 'rRNA'
-    elif re.search(s, lower) is not None:
-        new_name = 'rrn{}'.format(re.search(s, lower).group(1))
-        gene_type = 'rRNA'
-    else:
-        pattern = re.compile(r'[^a-z]*'
-                             '(?P<gene>[a-z]+)'
-                             '[^a-z0-9]*'
-                             '(?P<suffix>[a-z]|[0-9]+)')
-        match = re.search(pattern, lower)
-        try:
-            gene = match.group('gene')
-            suffix = match.group('suffix')
-        except Exception:
-            return old_name, 'bad_name'
-        new_name = '{}{}'.format(gene, suffix.upper())
-        # capitalize last letter
-        if len(new_name) > 3:
-            s = list(new_name)
-            if s[-1].isalpha():
-                new_name = '{}{}'.format(
-                    ''.join(s[:-1]), ''.join(s[-1]).upper())
-        gene_type = 'normal'
-    if len(lower) >= 15:
-        gene_type = 'suspicious_name'
-    return new_name, gene_type
-
-
-def plastid_rename():
-    """
-    Use name database.
-    """
-    pass
-
-
-def safe_average(x):
-    """
-    Safe average.
-    """
-    if len(x) == 0:
-        return 0
-    else:
-        return sum(x) / len(x)
-
-
-def safe_path(old):
-    """
-    Remove illegal character in file path or name.
-    """
-    return re.sub(r'\W', '_', old)
-
-
-def accessible(name: Path, type_: str) -> bool:
-    """
-    Check given path is accessible or not.
-    Given path does not exist.
-    Args:
-        name(Path): folder or file, absolute path
-        type_(str): 'folder' or 'file'
-    Return:
-        ok(bool): accessible or not
-    """
-    p = Path(name)
-    if type_ == 'folder':
-        try:
-            p.mkdir()
-            p.rmdir()
-            ok = True
-        except PermissionError:
-            ok = False
-    elif type_ == 'file':
-        try:
-            p.touch()
-            p.unlink()
-            ok = True
-        except PermissionError:
-            ok = False
-    else:
-        log.critical(f'Illegal type: {type_}')
-        ok = False
-    return ok
-
-
-def test_cmd(program, option='-version') -> bool:
-    """
-    Test given program and option is ok to run or not.
-    Args:
-        program(Path or str): program path, could be relative path if it can
-        be found in $PATH or %PATH%
-        option(str): option for program, usually use "-v" to show version to
-        test the program
-    Return:
-        success(bool): success or not
-    """
-    program = Path(program)
-    if program.exists():
-        program.chmod(0o755)
-    cmd = f'{program} {option}'
-    test = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL,
-                          stderr=subprocess.DEVNULL)
-    success = True if test.returncode == 0 else False
-    return success
-
-
-def get_third_party_path():
-    """
-    Get third_party folder.
-    If do not exist, create it.
-    If cannot access, report.
-    Return:
-        success(bool): ok or not
-        third_party(Path): absolute path of third_party folder
-    """
-    third_party = Path().home().absolute() / '.OGU'
-    success = False
-    if not third_party.exists():
-        log.debug(f'Create folder {third_party}')
-        try:
-            third_party.mkdir()
-        except Exception:
-            log.critical(f'Failed to create {third_party}.'
-                         'Please contact the administrator.')
-            return success, third_party
-    if not accessible(third_party/'test', 'file'):
-        log.critical(f'Failed to access {third_party}.'
-                     f'Please contact the administrator.')
-        return success, third_party
-    success = True
-    return success, third_party
-
-
-# todo test in linux and windows
-def get_software(software: str, url: str, filename: Path,
-                 third_party: Path, home_bin: Path, test_option='-version'):
-    log.warning(f'Cannot find {software}, try to install. May cost minutes')
-    try:
-        # 50kb/10s=5kb/s, enough for test
-        _ = urlopen(test_url, timeout=10)
-    except Exception:
-        log.critical('Cannot connect to Server.'
-                     'Please check your Internet connection.')
-        raise SystemExit(-1)
-    try:
-        # file is 10mb or larger
-        log.info(f'Downloading {filename.name} from {url}')
-        down = urlopen(f'{url}', timeout=100)
-    except Exception:
-        log.critical(f'Cannot download {software}. '
-                     f'Please manually download it from {url}')
-        raise SystemExit(-1)
-    down_file = filename
-    with open(down_file, 'wb') as out:
-        try:
-            _ = down.read()
-        except TimeoutError:
-            log.critical(f'Download {software} timeout.'
-                         f'Please manually download it from {url}')
-            raise SystemExit(-1)
-        out.write(_)
-    log.info(f'{filename.name} got. Installing...')
-    try:
-        # unpack_archive(down_file, third_party/fileinfo[system][1])
-        unpack_archive(down_file, third_party)
-    except Exception:
-        log.critical(f'The {software} file is damaged. '
-                     f'Please recheck your connection.')
-        raise SystemExit(-1)
-    if software == 'mafft.bat':
-        for i in ('bin', 'libexec'):
-            subfolder = home_bin.parent / 'mafftdir' / i
-            # windows use different path
-            if subfolder.exists():
-                for file in subfolder.iterdir():
-                    file.chmod(0o755)
-    assert test_cmd(home_bin, test_option)
-    log.info(f'{software} installed successfully.')
-    return True
-
-
-def get_blast(third_party=None, result=None) -> (bool, str):
-    """
-    Get BLAST location.
-    If BLAST was found, assume makeblastdb is found, too.
-    If not found, download it.
-    Args:
-        third_party(Path or None): path for install
-        result(Queue): return values
-    Return:
-        ok(bool): success or not
-        blast(str): blast path
-    """
-    if third_party is None:
-        third_party_ok, third_party = get_third_party_path()
-        if not third_party_ok:
-            return third_party_ok, ''
-    blast = 'blastn'
-    home_blast = third_party / 'ncbi-blast-2.13.0+' / 'bin' / blast
-    # in Windows, ".exe" can be omitted
-    # win_home_blast = home_blast.with_name('blastn.exe')
-    ok = False
-    # older than 2.8.1 is buggy
-    original_url = ('https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.13.0/'
-                    'ncbi-blast-2.13.0+')
-    file_prefix = 'ncbi-blast-2.13.0+'
-    fileinfo = {'Linux': file_prefix+'-x64-linux.tar.gz',
-                'Darwin': file_prefix+'-x64-macosx.tar.gz',
-                'Windows': file_prefix+'-win64.zip'}
-                #'Windows': file_prefix + '-x64-win64.tar.gz'}
-    system = platform.system()
-    filename = fileinfo[system]
-    down_url = f'{aws_url}{quote(filename)}'
-    # three software use different name pattern
-    down_file = third_party / filename
-    if test_cmd(blast):
-        ok = True
-        home_blast = str(blast)
-    elif test_cmd(home_blast):
-        ok = True
-        home_blast = str(home_blast)
-    else:
-        ok = get_software(blast, down_url, down_file, third_party, home_blast)
-    if result is not None and ok:
-        result.put(('BLAST', ok))
-    return ok, str(home_blast)
-
-
-def get_iqtree(third_party=None, result=None) -> (bool, str):
-    """
-    Get iqtree location.
-    If not found, download it.
-    Args:
-        third_party(Path or None): path for install
-        result(Queue): return values
-    Return:
-        ok(bool): success or not
-        iqtree(str): blast path
-    """
-    if third_party is None:
-        third_party_ok, third_party = get_third_party_path()
-        if not third_party_ok:
-            return third_party_ok, ''
-    iqtree = 'iqtree2'
-    # in Windows, ".exe" can be omitted
-    ok = False
-    original_url = 'https://github.com/iqtree/iqtree2/releases/download/v2.2.0/'
-    # platform: (filename, folder)
-    fileinfo = {'Linux': ('iqtree-2.2.2.2-Linux.tar.gz', 'iqtree-2.2.2.2-Linux'),
-                'Darwin': ('iqtree-2.2.2.2-MacOSX.zip', 'iqtree-2.2.2.2-MacOSX'),
-                'Windows': ('iqtree-2.2.2.2-Windows.zip',
-                            'iqtree-2.2.2.2-Windows')}
-    system = platform.system()
-    filename = fileinfo[system][0]
-    down_url = f'{aws_url}{quote(filename)}'
-    home_iqtree = third_party / fileinfo[system][1] / 'bin' / iqtree
-    down_file = third_party / fileinfo[system][0]
-    if test_cmd(iqtree):
-        ok = True
-        home_iqtree = str(iqtree)
-    elif test_cmd(home_iqtree):
-        ok = True
-    else:
-        ok = get_software(iqtree, down_url, down_file, third_party,
-                          home_iqtree)
-    if result is not None and ok:
-        result.put(('IQTREE', ok))
-    return ok, str(home_iqtree)
-
-
-def get_mafft(third_party=None, result=None) -> (bool, str):
-    """
-    Get mafft location.
-    If not found, download it.
-    Args:
-        third_party(Path or None): path for install
-        result(Queue): return values
-    Return:
-        ok(bool): success or not
-        mafft(str): mafft path
-    """
-    if third_party is None:
-        third_party_ok, third_party = get_third_party_path()
-        if not third_party_ok:
-            return third_party_ok, ''
-    system = platform.system()
-    mafft = 'mafft.bat'
-    # in Windows, ".exe" can be omitted
-    # win_home_blast = home_blast.with_name('blastn.exe')
-    ok = False
-    original_url = 'https://mafft.cbrc.jp/alignment/software/'
-    # system: {filename, folder}
-    fileinfo = {'Linux': ('mafft-7.511-linux.tgz', 'mafft-linux64'),
-                'Darwin': ('mafft-7.511-mac.zip', 'mafft-mac'),
-                'Windows': ('mafft-7.511-win64-signed.zip', 'mafft-win')}
-    home_mafft = third_party / fileinfo[system][1] / mafft
-    system = platform.system()
-    filename = fileinfo[system][0]
-    down_url = f'{aws_url}{quote(filename)}'
-    down_file = third_party / fileinfo[system][0]
-    # mafft use '--version' to test
-    test_option = '--version'
-    if test_cmd(mafft, test_option):
-        ok = True
-        home_mafft = str(mafft)
-    elif test_cmd(home_mafft, test_option):
-        ok = True
-    else:
-        ok = get_software(mafft, down_url, down_file, third_party, home_mafft,
-                          test_option=test_option)
-    if result is not None and ok:
-        result.put(('MAFFT', ok))
-    return ok, str(home_mafft)
-
-
-def get_all_third_party(skip_blast=True) -> bool:
-    """
-    Use three threads to speed up.
-    """
-    log.info('Try to locate or install all third-party software.')
-    third_party_ok, third_party = get_third_party_path()
-    if not third_party_ok:
-        return False
-    result_queue = Queue()
-    iqtree = Thread(target=get_iqtree, args=(third_party, result_queue),
-                    daemon=True)
-    mafft = Thread(target=get_mafft, args=(third_party, result_queue),
-                   daemon=True)
-    if not skip_blast:
-        blast = Thread(target=get_blast, args=(third_party, result_queue),
-                       daemon=True)
-        blast.start()
-        blast.join()
-    iqtree.start()
-    mafft.start()
-    iqtree.join()
-    mafft.join()
-    while not result_queue.empty():
-        name, ok = result_queue.get()
-        if ok:
-            log.info(f'Got {name}.')
-        else:
-            log.error(f'Failed to got {name}.')
-            return False
-    return True
-
-
-def parse_blast_tab(filename):
-    """
-    Parse BLAST result (tab format).
-    """
-    query = []
-    with open(filename, 'r', encoding='utf-8') as raw:
-        for line in raw:
-            if line.startswith('# BLAST'):
-                yield query
-                query = []
-            elif line.startswith('#'):
-                pass
-            else:
-                query.append(BlastResult(line))
-    pass
-
-
-def download_taxon(data_folder) -> Path:
-    zip_file = data_folder / 'taxdmp.zip'
-    if zip_file.exists():
-        pass
-    else:
-        url = 'https://ftp.ncbi.nih.gov/pub/taxonomy/taxdmp.zip'
-        with urlopen(url) as response, zip_file.open('wb') as out_file:
-            data = response.read()
-            out_file.write(data)
-    return zip_file
-
-
-def init_lineage():
-    """
-    Only called by setup.py
-    """
-    global name
-    data_folder = Path(
-        resource_filename(name, 'data/button1.png')).absolute().parent
-    zip_file = download_taxon(data_folder)
-    with ZipFile(zip_file, 'r') as dumpfile:
-        dumpfile.extract('names.dmp', path='.')
-        dumpfile.extract('nodes.dmp', path='.')
-    id_name = {}
-    id_rank = {}
-    superkingdoms = set()
-    kingdoms = set()
-    phyla = set()
-    classes = set()
-    animal_orders = set()
-    other_orders = set()
-    plant_family = set()
-    other_family = set()
-    genus = set()
-    species = set()
-    with open('names.dmp', 'r') as names:
-        for _ in names:
-            line = _.split(sep='|')
-            taxon_id = line[0].strip()
-            name = line[1].strip()
-            name_type = line[3].strip()
-            if name_type == 'scientific name':
-                id_name[taxon_id] = name
-    with open('nodes.dmp', 'r') as nodes:
-        for _ in nodes:
-            line = _.split(sep='|')
-            taxon_id = line[0].strip()
-            rank = line[2].strip()
-            id_rank[taxon_id] = rank
-    for taxon_id in id_name:
-        rank_name = id_rank[taxon_id]
-        taxon_name = id_name[taxon_id]
-        if rank_name == 'superkingdom':
-            superkingdoms.add(taxon_name)
-        elif rank_name == 'kingdom':
-            kingdoms.add(taxon_name)
-        elif rank_name == 'phylum':
-            phyla.add(taxon_name)
-        elif rank_name == 'class':
-            classes.add(taxon_name)
-        elif rank_name == 'order':
-            if not taxon_name.endswith('ales'):
-                animal_orders.add(taxon_name)
-            else:
-                other_orders.add(taxon_name)
-        elif rank_name == 'family':
-            if taxon_name.endswith('aceae'):
-                plant_family.add(taxon_name)
-            else:
-                other_family.add(taxon_name)
-        elif rank_name == 'genus':
-            genus.add(taxon_name)
-        elif rank_name == 'species':
-            species.add(taxon_name)
-
-    with open(data_folder / 'superkingdoms.csv', 'w') as out:
-        out.write(','.join(superkingdoms))
-    with open(data_folder / 'kingdoms.csv', 'w') as out:
-        out.write(','.join(kingdoms))
-    with open(data_folder / 'phyla.csv', 'w') as out:
-        out.write(','.join(phyla))
-    with open(data_folder / 'classes.csv', 'w') as out:
-        out.write(','.join(classes))
-    with open(data_folder / 'animal_orders.csv', 'w') as out:
-        out.write(','.join(animal_orders))
-    with open(data_folder / 'other_orders.csv', 'w') as out:
-        out.write(','.join(other_orders))
-    with open(data_folder / 'plant_families.csv', 'w') as out:
-        out.write(','.join(plant_family))
-    with open(data_folder / 'other_families.csv', 'w') as out:
-        out.write(','.join(other_family))
-    with open(data_folder / 'genus.csv', 'w') as out:
-        out.write(','.join(genus))
-    with open(data_folder / 'species.csv', 'w') as out:
-        out.write(','.join(species))
-    return
-
-
-def codon_usage(alignment):
-    pass
-
-
-def gap_analyze(gap_alignment):
-    """
-
-    Args:
-        gap_alignment: np.array
-
-    Returns:
-
-    """
-    pass
-
-
-check_system()
+#!/usr/bin/python3
+import re
+import logging
+import platform
+import subprocess
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
+from functools import lru_cache
+from importlib import resources
+from pathlib import Path
+from queue import Queue
+from shutil import unpack_archive
+from sys import argv, version_info
+from threading import Thread
+from urllib.parse import quote
+from urllib.request import urlopen
+from zipfile import ZipFile
+
+from Bio.Seq import Seq
+from OGU.global_vars import log, name, FMT, DATEFMT
+
+
+# hosting in non-free AWS S3 server
+aws_url = 'https://ogu2023.s3.ap-east-1.amazonaws.com/'
+test_url = 'https://s3.ap-east-1.amazonaws.com'
+# font family
+if platform.system() == 'Windows':
+    font_family = 'Arial'
+else:
+    font_family = 'Helvetica'
+
+
+class BlastResult:
+    # slightly faster than namedtuple
+    __slots = ('query_id', 'hit_id', 'query_seq', 'ident_num', 'mismatch_num',
+               'bitscore_raw', 'query_start', 'query_end', 'hit_start',
+               'hit_end')
+
+    def __init__(self, line):
+        record = line.strip().split('\t')
+        self.query_id, self.hit_id, self.query_seq = record[0:3]
+        (self.ident_num, self.mismatch_num, self.bitscore_raw,
+         self.query_start, self.query_end, self.hit_start,
+         self.hit_end) = [int(i) for i in record[3:]]
+
+    def __repr__(self):
+        fmt = ('query_id: {}\thit_id: {}\tbitscore_raw: {}\tquery_start:{}\t'
+               'query_end: {}\thit_start: {}\thit_end: {}')
+        return fmt.format(self.query_id, self.hit_id, self.bitscore_raw,
+                          self.query_start, self.query_end, self.hit_start,
+                          self.hit_end)
+
+
+def check_system():
+    """
+    # primer3-py is currently unavailable on Windows with Python 3.9/3.10
+    # 2023.1 solved.
+    f-strings are not available on Python 3.5 or older.
+    """
+    if version_info.minor < 9:
+        raise RuntimeError('Python 3.9 or newer is required.')
+    if platform.system() == 'Windows':
+        if version_info.minor > 11:
+            # raise RuntimeError('Python 3.7 or 3.8 is required.')
+            raise RuntimeError('Do not support python 3.12 or higher.')
+    return
+
+
+def arg_to_str(arg) -> str:
+    s = ''
+    arg_dict = vars(arg)
+    for key, value in arg_dict.items():
+        if isinstance(value, str):
+            pass
+        elif isinstance(value, Iterable):
+            value = ' '.join(value)
+        elif value is None:
+            continue
+        elif isinstance(value, bool):
+            if value:
+                value = ''
+            else:
+                # Assume all bool option using action='store_true'
+                continue
+        s += f' -{key} {value}'
+    return s
+
+
+def add_file_log(arg):
+    """
+    Add file handler if not exist.
+    Note that "log" is a global variable.
+    """
+    has_file_hdl = any([type(i)==logging.FileHandler for i in log.handlers])
+    if has_file_hdl:
+        pass
+    else:
+        log_file = arg.out / 'Log.txt'
+        log_file_handler = logging.FileHandler(log_file, mode='a')
+        log_file_handler.setLevel(logging.DEBUG)
+        log_file_handler.setFormatter(
+            logging.Formatter(fmt=FMT, datefmt=DATEFMT))
+        log.addHandler(log_file_handler)
+        log.debug('Add file handler.')
+        log.debug('Arguments:')
+        log.debug(' '.join(argv))
+    return
+
+
+def move(source: Path, dest, copy=False):
+    """
+    Move source to dest and return dest.
+    If set "copy", copy source to dest instead of move.
+    Because Path.rename could not move file across different filesystem or
+    drive, have to use copy and delete to implement "move".
+    Warning:
+        This function does not check whether dest exists or not.
+    Args:
+        source(Path): old path
+        dest(Path or str): new path
+        copy(bool): copy or move
+    Return:
+        dest(Path): new path
+    """
+    source = Path(source).absolute()
+    dest = Path(dest).absolute()
+    # avoid useless copy
+    # Path.samefile may raise FileNotFoundError
+    if source == dest:
+        log.debug(f'{source} and {dest} are same.')
+    else:
+        # read_bytes/write_bytes includes open, read/write and close steps
+        dest.write_bytes(source.read_bytes())
+        if not copy:
+            source.unlink()
+    return dest
+
+
+def init_out(arg):
+    """
+    Initilize output folder.
+    Args:
+        arg(NameSpace): arguments
+    Returns:
+        arg(NameSpace): arguments
+    """
+    if not hasattr(arg, 'out') or arg.out is None:
+        log.warning('Output folder was not set.')
+        log.info('\tUse "Result" instead.')
+        arg.out = Path().cwd().absolute() / 'Result'
+    else:
+        arg.out = Path(arg.out).absolute()
+    if arg.out.exists() and len(list(arg.out.iterdir())) == 0:
+        from OGU import global_vars
+        if not global_vars.global_dict.get('out_inited', False):
+            log.warning(f'Output folder {arg.out} exists.')
+            arg.out = arg.out / (arg.out.name+'_')
+            log.info(f'Use {arg.out} instead.')
+            if arg.out.exists():
+                log.error(f'{arg.out} exists, too!')
+                raise SystemExit(-1)
+        else:
+            pass
+    arg._gb = arg.out / 'GenBank'
+    arg._fasta = arg.out / 'Fasta'
+    arg._divide = arg.out / 'Divide'
+    arg._expand = arg.out / 'Expanded_fasta'
+    arg._unique = arg.out / 'Unique'
+    arg._align = arg.out / 'Alignment'
+    arg._evaluate = arg.out / 'Evaluate'
+    arg._primer = arg.out / 'Primer'
+    arg._tmp = arg.out / 'Temp'
+    try:
+        arg.out.mkdir()
+        arg._gb.mkdir()
+        arg._fasta.mkdir()
+        arg._divide.mkdir()
+        arg._expand.mkdir()
+        arg._unique.mkdir()
+        arg._align.mkdir()
+        arg._evaluate.mkdir()
+        arg._primer.mkdir()
+        arg._tmp.mkdir()
+    except Exception:
+        log.debug('Folder exists.')
+    out_inited = True
+    return arg
+
+
+def clean_tmp(filename: Path):
+    if filename.is_dir():
+        for i in filename.glob('*'):
+            i.unlink()
+    elif filename.is_file():
+        for i in filename.parent.glob(f'{filename.name}*'):
+            i.unlink()
+    return
+
+
+@lru_cache(maxsize=None)
+def gene_rename(old_name: str, genbank_format=False) -> (str, str):
+    """
+    Old doc:
+        Different name of same gene will cause data to be split to numerous
+        files instead of one and some data may be dropped.
+
+        For chloroplast genes, the author summarized various kinds of
+        annotation error of gene name or synonyms and try to use regular
+        expression to fix it.
+
+        Ideally, use BLAST to re-annotate sequence is the best(and slow) way to
+        find the correct name. This function only offers a "hotfix" which is
+        enough.
+    Rename plastid genes.
+    May be dangerous.
+    Will cache results.
+    Args:
+        old_name: old gene name
+        genbank_format: use style like "trnH-GUG" or "trnHgug"
+    Returns:
+        new_name(str): new name, if fail, return old name
+        gene_type(str): gene types, guessed from name
+    """
+    lower = old_name.lower()
+    # (trna|trn(?=[b-z]))
+    s = re.compile(r'(\d+\.?\d?)(s|rrn|rdna)')
+    if lower.startswith('trn'):
+        pattern = re.compile(r'([atcgu]{3})')
+        prefix = 'trn'
+        aa_letter = 'X'
+        try:
+            anticodon = Seq(re.search(pattern, lower[3:]).group(1))
+        except Exception:
+            return old_name, 'bad_name'
+        # rna editing? trnI-CAU
+        if anticodon == 'cau' and lower.startswith('trni'):
+            aa_letter = 'I'
+        # for trnfM-CAU
+        elif lower.startswith('trnfm'):
+            prefix = 'trnf'
+            aa_letter = 'M'
+        else:
+            try:
+                aa_letter = anticodon.reverse_complement_rna().translate().upper()
+                if aa_letter == '*':
+                    aa_letter = 'UNKNOWN'
+            except Exception:
+                return old_name, 'bad_name'
+            # anticodon = anticodon.transcribe()
+        if genbank_format:
+            new_name = f'{prefix}{aa_letter}-{anticodon.upper()}'
+        else:
+            new_name = f'{prefix}{aa_letter}_{anticodon.upper()}'
+        gene_type = 'tRNA'
+    elif lower.startswith('rrn'):
+        pattern = re.compile(r'(\d+\.?\d?)')
+        try:
+            number = re.search(pattern, lower).group(1)
+        except Exception:
+            return old_name, 'bad_name'
+        new_name = 'rrn{}'.format(number)
+        gene_type = 'rRNA'
+    elif re.search(s, lower) is not None:
+        new_name = 'rrn{}'.format(re.search(s, lower).group(1))
+        gene_type = 'rRNA'
+    else:
+        pattern = re.compile(r'[^a-z]*'
+                             '(?P<gene>[a-z]+)'
+                             '[^a-z0-9]*'
+                             '(?P<suffix>[a-z]|[0-9]+)')
+        match = re.search(pattern, lower)
+        try:
+            gene = match.group('gene')
+            suffix = match.group('suffix')
+        except Exception:
+            return old_name, 'bad_name'
+        new_name = '{}{}'.format(gene, suffix.upper())
+        # capitalize last letter
+        if len(new_name) > 3:
+            s = list(new_name)
+            if s[-1].isalpha():
+                new_name = '{}{}'.format(
+                    ''.join(s[:-1]), ''.join(s[-1]).upper())
+        gene_type = 'normal'
+    if len(lower) >= 15:
+        gene_type = 'suspicious_name'
+    return new_name, gene_type
+
+
+def plastid_rename():
+    """
+    Use name database.
+    """
+    pass
+
+
+def safe_average(x):
+    """
+    Safe average.
+    """
+    if len(x) == 0:
+        return 0
+    else:
+        return sum(x) / len(x)
+
+
+def safe_path(old):
+    """
+    Remove illegal character in file path or name.
+    """
+    return re.sub(r'\W', '_', old)
+
+
+def accessible(name: Path, type_: str) -> bool:
+    """
+    Check given path is accessible or not.
+    Given path does not exist.
+    Args:
+        name(Path): folder or file, absolute path
+        type_(str): 'folder' or 'file'
+    Return:
+        ok(bool): accessible or not
+    """
+    p = Path(name)
+    if type_ == 'folder':
+        try:
+            p.mkdir()
+            p.rmdir()
+            ok = True
+        except PermissionError:
+            ok = False
+    elif type_ == 'file':
+        try:
+            p.touch()
+            p.unlink()
+            ok = True
+        except PermissionError:
+            ok = False
+    else:
+        log.critical(f'Illegal type: {type_}')
+        ok = False
+    return ok
+
+
+def test_cmd(program, option='-version') -> bool:
+    """
+    Test given program and option is ok to run or not.
+    Args:
+        program(Path or str): program path, could be relative path if it can
+        be found in $PATH or %PATH%
+        option(str): option for program, usually use "-v" to show version to
+        test the program
+    Return:
+        success(bool): success or not
+    """
+    program = Path(program)
+    if program.exists():
+        program.chmod(0o755)
+    cmd = f'{program} {option}'
+    test = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL,
+                          stderr=subprocess.DEVNULL)
+    success = True if test.returncode == 0 else False
+    return success
+
+
+def get_third_party_path():
+    """
+    Get third_party folder.
+    If do not exist, create it.
+    If cannot access, report.
+    Return:
+        success(bool): ok or not
+        third_party(Path): absolute path of third_party folder
+    """
+    third_party = Path().home().absolute() / '.OGU'
+    success = False
+    if not third_party.exists():
+        log.debug(f'Create folder {third_party}')
+        try:
+            third_party.mkdir()
+        except Exception:
+            log.critical(f'Failed to create {third_party}.'
+                         'Please contact the administrator.')
+            return success, third_party
+    if not accessible(third_party/'test', 'file'):
+        log.critical(f'Failed to access {third_party}.'
+                     f'Please contact the administrator.')
+        return success, third_party
+    success = True
+    return success, third_party
+
+
+# todo test in linux and windows
+def get_software(software: str, url: str, filename: Path,
+                 third_party: Path, home_bin: Path, test_option='-version'):
+    log.warning(f'Cannot find {software}, try to install. May cost minutes')
+    try:
+        # 50kb/10s=5kb/s, enough for test
+        _ = urlopen(test_url, timeout=10)
+    except Exception:
+        log.critical('Cannot connect to Server.'
+                     'Please check your Internet connection.')
+        raise SystemExit(-1)
+    try:
+        # file is 10mb or larger
+        log.info(f'Downloading {filename.name} from {url}')
+        down = urlopen(f'{url}', timeout=100)
+    except Exception:
+        log.critical(f'Cannot download {software}. '
+                     f'Please manually download it from {url}')
+        raise SystemExit(-1)
+    down_file = filename
+    with open(down_file, 'wb') as out:
+        try:
+            _ = down.read()
+        except TimeoutError:
+            log.critical(f'Download {software} timeout.'
+                         f'Please manually download it from {url}')
+            raise SystemExit(-1)
+        out.write(_)
+    log.info(f'{filename.name} got. Installing...')
+    try:
+        # unpack_archive(down_file, third_party/fileinfo[system][1])
+        unpack_archive(down_file, third_party)
+    except Exception:
+        log.critical(f'The {software} file is damaged. '
+                     f'Please recheck your connection.')
+        raise SystemExit(-1)
+    if software == 'mafft.bat':
+        for i in ('bin', 'libexec'):
+            subfolder = home_bin.parent / 'mafftdir' / i
+            # windows use different path
+            if subfolder.exists():
+                for file in subfolder.iterdir():
+                    file.chmod(0o755)
+    assert test_cmd(home_bin, test_option)
+    log.info(f'{software} installed successfully.')
+    return True
+
+
+def get_blast(third_party=None, result=None) -> (bool, str):
+    """
+    Get BLAST location.
+    If BLAST was found, assume makeblastdb is found, too.
+    If not found, download it.
+    Args:
+        third_party(Path or None): path for install
+        result(Queue): return values
+    Return:
+        ok(bool): success or not
+        blast(str): blast path
+    """
+    if third_party is None:
+        third_party_ok, third_party = get_third_party_path()
+        if not third_party_ok:
+            return third_party_ok, ''
+    blast = 'blastn'
+    home_blast = third_party / 'ncbi-blast-2.13.0+' / 'bin' / blast
+    # in Windows, ".exe" can be omitted
+    # win_home_blast = home_blast.with_name('blastn.exe')
+    ok = False
+    # older than 2.8.1 is buggy
+    original_url = ('https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.13.0/'
+                    'ncbi-blast-2.13.0+')
+    file_prefix = 'ncbi-blast-2.13.0+'
+    fileinfo = {'Linux': file_prefix+'-x64-linux.tar.gz',
+                'Darwin': file_prefix+'-x64-macosx.tar.gz',
+                'Windows': file_prefix+'-win64.zip'}
+                #'Windows': file_prefix + '-x64-win64.tar.gz'}
+    system = platform.system()
+    filename = fileinfo[system]
+    down_url = f'{aws_url}{quote(filename)}'
+    # three software use different name pattern
+    down_file = third_party / filename
+    if test_cmd(blast):
+        ok = True
+        home_blast = str(blast)
+    elif test_cmd(home_blast):
+        ok = True
+        home_blast = str(home_blast)
+    else:
+        ok = get_software(blast, down_url, down_file, third_party, home_blast)
+    if result is not None and ok:
+        result.put(('BLAST', ok))
+    return ok, str(home_blast)
+
+
+def get_iqtree(third_party=None, result=None) -> (bool, str):
+    """
+    Get iqtree location.
+    If not found, download it.
+    Args:
+        third_party(Path or None): path for install
+        result(Queue): return values
+    Return:
+        ok(bool): success or not
+        iqtree(str): blast path
+    """
+    if third_party is None:
+        third_party_ok, third_party = get_third_party_path()
+        if not third_party_ok:
+            return third_party_ok, ''
+    iqtree = 'iqtree2'
+    # in Windows, ".exe" can be omitted
+    ok = False
+    original_url = 'https://github.com/iqtree/iqtree2/releases/download/v2.2.0/'
+    # platform: (filename, folder)
+    fileinfo = {'Linux': ('iqtree-2.2.2.2-Linux.tar.gz', 'iqtree-2.2.2.2-Linux'),
+                'Darwin': ('iqtree-2.2.2.2-MacOSX.zip', 'iqtree-2.2.2.2-MacOSX'),
+                'Windows': ('iqtree-2.2.2.2-Windows.zip',
+                            'iqtree-2.2.2.2-Windows')}
+    system = platform.system()
+    filename = fileinfo[system][0]
+    down_url = f'{aws_url}{quote(filename)}'
+    home_iqtree = third_party / fileinfo[system][1] / 'bin' / iqtree
+    down_file = third_party / fileinfo[system][0]
+    if test_cmd(iqtree):
+        ok = True
+        home_iqtree = str(iqtree)
+    elif test_cmd(home_iqtree):
+        ok = True
+    else:
+        ok = get_software(iqtree, down_url, down_file, third_party,
+                          home_iqtree)
+    if result is not None and ok:
+        result.put(('IQTREE', ok))
+    return ok, str(home_iqtree)
+
+
+def get_mafft(third_party=None, result=None) -> (bool, str):
+    """
+    Get mafft location.
+    If not found, download it.
+    Args:
+        third_party(Path or None): path for install
+        result(Queue): return values
+    Return:
+        ok(bool): success or not
+        mafft(str): mafft path
+    """
+    if third_party is None:
+        third_party_ok, third_party = get_third_party_path()
+        if not third_party_ok:
+            return third_party_ok, ''
+    system = platform.system()
+    mafft = 'mafft.bat'
+    # in Windows, ".exe" can be omitted
+    # win_home_blast = home_blast.with_name('blastn.exe')
+    ok = False
+    original_url = 'https://mafft.cbrc.jp/alignment/software/'
+    # system: {filename, folder}
+    fileinfo = {'Linux': ('mafft-7.511-linux.tgz', 'mafft-linux64'),
+                'Darwin': ('mafft-7.511-mac.zip', 'mafft-mac'),
+                'Windows': ('mafft-7.511-win64-signed.zip', 'mafft-win')}
+    home_mafft = third_party / fileinfo[system][1] / mafft
+    system = platform.system()
+    filename = fileinfo[system][0]
+    down_url = f'{aws_url}{quote(filename)}'
+    down_file = third_party / fileinfo[system][0]
+    # mafft use '--version' to test
+    test_option = '--version'
+    if test_cmd(mafft, test_option):
+        ok = True
+        home_mafft = str(mafft)
+    elif test_cmd(home_mafft, test_option):
+        ok = True
+    else:
+        ok = get_software(mafft, down_url, down_file, third_party, home_mafft,
+                          test_option=test_option)
+    if result is not None and ok:
+        result.put(('MAFFT', ok))
+    return ok, str(home_mafft)
+
+
+def get_all_third_party(skip_blast=True) -> bool:
+    """
+    Use three threads to speed up.
+    """
+    log.info('Try to locate or install all third-party software.')
+    third_party_ok, third_party = get_third_party_path()
+    if not third_party_ok:
+        return False
+    result_queue = Queue()
+    iqtree = Thread(target=get_iqtree, args=(third_party, result_queue),
+                    daemon=True)
+    mafft = Thread(target=get_mafft, args=(third_party, result_queue),
+                   daemon=True)
+    if not skip_blast:
+        blast = Thread(target=get_blast, args=(third_party, result_queue),
+                       daemon=True)
+        blast.start()
+        blast.join()
+    iqtree.start()
+    mafft.start()
+    iqtree.join()
+    mafft.join()
+    while not result_queue.empty():
+        name, ok = result_queue.get()
+        if ok:
+            log.info(f'Got {name}.')
+        else:
+            log.error(f'Failed to got {name}.')
+            return False
+    return True
+
+
+def parse_blast_tab(filename):
+    """
+    Parse BLAST result (tab format).
+    """
+    query = []
+    with open(filename, 'r', encoding='utf-8') as raw:
+        for line in raw:
+            if line.startswith('# BLAST'):
+                yield query
+                query = []
+            elif line.startswith('#'):
+                pass
+            else:
+                query.append(BlastResult(line))
+    pass
+
+
+def download_taxon(data_folder) -> Path:
+    zip_file = data_folder / 'taxdmp.zip'
+    if zip_file.exists():
+        pass
+    else:
+        url = 'https://ftp.ncbi.nih.gov/pub/taxonomy/taxdmp.zip'
+        with urlopen(url) as response, zip_file.open('wb') as out_file:
+            data = response.read()
+            out_file.write(data)
+    return zip_file
+
+
+def init_lineage():
+    """
+    Only called by setup.py
+    """
+    global name
+    data_folder = resources(name) / 'data'
+    zip_file = download_taxon(data_folder)
+    with ZipFile(zip_file, 'r') as dumpfile:
+        dumpfile.extract('names.dmp', path='.')
+        dumpfile.extract('nodes.dmp', path='.')
+    id_name = {}
+    id_rank = {}
+    superkingdoms = set()
+    kingdoms = set()
+    phyla = set()
+    classes = set()
+    animal_orders = set()
+    other_orders = set()
+    plant_family = set()
+    other_family = set()
+    genus = set()
+    species = set()
+    with open('names.dmp', 'r') as names:
+        for _ in names:
+            line = _.split(sep='|')
+            taxon_id = line[0].strip()
+            name = line[1].strip()
+            name_type = line[3].strip()
+            if name_type == 'scientific name':
+                id_name[taxon_id] = name
+    with open('nodes.dmp', 'r') as nodes:
+        for _ in nodes:
+            line = _.split(sep='|')
+            taxon_id = line[0].strip()
+            rank = line[2].strip()
+            id_rank[taxon_id] = rank
+    for taxon_id in id_name:
+        rank_name = id_rank[taxon_id]
+        taxon_name = id_name[taxon_id]
+        if rank_name == 'superkingdom':
+            superkingdoms.add(taxon_name)
+        elif rank_name == 'kingdom':
+            kingdoms.add(taxon_name)
+        elif rank_name == 'phylum':
+            phyla.add(taxon_name)
+        elif rank_name == 'class':
+            classes.add(taxon_name)
+        elif rank_name == 'order':
+            if not taxon_name.endswith('ales'):
+                animal_orders.add(taxon_name)
+            else:
+                other_orders.add(taxon_name)
+        elif rank_name == 'family':
+            if taxon_name.endswith('aceae'):
+                plant_family.add(taxon_name)
+            else:
+                other_family.add(taxon_name)
+        elif rank_name == 'genus':
+            genus.add(taxon_name)
+        elif rank_name == 'species':
+            species.add(taxon_name)
+
+    with open(data_folder / 'superkingdoms.csv', 'w') as out:
+        out.write(','.join(superkingdoms))
+    with open(data_folder / 'kingdoms.csv', 'w') as out:
+        out.write(','.join(kingdoms))
+    with open(data_folder / 'phyla.csv', 'w') as out:
+        out.write(','.join(phyla))
+    with open(data_folder / 'classes.csv', 'w') as out:
+        out.write(','.join(classes))
+    with open(data_folder / 'animal_orders.csv', 'w') as out:
+        out.write(','.join(animal_orders))
+    with open(data_folder / 'other_orders.csv', 'w') as out:
+        out.write(','.join(other_orders))
+    with open(data_folder / 'plant_families.csv', 'w') as out:
+        out.write(','.join(plant_family))
+    with open(data_folder / 'other_families.csv', 'w') as out:
+        out.write(','.join(other_family))
+    with open(data_folder / 'genus.csv', 'w') as out:
+        out.write(','.join(genus))
+    with open(data_folder / 'species.csv', 'w') as out:
+        out.write(','.join(species))
+    return
+
+
+def codon_usage(alignment):
+    pass
+
+
+def gap_analyze(gap_alignment):
+    """
+
+    Args:
+        gap_alignment: np.array
+
+    Returns:
+
+    """
+    pass
+
+
+check_system()
```

### Comparing `ogu-1.52/PKG-INFO` & `ogu-1.54/.pdm-build/ogu-1.52.dist-info/METADATA`

 * *Files identical despite different names*

