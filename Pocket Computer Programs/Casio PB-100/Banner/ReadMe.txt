Due to low memory on the "A" version of the Tandy PC-4 / PB-100, the bitmap data for the
banner program is stored as variables in BANMEM.BIN.  Load this before running the banner program:

DEFM 27
GET "BANMEM" $,A,A(52)