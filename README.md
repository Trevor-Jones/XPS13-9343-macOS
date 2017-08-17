# XPS13-9343-macOS 10.12

- Kexts used are in `/KEXTS/` Use `Kext Utility.app` to install to `/System/Library/Extensions/`
- Some info can be found in [this thread](https://www.tonymacx86.com/threads/guide-dell-xps-13-9343-sierra.206399/). However, the part about preference panes is bad, DO NOT FOLLOW THAT STEP.
- You may need VoodooPS2Controller.kext for keyboard and trackpad
- Patch the DSDT following [this](https://www.tonymacx86.com/threads/guide-patching-laptop-dsdt-ssdts.152573/) guide with these patches:
    - [bat] Dell XPS 13
    - [igpu] Brightness Fix (Haswell/Broadwell)
    - [sys] AC Adapted Fix
- Use clover configurator to replace the config.plist with the one in this repo
- Mount the USB EFI partition and copy all files to the EFI partition on the SSD
