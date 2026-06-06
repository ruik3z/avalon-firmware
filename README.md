# Avalon NetHunter Support Module

KernelSU / Magisk module for Avalon Kernel.

## Features

* Automatically loads RT5370 monitor mode driver stack at boot
* Bundles required firmware blobs
* Configures firmware search path automatically
* Supports RT5370-based USB wireless adapters
* Includes custom Kali Linux boot animation
* No manual insmod commands required after installation

## Loaded Modules

* cfg80211.ko
* mac80211.ko
* rt2x00lib.ko
* rt2x00usb.ko
* rt2800lib.ko
* rt2800usb.ko

## Firmware

Firmware files are automatically copied to:

/data/local/nhsystem/kali-arm64/lib/firmware

Firmware loader path is configured automatically during boot.

## Requirements

* Avalon Kernel
* KernelSU or Magisk
* USB OTG support
* RT5370-based wireless adapter

## Installation

1. Flash the module through KernelSU or Magisk.
2. Reboot.
3. Connect the adapter.
4. Verify monitor mode functionality.

## Notes

This module was built specifically for Avalon Kernel and may not function correctly on other kernels.

The included boot animation is mounted during early boot using post-fs-data.
