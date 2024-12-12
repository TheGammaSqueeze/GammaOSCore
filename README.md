![BannerLogo](https://github.com/user-attachments/assets/93cf5031-9b0c-44f0-ac4b-c2044da06b6e)

Information
----------------------------
GammaOS Core is a minimal version of Android 13 TV suited for low powered devices with chipsets such as the Rockchip RK3566 and with no touchscreen required.
It has been heavily modified to reduce memory footprint and introduce quality of life enhancements to your devices. 

### **A minimum of a 32GB A2 spec MicroSD card is recommended, with speeds similar to a Sandisk Extreme (A2 for gaming) or Samsung Pro Plus card. Don't use a low quality card, performance will be poor or the device may not boot at all.**
![image](https://github.com/user-attachments/assets/8ea78619-e608-4486-8ec9-d06572c74a0c)


Recommended cards: 
- https://www.samsung.com/uk/memory-storage/memory-card/memory-card-pro-plus-microsd-card-128gb-mb-md128sa-eu/
- https://shop.sandisk.com/en-gb/products/memory-cards/microsd-cards/sandisk-extreme-uhs-i-for-mobile-gaming-microsd?sku=SDSQXAH-064G-GN6GN

Supported Devices
----------------------------
**Anbernic**
- RG ARC-D / RG ARC-S
- RG353V / RG353VS
- RG353P / RG353PS
- RG353M
- RG503

**Powkiddy**
- RGB30
- RGB20SX
- RGB10MAX3
- RGB20 PRO
- X55

**GKD**
- Bubble (requires additional steps to run GammaOS Core) (Bluetooth and USB OTG not currently supported)


Features
----------------------------
- Boot from SD card, you can keep your existing eMMC install intact (if applicable)
- Includes RetroArch preinstalled and preconfigured. 
- Includes Daijisho preinstalled and preconfigured
- Includes MiXplorer (SD, FTP, Lan, Cloud and other storage explorers)
- Rooted, with Magisk support
- Quick Settings menu (by holding down Power button)
- Mouse emulation mode (by holding down Select and R1)
- Bluetooth Audio support
- MTP USB support for quick files access
- Improved CPU and Graphics performance on some units
- Improved battery life and standby time on some units
- Relaxed Scoped Storage enforcement, for easier access to your files
- (RK3566) HDMI output settings, insert HDMI cable, choose your setting and reboot for a better HDMI experience!

Shortcuts
----------------------------
**Global Shortcuts**
- Home button (on selected devices) + Right Stick Up/Down: Adjust brightness
- Home button (on selected devices) + Volume Button Up/Down: Adjust brightness
- Power Button (hold): Global shortcuts menu (Brightness, Performance Modes, Controller Settings, USB Options, Killing apps options)

**RetroArch (on devices with a Home/Back/FN button)**
- Home button (quick tap): Show RetroArch menu
- Home button (long press): Save state and exit RetroArch (will resume state on game relaunch). Useful with a launcher like ES-DE, similar to Game Switcher on OnionOS.

**RetroArch (all devices)**
- L3 + R3 (without hotkey): Show RetroArch menu
- Hotkey: Select or Home button
- L1: Slow Motion toggle
- L2: Save State
- R1: Fast Forward toggle
- R2: Load State
- X: Toggle FPS counter
- Y: Screenshot
- R3: Toggle Shader
- Right Stick Left/Right: Change Shader

Instructions (Windows only)
----------------------------
**NOTE: Do not try and use a tool like DD, Win32DiskImager or balenaEtcher, this will not work.**
- Ensure you have 7-Zip installed
- Download the relevant device image at the bottom of a release on this page (https://github.com/TheGammaSqueeze/GammaOSCore/releases) for your device (GammaOS_Core_Beta1_XXX.7z)
- Download SDDiskTool_v1.69.zip
- Extract the SDDiskTool_v1.69.zip and GammaOS_Core_Beta1_XXX.7z (ensuring you use the password provided)
- Ensuring that your MicroSD card is inserted into your card reader, open the SD_Firmware_Tool.exe in the SDDiskTool_v1.69 folder
![image](https://github.com/user-attachments/assets/96c5db3b-8c29-4ceb-8ac3-e377af63eb8c)
- Choose the SD Boot option in the application, then click the Firmware button. You will be asked to select your extracted disk image from the GammaOS_Core_Beta1_XXX.7z file
![image](https://github.com/user-attachments/assets/87f7872b-52b9-4d5b-8759-1cbec9fb7778)
- Press the Create button to begin flashing GammaOS Core to your MicroSD card (this may take a few tries to complete successfully)
![image](https://github.com/user-attachments/assets/74288a20-ea31-4e2e-a762-b4599fc26ed4)
- Once complete, eject the MicroSD card, insert this into your device and boot at you would like any Linux OS. 

Known Issues
----------------------------
- Vibration is not supported yet, this will come in a future release
- If you have used any OS that uses the mainline kernel (such as Rocknix), you will experience reboots instead of the device shutting down. This can be resolved by either a) Booting back into mainline (e.g Rocknix) and shutting down from there, or b) you will need to unplug your battery and plug it back in. This is a known issue between the compatibility of BSP and mainline kernels.


Changelog
----------------------------
- Beta2: Added memory improvements, added additional emulators, switched to Daijisho as default launcher, relaxed scoped storage completely, improved mouse emulation mode (right stick/trigger buttons simulate wheel scrolling), added GammaOS Tweaks menu to Settings (32bit, webview, memory clear toggles), moved swap from file to partition. 
- Beta1: Initial beta release
