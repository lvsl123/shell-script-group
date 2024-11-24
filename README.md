What the files above do

adjustall: 
- adjust the screen brightness and also other color problems
- requires xcalib and xrandr.
- may not work on wayland but works on xfce 4.18

isinvert: 
- holds either true or false as reference of the screen inversion
- both adjustall and invert will read this file
- only the shell script invert will change this file

invert: 
- invert/uninvert the screen and save the change to isinvert
