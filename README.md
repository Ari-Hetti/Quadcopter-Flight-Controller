
<h1 align="center">
Quadcopter Flight Controller
</h1>

<h3 align="center">
A Custom Flight Controller For a 5in FPV Quadcopter
</h3>

<p align="center">
  <a href="#key-features">Key Features</a> -
  <a href="#description">Description</a> -
  <a href="#components">Components</a> -
  <a href="#board-design">Board Design</a> -
  <a href="#bom">BOM</a> -
  <a href="#software">Software</a> -
  <a href="#credits">Credits</a> -
  <a href="#my-other-projects">My Other Projects</a> -
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
The reason why I built this project was because it seemed like a hard enough challenge to get me into proper pcb design while building something I can use and have fun with. I also built it so I can further my skills that I need to teach others about pcb design. I built [this project](https://stasis.hackclub.com/dashboard/projects/cmn58nljt00a101mzkp03c4fs) in Hackclub Statis using help from the Hackclub Blueprint Flight Controller Guide which I adapted for a multirotor build. On my project page in Statis, there are my journals I made during this project capturing my journey in this project.

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

## BOM
Name |	Purpose |	Quantity |	Total Cost (USD) |	Link |	Distributor
|----|----------|----------|-------------------|-------|-------------|  
PCBA |	Build Board |	2 |	29.91 |	 |	JLCPCB
PCB |	The Board |	5 |	2 |	 |	JLCPCB
32Khz Crystal |	Low Speed Clock |	5 |	0.36 |	https://jlcpcb.com/partdetail/SeikoEpson-Q13FC13500002/C48615 |	JLCPCB
25Mhz Crystal |	High Speed Clock |	2 |	0.15 |	https://jlcpcb.com/partdetail/YXC_CrystalOscillators-X322525MOB4SI/C9006 |	JLCPCB
27Mhz Crystal |	OSD Clock |	6 |	0.43 |	https://jlcpcb.com/partdetail/19392660-XL7EL89COI_111YLC27M/C18214311 |	JLCPCB
USB-C	 |Flashing Software |	20 |	1.27 |	https://www.lcsc.com/product-detail/C2765186.html |	LCSC
ICM-45686 |	Interial Measurement Unit |	2 |	35.78 |	https://jlcpcb.com/partdetail/TDKInvenSense-ICM45686/C22459454 |	JLCPCB
BMP280 |	Barometer | 	2 |	12.06 |	https://www.lcsc.com/product-detail/C83291.html?spm=wm.gwc.xh.7.cbm___wm.jsy.top.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeUlJRQVVbUTtW |	LCSC
Buzzer |	Help Find After Downed |	2 |	2.09 |	https://www.lcsc.com/product-detail/C18186314.html |	LCSC
LMR51430 |	3.3V Voltage Regulators |	2 |	1.81 |	https://jlcpcb.com/partdetail/TexasInstruments-LMR51430YFDDCR/C5219261 |	JLCPCB
TPS63070RNMR |	5V / 9V Voltage Regulators |	4 |	5.69 |	https://jlcpcb.com/partdetail/TexasInstruments-TPS63070RNMR/C109322 |	JLCPCB
AT7456E |	Displays Important Info On Video Out Feed |	3 |	11.16 |	https://jlcpcb.com/partdetail/ZHONGKEWEI-AT7456E/C82351 |	JLCPCB
STM32F722RET6 |	Microcontroller |	2 |	12.91 |	https://jlcpcb.com/partdetail/STMicroelectronics-STM32F722RET6/C118207 |	JLCPCB
Tactile Switch |	Boot / Reset Buttons |	4 |	0.22 |	https://jlcpcb.com/partdetail/XUNPU-TS_1088AR02016/C720477 |	JLCPCB
22k Resistor |	Voltage Divider |	20 |	0.002 |	https://jlcpcb.com/partdetail/26511-0402WGF2202TCE/C25768 |	JLCPCB
100k Resistor |	Voltage Divider Resistors |	20 |	0.0018 |	https://jlcpcb.com/partdetail/26484-0402WGF1003TCE/C25741 |	JLCPCB
39Ω Resistor |	Lower Feedback Resistor |	100 |	0.09 |	https://www.lcsc.com/product-detail/C185420.html?spm=wm.gwc.xh.12.cbm___wm.jsy.top.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeUlJRQVVbUTtW |	LCSC
402Ω Resistor |	Feedback Resistors |	20 |	0.08 |	https://www.lcsc.com/product-detail/C41042.html?spm=wm.gwc.xh.11.cbm___wm.jsy.top.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeUlJRQVVbUTtW |	LCSC
75Ω Resistor |	Video Out Resistor |	100 |	0.09 |	https://www.lcsc.com/product-detail/C25133.html?spm=wm.gwc.xh.10.cbm___wm.jsy.top.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeUlJRQVVbUTtW |	LCSC
1.5k Resistor |	Voltage LED / V Sense Resistors |	20 |	0 |	https://jlcpcb.com/partdetail/26610-0402WGF1501TCE/C25867 |	JLCPCB
1k Resistor |	Buzzer / Voltage LED / Current Sense Resistors |	20 |	0.01 |	https://jlcpcb.com/partdetail/12256-0402WGF1001TCE/C11702 |	JLCPCB
5.1k Resistor |	Pull-down / Voltage LED Resistors |	20 |	0.01 |	https://jlcpcb.com/partdetail/26648-0402WGF5101TCE/C25905 |	JLCPCB
10k Resistor |	General Purpose |	24 |	0.03 |	https://jlcpcb.com/partdetail/26487-0402WGF1002TCE/C25744 |	JLCPCB
33Ω Resistor |	Series Termination Resistor |	20 |	0.0016 |	https://jlcpcb.com/partdetail/25848-0402WGF330JTCE/C25105 |	JLCPCB
5.6uH Inductor |	Power Inductor |	5 |	0.85 |	https://www.lcsc.com/product-detail/C475914.html |	LCSC
1uH Inductor |	Power / EMI Inductor |	10 |	1.41 |	https://www.lcsc.com/product-detail/C435392.html |	LCSC
LED |	Voltage Detection |	6 |	0.07 |	https://jlcpcb.com/partdetail/Hubei_KENTOElec-KT0603W/C2290 |	JLCPCB
Diode |	Flyback / USB Diodes |	100 |	0.57 |	https://www.lcsc.com/product-detail/C917030.html?spm=wm.gwc.xh.14.cbm___wm.sxq.ssl.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeX1RSR1leVTsOAxUeFF5JWBYZEEoKFBINSQcJGk4%3D |	LCSC
4 Pin Connector |	Reciever Connector |	10 |	0.48 |	https://www.lcsc.com/product-detail/C2906270.html |	LCSC
5 Pin Connector |	Video Transmitter |	10 |	0.53 |	https://www.lcsc.com/product-detail/C2906271.html |	LCSC
6 Pin Connector |	Camera Connector |	10 |	0.51 |	https://www.lcsc.com/product-detail/C2906272.html |	LCSC
8 Pin Connector |	ESC Connector |	10 |	0.61 |	https://www.lcsc.com/product-detail/C5340778.html |	LCSC
TF Card |	Store Blackbox Flight Data |	5 |	0.88 |	https://www.lcsc.com/product-detail/C91145.html?spm=wm.gwc.xh.9.cbm___wm.gwc.ssl.gwc&lcsc_vid=RAcKAlZfRgcIX1ReFQJbUgBSRQMIXgJTTgVcAwJURlQxVlNRQVVeUlJRQVVbUTtW |	LCSC
47uF Capacitor |	Bulk Capacitors |	5 |	0.15 |	https://jlcpcb.com/partdetail/17464-CL21A476MQYNNNE/C16780 |	JLCPCB
1uF Capacitor |	Decoupling Capacitors |	20 |	0.03 |	https://jlcpcb.com/partdetail/53938-CL05A105KA5NQNC/C52923 |	JLCPCB
10uF Capacitor |	Decoupling Capacitors |	22 |	0.14 |	https://jlcpcb.com/partdetail/16204-CL05A106MQ5NUNC/C15525 |	JLCPCB
18pF Capacitor |	Load Capacitors |	22 |	0.02 |	https://jlcpcb.com/partdetail/1901-0402CG180J500NT/C1549 |	JLCPCB
100nF Capacitor |	Decoupling Capacitors |	36 |	0.05 |	https://jlcpcb.com/partdetail/1877-CL05B104KO5NNNC/C1525 |	JLCPCB
22uF Capacitor |	Decoupling Capacitors |	20 |	0.19 |	https://jlcpcb.com/partdetail/60514-CL10A226MQ8NRNC/C59461 |	JLCPCB
2.2uF Capacitor |	Decoupling Capacitors |	50 |	0.01 |	https://jlcpcb.com/partdetail/13164-CL05A225MQ5NSNC/C12530 |	JLCPCB


## Software
For this project I will be running [Betaflight 2025.12.2 ](https://betaflight.com/) (current stable version), which is an open-source firmware. Since I cant just put Betaflight in here, and I can't configure anything without the board, I will just put the .ioc file I used to confirm my pinouts to make sure that the board functions, let alone to run Betaflight. 

## Credits
This was made using:
- [KiCAD](https://www.kicad.org/) - PCB Design
- [STM32Cube MX](https://www.st.com/en/development-tools/stm32cubemx.html) - STM32 Pinout / Clock Setup
- [JLCPCB](https://jlcpcb.com/) - PCB Manufacturing / Assembly
- [LCSC](https://www.lcsc.com/) - Component Sourcing
- [Blueprint Guide](https://stasis.hackclub.com/starter-projects/split-keyboard) - Flight Controller Guide by [NotARoomba](https://github.com/notaroomba)

## My Other Projects
- [Split Keyboard](https://github.com/Ari-Hetti/Split-Keyboard) - A 32 Key Split Keyboard with Thumb Knobs that can be Powered Wired or Wirelessly.
- [Hexpad_Highway](https://github.com/Ari-Hetti/Hexpad_Highway) - A Small Macropad with 6 Switches, 1 Rotary encoder and 1 OLED display Encased in a 3d Printed Enclosure
- [FRC Badge V2](https://github.com/Ari-Hetti/FRC-Badge-V2) - Hexagonal 555 Timer LED Chaser Keychain
