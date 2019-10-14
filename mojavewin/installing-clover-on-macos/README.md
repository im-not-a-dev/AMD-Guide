# Installing Clover on macOS

Once your system is installed you won't want to boot with the USB drive each time...  
We will now assume you are reading this now from your macOS desktop.

### Installing Clover.

The most complete Hackintosh Bootloader. Boot OS X, Windows, and Linux on Mac or PC with UEFI or BIOS firmware.

Download the latest Clover package from [here](https://sourceforge.net/projects/cloverefiboot/)...

### Clover Installer Configuration.

From there you need to follow the steps on the installer but use the Customise option to correctly install for your System. Use the settings below,

**UEFI Motherboard Settings**

* Install Clover for UEFI only
* Install Clover in ESP
* UEFIDrivers: AptioMemoryFix - PartitionDxe - ApfsLoader, don't touch the pre-ticked options
* Install RC Scripts on target volume

**Legacy Motherboard Settings**

* Install Clover in ESP
* Boot0ss
* Clover EFI Sata
* Bios Drivers, 64 bit: ApfsLoader
* Install RC Scripts on target volume

Now to configure Clover for your System...

