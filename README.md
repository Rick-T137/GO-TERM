# GO-TERM

![GO!Term](https://github.com/Rick-T137/GO-TERM/assets/13721643/b899c87a-06a8-4fb4-8694-90f3c9109f9e)

## Simple terminal program for the Commodore VIC-20

This terminal program runs on an unexpanded VIC-20. You'll need a WiFi modem or some other communication 
device in order to use this. To run it:  

`LOAD "GO!TERM",8`

That will give you a program with just one line:

`0 SYS4109`

Now `RUN` the program and you'll be greeted by the terminal screen pictured above. Use the function keys 
to perform the following tasks:  

` F1 ` - Change Baud Rate (cycles between 300, 1200 and 2400)  
` F3 ` - Turn on "Light Mode" (white screen, blue characters, cyan border)  
` F5 ` - Turn on "Dark Mode" (black screen, cyan characters, black border)  
` F7 ` - Exit and return to BASIC  

The program is written entirely in machine language (except for the one line BASIC stub listed above). It uses
the built-in VIC-20 flashing cursor, so in theory there should be no "dangling lines" as often occurs if you 
use a hard character for your cursor.  

To "dial out", you can use standard Hayes AT commands. For example, to call the Live Wire BBS, you would type:  

`atdt vic-bbs.com:6502`

and then press `RETURN`. You can do this to call any Internet-connected BBS, but do note that GO!Term does no
character translation. It is most suitable for calling Commodore boards that support PETSCII mode.
