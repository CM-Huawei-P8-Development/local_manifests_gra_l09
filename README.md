# Huawei Ascend P8 LineageOS Manifest

## Instructions
- repo init -u git://github.com/LineageOS/android.git -b cm-13.0
- repo sync
- repo init -b cm-13.0
- git clone -b lineage-13.0 gra_l09_local_manifests --> .repo/local_manifests
- repo sync --force-sync (use python 2.7!)


## Repository branch name policy

To avoid confusion here's a simple policy for naming the branches.


For forks of the `cyanogenmod repository`
We use the same branch names for one **build set**.
Optionally we may add `[-any name]` for feature branches.
**A.e. `cm-13.0-ZNH5Y` or `cm-13.0-ZNH5Y-testing`**

The forked repositories itself should be named the same way as in the 
official cyanogenmod repository. However we may add `[_device]`
gra_l09/gra_ul00 in case it's device specific. Most likely 
the manifest and device tree.

The branch names of the device tree should be the same as for
the rest of the **build set**

---

For `kernels` we use 
`cm-<major cm version>-v<kernel-version>[-any name when tweaked]`.
We include the cm version since the official UPDATE.APP
includes more than just that what we build and this stuff depends
on the major android version.

**A.e. `cm-13-v3.10.61` or `cm-13-v3.10.61-xmod`.**

---

For maintained `3th party`. A.e. TWRP we use their branch name

---
