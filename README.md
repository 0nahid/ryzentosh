# OpenCore EFI for AMD Laptops (updated to Ventura 13.4)

## OpenCore version: 0.9.3

## macOS version: 13.4

My laptop: ASUS D509DJ-EJ030T

CPU: AMD Ryzen 5 3500U

GPU: AMD Radeon Vega 8

RAM: 12GB DDR4 2666MHz

SSD: 512GB NVMe

# Whats in the Box?

```
.
├── EFI
│   ├── BOOT
│   │   ├── BOOTx64.efi
│   │   ├── DisplayEngine.efi
│   │   ├── Loader.efi
│   │   ├── SREP_Config.cfg
│   │   ├── SetupBrowser.efi
│   │   ├── SuppressIFPatcher.efi
│   │   └── UiApp.efi
│   └── OC
│       ├── ACPI
│       │   ├── SSDT-EC.aml
│       │   ├── SSDT-HPET.aml
│       │   ├── SSDT-PLUG.aml
│       │   ├── SSDT-PNLF.aml
│       │   ├── SSDT-USBX.aml
│       │   └── SSDT-XOSI.aml
│       ├── Drivers
│       │   ├── HfsPlus.efi
│       │   ├── OpenCanopy.efi
│       │   └── OpenRuntime.efi
│       ├── Kexts
│       │   ├── AMDRyzenCPUPowerManagement.kext
│       │   ├── AirportItlwm.kext
│       │   ├── AmdTscSync.kext
│       │   ├── AppleALC.kext
│       │   ├── AppleMCEReporterDisabler.kext
│       │   ├── AsusSMC.kext
│       │   ├── BlueToolFixup.kext
│       │   ├── BrightnessKeys.kext
│       │   ├── ECEnabler.kext
│       │   ├── IntelBTPatcher.kext
│       │   ├── IntelBluetoothFirmware.kext
│       │   ├── Lilu.kext
│       │   ├── NVMeFix.kext
│       │   ├── NootedRed.kext
│       │   ├── RadeonSensor.kext
│       │   ├── RestrictEvents.kext
│       │   ├── SMCAMDProcessor.kext
│       │   ├── SMCBatteryManager.kext
│       │   ├── SMCLightSensor.kext
│       │   ├── SMCProcessorAMD.kext
│       │   ├── SMCRadeonGPU.kext
│       │   ├── USBToolBox.kext
│       │   ├── UTBMap.kext
│       │   ├── VirtualSMC.kext
│       │   ├── VoodooI2C.kext
│       │   ├── VoodooI2CHID.kext
│       │   └── VoodooPS2Controller.kext
│       ├── OpenCore.efi
│       ├── Resources
│       │   ├── Audio
│       │   ├── Font
│       │   ├── Image
│       │   └── Label
│       ├── Tools
│       │   └── CleanNvram.efi
│       └── config.plist
└── README.md
```

## Note:

- Please change MLB/ROM/Serial Number/UUID.
- There's no wifi support on my device because it's a realtek driver
