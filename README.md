# RGB PIXEL LAMP
A simple code for control a rgb led pixel ring.

**Main functions**
- [x] RGB SYNC EFFECT
- [x] Basic function
- [ ] Light dependent system
- [ ] Bluetooth control
- [ ] Temperature / humidity reading
```sh
#include <Adafruit_NeoPixel.h>
```

```sh
Adafruit_NeoPixel pixels = Adafruit_NeoPixel(LED, OUTPIN, NEO_GRB + NEO_KHZ800);
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
![alt text]()
