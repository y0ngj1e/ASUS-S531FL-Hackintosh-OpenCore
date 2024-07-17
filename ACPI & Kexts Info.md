# ACPI
- **SSDT-AWAC.aml**: To fix RTC clock and fix initial boot halt
- **SSDT-BATT.aml**: To enable full battery information readout on macOS and enable limit charging capacity
- **SSDT-dGPU-Off.aml**: Disables and fully shuts down Nvidia MX250 in macOS
- **SSDT-EC.aml**: To patch Embedded Controller name and stop kernel panic
- **SSDT-GPIO.aml**: Patch ELAN1200 TrackPad
- **SSDT-PLUG.aml**: Patch CPU Power Management
- **SSDT-PMC.aml**: To fix and enable native NVRAM and fix initial boot halt
- **SSDT-PNLFCFL.aml**: To patch display backlight
- **SSDT-SBUS-MCHC.aml**: Fix SMBus
- **SSDT-USBX.aml**: To power up all USB ports
- **ssdt_data.aml**: Data for CPUFriend

# Drivers
- **AudioDxe.efi**: Enable Boot chime in OpenCore
- **HfsPlus.efi**: HFS+ driver to load HFS+ formatted USB installers
- **OpenCanopy.efi**: Load OpenCore GUI
- **OpenRuntime.efi**: OpenCore's backbone
- **ResetNvramEntry.efi**: Enable the option to reset NVRAM

# Kexts
- **AirportItlwm.kext**: Enable Intel Wifi. For macOS 14.4+. Replace this kext if target version is lower.
- **AppleALC.kext**: Enable audio
- **AsusSMC.kext**: Enable battery charging limiter
- **BlueToolFixup.kext**: Bluetooth fix
- **BrightnessKeys.kext**: Fix brightness keys
- **CPUFriend.kext**: Further optimise CPU Power Management
- **CPUFriendDataProvider.kext**: 800MHz min freq & performance power state. Built for 14.5. Rebuild if using different version.
- **CpuTscSync.kext**: Fix CPU to prevent kernel panic
- **IntelBluetoothFirmware.kext**: Enable Intel Bluetooth
- **IntelBTPatcher.kext**: Intel Bluetooth fix
- **Lilu.kext**: Backbone of loading kexts
- **NVMeFix.kext**: Fix and power up NVMe drives
- **SMCBatteryManager.kext**: Enable battery readout
- **SMCProcessor.kext**: Enable CPU temp monitoring
- **USBToolBox.kext**: Map all USB ports
- **UTBMap.kext**: Map all USB ports
- **VirtualSMC.kext**: Backbone of the hackintosh
- **VoltageShift.kext**: Undervolt CPU. Build this kext on your system on post install
- **VoodooI2C.kext**: Enable full TrackPad support
- **VoodooI2CHID.kext**: Enable full TrackPad support
- **VoodooPS2Controller.kext**: Enable keybaord
- **WhateverGreen.kext**: Enable QE/CI on UHD 620
