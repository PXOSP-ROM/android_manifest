# PXOSP

PXOSP (Proton Xtended Open Source Project) is a fork based on ProtonAOSP to enchantment user experience with useful addition features.

## Getting source code

First, make sure you have an [Android build environment](https://source.android.com/setup/build/initializing) and the [repo tool](https://source.android.com/setup/build/downloading) set up. After that, run the following commands:

```
repo init -u https://github.com/PXOSP-ROM/android_manifest -b sc-v2
repo sync -c --force-sync --no-tags --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```

This is a large download that will take approximately 100 GB of disk space, so plan accordingly.

## Building

First, you need to make and sync device trees. After that you can continue:

```
. build/envsetup.sh
lunch pxosp_{codename}-user{debug}
m bacon
```

## Credits

* ProtonAOSP - For rom base
* LineageOS - For their apps/icons
* PixelExperience - For CAF repos
* All roms from where I picked any changes

Good luck & thanks for choosing us!
