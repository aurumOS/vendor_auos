[aurumOS](http://aurum.cf)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Init core trees without any device/kernel/vendor :

    $ repo init -u https://github.com/aurumOS/au_manifest.git -b mm

sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    lunch


You can also build (and see how long it took) for specific devices (eg. hammerhead) like this:

    . build/envsetup.sh
    lunch au_hammerhead-userdebug && time make goldingot

Remember to `make clean` every now and then!
