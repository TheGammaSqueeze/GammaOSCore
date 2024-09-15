This beta release is for Patreon supporters only. If you'd like the password to this build, please join my Patreon (Gamma Insider/Innovator tiers): https://www.patreon.com/GammaOS
----------------------------

Supported Devices
----------------------------
**Anbernic**
- RG ARC-D / RG ARC-S (GammaOS_Core_Beta1_RG_ARC.7z)
- RG353V / RG353VS (GammaOS_Core_Beta1_RG_353.7z)
- RG353P / RG353PS (GammaOS_Core_Beta1_RG_353.7z)
- RG353M (GammaOS_Core_Beta1_RG_353.7z)
- RG503 (GammaOS_Core_Beta1_RG_503.7z)

**Powkiddy**
- RGB30 (GammaOS_Core_Beta1_RGB30_RGB20SX.7z)
- RGB20SX (GammaOS_Core_Beta1_RGB30_RGB20SX.7z)
- RGB10MAX3 (GammaOS_Core_Beta1_RGB10MAX3.7z)

### **A minimum of a 32GB MicroSD card is recommended, with speeds similar to a Sandisk Ultra card.**

Information
----------------------------
GammaOS Core is a minimal version of Android 13 TV suited for low powered devices with chipsets such as the Rockchip RK3566 and with no touchscreen required.
It has been heavily modified to reduce memory footprint and introduce quality of life enhancements to your devices. 

Check out a demo of it here: https://www.youtube.com/watch?v=M8nKMQjlut0
[![GammaOS Core (Android 13) demo on Powkiddy RGB20SX
](https://i3.ytimg.com/vi/M8nKMQjlut0/maxresdefault.jpg)](https://www.youtube.com/watch?v=M8nKMQjlut0 "GammaOS Core (Android 13) demo on Powkiddy RGB20SX")

Features
----------------------------
- Boot from SD card, you can keep your existing eMMC install intact (if applicable)
- Includes RetroArch preinstalled and preconfigured. 
- Includes Plain Launcher preinstalled and preconfigured (credit: https://bokonon-yossarian.itch.io/plain-launcher)
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
- Download the relevant device image at the bottom of this page for your device (GammaOS_Core_Beta1_XXX.7z)
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
- Vibration is not supported yet, this will come in the next release
- If you have used any OS that uses the mainline kernel (such as Rocknix), you will experience reboots instead of the device shutting down. You will need to unplug your battery and plug it back in. This is a known issue between the compatibility of BSP and mainline kernels. 
- PPSSPP will incorrectly try to create its application directories on the root of your internal storage, you will need to change this within PPSPP (when installed) to a dedicated directory on the storage.


Changelog
----------------------------
- Beta1: Initial beta release
