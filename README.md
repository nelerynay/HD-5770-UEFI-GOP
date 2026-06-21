# HD-5770-UEFI-GOP
A modification for AMD Radeon HD 5770 Series to run UEFI GOP instead of legacy, and disable CSM.

## DISCLAIMER
Can break your GPU since we are doing straight flash to VBIOS. Proceed with caution.

## What you need
1. A Radeon HD 5770
2. your VBIOS
3. [GOPUpdater](https://github.com/YTEC-info/GOP_Updater/tree/main)
4. ATI Winflash
5. Python


## GUIDE
1. Prepare your VBIOS, you can do this by using GPU-Z and saving your current VBIOS.
2. Drag your VBIOS to GOPupd.bat
3. If there is 2 version Latest/Legacy, Select latest.
4. **PROCEED WITH CAUTION** If it tells you that your VBIOS doesn't have enough space for latest GOP and microcode, **please select B for microcode.** the reason for this is because VBIOS only have **1MB memory**, flashing more than that **can cause brick**
5. A 127 KB file is prepared, with the name "[GPUCodename]_updGOP.rom"
6. run ATI Winflash, click "Load image" and select the update VBIOS file.
7. Wait until the flash is done, and restart your system.
8. To make sure it's working, check GPU-Z under the "UEFI", if the checkmark is there it means you can disable CSM Compability in BIOS.

### Is it worth anything?
- hmmm.. I don't know, but it is worth it if you're planning to use this on MacPro, or Hackintosh machine.
- No performance gain I guess, but your OEM logo will be not streched to 1280x720p and display the native resolution.
