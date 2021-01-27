## Adafruit SPI Flash SD Card PCB

<a href="http://www.adafruit.com/products/4899"><img src="assets/4899.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit SPI Flash SD Card.

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4899

### Description

This breakout is for a fascinating chip - it looks like an SPI Flash storage chip (like the GD25Q16) but its really an SD card, in an SMT chip format. What that means is that you wire up like an SD card breakout, and use the SD card libraries you already have for your microcontroller. For example, you can use the built in SD library in Arduino, or for CircuitPython we have an sdcard library. The breakout will act just like a 512 MB sized card with FAT formatting (it's pre-formatted).

You might be wondering why you'd want such a thing - after all you can't plug it into a computer to get the files off like MicroSD cards. For some use cases, such as data logging in a high-vibration device where you don't want the SD card to come loose, or for when you need to reduce size, or when the microcontroller provides a USB mass storage interface, this chip could very useful.

Compared to plain SPI flash, this NAND memory chip handles all the wear leveling and ECC calculation. You don't have to manually erase blocks, you just write and read them like you would with any SD card.You can clock it up 50 MHz and the 'write speed class' is 8 (although you may not be able to get that fast with plain 1-bit SPI compared to SDIO).

We made this breakout to be a quickstart for this chip. We wired the chip in "SPI" mode, with a level shifters so you can use it with 3V or 5V logic easily. You also get a 3.3V regulator and a pullup on CS. Wire up the SPI pins to your microcontroller, use your favorite SD library and you'll be ready to rock in minutes!

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution.
See license.txt for additional details.
