Firmware Release Notes

Note - In order to update the firmware, you will need to place the PCUI into bootloader mode.  This can be done via the main menu, then Settings, then Update Firmware.  

The PCUI will reboot into it’s bootloader mode.  Plug the PCUI into a Mac or PC, and drag and drop the firmware file onto the removable drive that appears.  

The PCUI will decrypt the firmware file, verify the signature, and if it passes, it will pause for 5 seconds, flash, and reboot.  

Note that the PCUI bootloader is different from the Pico bootloader - if you use the bootsel button on the pico to get into the bootloader and drag and drop the PCUI firmware, it will be rejected as the Pico's bootloader cannot decrypt the firmware image.  You can easily determine which bootloader you are in by looking at the directory contents of the USB drive which appears on your computer.  If you see PCUI.txt, then you are in the PCUI's bootloader.  If you see another *UF2.txt file, then you are in the Pico's bootloader.


07-04-2026 - PCUI_V1.01_B1658.uf2

This release addresses protocol bugs for the Casio PB-100 series devices and the Casio PB-700 series devices.  The printer and cassette interface was rewritten based on actual wire captures.  For the PB-700 series, ASCII mode program transfers are now reliable.