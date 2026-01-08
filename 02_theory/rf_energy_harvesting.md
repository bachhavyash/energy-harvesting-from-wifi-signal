# RF Energy Harvesting Theory

## Overview
RF (Radio Frequency) energy harvesting is the process of capturing
electromagnetic waves from the environment and converting them into
usable electrical energy.

Ambient RF sources include Wi-Fi routers, cellular base stations,
Bluetooth devices, and broadcast transmitters. Among these,
Wi-Fi signals are widely available and continuously transmitted,
making them suitable for experimental energy harvesting.

---

## Wi-Fi as an RF Energy Source
Wi-Fi communication typically operates in the **2.4 GHz ISM band**.
Routers and access points emit RF signals continuously for data
transmission, even when no user is actively connected.

Although the power level of these signals is low, their omnipresence
makes them attractive for harvesting energy for **ultra-low-power devices**.

Key characteristics of Wi-Fi RF energy:
- Frequency: ~2.4 GHz
- Continuous transmission
- Short-range but widely available
- Non-intrusive and maintenance-free source

---

## RF-to-DC Conversion Principle
The RF energy captured by an antenna exists as an **alternating current (AC) signal**
at high frequency. This signal must be converted into **direct current (DC)**
before it can be stored or used.

The RF-to-DC conversion process involves:
1. Capturing RF energy using an antenna
2. Rectifying the high-frequency AC signal
3. Filtering and smoothing the DC output
4. Storing the energy for later use

---

## Role of Schottky Diode in Rectification
Schottky diodes are commonly used in RF energy harvesting systems due to:
- Low forward voltage drop
- High switching speed
- Low power loss at high frequencies

In this project, Schottky diodes are used to convert the weak RF signal
into a usable DC voltage, enabling efficient energy extraction even
from very low input power levels.

---

## Importance of Energy Storage
Due to the low and fluctuating nature of harvested RF energy,
instantaneous power output is insufficient to drive electronic loads.

Energy storage elements such as **supercapacitors** are therefore used to:
- Accumulate energy over time
- Provide a stable energy supply
- Enable intermittent but reliable operation

Energy storage is a critical component that bridges the gap between
ambient RF energy availability and device power requirements.

---

## Summary
RF energy harvesting from Wi-Fi signals provides a promising method
for powering low-power electronic devices without batteries.
However, practical implementation requires careful consideration of
antenna design, rectification efficiency, and energy storage strategy.
