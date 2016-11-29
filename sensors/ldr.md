# LDR


## `read`

How to send LDR values through *serial port*.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  Serial.begin(9600);
}

void loop() {
  int value = board.ldr.read();
  Serial.println(value);
  delay(100);
}
```

## `read`

How to send LDR values through *Bluetooth*.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.ldr.read();
  board.bluetooth.println(value);
  delay(100);
}
```

## `scaleTo`

How to scale LDR values.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.ldr.scaleTo(0, 99);
  board.ledmatrix.printInLandscape(value);
}
```