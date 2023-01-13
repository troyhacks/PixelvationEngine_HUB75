Software to drive HUB75 Panels over a APA102 Dataline. using the [Pixelvation board](https://github.com/Pixelvation/Pixelvation)
It uses the [SmartMatrix Library 4.0](https://github.com/pixelmatix/SmartMatrix) and the Arduino Core.

---
Configuration
---
Uncomment one of the lines between Line 7 and Line 12.

`MatrixHardware_ESP32_HUB75AdapterLite_V0` lines have the Hardware definitions for the Pixelvation PCB.
The `I2sIn1Bit`, `I2sIn2Bit`, `I2sIn4Bit` and `I2sIn8Bit` differences are how many APA102 inputs you want to have.


Then define your Matrix by entering the correct Values for `kMatrixWidth` and `kMatrixHeight`. 

The last line to configure, is the line that starts with `kPanelType`. There are a bunch of different paneltypes. Take a look in the file [MatrixComminHub75.h](https://github.com/pixelmatix/SmartMatrix/blob/master/src/MatrixCommonHub75.h) of the library. 
Choose a fitting one for your panel.

---
Installation
---
