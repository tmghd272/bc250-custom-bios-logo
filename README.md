# bc250-custom-bios-logo
BC250 BIOS custom boot logo theme — AMI OEM tool “ChangeLogo.exe” included for DIY logo modification

## Table of Contents
- [AMD BC-250 Custom AMI BIOS Logo](#amd-bc-250-custom-ami-bios-logo)
  - [Setup Tutorial](#setup-tutorial)
- [Making your own Custom Logo](#making-your-own-custom-logo)
  - [How to use AMI Change Logo Tool](#how-to-use-ami-change-logo-tool)
- [Logo Format Recommendations](#logo-format-recommendations)
- [Disclaimer](#disclaimer)

# AMD BC-250 Custom AMI BIOS Logo

The ROM file still contains the **unlocked chipset menu of P3.00**, it just comes with the custom boot logo I made.

- [Download the bc250-amd.rom here](bc250-amd.rom)

<img src="amd-bc250.png" width="400">

## Setup Tutorial

You will need to reflash your BIOS with the `bc250-amd.rom` (with my logo or your [custom logo](#making-your-own-custom-logo)), just like how you would if you followed the steps for flashing with an unlocked UMA Buffer/VRAM.

If you haven’t flashed the BIOS before, there are multiple ways of flashing it: CH341A (hardware method), AMI Firmware Update Utility (USB UEFI method), or software method (usually not recommended).

Here’s a YT video guide for the USB UEFI method by [Old Lamer](https://www.youtube.com/watch?v=dieD-CuBQr0)

Or a complete written guide for the USB UEFI method by [elektricm](https://elektricm.github.io/amd-bc250-docs/bios/flashing/#method-1-usb-flashing-efi-shell-method)

# Making your own Custom Logo.

You can make your own custom logo as well using AMI's software "[ChangeLogo.exe](ChangeLogo.exe)".

VirusTotal: https://www.virustotal.com/gui/file/aacf50e75f8c954047e93986315fc25cfa4619697c2f32f04889646c59fcdbd3

<img src="AMI's-Change-Logo-Tool.png" width="550">

## How to use AMI Change Logo Tool 

AMI Change Logo Tool should work on any American Megatrends-based BIOS, like ASUS, ASRock, Gigabyte, MSI, and others.

1.	Click **Load Image** and select the BIOS .rom file you want to modify.
2.	Click **Browse** under Save Logo and choose a BMP image you want to use as the logo.
3.	Click **Replace Logo** — that’s it!

# Logo Format Recommendations

From my experience, the best image logo format is:

BMP File Format

24-bit bit depth

672 × 378 (16:9)

96 DPI

Use black backgrounds — don’t use transparent backgrounds because it could cause visual glitches in the logo itself.

# Disclaimer

This project is for cosmetic purposes only and doesn’t affect performance.

Use at your own risk — use a hardware programmer (e.g., CH341A or Raspberry Pi) for recovery purposes.
