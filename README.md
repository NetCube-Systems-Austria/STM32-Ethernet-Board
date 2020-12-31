# STM32-Ethernet-Board
This product is an STM32F103C8T6 based, arduino compatible, microcontroller development board. It also integrates an ENC28J60 ethernet interface. Since the board uses the STM32F103, it is compatible with the Arduino IDE and most sketches written for boards like the BluePill.

Due to the layout of the board resembling a DIP-34 package, it can be experimented with in a breadboard, soldered into you own board, or just get plugged into a DIP socket.

Even though the board doesn't have many I/O pins, the most common interfaces, like USB,I2C,UART,SPI and CAN, are broken out. If you need more I/O pins, you can easily connect any port expander, like the PCF8574 to the board's I2C bus. The board itself requires a 3.3V power supply, but all broken out I/Os are 5V tolerant.

As the board uses the ENC28J60 as the ethernet controller, it can simply be used with the existing EtherCardSTM or the [UIPEthernet](https://github.com/UIPEthernet/UIPEthernet) library. When using the UIPEthernet library, even many existing ethernet sketches can be used on this board.

Since the ethernet controller uses the primary SPI bus and its built in slave select line, it does not require any special configuration of the library.

Future versions of the board will also include a partially-read-only ([24AA02E48T-I/OT](http://ww1.microchip.com/downloads/en/devicedoc/20002124g.pdf)) eeprom containing a world-wide unique mac address for the board.

## Getting your own
You can either just order the PCB and assemble it yourself,
or you can support me and buy it on ([Tindie](https://www.tindie.com/products/netcubesystemsat/stm32-ethernet-board/))
