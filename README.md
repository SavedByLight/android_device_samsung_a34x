# TWRP Device Tree for Samsung Galaxy A34 5G

The Galaxy A34 5G (codenamed _"a34x"_) is an upper-mid-range smartphone from Samsung.

It was announced and released in March 2023.

## Device specifications

| Feature                      | Specification                                                                  |
| ---------------------------: | :----------------------------------------------------------------------------- |
| Chipset                      | Mediatek Dimensity 1080                                                                    |
| CPU                          | Octa-core (2x2.6 GHz Cortex-A78 & 6x2.0 GHz Cortex-A55)                       |
| GPU                          | Mali-G68 MC4                                                                |
| Memory                       | 6GB / 8GB RAM (LPDDR4X)                                                        |
| Shipped OS                   | Android 13 (One UI 5.1), 4 major OS upgrades, received up to Android 16 (One UI 8.0) |
| Storage                      | 128GB / 256GB (UFS 2.2)                                                        |
| SIM                          | Single SIM (Nano-SIM) or Hybrid Dual SIM (Nano-SIM, dual stand-by)       |
| MicroSD                      | Up to 1TB                                                                      |
| Battery                      | 5000mAh Li-Po (non-removable), 25W fast charge                                 |
| Dimensions                   | 161.3 x 78.1 x 8.2 mm (6.35 x 3.07 x 0.32 in)                                  |
| Display                      | 6.6", 1080 x 2340 pixels, 19.5:9 ratio, Super AMOLED, 120Hz (~403 ppi density) |
| Rear Camera 1 (IMX582)       | 	48 MP, f/1.8, 26mm (wide), 1/2.0", 0.8µm, PDAF, OIS                                |
| Rear Camera 2 (S5K4HAYX)       | 8 MP, f/2.2, 123˚, (ultrawide), 1/4.0", 1.12µm                                         |
| Rear Camera 3 (GC5035)       | 5 MP (macro)                                                           |
| Front Camera (SR846D/HI1339) | 13 MP, f/2.2, 26mm (wide), 1/3.1", 1.12µm                                       |
| Fingerprint                  | EgisTec EL7XX (under display, optical)                                         |
| Sensors                      | Accelerometer, Gyro, Proximity (virtual), Compass, Hall IC, Grip               |
| Extras                       | Dual speakers, NFC                                                             |

## Kernel source 

Available at [https://opensource.samsung.com/uploadSearch?searchValue=A346BXXUBEYI7](https://opensource.samsung.com/uploadSearch?searchValue=A346BXXUBEYI7)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/TeamWin/android_device_samsung_a34x.git -b android-12.1 device/samsung/a34x
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_a34x-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2025 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```

## Contributors
 - [Fede2782](https://github.com/Fede2782)
 - [SavedByLight](https://github.com/SavedByLight)
 - [ravindu644](https://github.com/ravindu644) for OTG fix
 - [ChrolloUTA](https://github.com/ChrolloUTA)
