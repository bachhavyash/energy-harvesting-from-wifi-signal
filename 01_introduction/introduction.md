# Introduction

## Background
With the rapid growth of wireless communication and smart technologies,
there is an increasing demand for **sustainable and battery-free power solutions**
for electronic devices. The widespread deployment of Wi-Fi routers and access
points has created an opportunity to harvest energy from **ambient radio frequency (RF) signals**.

Wi-Fi networks operate continuously in most indoor and urban environments,
making them a promising source of low-level RF energy that would otherwise remain unused.

---

## Motivation
Many IoT and sensor-based systems rely on batteries, which:
- Require frequent replacement
- Increase maintenance cost
- Are unsuitable for remote or inaccessible locations

Energy harvesting from Wi-Fi signals provides a **maintenance-free and non-intrusive**
alternative for powering **ultra-low-power electronic devices**.

---

## Problem Statement
Although Wi-Fi signals are abundantly available, the **harvested energy is extremely low
and inconsistent**, making direct powering of devices impractical.

The key challenge addressed in this project is:
> How to reliably convert weak ambient Wi-Fi RF energy into usable electrical power
and utilize it effectively for low-power IoT devices.

---

## Proposed Approach
This project proposes an **energy harvesting and storage-based system**, where:
- RF energy is captured using a **2.4 GHz patch antenna**
- The signal is converted from RF to DC using a **Schottky diode-based rectifier**
- Energy is **stored first** in a supercapacitor
- Stored energy is later boosted and used to power low-power devices

By adopting an **energy-storage-first strategy**, the system ensures
more reliable and practical operation compared to direct RF powering.

---

## Significance of the Work
This project demonstrates the feasibility of:
- Harvesting ambient Wi-Fi energy
- Enabling **battery-free or battery-assisted IoT operation**
- Supporting sustainable and green electronic systems

The work highlights how commonly available wireless signals can be reused
as an alternative energy source for future IoT and smart electronic applications.
