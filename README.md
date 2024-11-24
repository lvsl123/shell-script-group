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

bashrc:
- straight from ubuntu with change in ls and command prompt (user@archlinux) colors

Ways to use the files:
- adjustall: put the file along with a list of scripts that will run once you login the gui so it will do all the adjustment autonatically
- the command is /home/js/adjustall 1
- <img src='https://raw.githubusercontent.com/lvsl123/shell-script-group/refs/heads/main/adjustall.png'></img>
