## Installation
1. Flash the module using KernelSU or Magisk.

2. Reboot the device.

3. Connect the supported adapter or SDR device.

4. Launch NetHunter and begin using the device.

## Notes
This module was designed specifically for Avalon Kernel.

Compatibility on other kernels is not guaranteed.

For Kali NetHunter installation and setup instructions, refer to the [NetHunter setup guide](https://github.com/ruik3z/nethunter-guide) repository.

# Miscellanous Details, Adapter Support, etc.

# Avalon Firmware
KernelSU / Magisk module providing external wireless adapter, SDR and NetHunter support for Avalon Kernel.

## Features
- Automatically loads supported wireless and SDR driver stacks during boot

- Bundles required firmware blobs for supported adapters

- Configures Linux firmware search paths automatically
a
- Enables plug-and-play support for compatible USB WiFi adapters

- Provides Software Defined Radio (SDR) driver support for compatible RTL2832-based devices

- Eliminates the need for manual module loading after every reboot

## Included Support
### Wireless Adapters
Support is provided for a wide range of chipsets used by common USB wireless adapters, including:

- MediaTek MT7601U

- Ralink RT2500USB

- Ralink RT2800USB family

- Realtek RTL8187

- Realtek RTL8192CU

- Realtek RTL8XXXU family

- ZyDAS ZD1201

- ZyDAS ZD1211 / ZD1211B

- Wireless RNDIS adapters

### SDR Devices
Support is included for RTL2832-based SDR receivers and related frontend components.

## Firmware Handling
Firmware files are automatically copied to:

`/data/local/nhsystem/kali-arm64/lib/firmware`

The Linux firmware loader path is configured automatically during boot.

No manual firmware configuration is required.

## Requirements
- Avalon Kernel

- KernelSU or Magisk

- USB OTG support

- Compatible wireless adapter or SDR device
