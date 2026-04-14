
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
**Schematics:**
<img width="1182" height="817" alt="image" src="https://github.com/user-attachments/assets/320a62d6-e9f1-472d-b7bf-82375f5a095a" />
<img width="1386" height="620" alt="image" src="https://github.com/user-attachments/assets/e2466c5b-f291-462e-bab7-c7191d7d31dc" />
<img width="518" height="650" alt="image" src="https://github.com/user-attachments/assets/a31414fa-ef0c-4d4f-9df4-07c37512ca9a" />
<img width="1155" height="793" alt="image" src="https://github.com/user-attachments/assets/a7167f07-952a-4839-8e9d-0e253ab26932" />
<img width="1096" height="619" alt="image" src="https://github.com/user-attachments/assets/79a86c84-d475-453f-9bfa-e03fb5725655" />
**PCB:**

<img width="810" height="860" alt="image" src="https://github.com/user-attachments/assets/e7a552be-b079-4cb4-973d-7975f009bea3" />
<img width="818" height="857" alt="Screenshot 2026-04-14 111123" src="https://github.com/user-attachments/assets/8d0f8acb-d26c-44b0-bd58-c2259e88e94f" />
<img width="822" height="863" alt="Screenshot 2026-04-14 111138" src="https://github.com/user-attachments/assets/87f47743-db63-4dc4-8000-5e9e84b5caac" />

**3D View:**
<img width="1918" height="930" alt="Flight Controller Top Down" src="https://github.com/user-attachments/assets/8eedc2e3-7572-490f-a4bc-e9d766b1fcfc" />
<img width="1724" height="930" alt="Flight Controller Close Up" src="https://github.com/user-attachments/assets/06098a5c-1afa-4593-bb81-3540d4a8b3c4" />


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
