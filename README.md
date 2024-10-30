# Android device tree for samsung SM-A202F (a20e)

# How-to compile it:

 - twrp-11 Manifest
```
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11
```
 - Sync
```
repo sync
```
 - Clone TheNoobDevs-Staging twrp tree
```
git clone https://github.com/TND-STAGING/android_device_samsung_a20e.git -b twrp-11 device/samsung/a20e
```
 - Prepare
```
export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_a20e-eng
```
 - Run the Build Command
```
mka recoveryimage
