# RGB PIXEL LAMP
###### Premise
**This project isn't completed** <\ br>
My idea is create a dynamic lamp, this lamp have a lot functions as electric save energy, remote control and more. 
###### Download library
*Adafruit_NeoPixel* I use this library for control of led pixel [DOWNLOAD](https://github.com/adafruit/Adafruit_NeoPixel).
## Main functions
- [x] RGB SYNC EFFECT
- [x] Basic function
- [ ] Light dependent system
- [ ] Bluetooth control
- [ ] Temperature / humidity reading

# LED PIXEL SYSTEM 
```sh
#include <Adafruit_NeoPixel.h>
```
```sh
int  LED=28;
byte OUTPIN=6;
```
```sh
Adafruit_NeoPixel pixels = Adafruit_NeoPixel(LED, OUTPIN, NEO_GRB + NEO_KHZ800);
```
```sh
void setup() {
  pixels.begin();
}
```
```sh
void loop() {
    for(int i=0;i<LED;i++){
    pixels.setPixelColor(i, pixels.Color(255,0,0));
    pixels.show(); 
    delay(50); 
   }
  for(int i=0;i<LED;i++){
    pixels.setPixelColor(i, pixels.Color(0,255,0));
    pixels.show(); 
    delay(100); 
   }
   for(int i=0;i<LED;i++){
    pixels.setPixelColor(i, pixels.Color(0,0,255));
    pixels.show(); 
    delay(50); 
   }
   for(int i=0;i<LED;i++){
   pixels.setPixelColor(i, pixels.Color(255,255,255));
    pixels.show(); 
    delay(10);
   }
   delay(5000);
}
```
