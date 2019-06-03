# MCUDev DevEBox STM32F407VET6

MicroPython board definition files for the MCUDev black STM32F407VET6 mini dev board.

**Markings:** DevEBox STM32F4XX_M Ver:V2.0 SN:1810

![board](docs/STM32F407VET6.jpg)

You can buy one for around $10 USD on [Taobao](https://item.taobao.com/item.htm?id=582677940441)

### Build and deploy the firmware:

* Clone the board definitions to your [MicroPython](https://github.com/micropython/micropython) `ports/stm32/boards` folder.

```
cd micropython/ports/stm32/boards
git clone https://github.com/mcauser/MCUDEV_DEVEBOX_F407VET6.git
```

* Disconnect the board from USB
* Set BOOT0 to ON by connecting pin BT0 to 3V3
* Connect the board via USB

```
cd micropython/ports/stm32
make BOARD=MCUDEV_DEVEBOX_F407VET6
make BOARD=MCUDEV_DEVEBOX_F407VET6 deploy
```

* Disconnect the board from USB
* Set BOOT0 to OFF by connecting pin BT0 to GND
* Connect the board via USB

```
screen /dev/tty.usbmodem1422
```

### Exposed Port Pins

* PA0-PA12, PA15
* PB0-PB1, PB3, PB5-PB15
* PC0-PC13
* PD0-PD15
* PE0-PE15

### Specifications:

* STM32F407VET6 ARM Cortex M4
* 168MHz, 210 DMIPS / 1.25 DMIPS / MHz
* 1.8V - 3.6V operating voltage
* 8MHz system crystal
* 32.768KHz RTC crystal
* 2.54mm pitch pins
* SWD header
* 512KByte Flash, 192 + 4 KByte SRAM
* 3x SPI, 3x USART, 2x UART, 2x I2S, 3x I2C
* 1x FSMC, 1x SDIO, 2x CAN
* 1x USB 2.0 FS / HS controller (with dedicated DMA)
* 1x USB HS ULPI (for external USB HS PHY)
* Micro SD
* Winbond W25Q16 16Mbit SPI Flash
* 1x 10/100 Ethernet MAC
* 1x 8 to 12-bit Parallel Camera interface
* 3x ADC (12-bit / 16-channel)
* 2x DAC (12-bit)
* 12x general timers, 2x advanced timers
* AMS1117-3.3V: 3.3V LDO voltage regulator, max current 800mA
* Micro USB for power and comms
* Power LED D1
* User LED D2 (PA6) active low
* Reset button, 1x user buttons K0
* 2x22 side pins
* TFT/OLED socket
* M3 mounting holes
* Dimensions: 40.89mm x 68.59mm

### Links:

* [STM32F407VG on st.com](https://www.st.com/content/st_com/en/products/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus/stm32-high-performance-mcus/stm32f4-series/stm32f407-417/stm32f407ve.html)
* [Buy on Taobao](https://item.taobao.com/item.htm?id=582677940441)
* [Buy on AliExpress](https://www.aliexpress.com/item/32985219862.html)

## License

Licensed under the [MIT License](http://opensource.org/licenses/MIT).
