These programs are from the FA-10 Owners Manual.  I used these to test the plotter emulation for the PCUI to ensure each sample plotter function was properly simulated in the PCUI internal canvas.

The only change to these programs was I added LPRINT CHR$(28);CHR$(46) at the end of the programs in order to signal to the PCUI to end plotter mode and print the internal canvas to the attached printer.

These should be loaded into the PB-700/PB-770 in ASCII mode:

Example:

LOAD "PLOTTST6",A


PLOTTST1.txt - DRAW
PLOTTST2.txt - Circles
PLOTTST3.txt - Relative Draw / Move
PLOTTST4.txt - Relative Move /Quadrangle
PLOTTST5.txt - Circles / Axis
PLOTTST6.txt - Grid / Line Type
PLOTTST7.txt - Line Scale
PLOTTST8.txt - Alpha Scale
PLOTTST9.txt - Alpha Rotate
PLOTTSTA.txt - Space
PLOTTSTB.txt - Programming Example No. 1
PLOTTSTC.txt - Programming Example No. 2
PLOTTSTD.txt - Trig Function Table
PLOTTSTE.txt - Pie Chart
PLOTTSTF.txt - Home 
PLOTTSTG.txt - Floor Plan
