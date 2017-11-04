#PCB Design

The schematic and PCB design files for an MSP430FR2311IPW16R breakout board were designed in order to create a 
printed circuit board with headers that give direct access to the IC chip leads.

## Schematic Design

The 16 pin MSP430FR2311 chip was used in this design as it provides enough pins for the uses we would be needing it for. Each of the 16 pins were sent to headers, 8 per side, in order to grant ease of access to connect them to other components or for use on a breadboard. Apart from the direct connections, a 100nF bypass capacitor is placed between VSS and VCC in order to ground AC noise, a 10nF bulk capacitor is placed in parallel with that in order to regulate the voltages provided to the processor, and the reset circuitry consists of a 1nF capacitor that helps with debouncing and a 47k resistor that is used as a pull-up resistor.

## PCB Design

The dimensions of the PCB are 0.975 inches in length, 0.95 inches in width, and 0.039 inches in height. The board is 2-sided with an internal ground plane and is within the limitations of the machinery used to create it. In order to make the design work well, the ground plane was broken for three of the connections which does not affect the purpose of the plane.

###Bill of Materials
| RefDes      | Name     	   | Value | Quantity |
| ----------- | ------------------ | ----- | -------- | 
| C1          | CAP_0805 	   | 100nF | 1 |
| C2          | CAP_0805 	   | 10nF  | 1 |
| C3          | CAP_0805	   | 1nF   | 1 |
| J1          | 64456_8 	   | n/a   | 1 |
| J2          | 64456_8 	   | n/a   | 1 |
| R1          | RES_0805 	   | 47k   | 1 |
| U1          | MSP430FR2311IPW16R | n/a   | 1 |
