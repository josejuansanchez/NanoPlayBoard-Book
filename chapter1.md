# El potenciómetro

GitBook allows you to organize your book into chapters, each chapter is stored in a separate file like this one.

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