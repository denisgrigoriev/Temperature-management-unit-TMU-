# Temperature Management unit / Thermal management unit

A low-power, localized thermal regulation module designed to keep sensitive host electronics within operating temperature limits in sub-zero environments

## Overview:

Commercial and industrial-grade electronics often suffer unpredictable behavior, clock instability, or complete failure when exposed to ambient temperatures below -40°C.
The Temperature Management Unit (TMU) is a compact PCB module mounted directly onto critical host circuit boards. It monitors ambient conditions with high precision and automatically engages a localized surface heating element to ensure stable, reliable host system operation.

 ## Key Features
- High-Accuracy Thermal Sensing: Driven by the TI TMP117, providing readings over I2C
- Smooth Thermal Regulation: Uses PWM gate driving and soft-start thermal ramping to mitigate thermal shock and mechanical stress on PCB substrates.

 ## Schematic
 - 0.1uf capacitors are used to filter high frequency noise.
 - 10uf capacitors are used to filter low frequency noise from the batteries.
 - 10k ohm resisters are used as to pullup/pulldown.
 - 4.7k ohm resisters are used to pullup (for i2c; 4.7k ohms are a standard in i2c).
 - Mosfets act like a digitally controlled switch; turning it off and on many times is used to control the temperature.
 <img width="758" height="544" alt="image" src="https://github.com/user-attachments/assets/b2e2acae-1800-47fc-ac87-aa21ac3ab841" />


## Bill of Materials (BOM)

| Component | Cost | Source |
| :--- | :--- | :--- |
| [Adafruit TMP117 ±0.1°C High Accuracy I2C Temperature Sensor (STEMMA QT / Qwiic)](https://thepihut.com/products/adafruit-tmp117-0-1-c-high-accuracy-i2c-temperature-sensor) | £11.10 / $15.00 | The PiHut |
| [Atmel ATtiny85 20MHz](https://thepihut.com/products/atmel-attiny85-20mhz) | £2.50 / $3.38 | The PiHut |
| [2pcs AO3400A Logic Level (3.3v) MOSFET fits 2.54mm Perfboard, Breadboard, Vero](https://www.ebay.co.uk/itm/267687635215) | £1.69 / $2.28 | Ebay |
| [Resistor Packs (1/4 Watt, ±1%)(4.7k)](https://thepihut.com/products/resistor-packs) | £1 / $1.35 | The PiHut |
| [Resistor Packs (1/4 Watt, ±1%)(10k)](https://thepihut.com/products/resistor-packs) | £1 / $1.35 | The PiHut |
