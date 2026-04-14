
<h1 align="center">
Quadcopter Flight Controller
</h1>

<h3 align="center">
A Small Flight Controller For a 5in FPV Quadcopter
</h3>

<p align="center">
  <a href="#key-features">Key Features</a> -
  <a href="#description">Description</a> -
  <a href="#components">Components</a> -
  <a href="#board-design">Board Design</a> -
  <a href="#credits">Credits</a> -
</p>

## Key Features
- **STM32F7 MCU**
- **Connectivity: Pin Connectors and Pads**
- **Video: Built In On Screen Display IC**
- **Voltage: 3 Voltage Regulators - 3.3V, 5V, 9V**
- **Storage: Blackbox SD Card**
- **2 Layer PCB: Very Compact Design**

## Description
A small, drone stackup compatible, flight controller built using the STM32F722RET6 MCU to handle components like 3 voltage regulators, IMU, Barometer, OSD, USB-C, and SD Card. The board is also a very compact design for 2 layers featuring everything that other boards do like connectors, pads, buzzers, indication LEDS, and BOOT/RESET buttons.

## Components
- STM32F722RET6 (MCU)
- ICM-45686 (IMU)
- BMP280 (Barometer)
- AT7456E (OSD)
- TPS63070RNMR (5V/9V Regulators)
- LMR51430 (3.3V Regulator)

## Board Design


## Credits
This was made using:
- [KiCAD](https://www.kicad.org/) - PCB Design
- [STM32Cube MX](https://www.st.com/en/development-tools/stm32cubemx.html) - STM32 Pinout / Clock Setup
- [JLCPCB](https://jlcpcb.com/) - PCB Manufacturing / Assembly
- [LCSC](https://www.lcsc.com/) - Component Sourcing
- [Blueprint Guide](https://stasis.hackclub.com/starter-projects/split-keyboard) - Flight Controller Guide

## My Other Projects
- [Split Keyboard](https://github.com/Ari-Hetti/Split-Keyboard) - A Small 32 Key Split Keyboard with Thumb Knobs that can be Powered Wired or Wirelessly.
- [Hexpad_Highway](https://github.com/Ari-Hetti/Hexpad_Highway) - A Small mMcropad with 6 Switches, 1 Rotary encoder and 1 Oled display Encased in a 3d Printed Enclosure
- [FRC Badge V2](https://github.com/Ari-Hetti/FRC-Badge-V2) - Hexagonal 555 timer LED Chaser Keychain
