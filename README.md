# ESP32-C3-MAX7219-Scrolling-Text

I've found a lot of esp32 scrolling display firmware using md_parola lib. none was working on my no brand supermini esp32-c3!
at least i've made it by myself using modding this one https://github.com/astatio/MAX7219-ESP32-C3-Marquee. it was working but it was not possible
to change the scrolling text via wifi.
My version create an access point called "PUPAZZINO access point". To change the scrolling text is now very easy.

1) Flash scroll3.bin using espwebtools or what do you like to use (push the flash switch connecting usb if required) and reset
2) connect to the access point (if your phone warns you about no internet connection and no key, go ahead)
3) type http://192.168.4.1 on your browser.
4) put new text on the box and click "update display".

connections:

7219 DIN_PIN -----> ESP GPIO5;

7219 CLK_PIN -----> ESP GPIO6;

7219 CS_PIN ------> ESP GPIO7;

7219 GND ---------> ESP GND;

7219 VCC----------> ESP 5V.

Have Fun. PUPAZZINO. Please follow me (pupazzino1) on Instagram.   
