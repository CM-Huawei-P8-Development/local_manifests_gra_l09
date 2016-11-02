# Huawei Ascend P8 CM Manifest

## Instructions
- repo init -u git://github.com/CyanogenMod/android.git -b cm-13.0
- repo sync
- repo init -b stable/cm-13.0-ZNH5Y
- git clone gra_l09_local_manifests --> .repo/local_manifests
- repo sync --force-sync (use python 2.7!)


## Repository branch name policy

To avoid confusion here's a simple policy for naming the branches.


For ´device trees´ and forks of the ´cyanogenmod repository´
We use the same branch names for one **build set**.
Optionally we may add ´[-any name]´ for feature branches.

**A.e. ´cm-13.0-ZNH5Y´ or ´cm-13.0-ZNH5Y-testing´**


For ´kernels´ we use ´cm-<major cm version>-<kernel-version>[-any name when 
tweaked]´.

**A.e. ´cm-13-v3.10.61´ or ´cm-13-v3.10.61-xmod´.**


For maintained ´3th party´. A.e. TWRP we use their branch name


The device trees itself should be named the same way as in the 
official cyanogenmod repository. However we may add ´[_device]´
gra_l09/gra_ul00 in case it's device specific.
