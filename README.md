What's this?
------------

Scripts and patches to compile [Fennec F-Droid](https://f-droid.org/packages/org.mozilla.fennec_fdroid/). They remove proprietary chunks from Mozilla code, rebrand Firefox to Fennec and build it. You can assemble your own APK in the very same way as F-Droid by cloning [recipes](https://gitlab.com/fdroid/fdroiddata) and running

    fdroid build org.mozilla.fennec_fdroid:VERCODE

where VERCODE is a version code number.

Want to translate the description?
----------------------------------

Feel free to translate the Fennec F-Droid [description](https://f-droid.org/packages/org.mozilla.fennec_fdroid/) via [Codeberg Translate](https://translate.codeberg.org/projects/fennec/).

Variants
--------
fennecbuild offers two variants: the default vanilla named Fennec F-Droid and a privacy & security hardened option named FrozenFennec.
FrozenFennec can and does break websites, please see frozenfennec-notes.md for workarounds.

Licenses
--------

The scripts are licensed under the GNU Affero General Public License version 3 or later.

Changes in the patch are licensed according to the header in the files this patch adds or modifies (Apache 2.0 or MPL 2.0).

The artwork is licensed under the MPL 2.0.

External assets such as userjs-arkenfox.js and userjs-brace.js are licensed MIT and AGPL-3.0-or-later respectively.
