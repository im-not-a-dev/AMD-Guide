# Kexts

## What kexts do you need?

#### What is absolutely required?

[_VirtualSMC.kext_](https://github.com/acidanthera/VirtualSMC) \(Or [FakeSMC.kext](https://github.com/RehabMan/OS-X-FakeSMC-kozlek)\) is as aforementioned essential. This kext is what tells macOS "Yes this is a real Mac", emulating the functionality of the SMC on real Mac's. Without it, no Hackintosh.

[_NullCPUPowerManagement.kext_](https://github.com/corpnewt/NullCPUPowerManagement) _-_ This kext disables CPU Power Management, as that is not supported on AMD chips.

### Where can I find these kexts?

All the kexts shown here are available for download on the [_**kext repo**_](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw) _****_provided and maintained by Goldfish64. All these kexts are automagically built when a new kext update is commited.

### Ethernet

* _​_[_IntelMausiEthernet.kext_](https://github.com/Mieze/IntelMausiEthernet) - this works with most newer Intel LAN chipsets
* \_\_[_AppleIntelE1000e.kext_](https://sourceforge.net/projects/osx86drivers/) - this works with older Intel LAN chipsets - but can cause KPs on newer chipsets
* _​_[_AtherosE2200Ethernet.kext_](https://github.com/Mieze/AtherosE2200Ethernet) - this works for most Atheros or Killer networking chipsets
* _​_[_RealtekRTL8111.kext_](https://github.com/Mieze/RTL8111_driver_for_OS_X) - this works with most gigabit Realtek LAN chipsets
* _​_[_RealtekRTL8100.kext_](https://github.com/Mieze/RealtekRTL8100) - for 10/100 Realtek LAN chipsets

### Graphics

* \_\_[_Whatevergreen.kext_ ](https://github.com/acidanthera/WhateverGreen)_-_ this kext fixes a lot of GPU related issues.
* \_\_[_Lilu.kext_](https://github.com/acidanthera/Lilu) _-_ this kext acts as a loader for other kexts. More specifically it can patch kexts, processes and libraries.

### WiFi and Bluetooth <a id="wifi-and-bluetooth"></a>

\(I myself don't use bluetooth nor WiFi so I don't have knowledge in that, but here is some information on the subject by CorpNewt. _Check **Credits** for more info_\)  
  
`Apple is pretty minimal with their WiFi support, so I'll only cover the two main chipsets I'm familiar with. I've used a BCM94360CD + PCIe adapter, and BCM94352HMB/BCM94352Z in my Hackintoshes. The BCM94360CD worked OOB with no extras as it's a native card. For the BCM94352 flavors, I've been using` [_`AirportBrcmFixup.kext`_](https://github.com/acidanthera/AirportBrcmFixup) `and the companion` [_`Lilu.kext`_](https://github.com/vit9696/Lilu/releases) `for WiFi setup and` _`BrcmBluetoothInjector.kext`_ `(on 10.13.6+) or` _`BrcmPatchRAM2.kext`_ `alongside` _`BrcmFirmwareData.kext`_ `- all of the Brcm* kexts are from RehabMan's` [_`OS-X-BrcmPatchRAM`_](https://github.com/RehabMan/OS-X-BrcmPatchRAM) `repo.`

### Audio

* \_\_[_AppleALC.kext_](https://github.com/acidanthera/AppleALC) _-_ this kext supports most of the commonly used codecs, with the best quality.

### Extra

Depending on what hardware you have in your machine you might need some other kexts. This list is more to be used to give you a general idea, you will probably have to do some google-fu.

The safest way is to inject these into the system using Clover.

```text
CLOVER -> EFI -> CLOVER -> kext -> Other
```

