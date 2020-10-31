# Jupiter_Ace_Expansion_Bus
Provides a selection of Adapter boards for Jupiter Ace Bus Expansion

Created in KiCAD with Gerber files included.

There are 3 discrete boards in this repository:

* Ace to 50-Way - Adapts the Jupiter Ace external expansion bus to a 50-Way IDC header. 

* 50-Way to Ace - Adapts the 50-Way IDC header back an Ace-Bus format for legacy expansion peripherals

* Buffered 50-Way - Buffers address, data, clock and selected control lines with external input on Pin 50 'BufDir'. The BufDir signal is intended to be driven low by any given external device select signal. Each input signal can be connected via a schottky diode e.g. BAT85 to the BufDir input. Decoding of the select signals is expected to be 'one-hot' and handled by the expansion peripheral(s). This will allow the buffered interface board to correctly set the direction of the read data signals.

Note the conventional 50-way header pinout is 'reversed' on this design such that pin 1 corresponds to the leftmost pins on the IDC header, this was a concious choice in order to create more of the 1:1 connection with the Ace Bus. 
