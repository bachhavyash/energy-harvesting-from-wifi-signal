# Experimental Results and Performance Analysis

## Overview
This section presents the experimental observations and performance
analysis of the RF energy harvesting system implemented in this project.

The results reflect real-world behavior of ambient Wi-Fi energy harvesting,
highlighting both its potential and limitations.

---

## Observed Output Characteristics
The harvested RF energy from Wi-Fi signals was observed to be:
- Extremely low in magnitude (microwatt to milliwatt range)
- Highly dependent on distance from the Wi-Fi source
- Sensitive to antenna orientation and surrounding environment

These characteristics are inherent to ambient RF energy harvesting systems.

---

## Effect of Distance and Orientation
Key observations include:
- Output voltage decreases rapidly with increased distance from the router
- Proper alignment of the patch antenna significantly improves energy capture
- Obstructions such as walls and metal objects reduce harvesting efficiency

This confirms the directional and short-range nature of Wi-Fi energy harvesting.

---

## Energy Storage Behavior
The supercapacitor played a critical role in system operation:
- Energy accumulated gradually over time
- Stored energy enabled intermittent operation of the load
- Voltage stability improved after sufficient charging duration

Energy storage allowed the system to operate even when instantaneous
harvested power was insufficient.

---

## ESP32 Operation Results
The ESP32 successfully demonstrated:
- Booting after sufficient energy accumulation
- Operation in deep-sleep mode to conserve energy
- Intermittent task execution (LED blinking / basic operations)

Continuous operation was not feasible, but **intermittent and reliable
operation was achieved**, validating the system design.

---

## Performance Limitations
Despite successful demonstration, the system has inherent limitations:
- Low conversion efficiency
- Short effective harvesting range
- Unsuitability for high-power devices

These limitations are consistent with existing RF energy harvesting research.

---

## Summary
The experimental results confirm that harvesting energy from ambient
Wi-Fi signals is feasible for powering ultra-low-power devices when
combined with energy storage and intelligent power management.
