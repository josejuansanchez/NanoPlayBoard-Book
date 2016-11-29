# Potentiometer

## `read`

How to send potentiometer values through *serial port*.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  Serial.begin(9600);
}

void loop() {
  int value = board.potentiometer.read();
  Serial.println(value);
  delay(100);
}
```

## `read`

How to send potentiometer values through *Bluetooth*.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.read();
  board.bluetooth.println(value);
  delay(100);
}
```

## `scaleTo`

How to scale potentiometer values.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.scaleTo(0, 99);
  board.ledmatrix.printInLandscape(value);
  delay(100);
}
```