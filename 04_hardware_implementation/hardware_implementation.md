# Hardware Implementation

## Overview
This section describes the practical implementation of the RF energy
harvesting system, including PCB preparation, component selection,
assembly, and soldering.

The hardware implementation was carried out with a focus on reliability,
compactness, and minimal energy loss.

---

## PCB Design and Layout
A dedicated PCB was designed to integrate all system components,
including the rectifier circuit, energy storage elements, DC-DC boost
converter, and load interface.

Key considerations during PCB design:
- Short signal paths to reduce RF losses
- Proper grounding to minimize noise
- Compact layout for efficient integration
- Adequate spacing for high-frequency signals

---

## PCB Fabrication Process
The PCB fabrication involved the following steps:

1. Cleaning the copper-clad board
2. Transferring the circuit layout onto the PCB
3. Etching excess copper using ferric chloride solution
4. Drilling component mounting holes
5. Cleaning and finishing the etched board

Safety precautions were followed while handling chemicals during the
etching process.

---

## Component Mounting
After PCB preparation, components were mounted carefully:

- Schottky diodes and capacitors were placed close to the rectifier stage
- Supercapacitor was positioned to minimize discharge path length
- DC-DC boost converter module was securely connected
- ESP32 was connected as the load device

Proper orientation and solder joint quality were ensured to avoid
performance degradation.

---

## Soldering Technique
Manual soldering was used for component assembly.

Important soldering practices followed:
- Clean soldering iron tip
- Minimal solder usage to avoid short circuits
- Proper wetting of solder joints
- Adequate cooling time after soldering

Good soldering quality was essential to ensure low resistance paths
and reliable long-term operation.

---

## Testing and Verification
After assembly, the hardware was tested to verify:
- Continuity of connections
- Proper charging of the supercapacitor
- Stable voltage output from the boost converter
- Correct operation of the ESP32 under harvested energy conditions

---

## Summary
The hardware implementation validates the practical feasibility of
RF energy harvesting from Wi-Fi signals using low-cost components
and standard PCB fabrication techniques.
