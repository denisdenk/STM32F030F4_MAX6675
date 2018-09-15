STM32f030F4P6 + MAX6675
===================

This example includes the code to connect the **MAX6675** converter chip to the **STM32F030F4P6** microcontroller. The temperature data is output via the UART interface at 115200 baud.

The code for the microcontroller is written in C using the HAL library from ST. 

The chip is connected as follows:

| MAX6675 PIN  | STM32 PIN 
| :----------- | ----: | 
| VCC          | 3V3   |    
| GND          | GND   |  
| SO           | PA6   |  
| SCK		       | PA5   |
| CS           | PA4   |


I used a Chinese board with this microcontroller, and on this board, the UART interface is connected as follows:

| STM32F030 PIN | UART PIN 
| :-----------  | ----: | 
| PA10          | RX    |    
| PA9           | TX    | 

When connecting the microcontroller to the USB-UART (like cp2102 ch340 ft232 etc.) adapter, you should connect the RX of the microcontroller to the TX of the adapter board.
![Иллюстрация к проекту](http://www.haoyuelectronics.com/Attachment/STM32F030-Dev-Board/STM32F030-Dev-Board-4.jpg)
![Иллюстрация к проекту](https://img.dxcdn.com/productimages/sku_434632_1.jpg)
