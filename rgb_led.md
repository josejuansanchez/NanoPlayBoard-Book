# RGB Led

## `on & off`

How to switch on and off the RGB LED.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.on();
  delay(1000);
  board.rgb.off();
  delay(1000);
}
```

## `setColor`

How to set the LED color using a HEX value.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.setColor("#FF0000");
  delay(1000);
  board.rgb.setColor("#00FF00");
  delay(1000);
  board.rgb.setColor("#0000FF");
  delay(1000);
}
```

## `setColor`

How to set the LED color using a RGB value.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.setColor(255, 0, 0);  
  delay(500);
  board.rgb.setColor(0, 255, 0);
  delay(500);
  board.rgb.setColor(0, 0, 255);  
  delay(500);
}
```

## `setIntensity`

How to set the brightness of the LED.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  board.rgb.setColor("FF0000");
}

void loop() {
  int intensity = board.potentiometer.scaleTo(0, 99);
  board.rgb.setIntensity(intensity);
  board.ledmatrix.printInLandscape(intensity);
}
```

## `toggle`

How to toggle the current state of the LED.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.rgb.toggle();
  delay(1000);
}
```

