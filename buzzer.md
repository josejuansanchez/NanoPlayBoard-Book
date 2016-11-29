# Buzzer

## `playTone`

How to play tones on the buzzer.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  int value = board.potentiometer.read();
  board.buzzer.playTone(value);
  delay(100); 
}
```

