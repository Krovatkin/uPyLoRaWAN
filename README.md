# Villedepommes' Notes


* Flush w/ the generic [esp32 rom](https://micropython.org/download/esp32/) like so `esptool.exe --chip esp32 --port COM4 --baud 460800 write_flash -z 0x1000 esp32-20210418-v1.15.bin`
* `pip install esptool`
* `pip install adafruit-ampy`
* copy the following files with `ampy put` 
    * boot.py
    * config.py
    * examples
    * sx127x.py
    * uPySensors
    * main.py
* `ampy run main.py` 
    * if this command doesn't work manually run the commands via REPL
    * there needs to be two versions of `main.py`. One for a receiver and another one for a transmitter
# uPyLora
ESP32 using MicroPython meets lora. 

This repo includes an sx127x micropython driver to communicate between two devices using LoRa. 

For the LoRaWAN repository click on [here](https://github.com/lemariva/uPyLoRaWAN/tree/LoRaWAN).

# Setup
Check out these articles for more information:
* [M5Stack Atom Matrix: LoRaWAN node running MicroPython](https://lemariva.com/blog/2020/03/m5stack-atom-lorawan-node-running-micropython)
* [Tutorial: ESP32 running MicroPython sends data over LoRaWAN](https://lemariva.com/blog/2020/02/tutorial-micropython-esp32-sends-data-over-lorawan)

# Hardware
* [Wemos® TTGO LORA32 868/915Mhz](https://www.banggood.com/2Pcs-Wemos-TTGO-LORA32-868915Mhz-ESP32-LoRa-OLED-0_96-Inch-Blue-Display-p-1239769.html?p=QW0903761303201409LG) board.

# Revision
* 0.1 first commit

# Licenses
* Apache 2.0

# References
* Basically based on: [Wei1234c GitHub](https://github.com/Wei1234c/SX127x_driver_for_MicroPython_on_ESP8266). The original project was cleaned and made compatible with the [Wemos® TTGO LORA32 868/915Mhz](https://www.banggood.com/2Pcs-Wemos-TTGO-LORA32-868915Mhz-ESP32-LoRa-OLED-0_96-Inch-Blue-Display-p-1239769.html?p=QW0903761303201409LG) board.
