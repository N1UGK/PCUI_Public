Firmware Release Notes

Note - In order to update the firmware, you will need to place the PCUI into bootloader mode.  This can be done via the main menu, then Settings, then Update Firmware.  

The PCUI will reboot into it’s bootloader mode.  Plug the PCUI into a Mac or PC, and drag and drop the firmware file onto the removable drive that appears.  

The PCUI will decrypt the firmware file, verify the signature, and if it passes, it will pause for 5 seconds, flash, and reboot.  

Note that the PCUI bootloader is different from the Pico bootloader - if you use the bootsel button on the pico to get into the bootloader and drag and drop the PCUI firmware, it will be rejected as the Pico's bootloader cannot decrypt the firmware image.  You can easily determine which bootloader you are in by looking at the directory contents of the USB drive which appears on your computer.  If you see PCUI.txt, then you are in the PCUI's bootloader.  If you see another *UF2.txt file, then you are in the Pico's bootloader.

08-04-2025 - PCUI_V1.15_B2364.uf2

Added Hex Translation feature for printing from pocket computers with limited range of byte output.
Fixed plotter emulation for Casio models, bytes were not converted to ASCII before being dispatched to the plotter emulator.
Fixed plotter emulation for Sharp models, bytes were not routed to the plotter emulator.
Fixed race condition when exiting printer mode (CE-126 compatibles) during the 1.4 second EOL pause timer.
Added proper handling for when a PC or Mac host "ejects" our SD card passthrough.
Fixed issue where send menu options disappear when exiting SD card passthrough mode (some Sharp modes).
Added a settling delay for parallel port output before reading "busy" pin, enabled via Slow Printer in Printer menu.
Added Program Repo feature which allows browsing of the public GitHub Pocket Computer Programs folder to view and install programs per model, from the PCUI.
Added screen saver to prevent OLED burn in
Fixed issue where PNG and AGIF plotter emulation output was not saved if no printer is selected or if a non-graphics capable printer was selected.
Fixed PC-1245 tokenization issue with the "?" character and spacing causing keywords to fall through.

07-29-2025 - PCUI_V1.14_B2080.uf2

Fixed issue with Casio models which used the FA-3 cassette interface, timing issue with tape loading was present on the release build, debug builds unaffected.
Fixed issue with Sharp models, CE-126P compatibles, printing support in release mode, timing issue.
Fixed Casio FX-702P, open detect and printing support, timing issue in release mode.
Added RTS/CTS flow control support for RS-232 port.
Added preliminary Sharp PC-1260 and PC-1280 support, which is a combination of existing 1401 support (for tape) and 1245 support (for the printer).
Corrected last 4 pins displayed in self-set mode, buffer test.
Fixed display of mode "None" and menu option for this model/mode.  None now appears in the menu, and PCUI will be displayed on the home screen.
Updated frequency out generator in self-test mode for Pico2 (was set based on Pico1).
Added OE and Direction toggling for level shifting pocket computer buffer in self-test mode.

07-18-2026 - PCUI_V1.13_B1996.uf2

Fixed SD card mount issue after bootloader session, SD card mount failed.
Added debug output option when saving programs and variables.  This debug.bin will contain all framing and content received.

07-17-2026 - PCUI_V1.12_B1975.uf2

Fixed Sharp PC-1245 printer bug - an extra bit was introduced from an erroneous SEL2, BUSY pulse in some printing scenarios. 

07-16-2026 - PCUI_V1.11_B1968.uf2

Fixed tokenization and detokenization issues for Sharp PC-1245. 
Fixed SD card folder for Sharp PC-1245 (was incorrectly using PC-1246).
Added WIFI.TXT support (see owners manual for description).
Fixed issue where SD card removal (while powered on) would cause reboot if config is the same (unchanged).
SD card subfolders automatically created when mode is selected, rather than on-demand during save.
When in an empty BASIC folder, the web interface did not show the Create New button.

07-10-2026 - PCUI_V1.10_B1776.uf2

Support added for the Sharp PC-1210/PC-1211/PC-1212 (tested only on the PC-1211 / TRS-80 PC-1).  
Wi-Fi printer support using mDNS browser, HP LaserJet PCL modes only

07-04-2026 - PCUI_V1.01_B1658.uf2

This release addresses protocol bugs for the Casio PB-100 series devices and the Casio PB-700 series devices.  The printer and cassette interface was rewritten based on actual wire captures.  For the PB-700 series, ASCII mode program transfers are now reliable.

