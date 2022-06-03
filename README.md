# CAN BUS Red Yellow Green Stoplight (can_ryg)
Summer project with CAN connected devices that simulate a stoplight. Three devices will take turns displaying red, yellow, and green. The status will be updated via a Wi-Fi GUI.

## Updates:

+ Future
+ 5/31/2022 - Received SPI -> CAN boards. They use a MCP2515 chip that I will interface with using SPI.
  + My next goal is to use the Analog Discovery 2 (AD2) [(Amazon Purchase)](https://digilent.com/shop/analog-discovery-2-100ms-s-usb-oscilloscope-logic-analyzer-and-variable-power-supply/?gclid=CjwKCAjwv-GUBhAzEiwASUMm4m5055qDvtA0vQVgSKHWfF5posYgGCk8NiQnRaYt99fyTiaV42Nt7xoCv-8QAvD_BwE) protocol analyzer to check the operation of the devices. Reviews show that some have received bad units.
  + I will first take a Seeeduino v4.2 [(Digikey Purchase)](https://www.digikey.com/en/products/detail/seeed-technology-co-ltd/102010026/5774914?s=N4IgTCBcDaIIwAYwMUgbCAugXyA) that I have on hand and setup SPI on it. I will check this connection with the AD2.
  + I will then determine how to operate the MCP2515 using SPI and attempt to generate messages on the CAN bus, which I will also monitor with the AD2 protocol analyzer.
  + I will do this with all three MCP2515 boards to ensure they work.
+ 5/28/2022 - Still planning project. Identifying goals and possible paths towards those goals.
  + Ordered three SPI -> CAN development boards [(Amazon Purchase)](https://www.amazon.com/gp/product/B07J9KZ4L4/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1). Plan is to use RPI 4B, ESP32-WROOM32D, and an MSP432.
  + Installed Raspberry Pi OS (64 bit) on RPI 4B in preparation. Unsure of how SPI will be accessed.
  + Will likely use Arduino IDE for ESP32. SPI library exist.
  + Unsure of IDE for MSP432. Will decide later. Look into CCS / uVision. Look into CMSIS-DAP and libraries.
+ 5/26/2022 - Decided to begin project.
