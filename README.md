# pico-lora
LoRa communication library for Raspberry Pi RP2040 Microcontroller. 

This library is written for RP2040 C++ SDK.

## Supported Hardware
 * RP2040 boards
    * Raspberry Pi Pico
 * Semtech SX1276/77/78/79 based LoRa boards

### Default Pinout

| Raspberry Pi Pico | RP2040-Zero | Semtech SX1278 |
| ----------------- | -------------- | -------------- |
| 3.3V | 3.3V | VCC |
| GND | GND | GND |
| GPIO 18 | GPIO 2 | SCK |
| GPIO 19 | GPIO 3 | MOSI |
| GPIO 16 | GPIO 4 | MISO |
| GPIO 7 | GPIO 7 | DIO0 / G0 |
| GPIO 8 | GPIO 8 | NSS / CS |
| GPIO 9 | GPIO 6 | RESET |
| GPIO 10 | GPIO 5 | DIO1 / G1 |

Default Pinout can be overridden with setPins() function

## Installation

1. [Set up the Pico C/C++ SDK](https://github.com/raspberrypi/pico-sdk)
2. Download module from git and open directory
```sh
git clone https://github.com/crystalxdesign/pico-lora.git
cd ./pico-lora
```
3. Set `PICO_SDK_PATH`
```sh
export PICO_SDK_PATH="path to pico-sdk"
```
4. Create `build` directory then run `cmake` and `make`:
```sh
mkdir build
cd build
cmake ..
make
```
## Notes
Currently this is only tested on Raspberry Pi Pico and Semtech1278 board. Feel free to reach out for any bugs or support.

## References
This [project](https://github.com/akshayabali/LoRa-RP2040) is based on LoRa Library for Arduino:[sandeepmistry/arduino-LoRa](https://github.com/sandeepmistry/arduino-LoRa)
