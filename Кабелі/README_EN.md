[🇺🇸 Read in English](README_EN.md) | [🇺🇦 Читати Українською](README.md)

# Cables

To connect the control unit with the remote unit of the station, as well as to connect peripheral devices to them, cables made of shielded multi-core copper twisted pair are used.

## Set 1 - Main Trunk

This set is designed to connect the control unit and the remote unit of the station. The standard main cable is 2 meters long and is placed in the station case in the transport position. Depending on the tasks, the set can be supplemented with additional main cables, for example, a 5-8 meter cable for working with a repeater from cover, and 25-50 meters for stationary operation from cover.

<img width="600" alt="General view of Set 1 cables" src="picture/general_view_of_cables_set_1.jpg" />

The start of the standard main cable is connected to the control unit, and its end to the remote unit concentrator.

A cable joiner (coupler) is used to connect the standard main cable to an additional one. The end of the standard main cable is connected to one connector of the coupler, and the start of the additional main cable to the second connector; the end of the additional main cable is connected to the remote unit concentrator accordingly.

In case of using a repeater, the end of the standard main cable is connected to the repeater input, and the start of the additional main cable to the repeater output; the end of the additional main cable is connected to the remote unit concentrator.

<img width="800" alt="Schematic diagram of Set 1 cables" src="schematic_diagram/schematic_diagram_of_cables_set_1.JPG" />

## Set 2 - Control Subsystem

This set is designed for the internal connection of the control subsystem components. The set consists of two cables: for the JR module (long cable) and the TX unit (short cable). The start of the cable connecting the JR module for the control transmitter to the station control unit is connected to the control unit, and the end to the JR module. The start of the cable connecting the TX unit to the remote unit concentrator is connected to the concentrator, and the end to the TX unit.

<img width="800" alt="Schematic diagram of Set 2 control subsystem cables" src="schematic_diagram/schematic_diagram_of_the_control_subsystem_cables_set_2.JPG" />

### Please Note!
<ul>
<li>When manufacturing cables, the cable shield is connected to the common wire (GND) on the connector only on one side to prevent ground loops.</li>
<li>The side of the cable where the shield is connected to the common wire is the start of the cable. The start of the cable is marked with heat shrink tubing, while the color of the heat shrink also indicates the cable type (blue color - control subsystem cables).</li>
<li>When manufacturing cables, the entry hole of the connector housings must be enlarged with a needle file to the diameter of the cable used.</li>
</ul>

<img width="600" alt="Soldering the connector on a Set 1 cable" src="picture/view_of_soldered_connector.jpg" />

## List of Required Components for Manufacturing Cables

| Name | Quantity | Note |
| :--- | :--- | :---: |
| GX20-8 pin Cable Socket (female) | 2 pcs | For the standard main cable |
| GX12-6 pin Cable Socket (female) | 4 pcs | For control subsystem cables and coupler |
| Shielded multi-core copper cable | as needed | Flexible twisted pair, e.g., LiYCY |
| Heat shrink tubing (various colors) | as needed | For marking the "start" of the cable |
