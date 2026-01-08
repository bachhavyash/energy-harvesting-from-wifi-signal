# System Architecture and Design

## Overview
The proposed system is designed to harvest ambient Wi-Fi RF energy,
convert it into usable electrical power, store it efficiently, and
utilize it to power low-power electronic devices.

The architecture follows a **stage-wise energy flow**, ensuring minimal
loss and reliable operation despite the low and intermittent nature of
Wi-Fi energy.

---

## Block-Level Architecture
The complete system consists of the following functional stages:

1. RF Energy Capture (Patch Antenna)
2. RF-to-DC Conversion (Rectifier Circuit)
3. Energy Storage (Supercapacitor)
4. Voltage Boosting (DC-DC Converter)
5. Load Operation (ESP32)

Each stage is optimized to handle extremely low power levels.

---

## RF Energy Capture – Patch Antenna
A **2.4 GHz patch antenna** is used to capture Wi-Fi RF signals emitted
by routers and access points.

### Key Reasons for Using a Patch Antenna:
- Directional radiation pattern improves energy capture
- Compact and flat structure suitable for PCB integration
- Efficient operation at Wi-Fi frequency band (2.4 GHz)

The antenna converts electromagnetic RF waves into a high-frequency
electrical AC signal, which is fed to the rectifier stage.

---

## RF-to-DC Conversion – Rectifier Circuit
The captured RF signal is rectified using a **Schottky diode-based
rectifier circuit**.

### Role of the Rectifier:
- Converts high-frequency AC signal into DC voltage
- Minimizes energy loss due to low forward voltage drop
- Enables energy extraction from very weak RF signals

Schottky diodes are preferred due to their high-speed switching and
low power dissipation.

---

## Energy Storage – Supercapacitor
Since harvested RF energy is weak and fluctuating, direct powering of
devices is not practical.

A **supercapacitor (1F)** is used as an energy storage element to:
- Accumulate energy over time
- Smooth voltage variations
- Act as an energy buffer between harvesting and usage

The supercapacitor enables **energy availability on demand**, allowing
the system to operate reliably.

---

## Voltage Boosting – DC-DC Converter
The stored voltage in the supercapacitor is typically low (below the
operating voltage of microcontrollers).

An **MT3608 DC-DC boost converter** is used to:
- Step up low DC voltage to a usable level (3.3V / 5V)
- Provide regulated voltage to the load
- Improve system usability with low-energy sources

---

## Load Operation – ESP32
The ESP32 microcontroller is used to demonstrate the practical
utilization of harvested energy.

### Power Management Strategy:
- Operates in deep-sleep mode to minimize energy consumption
- Wakes up only when sufficient energy is available
- Performs limited tasks such as LED blinking or data transmission
- Returns to sleep to conserve energy

This intermittent operation strategy ensures compatibility with
energy harvesting constraints.

---

## Summary
The system architecture combines RF harvesting, energy storage,
and intelligent power management to enable practical battery-free
or battery-assisted IoT operation using ambient Wi-Fi signals.
