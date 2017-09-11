Aquaris E5 HD - LineageOS 13.0
==============

### Full Compilation guide:

     * repo init -u git://github.com/LineageOS/android.git -b cm-13.0

     * repo sync --force-sync 

     * . build/envsetup.sh

     * lunch lineage_vegetahd-userdebug

### Recovery Compilation (TWRP Variant):

  LineageOS root / source directory:

     * git clone https://github.com/LineageOS/android_external_busybox external/busybox
     * git clone https://github.com/OmniROM/android_bootable_recovery bootable/recovery-twrp
     * source build/envsetup.sh
     * lunch
     * lineage_vegetahd-eng
     * export WITH_TWRP=true
     * mka recoveryimage

### For apply the patches (only tested on lineage os):

  In the device tree directory (device/bq/vegetahd):

     * . apply-patches.sh

### Thanks to (In alphabetichal order):

 * Assusdan
 * sultanxda
 * Varun Chitre
 * Vo-1
 * Zormax
