# altair-8800-again
The Altair 8800 Again! Project Repository

Link to the EasyEDA project files:  
https://easyeda.com/dherrendoerfer/altair8800again  
https://easyeda.com/dherrendoerfer/altair8800again-panel (Front panel switch sample)  

Link to the Teensy firmware fork of the Altair8800 repo:  
https://github.com/dherrendoerfer/Altair8800

Further required libraries to use the Teensy code:  
https://github.com/dherrendoerfer/uVGA  
https://github.com/PaulStoffregen/WS2812Serial  

### some hints:
The Teensy microcontroler does not have as many IO pins as the Arduino Due does, so we need to work around that.  
The front panel switches are read as a 8x4 matrix requiring 12 data pins, and the LEDs are handled using WS2812 addressable modules.
This (kind-of) messes with the real-time nature of the LED display, but I tried to work around that a bit.  
The Teensy provides a VGA out and PS/2 keyboard in for limited terminal support directly.  
There are provisions for audio in and out to read and write audio data at 300bps.  
One serial link is provided for RS/232 connections to a terminal.

### Configuration:  
All serial ports, as well as the VGA and audio interface can be configured directly through the Altair config interface via the master terminal.  
The default configuration has the master terminal on the Teensy USB port.  
The available PCBs have a power plug. Polarity and voltage is 5V center pin positive.  

Enjoy !


Donations:  
If you would like to make a donation to keep this project and others going you can do so at:  
https://www.paypal.me/dherrendoerfer  
This helps a lot !
