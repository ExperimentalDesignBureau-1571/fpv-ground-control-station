[🇺🇸 Read in English](README_EN.md) | [🇺🇦 Читати Українською](README.md)

# Remote Unit Concentrator

The remote unit concentrator provides power distribution, concentration, and switching of signals for peripheral devices of the remote unit.

<img width="800" alt="General view of the remote unit concentrator" src="picture/general_view_concentrator_of_the_remote_unit.png" />

## Short Technical Parameters of the Remote Unit Concentrator

| Parameter | Value | Note |
| :--- | :--- | :---: |
| Input Voltage | 6S Li-ion/LiPo Battery (Min. 22.2V Max. 25.2V) | Powered through XS1 connector from the station control unit |
| Power Bus | +BAT | Direct from the station control unit battery |
| Auxiliary Bus | +5V | Formed by a DC-DC converter |
| Number of Video Inputs | 2 | XS3, XS4 |
| Input Video Signal Type | Analog Composite (CVBS) | Analog composite signal |
| Output Video Signal Type | Analog Differential | Signal conversion and amplification by the VA-Do-2/2 module with subsequent transmission over twisted pair |
| Video Input Selection | Remote | Switching from the station control unit side |
| VRX Control | Supported | Via ELRS Backpack (XS3 or XS4 video inputs) or wired connection (XS3 only) |
| TX Interface | Digital (differential) | XS2 data transmission over twisted pair |
| Power Protection | TVS Diode | Protection against inductive spikes and overvoltage |
| Cooling | Passive | Copper heatsinks + ventilation holes |
| Shielding | Yes | Copper shields |

### Interfaces

| Connector | Purpose | Main Signals | Note |
| :--- | :--- | :---: | :---: |
| XS1 (GX20-8) | Connection to control unit | +BAT, GND, differential lines | Power and signal exchange |
| XS2 (GX12-6) | TX unit connection | +BAT, GND, differential line | |
| XS3 (GX12-6) | Video Input 1, VRX1 connection | +BAT, GND, CVBS, differential line | First video input, supports control via twisted pair |
| XS4 (GX12-6) | Video Input 2, VRX2 connection | +BAT, GND, CVBS | Additional video input |

## Circuitry and Functionality of the Remote Unit Concentrator

<img width="800" alt="Remote unit concentrator schematic diagram" src="schematic_diagram/schematic_diagram_concentrator_of_the_remote_unit.JPG" />

The remote unit concentrator is powered through the XS1 connector, which receives voltage from the station control unit powered by a 6S3P Li-ion/LiPo battery. From the XS1 connector, power is supplied to the GND bus and the +BAT bus, from where it branches to the XS2, XS3, and XS4 connectors to power peripheral devices and the voltage converter that forms the +5V bus for the video amplifier. To protect the remote unit's peripheral devices from transient processes in the line connecting it to the station control unit (caused by its inductive component), a 1.5KE33A type semiconductor voltage suppressor is used.

The TX unit connects to the XS2 connector; information exchange between it and the station control unit is carried out over a twisted pair.

VRX units or other video signal sources connect to the XS3 and XS4 connectors. The composite video signal from the XS3 and XS4 connectors enters the video amplifier, which converts the composite signal into a differential one and transmits it via twisted pair to the station control unit. There, after reverse conversion, it branches to the peripheral video devices of the station control unit. Selection of the active video input (XS3 or XS4) is performed from the station control unit side. The XS3 video input has the capability for additional information exchange with the station control unit via twisted pair for remote control of the video receiver.

Thermal stability of the video amplifier and voltage converter is ensured by copper cooling heatsinks and ventilation holes in the concentrator housing. The copper heatsinks are connected to the common GND wire. Together with the side shield of the concentrator board and the shield on the concentrator cover (also connected to the GND bus), they minimize parasitic interference on the video amplifier.

The remote unit concentrator has a fairly high mounting density and involves working with different voltage levels. Successful assembly requires schematic reading skills and experience in performing medium-complexity mounting work.

<img width="600" alt="Remote unit concentrator assembly process" src="picture/installation_view.jpg" />

## List of Required Components for Manufacturing One Remote Unit Concentrator

