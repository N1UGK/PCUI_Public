These programs are from the FA-10 Owners Manual.  I used these to test the plotter emulation for the PCUI to ensure each sample plotter function was properly simulated in the PCUI internal canvas.

These programs were modified for the PB-100 as follows.  The PB-100 cannot output the escape codes necessary to enable graphics mode, those bytes come off the bus as spaces (they're outside the FP-12S printable character range).  The PCUI has a "hex translation" feature, which allows any byte to be pushed to the printer port on the PCUI using an escape sequence then the hexadecimal digit(s) to output.  For example "?X010203" would output 0x01 0x02 0x03.


PLOTTSTC.txt - Programming Example No. 2
