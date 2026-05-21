[🇺🇸 Read in English](README_EN.md) | [🇺🇦 Читати Українською](README.md)

# Cables

Shielded multi-core twisted pair copper cables are used to connect the station control unit with the external unit, as well as to connect peripheral devices to them.

## Set 1 - Main cable set

This set is intended for connecting the station control unit with the external unit.

The standard main cable has a length of 2 meters and is stored inside the station case during transportation.

<img width="600" alt="General view of cable set 1" src="picture/general_view_of_cables_set_1.jpg" />

Depending on operational requirements, the set can be supplemented with additional main cables, for example:

<ul>
<li>5-8 meter cable for relay operation from cover</li>
<li>25-50 meter cable for stationary operation from cover</li>
</ul>

The following cable types can be used for manufacturing the main cable set:

<ul>
<li>RVSP twisted pair 8x0.5 mm² / 20 AWG</li>
<li>RVSP twisted pair 8x0.3 mm² / 22 AWG</li>
<li>LAPP UNITRONIC LiYCY (TP) 4X2X0.5</li>
<li>LAPP UNITRONIC LiYCY (TP) 4X2X0.25</li>
</ul>

The maximum cable length depends on the cable type:

<ul>
<li>for cables with a conductor cross-section of 0.5 mm² - maximum length up to 50 meters</li>
<li>for cables with a conductor cross-section of 0.25–0.3 mm² - maximum length up to 25 meters</li>
</ul>

<img width="800" alt="Schematic diagram of cable set 1" src="schematic_diagram/schematic_diagram_of_cables_set_1.JPG" />

### Please note!

<ul>
<li>When manufacturing the cables, the cable shield must be connected to the common ground only on one side of the connector to prevent ground loop formation.</li>

<li>The side of the cable where the shield is connected to the common ground is considered the beginning of the cable. The cable beginning is marked with heat-shrink tubing.</li>

<li>When using cables with a 0.5 mm² conductor cross-section, the connector housing inlet must be enlarged with a file according to the cable diameter.</li>
</ul>

<img width="600" alt="View of soldered connectors of cable set 1" src="picture/view_of_soldered_cable_connectors_set_1.jpeg" />

### Required components for manufacturing one standard main cable

| Item | Quantity | Note |
| :--- | :--- | :---: |
| RVSP twisted pair 8x0.5 mm² / 20 AWG or equivalent cable | 2 meters | Main cable |
| GX20-8 pin cable connector (female) | 2 pcs |  |
| Heat-shrink tubing | As required | Cable marking |

## Cable connector for Set 1

<img width="800" alt="Schematic diagram of cable connector for set 1" src="schematic_diagram/schematic_diagram_of_the_cable_connector_set_1.JPG" />

Structurally, the connector is made in a compact enclosure containing connectors interconnected according to the corresponding electrical schematic.

<img width="600" alt="Cable connector assembly example" src="picture/connector_assembly_example.jpg" />

### Required components for manufacturing one connector

| Item | Quantity | Note |
| :--- | :--- | :---: |
| GX20-8 pin panel connector (male) | 2 pcs |  |
| 20 AWG copper wire with silicone insulation, red | 110 mm |  |
| 20 AWG copper wire with silicone insulation, black | 440 mm |  |
| 20 AWG copper wire with silicone insulation, yellow | 330 mm |  |
| M3x40 DIN 965 screw | 4 pcs |  |
| M3 DIN 934 nut | 4 pcs |  |
| Part 1 — 3D printed | 1 pc |  |
| Part 2 — 3D printed | 1 pc |  |

## Set 2 - Peripheral

This set is intended for connecting peripheral devices to the station control unit and the external unit.

The set includes:

<ul>
<li>VRX block connection cables (yellow heat-shrink marking)</li>
<li>control subsystem cables (blue heat-shrink marking)</li>
</ul>

<img width="600" alt="General view of cable set 2" src="picture/general_view_of_cables_set_2.jpg" />

## VRX block connection cables

Depending on the station configuration, two cable variants can be used. They differ by the ability to transmit control signals to the VRX block.

If the VRX block is controlled manually or via ELRS Backpack, the first cable variant is used.

If control is performed through the ground station communication lines, the second cable variant is used.

The beginning of the cable is connected to the external unit concentrator, and the end of the cable is connected to the VRX block.

<img width="800" alt="Schematic diagram of VRX block connection cables set 2" src="schematic_diagram/schematic_diagram_of_cables_VRX_blocks_set_2.JPG" />

### Please note!

<ul>
<li>When manufacturing the cables, the cable shield must be connected to the common ground only on one side of the connector to prevent ground loop formation.</li>

<li>The side of the cable where the shield is connected to the common ground is considered the beginning of the cable. The cable beginning is marked with heat-shrink tubing. The heat-shrink tubing color also indicates the cable type (yellow color - VRX block connection cables).</li>

<li>When manufacturing the cables, the connector housing inlet must be enlarged with a file according to the cable diameter.</li>
</ul>

### Required components for manufacturing one VRX block connection cable

| Item | Quantity | Note |
| :--- | :--- | :---: |
| LAPP UNITRONIC LiYCY (TP) 2x2x0.25 or LAPP UNITRONIC LiYCY (TP) 3x2x0.14 | 120 mm |  |
| GX12-6 pin cable connector (female) | 2 pcs |  |

## Control subsystem cables

This type of cable is used for connecting:

<ul>
<li>JR module adapter for the radio controller (long cable)</li>
<li>TX unit (short cable)</li>
</ul>

<img width="800" alt="Schematic diagram of control subsystem cables" src="schematic_diagram/schematic_diagram_of_the_control_subsystem_cables_set_2.JPG" />

The beginning of the cable connecting the TX unit to the external unit concentrator must be connected to the concentrator, while the end must be connected to the TX unit.

### Please note!

<ul>
<li>When manufacturing the cables, the cable shield must be connected to the common ground only on one side of the connector to prevent ground loop formation.</li>

<li>The side of the cable where the shield is connected to the common ground is considered the beginning of the cable. The cable beginning is marked with heat-shrink tubing. The heat-shrink tubing color also indicates the cable type (blue color - control subsystem cables).</li>

<li>When manufacturing the cables, the connector housing inlet must be enlarged with a file according to the cable diameter.</li>
</ul>

### Required components for manufacturing one control subsystem cable set

| Item | Quantity | Note |
| :--- | :--- | :---: |
| LAPP UNITRONIC LiYCY (TP) 2x2x0.25 | 1120 mm | 1000 mm — long cable, 120 mm — short cable |
| GX12-6 pin cable connector (female) | 4 pcs |  |
