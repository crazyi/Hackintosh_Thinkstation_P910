# Thinkstation P910 Hackintosh

## Notice: If you need to edit config.plist, don't use Clover/OpenCore configurator, use Xcode or [ProperTree](https://github.com/corpnewt/ProperTree) instead.

## Introduction

Clover and Opencore efi for Thinkstation P910 Hackintosh High Sierra

Clover efi origined from [KGP](https://github.com/KGP/X99-EFI-Folder-Distributions),  detailed guide from him can be found on [InsanelyMac](https://www.insanelymac.com/forum/topic/331703-how-to-build-your-own-mac-pro-based-on-broadwell-eep-haswell-eep-and-x99-successful-buildextended-guide/)

Opencore efi was a tanslation of the Clover one with my patch to auto detect Broadwell-EP cpu [#585](https://github.com/acidanthera/bugtracker/issues/585)

Both efis can be easily updated to the latest macOS Catalina by using the kernel and kexts patches colleted by [nmano](https://www.insanelymac.com/forum/topic/335650-kernelandkextpatches-1013x1014x1015x-x99/) 

## Hardware:

CPU: **Intel(R) Xeon(R) CPU E5-2650 v4 @ 2.20GHz**

Graphics: **NVIDIA Quadro K620**

Motherboard: **C610/X99 series chipset**

Monitor: **Dell U2715H**

Sound Card: **ALC662**

Wireless Card: **FV-T919 (BCM94360CD, 4 antennas)**

Ethernet Card: **Intel I210/I218-LM)**

## Bios

- `VT-x`: **Enabled**;
- `Above 4G decoding`: **Enabled**;
- `Hyper Threading`: **Enabled**;
- `Execute Disable Bit`: **Enabled**;
- `EHCI/XHCI Hand-off`: **Enabled**;
- `CSM Support`: **Enabled**;

- `Secure Boot`: **Disabled**;

- `UEFI/Legacy Boot`: **Optional**.

## What works

- Sleep / Wake
- Wifi and Bluetooth (BCM94360CD)
- Handoff, Continuity, AirDrop
- iMessage, FaceTime, App Store, iTunes Store (Change Config.plist -> PlatformInfo -> Generic -> MLB and SystemSerialNumber)
- Ethernet
- Onboard audio
- SSD TRIM
- USB 2.0 / USB 3.0
- DP port


## Credits

- [KGP](https://github.com/kgp)
- [EchoEsprit](https://github.com/EchoEsprit)
