These programs are from the PB-700/PB-770 Owners Manual.  I used these to test the plotter emulation for the PCUI to ensure each sample plotter function was properly simulated in the PCUI internal canvas.

The only change to these programs was I added LPRINT CHR$(28);CHR$(37) at the beginning of the programs to signal to the PCUI that plotter mode was to be enabled, and at the end of the program LPRINT CHR$(28);CHR$(46) to signal to the PCUI to end plotter mode and print the internal canvas to the attached printer.

These should be loaded into the PB-700/PB-770 in ASCII mode:

Example:

LOAD "PLOTTST6",A