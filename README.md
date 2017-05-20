Adafruit_DotStar
================

Updated to use [SPI_Master.h](https://github.com/redbear/nRF5x/blob/341f6adff63fafefc474e927af3af260d3977004/arduino/arduino-1.8.0/hardware/RBL/RBL_nRF52832/libraries/SPI_Master/SPI_Master.h) instead of ```SPI.h``` to compile for **NRF52** devices such as the [RedBear Nano v2](https://github.com/redbear/nRF5x/).

**Scope**
Checks if ```NRF52``` is defined, and then includes ```SPI_Master.h```.
Also adds ```#define SPI SPI_Master``` so that all other code can remain similar.

**Limitations**
Hopefully no new limitations introduced.

**Test**
Tested with [DotStarMatrix](https://github.com/adafruit/Adafruit_DotStarMatrix) library example: [matrixtest](https://github.com/adafruit/Adafruit_DotStarMatrix/blob/master/examples/matrixtest/matrixtest.pde)