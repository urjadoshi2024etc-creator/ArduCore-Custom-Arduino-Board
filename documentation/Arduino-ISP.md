# Programming ArduCore with Arduino ISP

ArduCore uses a DIP ATmega328P and does not have a dedicated USB programmer.

Another Arduino can be used as an ISP programmer to program the ATmega328P.

## Programming Process

1. Upload the `ArduinoISP` example to another Arduino.
2. Connect the Arduino ISP to the ArduCore programming pins.
3. Connect VCC and GND.
4. Connect the SPI signals.
5. Connect RESET from the programmer to the ATmega328P.
6. Burn the bootloader if required.
7. Upload the desired firmware.

## ISP Connections

| Signal | Function |
|---|---|
| VCC | Power |
| GND | Ground |
| MOSI | SPI data |
| MISO | SPI data |
| SCK | SPI clock |
| RESET | ATmega328P reset |

## Status

Programming will be tested after the PCB is fabricated and assembled.
