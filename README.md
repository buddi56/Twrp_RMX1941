TWRP Device Tree for Realme C2
===========================================

The Realme C2 is a budget range smartphone from Realme, announced in April 2019.

## Status

**Working**:

1. MTP
2. Backup and Restore
3. Flash GSI
4. Screenshots now renders correct color
5. OTG Works

**Not working**:

1. Decryption


## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
OS	| Android 9.0 (pie)	
CPU     | Octa-core 2.0 GHz Cortex-A53
Chipset | Mediatek MT6762 Helio P22 (12 nm)
GPU     | PowerVR GE8320
Memory  | 2GB/3GB RAM
Storage | 16GB/32GB
MicroSD | up to 64 GB (dedicated slot)
Battery | Non-removable Li-Ion 4000 mAh battery
Resolution | 720 x 1560 pixels, 19.5:9 ratio (~282 ppi density)
Camera (Rear)  | 13 MP, f/2.2, 1/3.1", 1.12µm, PDAF & 2 MP, f/2.4, (depth)
Rear Camera Features | LED flash, HDR, panorama
Video	| 1080p@30fps	
Camera (Front)  | 5 MP, f/2.0, 1/5", 1.12µm
Features| Accelerometer, proximity, compass	

## Device picture

![Realme C2](https://assets.mspimages.in/c/tr:w-1000,h-1000,c-at_max/15600-42-2.jpg "Realme C2")



## Getting Started ##
---------------

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

# repo init

To initialize your local repository using the OMNIROM trees to build TWRP, use a command like this:

    repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

# repo sync

 Then to sync up:

    repo sync 

## To Build ##
---------------

Build the TWRP recovery using below command.

    cd <source-dir>; export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_RMX1941-eng; mka recoveryimage

## NOTE

Most of the work here is from internet. Thanks to all the members involved in TWRP project, example DTs and testers.
