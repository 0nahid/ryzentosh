# OpenCore EFI for AMD Laptops (updated to Ventura 13.6.1)

## OpenCore version: 0.9.5

## macOS version: 13.6.1

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
│   │   └── BOOTx64.efi
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
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── AMDRyzenCPUPowerManagement
│       │   │       └── _CodeSignature
│       │   │           └── CodeResources
│       │   ├── AirportItlwm.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── AirportItlwm
│       │   ├── AppleALC.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── AppleALC
│       │   ├── AppleMCEReporterDisabler.kext
│       │   │   └── Contents
│       │   │       └── Info.plist
│       │   ├── AsusSMC.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── AsusSMC
│       │   ├── BlueToolFixup.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── BlueToolFixup
│       │   ├── BrightnessKeys.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── BrightnessKeys
│       │   ├── ECEnabler.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── ECEnabler
│       │   ├── HoRNDIS.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── HoRNDIS
│       │   │       ├── Resources
│       │   │       │   └── en.lproj
│       │   │       │       └── InfoPlist.strings
│       │   │       └── _CodeSignature
│       │   │           └── CodeResources
│       │   ├── IntelBTPatcher.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── IntelBTPatcher
│       │   ├── IntelBluetoothFirmware.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── IntelBluetoothFirmware
│       │   ├── Lilu.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── Lilu
│       │   ├── NootedRed.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── NootedRed
│       │   ├── RadeonSensor.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── RadeonSensor
│       │   ├── RealtekCardReader.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── RealtekCardReader
│       │   │       └── Resources
│       │   │           └── LICENSE
│       │   ├── RestrictEvents.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── RestrictEvents
│       │   ├── Ryzen-CtlnaAHCIPort.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── CtlnaAHCIPort
│       │   │       ├── _CodeSignature
│       │   │       │   └── CodeResources
│       │   │       └── version.plist
│       │   ├── SMCAMDProcessor.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── SMCAMDProcessor
│       │   │       └── _CodeSignature
│       │   │           └── CodeResources
│       │   ├── SMCBatteryManager.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── SMCBatteryManager
│       │   │       └── Resources
│       │   │           └── SSDT-BATC.dsl
│       │   ├── SMCLightSensor.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── SMCLightSensor
│       │   ├── SMCProcessorAMD.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── SMCProcessorAMD
│       │   ├── SMCRadeonGPU.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── SMCRadeonGPU
│       │   ├── USBToolBox.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── USBToolBox
│       │   ├── UTBMap.kext
│       │   │   └── Contents
│       │   │       └── Info.plist
│       │   ├── VirtualSMC.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── VirtualSMC
│       │   ├── VoodooI2C.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       ├── MacOS
│       │   │       │   └── VoodooI2C
│       │   │       └── PlugIns
│       │   │           ├── VoodooGPIO.kext
│       │   │           │   └── Contents
│       │   │           │       ├── Info.plist
│       │   │           │       └── MacOS
│       │   │           │           └── VoodooGPIO
│       │   │           ├── VoodooI2CServices.kext
│       │   │           │   └── Contents
│       │   │           │       ├── Info.plist
│       │   │           │       └── MacOS
│       │   │           │           └── VoodooI2CServices
│       │   │           └── VoodooInput.kext
│       │   │               └── Contents
│       │   │                   ├── Info.plist
│       │   │                   ├── MacOS
│       │   │                   │   └── VoodooInput
│       │   │                   └── _CodeSignature
│       │   │                       └── CodeResources
│       │   ├── VoodooI2CHID.kext
│       │   │   └── Contents
│       │   │       ├── Info.plist
│       │   │       └── MacOS
│       │   │           └── VoodooI2CHID
│       │   └── VoodooPS2Controller.kext
│       │       └── Contents
│       │           ├── Info.plist
│       │           ├── MacOS
│       │           │   └── VoodooPS2Controller
│       │           └── PlugIns
│       │               ├── VoodooInput.kext
│       │               │   └── Contents
│       │               │       ├── Info.plist
│       │               │       ├── MacOS
│       │               │       │   └── VoodooInput
│       │               │       └── _CodeSignature
│       │               │           └── CodeResources
│       │               ├── VoodooPS2Keyboard.kext
│       │               │   └── Contents
│       │               │       ├── Info.plist
│       │               │       └── MacOS
│       │               │           └── VoodooPS2Keyboard
│       │               ├── VoodooPS2Mouse.kext
│       │               │   └── Contents
│       │               │       ├── Info.plist
│       │               │       └── MacOS
│       │               │           └── VoodooPS2Mouse
│       │               └── VoodooPS2Trackpad.kext
│       │                   └── Contents
│       │                       ├── Info.plist
│       │                       └── MacOS
│       │                           └── VoodooPS2Trackpad
│       ├── OpenCore.efi
│       ├── Resources
│       │   ├── Audio
│       │   │   ├── AXEFIAudio_Beep.mp3
│       │   │   ├── AXEFIAudio_Click.mp3
│       │   │   ├── AXEFIAudio_VoiceOver_Boot.mp3
│       │   │   ├── AXEFIAudio_ar_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ar_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ar_Password.mp3
│       │   │   ├── AXEFIAudio_ar_Username.mp3
│       │   │   ├── AXEFIAudio_ar_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ar_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ar_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_ca_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ca_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ca_Password.mp3
│       │   │   ├── AXEFIAudio_ca_Username.mp3
│       │   │   ├── AXEFIAudio_ca_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ca_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ca_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_cs_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_cs_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_cs_Password.mp3
│       │   │   ├── AXEFIAudio_cs_Username.mp3
│       │   │   ├── AXEFIAudio_cs_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_cs_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_cs_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_da_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_da_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_da_Password.mp3
│       │   │   ├── AXEFIAudio_da_Username.mp3
│       │   │   ├── AXEFIAudio_da_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_da_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_da_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_de_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_de_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_de_Password.mp3
│       │   │   ├── AXEFIAudio_de_Username.mp3
│       │   │   ├── AXEFIAudio_de_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_de_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_de_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_el_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_el_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_el_Password.mp3
│       │   │   ├── AXEFIAudio_el_Username.mp3
│       │   │   ├── AXEFIAudio_el_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_el_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_el_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_en_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_en_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_en_Password.mp3
│       │   │   ├── AXEFIAudio_en_Username.mp3
│       │   │   ├── AXEFIAudio_en_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_en_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_en_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_es_419_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_es_419_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_es_419_Password.mp3
│       │   │   ├── AXEFIAudio_es_419_Username.mp3
│       │   │   ├── AXEFIAudio_es_419_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_es_419_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_es_419_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_es_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_es_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_es_MX_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_es_MX_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_es_MX_Password.mp3
│       │   │   ├── AXEFIAudio_es_MX_Username.mp3
│       │   │   ├── AXEFIAudio_es_MX_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_es_MX_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_es_MX_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_es_Password.mp3
│       │   │   ├── AXEFIAudio_es_Username.mp3
│       │   │   ├── AXEFIAudio_es_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_es_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_es_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_fi_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_fi_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_fi_Password.mp3
│       │   │   ├── AXEFIAudio_fi_Username.mp3
│       │   │   ├── AXEFIAudio_fi_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_fi_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_fi_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_fr_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_fr_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_fr_Password.mp3
│       │   │   ├── AXEFIAudio_fr_Username.mp3
│       │   │   ├── AXEFIAudio_fr_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_fr_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_fr_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_he_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_he_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_he_Password.mp3
│       │   │   ├── AXEFIAudio_he_Username.mp3
│       │   │   ├── AXEFIAudio_he_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_he_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_he_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_hi_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_hi_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_hi_Password.mp3
│       │   │   ├── AXEFIAudio_hi_Username.mp3
│       │   │   ├── AXEFIAudio_hi_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_hi_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_hi_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_hu_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_hu_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_hu_Password.mp3
│       │   │   ├── AXEFIAudio_hu_Username.mp3
│       │   │   ├── AXEFIAudio_hu_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_hu_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_hu_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_id_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_id_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_id_Password.mp3
│       │   │   ├── AXEFIAudio_id_Username.mp3
│       │   │   ├── AXEFIAudio_id_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_id_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_id_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_it_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_it_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_it_Password.mp3
│       │   │   ├── AXEFIAudio_it_Username.mp3
│       │   │   ├── AXEFIAudio_it_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_it_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_it_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_ja_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ja_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ja_Password.mp3
│       │   │   ├── AXEFIAudio_ja_Username.mp3
│       │   │   ├── AXEFIAudio_ja_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ja_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ja_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_ko_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ko_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ko_Password.mp3
│       │   │   ├── AXEFIAudio_ko_Username.mp3
│       │   │   ├── AXEFIAudio_ko_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ko_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ko_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_nl_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_nl_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_nl_Password.mp3
│       │   │   ├── AXEFIAudio_nl_Username.mp3
│       │   │   ├── AXEFIAudio_nl_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_nl_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_nl_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_no_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_no_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_no_Password.mp3
│       │   │   ├── AXEFIAudio_no_Username.mp3
│       │   │   ├── AXEFIAudio_no_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_no_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_no_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_pl_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_pl_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_pl_Password.mp3
│       │   │   ├── AXEFIAudio_pl_Username.mp3
│       │   │   ├── AXEFIAudio_pl_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_pl_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_pl_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_pt_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_pt_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_pt_PT_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_pt_PT_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_pt_PT_Password.mp3
│       │   │   ├── AXEFIAudio_pt_PT_Username.mp3
│       │   │   ├── AXEFIAudio_pt_PT_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_pt_PT_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_pt_PT_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_pt_Password.mp3
│       │   │   ├── AXEFIAudio_pt_Username.mp3
│       │   │   ├── AXEFIAudio_pt_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_pt_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_pt_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_ro_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ro_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ro_Password.mp3
│       │   │   ├── AXEFIAudio_ro_Username.mp3
│       │   │   ├── AXEFIAudio_ro_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ro_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ro_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_ru_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_ru_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_ru_Password.mp3
│       │   │   ├── AXEFIAudio_ru_Username.mp3
│       │   │   ├── AXEFIAudio_ru_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_ru_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_ru_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_sk_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_sk_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_sk_Password.mp3
│       │   │   ├── AXEFIAudio_sk_Username.mp3
│       │   │   ├── AXEFIAudio_sk_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_sk_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_sk_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_sv_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_sv_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_sv_Password.mp3
│       │   │   ├── AXEFIAudio_sv_Username.mp3
│       │   │   ├── AXEFIAudio_sv_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_sv_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_sv_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_th_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_th_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_th_Password.mp3
│       │   │   ├── AXEFIAudio_th_Username.mp3
│       │   │   ├── AXEFIAudio_th_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_th_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_th_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_tr_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_tr_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_tr_Password.mp3
│       │   │   ├── AXEFIAudio_tr_Username.mp3
│       │   │   ├── AXEFIAudio_tr_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_tr_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_tr_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_zh_CN_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_zh_CN_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_zh_CN_Password.mp3
│       │   │   ├── AXEFIAudio_zh_CN_Username.mp3
│       │   │   ├── AXEFIAudio_zh_CN_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_zh_CN_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_zh_CN_VoiceOverOn.mp3
│       │   │   ├── AXEFIAudio_zh_TW_AccountLocked.mp3
│       │   │   ├── AXEFIAudio_zh_TW_AccountLockedTryLater.mp3
│       │   │   ├── AXEFIAudio_zh_TW_Password.mp3
│       │   │   ├── AXEFIAudio_zh_TW_Username.mp3
│       │   │   ├── AXEFIAudio_zh_TW_UsernameOrPasswordIncorrect.mp3
│       │   │   ├── AXEFIAudio_zh_TW_VoiceOverOff.mp3
│       │   │   ├── AXEFIAudio_zh_TW_VoiceOverOn.mp3
│       │   │   ├── OCEFIAudio_VoiceOver_Boot.mp3
│       │   │   ├── OCEFIAudio_en_1.mp3
│       │   │   ├── OCEFIAudio_en_2.mp3
│       │   │   ├── OCEFIAudio_en_3.mp3
│       │   │   ├── OCEFIAudio_en_4.mp3
│       │   │   ├── OCEFIAudio_en_5.mp3
│       │   │   ├── OCEFIAudio_en_6.mp3
│       │   │   ├── OCEFIAudio_en_7.mp3
│       │   │   ├── OCEFIAudio_en_8.mp3
│       │   │   ├── OCEFIAudio_en_9.mp3
│       │   │   ├── OCEFIAudio_en_AbortTimeout.mp3
│       │   │   ├── OCEFIAudio_en_ChooseOS.mp3
│       │   │   ├── OCEFIAudio_en_Default.mp3
│       │   │   ├── OCEFIAudio_en_DiskImage.mp3
│       │   │   ├── OCEFIAudio_en_EnterPassword.mp3
│       │   │   ├── OCEFIAudio_en_ExecutionFailure.mp3
│       │   │   ├── OCEFIAudio_en_ExecutionSuccessful.mp3
│       │   │   ├── OCEFIAudio_en_External.mp3
│       │   │   ├── OCEFIAudio_en_ExternalOS.mp3
│       │   │   ├── OCEFIAudio_en_ExternalTool.mp3
│       │   │   ├── OCEFIAudio_en_LetterA.mp3
│       │   │   ├── OCEFIAudio_en_LetterB.mp3
│       │   │   ├── OCEFIAudio_en_LetterC.mp3
│       │   │   ├── OCEFIAudio_en_LetterD.mp3
│       │   │   ├── OCEFIAudio_en_LetterE.mp3
│       │   │   ├── OCEFIAudio_en_LetterF.mp3
│       │   │   ├── OCEFIAudio_en_LetterG.mp3
│       │   │   ├── OCEFIAudio_en_LetterH.mp3
│       │   │   ├── OCEFIAudio_en_LetterI.mp3
│       │   │   ├── OCEFIAudio_en_LetterJ.mp3
│       │   │   ├── OCEFIAudio_en_LetterK.mp3
│       │   │   ├── OCEFIAudio_en_LetterL.mp3
│       │   │   ├── OCEFIAudio_en_LetterM.mp3
│       │   │   ├── OCEFIAudio_en_LetterN.mp3
│       │   │   ├── OCEFIAudio_en_LetterO.mp3
│       │   │   ├── OCEFIAudio_en_LetterP.mp3
│       │   │   ├── OCEFIAudio_en_LetterQ.mp3
│       │   │   ├── OCEFIAudio_en_LetterR.mp3
│       │   │   ├── OCEFIAudio_en_LetterS.mp3
│       │   │   ├── OCEFIAudio_en_LetterT.mp3
│       │   │   ├── OCEFIAudio_en_LetterU.mp3
│       │   │   ├── OCEFIAudio_en_LetterV.mp3
│       │   │   ├── OCEFIAudio_en_LetterW.mp3
│       │   │   ├── OCEFIAudio_en_LetterX.mp3
│       │   │   ├── OCEFIAudio_en_LetterY.mp3
│       │   │   ├── OCEFIAudio_en_LetterZ.mp3
│       │   │   ├── OCEFIAudio_en_Loading.mp3
│       │   │   ├── OCEFIAudio_en_OtherOS.mp3
│       │   │   ├── OCEFIAudio_en_PasswordAccepted.mp3
│       │   │   ├── OCEFIAudio_en_PasswordIncorrect.mp3
│       │   │   ├── OCEFIAudio_en_PasswordRetryLimit.mp3
│       │   │   ├── OCEFIAudio_en_Reloading.mp3
│       │   │   ├── OCEFIAudio_en_ResetNVRAM.mp3
│       │   │   ├── OCEFIAudio_en_Restart.mp3
│       │   │   ├── OCEFIAudio_en_SIPIsDisabled.mp3
│       │   │   ├── OCEFIAudio_en_SIPIsEnabled.mp3
│       │   │   ├── OCEFIAudio_en_Selected.mp3
│       │   │   ├── OCEFIAudio_en_ShowAuxiliary.mp3
│       │   │   ├── OCEFIAudio_en_Shutdown.mp3
│       │   │   ├── OCEFIAudio_en_Timeout.mp3
│       │   │   ├── OCEFIAudio_en_UEFI_Shell.mp3
│       │   │   ├── OCEFIAudio_en_Welcome.mp3
│       │   │   ├── OCEFIAudio_en_Windows.mp3
│       │   │   ├── OCEFIAudio_en_macOS.mp3
│       │   │   ├── OCEFIAudio_en_macOS_Recovery.mp3
│       │   │   ├── OCEFIAudio_en_macOS_TimeMachine.mp3
│       │   │   ├── OCEFIAudio_en_macOS_UpdateFw.mp3
│       │   │   ├── OCEFIAudio_ru_1.mp3
│       │   │   ├── OCEFIAudio_ru_2.mp3
│       │   │   ├── OCEFIAudio_ru_3.mp3
│       │   │   ├── OCEFIAudio_ru_4.mp3
│       │   │   ├── OCEFIAudio_ru_5.mp3
│       │   │   ├── OCEFIAudio_ru_6.mp3
│       │   │   ├── OCEFIAudio_ru_7.mp3
│       │   │   ├── OCEFIAudio_ru_8.mp3
│       │   │   ├── OCEFIAudio_ru_9.mp3
│       │   │   ├── OCEFIAudio_ru_AbortTimeout.mp3
│       │   │   ├── OCEFIAudio_ru_ChooseOS.mp3
│       │   │   ├── OCEFIAudio_ru_Default.mp3
│       │   │   ├── OCEFIAudio_ru_DiskImage.mp3
│       │   │   ├── OCEFIAudio_ru_EnterPassword.mp3
│       │   │   ├── OCEFIAudio_ru_ExecutionFailure.mp3
│       │   │   ├── OCEFIAudio_ru_ExecutionSuccessful.mp3
│       │   │   ├── OCEFIAudio_ru_External.mp3
│       │   │   ├── OCEFIAudio_ru_ExternalOS.mp3
│       │   │   ├── OCEFIAudio_ru_ExternalTool.mp3
│       │   │   ├── OCEFIAudio_ru_LetterA.mp3
│       │   │   ├── OCEFIAudio_ru_LetterB.mp3
│       │   │   ├── OCEFIAudio_ru_LetterC.mp3
│       │   │   ├── OCEFIAudio_ru_LetterD.mp3
│       │   │   ├── OCEFIAudio_ru_LetterE.mp3
│       │   │   ├── OCEFIAudio_ru_LetterF.mp3
│       │   │   ├── OCEFIAudio_ru_LetterG.mp3
│       │   │   ├── OCEFIAudio_ru_LetterH.mp3
│       │   │   ├── OCEFIAudio_ru_LetterI.mp3
│       │   │   ├── OCEFIAudio_ru_LetterJ.mp3
│       │   │   ├── OCEFIAudio_ru_LetterK.mp3
│       │   │   ├── OCEFIAudio_ru_LetterL.mp3
│       │   │   ├── OCEFIAudio_ru_LetterM.mp3
│       │   │   ├── OCEFIAudio_ru_LetterN.mp3
│       │   │   ├── OCEFIAudio_ru_LetterO.mp3
│       │   │   ├── OCEFIAudio_ru_LetterP.mp3
│       │   │   ├── OCEFIAudio_ru_LetterQ.mp3
│       │   │   ├── OCEFIAudio_ru_LetterR.mp3
│       │   │   ├── OCEFIAudio_ru_LetterS.mp3
│       │   │   ├── OCEFIAudio_ru_LetterT.mp3
│       │   │   ├── OCEFIAudio_ru_LetterU.mp3
│       │   │   ├── OCEFIAudio_ru_LetterV.mp3
│       │   │   ├── OCEFIAudio_ru_LetterW.mp3
│       │   │   ├── OCEFIAudio_ru_LetterX.mp3
│       │   │   ├── OCEFIAudio_ru_LetterY.mp3
│       │   │   ├── OCEFIAudio_ru_LetterZ.mp3
│       │   │   ├── OCEFIAudio_ru_Loading.mp3
│       │   │   ├── OCEFIAudio_ru_OtherOS.mp3
│       │   │   ├── OCEFIAudio_ru_PasswordAccepted.mp3
│       │   │   ├── OCEFIAudio_ru_PasswordIncorrect.mp3
│       │   │   ├── OCEFIAudio_ru_PasswordRetryLimit.mp3
│       │   │   ├── OCEFIAudio_ru_Reloading.mp3
│       │   │   ├── OCEFIAudio_ru_ResetNVRAM.mp3
│       │   │   ├── OCEFIAudio_ru_Restart.mp3
│       │   │   ├── OCEFIAudio_ru_SIPIsDisabled.mp3
│       │   │   ├── OCEFIAudio_ru_SIPIsEnabled.mp3
│       │   │   ├── OCEFIAudio_ru_Selected.mp3
│       │   │   ├── OCEFIAudio_ru_ShowAuxiliary.mp3
│       │   │   ├── OCEFIAudio_ru_Shutdown.mp3
│       │   │   ├── OCEFIAudio_ru_Timeout.mp3
│       │   │   ├── OCEFIAudio_ru_UEFI_Shell.mp3
│       │   │   ├── OCEFIAudio_ru_Welcome.mp3
│       │   │   ├── OCEFIAudio_ru_Windows.mp3
│       │   │   ├── OCEFIAudio_ru_macOS.mp3
│       │   │   ├── OCEFIAudio_ru_macOS_Recovery.mp3
│       │   │   ├── OCEFIAudio_ru_macOS_TimeMachine.mp3
│       │   │   └── OCEFIAudio_ru_macOS_UpdateFw.mp3
│       │   ├── Font
│       │   │   ├── Font_1x.bin
│       │   │   ├── Font_1x.png
│       │   │   ├── Font_2x.bin
│       │   │   └── Font_2x.png
│       │   ├── Image
│       │   │   └── Acidanthera
│       │   │       ├── Chardonnay
│       │   │       │   ├── AppleRecv.icns
│       │   │       │   ├── AppleTM.icns
│       │   │       │   ├── BtnFocus.icns
│       │   │       │   ├── Cursor.icns
│       │   │       │   ├── Dot.icns
│       │   │       │   ├── Enter.icns
│       │   │       │   ├── ExtAppleRecv.icns
│       │   │       │   ├── ExtAppleTM.icns
│       │   │       │   ├── ExtHardDrive.icns
│       │   │       │   ├── HardDrive.icns
│       │   │       │   ├── Left.icns
│       │   │       │   ├── Lock.icns
│       │   │       │   ├── Password.icns
│       │   │       │   ├── Restart.icns
│       │   │       │   ├── Right.icns
│       │   │       │   ├── Selected.icns
│       │   │       │   ├── Selector.icns
│       │   │       │   ├── SetDefault.icns
│       │   │       │   ├── Shell.icns
│       │   │       │   ├── ShutDown.icns
│       │   │       │   ├── Tool.icns
│       │   │       │   └── Windows.icns
│       │   │       ├── GoldenGate
│       │   │       │   ├── AppleRecv.icns
│       │   │       │   ├── AppleTM.icns
│       │   │       │   ├── BtnFocus.icns
│       │   │       │   ├── Cursor.icns
│       │   │       │   ├── Dot.icns
│       │   │       │   ├── Enter.icns
│       │   │       │   ├── ExtAppleRecv.icns
│       │   │       │   ├── ExtAppleTM.icns
│       │   │       │   ├── ExtHardDrive.icns
│       │   │       │   ├── HardDrive.icns
│       │   │       │   ├── Left.icns
│       │   │       │   ├── Lock.icns
│       │   │       │   ├── Password.icns
│       │   │       │   ├── Restart.icns
│       │   │       │   ├── Right.icns
│       │   │       │   ├── Selected.icns
│       │   │       │   ├── Selector.icns
│       │   │       │   ├── SetDefault.icns
│       │   │       │   ├── Shell.icns
│       │   │       │   ├── ShutDown.icns
│       │   │       │   ├── Tool.icns
│       │   │       │   └── Windows.icns
│       │   │       └── Syrah
│       │   │           ├── AppleRecv.icns
│       │   │           ├── AppleTM.icns
│       │   │           ├── BtnFocus.icns
│       │   │           ├── Cursor.icns
│       │   │           ├── Dot.icns
│       │   │           ├── Enter.icns
│       │   │           ├── ExtAppleRecv.icns
│       │   │           ├── ExtAppleTM.icns
│       │   │           ├── ExtHardDrive.icns
│       │   │           ├── HardDrive.icns
│       │   │           ├── Left.icns
│       │   │           ├── Lock.icns
│       │   │           ├── Password.icns
│       │   │           ├── Restart.icns
│       │   │           ├── Right.icns
│       │   │           ├── Selected.icns
│       │   │           ├── Selector.icns
│       │   │           ├── SetDefault.icns
│       │   │           ├── Shell.icns
│       │   │           ├── ShutDown.icns
│       │   │           ├── Tool.icns
│       │   │           └── Windows.icns
│       │   └── Label
│       │       ├── Apple.l2x
│       │       ├── Apple.lbl
│       │       ├── AppleRecv.l2x
│       │       ├── AppleRecv.lbl
│       │       ├── AppleTM.l2x
│       │       ├── AppleTM.lbl
│       │       ├── EFIBoot.l2x
│       │       ├── EFIBoot.lbl
│       │       ├── Other.l2x
│       │       ├── Other.lbl
│       │       ├── ResetNVRAM.l2x
│       │       ├── ResetNVRAM.lbl
│       │       ├── SIPDisabled.l2x
│       │       ├── SIPDisabled.lbl
│       │       ├── SIPEnabled.l2x
│       │       ├── SIPEnabled.lbl
│       │       ├── Shell.l2x
│       │       ├── Shell.lbl
│       │       ├── Tool.l2x
│       │       ├── Tool.lbl
│       │       ├── Windows.l2x
│       │       └── Windows.lbl
│       ├── Tools
│       │   └── CleanNvram.efi
│       └── config.plist
└── README.md
```

## Note:

- Please change MLB/ROM/Serial Number/UUID.
- There's no wifi support on my device because it's a realtek driver