| Name | Quantity | Note |
| :--- | :--- | :---: |
| VideoLink VA-Do-2/2 Video Amplifier | 1 pc | Ukrainian-made module [Purchase VideoLink VA-Do-2/2](https://sezam.video/shop/videopidsilyuvach-z-simetrichnim-vihodom-aktivniy-balun-videolink-va-do-22/) |
| GUTI ELECTRONICS mBEC12S Voltage Converter | 1 pc | Ukrainian analog of Matek BEC 12S [Purchase GUTI ELECTRONICS mBEC12S](https://prom.ua/ua/p2814749850-otechestvennyj-analog-matek.html) |
| GX20-8 pin Panel Plug (male) | 1 pc | XS1 |
| GX12-6 pin Panel Plug (male) | 3 pcs | XS2-XS4 |
| 1.5 mm Single-sided PCB fiberglass | 34 mm x 16 mm | Power bus board |
| TVS Diode 1.5KE33A DO201AD | 1 pc | |
| Self-adhesive copper tape (50 mm wide; 0.05 mm thick) | 156 mm | Concentrator cover shield |
| Self-adhesive copper tape (8 mm wide; 0.05 mm thick) | 286 mm | Concentrator board side shield |
| 0.8 mm thick sheet copper | 100 mm x 38 mm | Large concentrator board heatsink |
| 0.8 mm thick sheet copper | 30 mm x 19 mm | Voltage converter heatsink |
| 0.8 mm thick sheet copper | 48 mm x 26 mm | Video amplifier heatsink |
| 1 mm Silicone thermal pad 6W/m.k | 18 mm x 16 mm | Heat dissipation from converter to large board heatsink |
| 1.5 mm Silicone thermal pad 6W/m.k | 18 mm x 16 mm | Heat dissipation from converter to its heatsink |
| 2 mm Silicone thermal pad 6W/m.k | 30 mm x 27 mm - 2 pcs | Heat dissipation from video amplifier to large board heatsink |
| 1.5 mm Silicone thermal pad 6W/m.k | 27 mm x 27 mm | Heat dissipation from video amplifier to its heatsink |
| 20 AWG silicone copper wire (Black) | 810 mm | |
| 20 AWG silicone copper wire (Red) | 810 mm | |
| 26 AWG silicone copper wire (Black) | 120 mm | |
| 26 AWG silicone copper wire (Red) | 60 mm | |
| 26 AWG silicone copper wire (Green) | 410 mm | |
| 26 AWG silicone copper wire (Blue) | 290 mm | |
| 28 AWG silicone copper wire (Black) | 680 mm | |
| RG-316 Coaxial cable | 500 mm | |
| M2x6 DIN 7985 Screw | 4 pcs | |
| M2x8 DIN 7985 Screw | 11 pcs | |
| M2 DIN 125 Washer | 15 pcs | |
| M2 DIN 934 Nut | 15 pcs | |
| M3x18 DIN 7985 A2 Screw | 6 pcs | |
| M3x20 DIN 7985 A2 Screw | 5 pcs | |
| M3x25 DIN 965 Screw | 3 pcs | |
| M3x30 DIN 965 Screw | 5 pcs | |
| M3x40 DIN 965 Screw | 3 pcs | |
| M3 DIN 125 Washer | 12 pcs | |
| M3 DIN 9021 Washer | 5 pcs | |
| M3 DIN 934 Nut | 22 pcs | |
| M3 DIN 315 Wing nut | 5 pcs | |
| Part 1 - 3D print | 1 pc | |
| Part 2 - 3D print | 1 pc | |
| Part 3 - 3D print | 1 pc | |
| Part 4 - 3D print | 1 pc | |

## 3D Printing Settings and Material

| Parameter | Value |
| :---: | :---: |
| Perimeters | 4 |
| Top/Bottom solid layers | 5 |
| Infill density | 40% |
| Infill pattern | Gyroid |
| Supports | Tree |

Material: coPET black MonoFilament

## Hardware Usage Detail

| Name | Type/Size | Quantity | Note |
| :--- | :--- | :---: | :---: |
| Screw | M3x25 DIN 965 | 3 pcs | Fastening the concentrator connector block cover |
| Screw | M3x40 DIN 965 | 3 pcs | Fastening the concentrator connector block cover |
| Nut | M3 DIN 934 | 6 pcs | Fastening the concentrator connector block cover |
| Screw | M2x8 DIN 7985 | 3 pcs | Fastening large heatsink to concentrator board |
| Washer | M2 DIN 125 | 3 pcs | Fastening large heatsink to concentrator board |
| Nut | M2 DIN 934 | 3 pcs | Fastening large heatsink to concentrator board |
| Screw | M2x8 DIN 7985 | 4 pcs | Fastening VA-Do-2/2 module heatsink to concentrator board |
| Washer | M2 DIN 125 | 4 pcs | Fastening VA-Do-2/2 module heatsink to concentrator board |
| Nut | M2 DIN 934 | 4 pcs | Fastening VA-Do-2/2 module heatsink to concentrator board |
| Screw | M2x8 DIN 7985 | 4 pcs | Fastening mBEC 12S converter heatsink to concentrator board |
| Washer | M2 DIN 125 | 4 pcs | Fastening mBEC 12S converter heatsink to concentrator board |
| Nut | M2 DIN 934 | 4 pcs | Fastening mBEC 12S converter heatsink to concentrator board |
| Screw | M2x6 DIN 7985 | 4 pcs | Fastening power bus board to concentrator board |
| Washer | M2 DIN 125 | 4 pcs | Fastening power bus board to concentrator board |
| Nut | M2 DIN 934 | 4 pcs | Fastening power bus board to concentrator board |
| Screw | M3x18 DIN 7985 A2 | 6 pcs | Fastening concentrator board to base |
| Washer | M3 DIN 125 | 12 pcs | Fastening board to base (2 washers per screw) |
| Nut | M3 DIN 934 | 6 pcs | Fastening concentrator board to base |
| Screw | M3x30 DIN 965 | 5 pcs | Fastening concentrator cover |
| Nut | M3 DIN 934 | 5 pcs | Fastening concentrator cover |
| Screw | M3x20 DIN 7985 A2 | 5 pcs | Additional fastening in concentrator cover |
| Washer | M3 DIN 9021 | 5 pcs | Additional fastening in concentrator cover |
| Nut | M3 DIN 934 | 5 pcs | Additional fastening in concentrator cover |
| Wing nut | M3 DIN 315 | 5 pcs | Additional fastening in concentrator cover |

## Wire Usage Detail

XS1
| Type | Length | Note |
| :--- | :--- | :---: |
| 20 AWG black | 170 mm | XS1 - concentrator board GND bus |
| 20 AWG red | 170 mm | XS1 - concentrator board +BAT bus |
| 26 AWG green | 150 mm | XS1 - VA-Do-2/2 |
| 26 AWG blue | 150 mm | XS1 - VA-Do-2/2 |
| 26 AWG green | 60 mm | XS1 - XS2 |
| 26 AWG blue | 60 mm | XS1 - XS2 |
| 26 AWG green | 80 mm | XS1 - XS3 |
| 26 AWG blue | 80 mm | XS1 - XS3 |

XS2
| Type | Length | Note |
| :--- | :--- | :---: |
| 20 AWG black | 190 mm | XS2 - concentrator board GND bus |
| 20 AWG red | 190 mm | XS2 - concentrator board +BAT bus |

XS3
| Type | Length | Note |
| :--- | :--- | :---: |
| 20 AWG black | 220 mm | XS3 - concentrator board GND bus |
| 20 AWG red | 220 mm | XS3 - concentrator board +BAT bus |
| RG-316 | 250 mm | XS3 - VA-Do-2/2 |

XS4
| Type | Length | Note |
| :--- | :--- | :---: |
| 20 AWG black | 230 mm | XS4 - concentrator board GND bus |
| 20 AWG red | 230 mm | XS4 - concentrator board +BAT bus |
| RG-316 | 250 mm | XS4 - VA-Do-2/2 |

mBEC 12S Voltage Converter
| Type | Length | Note |
| :--- | :--- | :---: |
| 26 AWG black | 60 mm | mBEC 12S - concentrator board GND bus |
| 26 AWG red | 60 mm | mBEC 12S - concentrator board +BAT bus |
| 26 AWG green | 60 mm | mBEC 12S - concentrator board +5V bus |

VA-Do-2/2 Module
| Type | Length | Note |
| :--- | :--- | :---: |
| 26 AWG black | 60 mm | VA-Do-2/2 - concentrator board GND bus |
| 26 AWG green | 60 mm | VA-Do-2/2 - concentrator board +5V bus |
| 28 AWG black | 50 mm | VA-Do-2/2 - RG-316 cable shield from XS3 |
| 28 AWG black | 50 mm | VA-Do-2/2 - RG-316 cable shield from XS4 |

Heatsinks and Shields
| Type | Length | Note |
| :--- | :--- | :---: |
| 28 AWG black | 170 mm | Large board heatsink - concentrator board GND bus |
| 28 AWG black | 60 mm | VA-Do-2/2 module heatsink - concentrator board GND bus |
| 28 AWG black | 60 mm | mBEC 12S converter heatsink - concentrator board GND bus |
| 28 AWG black | 120 mm | Concentrator board side shield - concentrator board GND bus |
| 28 AWG black | 170 mm | Front shield on concentrator cover - concentrator board GND bus |
