Binary Clock Desktop Gagdet for Windows 7

This binary clock gadget is just a little sample application i wrote to 
investigate the possibilities Windows 7 offers for gagdet authors. When I 
finished the gagdet I liked it enough to keep it on my desktop.

HOW TO INSTALL:
Just double click on the file. It will be added to your list of installed 
gadgets. You then can add it to your desktoo by right clicking of your desktop.
Choose "Gadget" and then drag & drop the "Binary Clock" onto your desktop.

HOW TO USE:
The clock is composed of a 6x4 grid of black dots. Each column of the grid 
represents one decimal digit of the time format "HHMMSS". So the first two 
columns display the hours, the next two columns display the minutes, the 
remaining two columns display the seconds.

      HH|MM|SS|
      --+--+--+----
        |  |  | x 8
  +    o|o | o| x 4
  +     | o|  | x 2
  +   oo| o|o | x 1
      --+--+--+----
  =   15|43|14|      => It's 15:43:14

The value of each column is displayed as a list of 4 binary digits. A black dot
represents a binary 1, a missing black dot represents a binary 0. Multiply the
binary value of the top row with 8, of the second row with 4, the third row with
2 and the fourth row with 1 and add these values. Concatenate these numbers and
you'll have to current time.


CONTENTS:
The gagdet is made of 3 components:

- The gadget.xml file identifies the gadget as a Windows 7 desktop gadget and 
  stores some additional meta information about the script.
- BinaryClock.html is the user interface of the gadget and gets displayed 
  automatically. It also contains the JScript code that animates the clock.
- The images folder contains two images: blank.png is a transparent 
  placeholder, dot.png is used to render a binary 1.
  
