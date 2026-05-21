[🇺🇸 Read in English](README_EN.md) | [🇺🇦 Читати Українською](README.md)

# Unit based on SKYZONE SteadyView X 5G VRX

The VRX unit based on the Skyzone SteadyView X 5G video receiver is a functional module mounted on the remote unit and designed to receive analog video signals in the 4.9–5.9 GHz range with subsequent feeding into the ground station's communication lines. To reduce screen light emission, a masking cover can be installed. The appearance of the VRX unit with and without the masking cover is shown in the following figure.

<img width="600" alt="General view of the VRX unit based on the Skyzone SteadyView X 5G video receiver" src="picture/general_view_of_the_Skyzone_SteadyView_X_5G_VRX_unit.png" />

## Short Technical Parameters of the VRX Unit based on the Skyzone SteadyView X 5G Video Receiver

| Parameter | Value | Note |
|----------|---------|---------|
| Input voltage | 6S Li-ion/LiPo battery (Min. 22.2V Max. 25.2V) | Powered from the remote unit concentrator |
| Frequency range | 4.9–5.9 GHz | |
| Control | Manual or remote | Via stock controls or ELRS Backpack |
| Output video signal type | Analog composite (CVBS) | |

### Interfaces

| Connector | Purpose | Main Signals | Note |
|--------|------------|----------------|----------|
| XS1 (GX12-6) | Connection to the remote unit concentrator | +BAT, GND, CVBS | |

## Circuitry and Functionality

The VRX unit is powered through the XS1 connector from the +BAT bus of the remote unit concentrator. The output CVBS signal from the video receiver is transmitted via XS1 to the ground station's communication lines.

<img width="800" alt="Schematic diagram of the VRX unit based on the Skyzone SteadyView X 5G video receiver" src="schematic_diagram/schematic_diagram_vrx_block_skyzone_steadyview_x.JPG" />

The connection of the video receiver to the XS1 connector is made using 26 AWG copper wires with silicone insulation. The red wire (+BAT) is connected to the cathode of the TVS diode, the black wire (GND) to the negative terminal of the capacitor, and the yellow wire (CVBS) to the sixth pin of the RXPORT100 V1.1 board connector of the Skyzone SteadyView X 5G video receiver.

<img width="600" alt="Connecting wires to the RXPORT100 V1.1 board" src="picture/сonnecting_wires_to_the_board_RXPORT100_V1.1.jpg" />

Channel control is carried out by the stock video receiver controls or through the ELRS Backpack.

## List of Required Components for Manufacturing One VRX Unit

| Name | Quantity | Note |
| :--- | :--- | :---: |
| VRX Skyzone SteadyView X 5G video receiver kit | 1 pc | |
| 90-degree SMA Female to SMA Male adapter | 2 pcs | |
| GX12-6 pin (male) panel mount plug | 1 pc | XS1 |
| Double-sided 2mm acrylic tape | 100 mm | Mounting VRX Skyzone SteadyView X 5G to Part 1 |
| 2x8 DIN 7982 self-tapping screw | 8 pcs | Mounting Part 2 and Part 3 to Part 1 |
| 26 AWG black silicone insulated copper wire | 150 mm | VRX Skyzone SteadyView X 5G -> XS1 |
| 26 AWG red silicone insulated copper wire | 150 mm | VRX Skyzone SteadyView X 5G -> XS1 |
| 26 AWG yellow silicone insulated copper wire | 150 mm | VRX Skyzone SteadyView X 5G -> XS1 |
| Part 1 - 3D print | 1 pc | |
| Part 2 - 3D print | 1 pc | |
| Part 3 - 3D print | 1 pc | |

## 3D Printing Settings and Material

| Parameter | Value |
| :---: | :---: |
| Perimeters | 4 |
| Top/Bottom solid layers | 5 |
| Infill density | 40% |
| Infill pattern | Gyroid |
| Supports | Tree |

Material: coPET black MonoFilament
