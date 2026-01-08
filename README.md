# Energy Harvesting from Wi-Fi Signals
### A Battery-Free RF Energy Harvesting System for Low-Power IoT Devices

---

## 📌 Project Overview
This project focuses on the design and experimental implementation of an
RF energy harvesting system that captures ambient 2.4 GHz Wi-Fi signals
and converts them into usable DC power.

The system is designed for **battery-free or battery-assisted IoT operation**
by harvesting, storing, and intelligently utilizing ambient RF energy.

---

## 🎯 Objectives
- Harvest ambient Wi-Fi (2.4 GHz) RF energy
- Convert RF energy into DC power
- Store harvested energy for later use
- Power low-power devices reliably using stored energy

---

## 🔋 Energy Storage & Continuous Operation Strategy

Ambient Wi-Fi energy is inherently **low and inconsistent**, making it
unsuitable for directly powering electronic devices in real time.
To overcome this limitation, the system adopts an
**energy-storage-first approach**.

The harvested RF energy is first converted to DC and stored in an
**energy storage element (supercapacitor)**.
The stored energy is then used to power the load **only when sufficient
energy has been accumulated**.

### Why Energy Storage Is Necessary
- Wi-Fi signals do not provide constant power levels
- Instantaneous harvested power is very low
- Direct powering leads to unstable operation

### Benefits of Energy Storage
- Enables continuous system availability
- Allows devices to operate on-demand
- Supports intermittent but reliable operation
- Makes the system practical for real-world IoT use cases

By storing energy first and utilizing it intelligently, the system ensures
that devices receive power **when required**, rather than depending on
momentary RF energy availability.

---

## 📂 Repository Structure (Work in Progress)
This repository is being built step-by-step with proper documentation,
design explanation, and experimental results.
