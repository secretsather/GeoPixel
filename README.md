# GeoPixel

Arduino Library for use with ESP32 &amp; WS2812 LEDs that encodes RGB to SPI w/ DMA for Communication

## Acknowledgment

Special thanks to [Hideakitai](https://github.com/hideakitai) for creating [ESP32DMASPI](https://github.com/hideakitai/ESP32DMASPI) for which this would not be possible. The original source file [ESP32DMASPIMaster.h](https://github.com/hideakitai/ESP32DMASPI/blob/main/ESP32DMASPIMaster.h) has been included here for completeness, and is licensed under the MIT License, which is found in ./third_party_code

## Brief

(to be populated at a later date) This is a no-frills, bare bones implementation to use SPI for communication with WS2812 LED strips or panels. 

## Prerequisites

The things you need before installing

* Arduino IDE (created on 2.3.2)
* Tested on ESP32S2 "S2 Mini;" however, this appears to be compatible with all ESP32 variants S2, S3, C3. 
* WS2812 Panel or Strip

## Installation

```
$ In Arduino IDE, Select 'Sketch >> Include Library >> Add .ZIP Library...'
$ Select .ZIP from this repository
$ Include usage code within sketch
```

## Usage

```C++
#include <GeoPixel.h>

GeoPixel<64, 16> panel;  // <X,Y>

void setup(){
}

void loop(){
}
```

## Additional Thoughts

* Your pinout may differ. You should check the pin definitions of your board and determine the MISO pin for the SPI that is enabled.
