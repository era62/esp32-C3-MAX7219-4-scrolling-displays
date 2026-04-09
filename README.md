# ESP32-C3-MAX7219-Scrolling-Text

I've found a lot of esp32 scrolling display firmware using md_parola lib. none was working on my no brand supermini esp32-c3!
at least i've made it by myself using modding this one https://github.com/astatio/MAX7219-ESP32-C3-Marquee. it was working but it was not possible
to change the scrolling text via wifi.
My version create an access point called "PUPAZZINO access point". To change the scrolling text is now very easy.

You need:
ESP32-c3 board
MAX 7219 4 digit 8x8 display
Solder and/or jumper wires.
Usb power supply.
If you want to 3dprint a case you can look here https://www.printables.com/model/959767-max7219-led-matrix-box/files

1) Flash scroll3.bin using espwebtools or what do you like to use (push the flash switch connecting usb if required) and reset
2) Connect to the access point (if your phone warns you about no internet connection and no key, go ahead)
3) Type http://192.168.4.1 on your browser.
4) Put new text on the box and click "update display".

connections:

7219 DIN_PIN -----> ESP GPIO5;

7219 CLK_PIN -----> ESP GPIO6;

7219 CS_PIN ------> ESP GPIO7;

7219 GND ---------> ESP GND;

7219 VCC----------> ESP 5V.

Have Fun. PUPAZZINO. Please follow me (pupazzino1) on Instagram.   
