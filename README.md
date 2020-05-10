![Evolution X](https://github.com/Evolution-X/manifest/raw/ten/EvoBanner.png)

# Evolution X #

[![Download Evolution X](https://img.shields.io/sourceforge/dt/evolution-x.svg)](https://sourceforge.net/projects/evolution-x/files/latest/download)

I would advise NOT using anything in my github account. I am learning how this all works and accept zero responsibility if you use anything and it breaks something. Thanks. Feel free to use the projects i've forked from though.

The ten-opengapps branch is for my personal learning. Some devices dont have enough system partition space for full pixel gapps. Also some of the Pixel apps are for arm64 only.

NOTES FOR ME.

-Once you have sync'd all repos from the manifest, and just before building, you need to grab the gapps packages by running the following inside /vendor/gapps

repo forall -c git lfs pull

-There is no TrichromeLibraryGoogle for arm 32 bit devices. You may therefore have to remove the following file to compile

vendor/opengapps/build/modules/TrichromeLibrary/Android.mk

