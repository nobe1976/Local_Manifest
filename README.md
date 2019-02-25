Local Manifest for DU builds
=============================

Getting Started
======================

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com).

First init the source.
======================

$ repo init -u git://github.com/DirtyUnicorns/android_manifest.git -b p9x-caf

Then:
-------------------------
$ mkdir -p .repo/local_manifests

Curl in the local_manifests
-------------------------
$ curl -L -o .repo/local_manifests/local_manifests.xml -O -L https://raw.github.com/nobe1976/Local_Manifest/master/D850-manifest.xml


Then Watch it Fly
=================

$ repo sync --force-sync -j$( nproc --all )
