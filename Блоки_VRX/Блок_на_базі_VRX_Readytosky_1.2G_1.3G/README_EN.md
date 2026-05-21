[🇺🇸 Read in English](README_EN.md) | [🇺🇦 Читати Українською](README.md)

# Unit based on Readytosky 1.2G/1.3G VRX

The VRX unit based on the Readytosky 1.2–1.3 GHz 9CH video receiver is a functional module mounted on the remote unit and designed to receive analog video signals in the 1.2–1.3 GHz range with subsequent feeding into the ground station's communication lines.

<img width="400" alt="General view of the 1.2–1.3 GHz VRX unit based on the Readytosky receiver" src="picture/general_view_of_the_1.2_1.3_GHz_VRX_unit.png" />

## Short Technical Parameters of the VRX Unit based on the Readytosky 1.2–1.3 GHz 9CH Receiver

| Parameter | Value | Note |
|----------|---------|---------|
| Input voltage | 6S Li-ion/LiPo battery (Min. 22.2V Max. 25.2V) | Powered by the remote unit concentrator |
| Frequency range | 1060–1380 MHz | 9 channels (1080/1120/1160/1200/1240/1280/1320/1360/1258 MHz) |
| Control | Manual | Via the stock channel selector |
| Output video signal type | Analog composite (CVBS) | |

### Interfaces

| Connector | Purpose | Main Signals | Note |
|--------|------------|----------------|----------|
| XS1 (GX12-6) | Connection to the remote unit concentrator | +BAT, GND, CVBS | |

## Circuitry and Functionality

The VRX unit is powered through the XS1 connector from the +BAT bus of the remote unit concentrator. The output CVBS signal from the video receiver is transmitted via XS1 to the ground station's communication lines. Channel control is managed by the stock video receiver selector.

<img width="800" alt="Schematic diagram of the VRX unit based on the Readytosky 1.2–1.3 GHz 9CH video receiver" src="schematic_diagram/schematic_diagram_vrx_block_readytosky_1.2g_1.3g.JPG" />

## List of Required Components for Manufacturing One VRX Unit

| Name | Quantity | Note |
| :--- | :--- | :---: |
| Readytosky 1.2–1.3 GHz 9CH video receiver kit | 1 pc | |
| 90-degree SMA Female to SMA Male adapter | 1 pc | |
| GX12-6 pin (male) panel mount plug | 1 pc | XS1 |
| M2x18 DIN 7985 Screw | 1 pc | Mounting the video receiver to Part 1 |
| M2 DIN 934 Nut | 1 pc | Mounting the video receiver to Part 1 |
| 2x8 DIN 7982 Self-tapping screw | 8 pcs | Mounting Part 2 and Part 3 to Part 1 |
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
