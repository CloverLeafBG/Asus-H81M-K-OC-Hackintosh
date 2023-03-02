# Asus-H81M-K-OC-Hackintosh

OpenCore based EFI for Asus H81M-K


![ASus](https://user-images.githubusercontent.com/93620854/213602398-cd8d3cd7-991e-466b-beeb-ee048b02e671.png)



## Tested macOS Version

- macOS Catalina 10.15.7
- macOS BigSur 11.7.3
- macOS Monterey 12.6.3


## System Configuration


- Motherboard:  Asus H81M-K 
- CPU: Intel Xeon E3-1226 V3 (no iGPU) + intel stock cooler
- Socket: LGA1150
- RAM: 2x4GB DDR3 @ 1600 Mhz
- GPU: Sapphire HD 7750 Ultimate 1GB Fanless (1x DVI , 1x HDMI 1.4a , 1x DisplayPort 1.2)
- SSD: Samsung 840 EVO 250 GB


### BIOS Version

3604

 
### Bootloader

OpenCore 0.8.8


### SMBIOS

Macmini7,1


## BIOS Settings
 

### Enable:

 
- EHCI Hand-off
- Intel xHCI Mode
- Sata Mode: AHCI
- iGPU Memory: 64MB (if using iGPU only)
- Execute Disable Bit
- OS type: Windows 10 UEFI mode
- Intel Virtualization

 

### Disable:

- Fast Boot
- Secure Boot
- Serial/Com Port
- VT-d
- Parallel Port


## What's working

 - [x] Sleep, Restart, Shutdown
 
 - [x] CPU - Speedstep and power management

 - [x] dGPU - Fully working QE/CI , Metal support + audio over HDMI (radpg=15 used for propper GPU initialization) 
 
 - [x] USB2.0 , USB3.0
 
 - [x] Audio - ALC887
 
 - [x] Ethernet - Realtek 8111
 


## What's not working

- So far everything is working great

## Not tested

- iGPU - my CPU doesn't have iGPU so I am not able to test it



## Additional Notes

- Kext signing is disabled so I can use chris1111's web drivers for my TP-Link T3U adapter - https://github.com/chris1111/Wireless-USB-Big-Sur-Adapter

- MacOS Monterey will only boot with model Macmini7,1 !!! All other OS versions will boot normally with both Macmini7,1 or iMac15,1

- Don't forget to generate your own SMBIOS with https://github.com/corpnewt/GenSMBIOS. 

## ENJOY!
