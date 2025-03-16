LemonageOS
===========

Getting started
---------------

To get started with Android, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the LemonageOS trees, use a command like this:
```
repo init -u https://github.com/LemonageOS/android_manifest.git -b lineage-18.1 --git-lfs
```
Then to sync up:
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

Building LemonageOS
-------------------

Initialize the ROM environment with the envsetup.sh script

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed

```bash
lunch lineage_codename-buildtype
```

Start compilation

```bash
mka bacon
```