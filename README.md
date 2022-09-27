# TWRP device tree for ASUS ZC500TG (Z00VD)

<p align="center">
  <img height="600" src="/preview.png?raw=true">
</p>

Basic        | Spec Sheet
------------:|:-------------------------
CPU          | Quad-core 1.3 GHz Cortex-A7
Chipset      | Mediatek MT6580 (28 nm)
GPU          | Mali-400MP2
Memory/RAM   | 2GB
Storage      | 8GB/16GB
Battery      | Li-Po 2070 mAh (removable)
Dimensions   | 144.5 x 71 x 10 mm (5.69 x 2.80 x 0.39 in)
Display      | 5.0"IPS LCD Display (720 x 1280)
Rear Camera  | 8 MP, f/2.0, AF
Front Camera | 2 MP, f/2.4
Release Date | August 2015

# ANDROID 10 
# KERNEL 4.9.188

<p align="center">
  <img height="600" src="/preview1.png?raw=true">
</p>



## Build instructions
- Initialize the source tree -
  ```bash
  repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
  ```
  You may optionally pass `--depth=1` to save space, like so:
  ```bash
  repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
  ```
- Then to sync up
  ```bash
  repo sync
  ```
- Clone this repository -
  ```bash
  git clone https://github.com/xmxnRzxRangkuti/tree_twrp_asus_z00vd device/asus/z00vd
  ```
- Build -
  ```bash
  source build/envsetup.sh
  export ALLOW_MISSING_DEPENDENCIES=true
  lunch omni_ASUS_Z00VD-eng
  mka recoveryimage
  ```


# xmxnRzxRangkuti