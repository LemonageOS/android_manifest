LemonageOS
===========

 ### Instructions
 1. Make sure you have a build environment setup.
 2. Run the following commands to sync LemonageOS source

```bash
mkdir lemonage && cd lemonage
```
```bash
repo init -u https://github.com/LemonageOS/android_manifest -b lineage-18.1
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

 3. Once the source is downloaded prepare your trees and build.
