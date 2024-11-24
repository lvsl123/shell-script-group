Bash scripts to brighten the day in linux

What the files above do

adjustall: 
- How to use - ./adjustall <value from 0.24 to 1.1>
- adjust the screen brightness and also other color problems
- requires xcalib and xrandr. Having bc (calculator in command line) is highly recommended. If you don't want to have autocheck for brightness value errors then you can hardcode the variable brightnessValue or remove all the checks. Do it in your own risk, as setting the wrong brightness especially via command line can make you unable to view the contents of the screen
- may not work on wayland but works on xfce 4.18

isinvert: 
- holds either true or false as reference of the screen inversion
- both adjustall and invert will read this file
- only the shell script invert will change this file

invert: 
- invert/uninvert the screen and save the change to isinvert

bashrc:
- straight from ubuntu with change in ls and command prompt (user@archlinux) colors
- put it in your home directory and change filename to .bashrc to use the script. It might occur that you already have the same file in your home directory. Backup that file up first before using this bashrc. For more info please refer to your linux distribution.

Ways to use the files:
- adjustall: put the file along with a list of scripts that will run once you login the gui so it will do all the adjustment autonatically
- the command is /home/js/adjustall 1
- <img src='https://raw.githubusercontent.com/lvsl123/shell-script-group/refs/heads/main/adjustall.png'></img>
