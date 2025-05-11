<h1 align="center">🍏 Hackintosh on Dell OptiPlex 5040</h1>

<p align="center">
  Bringing macOS to life on a stable Skylake desktop machine using OpenCore.
</p>

---

## 🖥️ System Specifications

| Component        | Details                                         |
|------------------|--------------------------------------------------|
| **Model**        | Dell OptiPlex 5040 (Desktop Tower)              |
| **CPU**          | Intel Core i7-6700 (4 Cores / 8 Threads, 3.4 GHz)|
| **iGPU**         | Intel HD Graphics 530                           |
| **Audio**        | Realtek ALC255 (via AppleALC)                   |
| **Ethernet**     | Intel Ethernet Connection (2) I219-V            |
| **Storage**      | 128GB SSD (HS-SSD-E100), 256GB SSD, 500GB HDD   |
| **Monitor**      | HP EliteDisplay E243 – 23.8" IPS LCD (HDMI)     |
| **RAM**          | 2×8GB DDR3 @ 1600MHz (SK hynix)                 |

---

## ✅ What Works

- Intel HD 530 Graphics Acceleration (QE/CI)  
- Audio via `AppleALC.kext`  
- Ethernet via `IntelMausi.kext`  
- All USB 2.0 / 3.0 Ports (with custom `USBMap.kext`)  
- Native shutdown and restart  
- HDMI Display Output  
- App Store, iMessage, iCloud (with proper SMBIOS)  

---

## ❌ What Doesn't Work

- Sleep (may require DSDT patches)  
- AirDrop (unless Broadcom card is installed)  
- Integrated Wi-Fi (not available by default)  

---

## 🔧 Bootloader & Kexts

- **Bootloader**: OpenCore 0.9.x  
- **macOS Tested**: Ventura and newer 
- **Kexts Used**:
  - `Lilu.kext`
  - `WhateverGreen.kext`
  - `AppleALC.kext`
  - `IntelMausi.kext`
  - `VirtualSMC.kext`
  - `USBMap.kext`
  - ...

---

## 🧩 BIOS Settings (Recommended)

- Disable Secure Boot  
- Set SATA Mode to AHCI  
- Enable UEFI Boot Mode  
- Disable VT-d (unless using `DisableIoMapper`)  
- Enable Legacy Option ROMs  

---

## 🙏 Credits

- 🍏 **Apple** – for macOS  
- ⚙️ **Acidanthera** – OpenCore and essential kexts  
- 📖 **Dortania** – for the OpenCore Install Guide  
- 🧰 **CorpNewt** – for USBToolBox and GenSMBIOS  
- 💡 **Hackintosh Community** – for support and testing  

