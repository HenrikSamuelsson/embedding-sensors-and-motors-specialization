# 🌡️ Video 5 – Thermistors Basic Facts

## 📚 Overview

This video introduces **thermistors**, focusing on their material properties, temperature range, packaging, accuracy, and common embedded applications. It also sets the stage for upcoming discussions on calibration and integration into embedded systems.

---

## 🧪 What Is a Thermistor?

- **Thermistor** = Thermally sensitive resistor.
- Made from **sintered semiconductor or metal oxide** materials.
- Most thermistors are **NTC (Negative Temperature Coefficient)**:
  - **Resistance decreases** significantly with temperature rise.
- They exhibit **nonlinear** temperature vs. resistance behavior that is highly **material dependent**.

---

## 🔢 Key Characteristics

- **Base Resistance** (measured at **25 °C**):
  - Common values: **2,252 Ω** and **10,000 Ω**.
- **Accuracy**:
  - Typically **±0.1 °C to ±0.2 °C** with proper calibration.
- **Temperature Range**:
  - **−50 °C to +70 °C** for narrow-band use (e.g., smartphones).
  - Up to **200 °C** using higher base resistances (e.g., **30kΩ or 50kΩ**).

---

## 🧰 Common Applications

- **Overheating protection** in:
  - Smartphones
  - PCs
  - Laptops
- **LCD contrast compensation**:
  - LCD contrast fades at high temps.
  - Thermistor measures internal temp and adjusts signal.
- **Modern thermostats**:
  - Replaces older **bi-metallic strips**.
- **Lithium battery monitoring**:
  - Now standard for **airline-safe battery design**.
  - Thermistors are embedded inside batteries and available commercially (e.g., $11.90 on eBay).

---

## 🛠️ Thermistor Packaging Options

- **IC-form**:  
  - Example: `Microchip MCP9700`
- **Metal probe**:  
  - Designed for **fluid immersion**.
  - Examples:
    - `Vishay NTCAIMME3C90373` – 10kΩ probe
    - `U.S. Sensor H11195` – Straight aluminum probe
- **Through-hole**:  
  - Example: `Measurement Specialties 44008RC`
  - Easy to mount on a PCB.

---

## ↺ What’s Next

- Explore the **core technology** of thermistors.
- Learn the **nonlinear calibration equations**.
- Understand how to **integrate thermistors** into embedded systems.

