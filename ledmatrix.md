# Led Matrix

## `print`

How to display a scrolling text message on the LED matrix.

### Example 1

This example shows how to display a scrolling text message on the LED dot matrix.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {

}

void loop() {
  board.ledmatrix.print("H o l a  m u n d o!");
}
```

### Example 2

The `setScrollSpeed` method allows you to control the scroll speed that is used to display the text on the LED dot matrix.

```c++
#include <NanoPlayBoard.h>

NanoPlayBoard board;

void setup() {
  board.ledmatrix.setScrollSpeed(10);
}

void loop() {
  board.ledmatrix.print("H o l a  m u n d o!");
}
```
