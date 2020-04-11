# MFOS-SVF
Eurorack adaptation of the MFOS "Oldie But Goody" state variable filter

This is a Eurorack version of a state variable voltage controlled filter by Ray Wilson of musicfromouterspace.com. At that site there is a state variable VCF listed under "Analog Synthesizer Modules" but this project is based on another, earlier design listed under "Oldies But Goodies" at http://musicfromouterspace.com/index.php?MAINTAB=SYNTHDIY&PROJARG=OLDIESBUTGOODIES/VCF/vcfstatevar.html&VPW=2087&VPH=905.

Wilson's design was for a module in his own preferred format, with ±12V and ground soldered to the board and panel hardware mounted to the panel and wired to the board. This version has a Eurorack power connector and has panel hardware mounted to a panel PCB coupled to a main PCB with most of the circuitry.

Included in this repository are KiCad-format schematics and PCB designs for the two circuit boards, as well as an Inkscape .svg file for the panel design and a KiCad-format "PCB" for fabrication of the panel by a PCB company.

The schematics are closely based upon Wilson's original and are governed by licensing information at http://musicfromouterspace.com. The PCB layouts and panel design are new, by Richard Holmes.

BOMs are here:
https://github.com/holmesrichards/MFOS-SVF/blob/master/OBG-SVF-mainPCB/OBG-SVF-mainpcb.html
and here:
https://github.com/holmesrichards/MFOS-SVF/blob/master/OBG-SVF-panelPCB/OBG-SVF-panelpcb.html

## Build notes

Pretty standard. Panel PCB and main PCB joined with 2x6 pin header/socket. Use two 10 mm M3 spacers and four M3 screws to hold them together.

This time most of the components go on the panel-facing side. The power header and trimmer go on the other side. I intended the electrolytics to go on the panel-facing side but mine were too tall to fit between the boards so I mounted them on the other side.

The trimmer adjusts V/Oct response. Adjust it so a change of 1 octave (1V) on the CV input results in a change of 18 mV at the base of Q1.

![module pic](https://github.com/holmesrichards/MFOS-SVF/blob/master/Images/IMG_20200320_130106.jpg?raw=true)
