These programs are from the FA-10 plotter Owners Manual.  I used these to test the plotter emulation for the PCUI to ensure each sample plotter function was properly simulated in the PCUI internal canvas.

These programs were modified for the PC-1245 as follows.  The PC-1245 cannot output the escape codes necessary to enable graphics mode, those bytes come off the bus as spaces (they are outside the FP-12S printable character range).  The PCUI has a "hex translation" feature, which allows any byte to be pushed to the printer port on the PCUI using an escape sequence then the hexadecimal digit(s) to output.  For example "?X010203" would output 0x01 0x02 0x03.

This translation feature allows pocket computers such as the PC-1245 (and similar models) to use the plotter emulation feature in the PCUI and/or real plotters connected to the PCUI.


PLOTSTC.txt - Circles (Programming Example No. 2)
