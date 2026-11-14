# PCUI (Pocket Computer Universal Interface)
This is the official repo for firmware updates for the PCUI, owners manuals, and general information.  Further, this repo contains a collection of programs for various pocket computers and calculators supported by the PCUI.

<img alt="Image2" src="https://n1ugk.com/wp-content/uploads/2025/12/PCUI.png" />

## Development History

https://n1ugk.com/2025/12/pocket-computer-universal-interface/

## Features Summary

+ Provides cassette interface emulation to read and write programs and data directly to and from a micro SD card.
+ Provides a printer interface between the pocket computer or calculator and most standard “line printers” such as dot matrix, thermal receipt printers, serial, parallel, and Wi-Fi.
+ Supports printing of custom glyphs, including math, scientific and engineering symbols unique to each model.
+ Works independently without a computer and can be powered by a single 18650 lithium ion rechargeable battery.
+ OLED screen with user-friendly menu system and operating modes
+ Interface packs provide connectivity to each supported model, no need for OEM connection cables.
+ Updatable firmware and PC or Mac connectivity via USB for mounting micro SD card
+ Plotter emulation mode to provide printouts of plots using modern printers allowing programs which leveraged plotter features to be used on modern printers.
+ ASCII BASIC conversion to tokenized BASIC “on the fly”, allowing for program edits and program creation on a Mac or PC and directly sending it to a pocket computer.
+ Wi-Fi connectivity and web interface for program viewing, editing, UI control, printing, and status.
+ Online program library browsing and installing directly from GitHub allows you to view community released programs for various models of pocket computers directly from the PCUI.
+ True low-level cassette interface integration - byte level retrieval and storage of programs and data images, not just a simple "record" and "playback" mechanism.

## Supported Models

The following models are currently supported with more models in progress:

+ Texas Instruments	Graph Link Graphing Calculators
  + TI-82*, TI-85*, TI-86*, TI-89*, TI-92*, TI-92 Plus*, Voyage 200*
+ Sharp 9-pin “CE-121” / “CE-122” Compatibles
  + PC-1210, PC-1211, PC-1212, TRS-80 PC-1*
+ Sharp	Older 11-pin “CE-126P” Compatibles
  + PC-1245, PC-1246, PC-1246S, PC-1247, PC-1248, Tandy PC-8*
  + PC-1250, PC-1250A, PC-1251, PC-1251H, PC-1255, Tandy PC-3* and PC-3 A/B*, PC-1270
+ 11-pin “CE-126P” Compatibles
  + PC-1260, PC-1280
+ Sharp	Newer 11-pin “CE-126P” Compatibles
  + PC-1401, PC-1403*, PC-1421, PC-1430, PC-1450, EL-5500, EL-5500 II, EL-5500III*
+ Casio	12-pin PB-100 Series FP-12(S) Compatibles
  + PB-100, PB-110, PB-120, PB-200, PB-400, PB-410*, FX-700P, FX-710P, Tandy PC-4 Version B*, TRS-80 PC-4 Version A*
+ Casio	12-pin FX “Clamshell” Series
  + FX-770P, FX-780P, FX-781P, FX-785P, FX-790P, FX-791P, FX-795P, Tandy PC-5*, Tandy PC-6*
+ Casio	15-pin “FA-10” Compatibles
  + PB-700*, PB-770*
+ Casio	FX-702P*, FX-602P*

_*Tested and Verified, others should work since they use the same interface_

The PCUI Owners manual can be found in the [Documentation](./Documentation/) folder.

Firmware updates can be found in the [Firmware](./Firmware/) folder.

## 3D Printed Case

The PCUI has a case which can printed with a 3D printer.  The case STEP files are in the hardware folder.  The case includes all 3D models needed - both the top and bottom halves of the case, the 4 buttons, the two pocket computer connector covers, and the slide switch.

In addition to the PCUI case, there will be several "docking station" style model files as well.  For example, there is a TRS-80 PC-4 / Casio PB-100 series dock available for printing.  The interface pack fits inside of the 3D printed dock, providing a stable platform for connecting the pocket computer to the PCUI.  Similar models will be created for other pocket computers and made available as well.

<img width="1032" height="688" alt="image" src="https://github.com/user-attachments/assets/22707e4c-9303-4f2e-b1bb-99b9168f99e6" />

## Purchasing a Kit or Fully Assembled PCUI

A PCUI can be purchased as a kit or fully assembled.  

+ PCUI Kit - includes pre-flashed Pico 2 W, Main PCB and all components.  Interface pack kits are add-ons.  
  + Assembly instructions are located in the [Documentation](./Documentation/) folder.
  + The BOM, 3D model, KiCad Projects are located in the [Hardware](./Hardware/) folder.
+ PCUI Fully Assembled - includes a fully assembled PCUI and chosen interface pack add-ons.
+ To purchase a PCUI, <a href="https://www.tindie.com/products/n1ugk/pocket-computer-universal-interface-pcui/">click here</a>.
