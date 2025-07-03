# 📐 Video 6 – Thermistors: How They Work

## 🧠 Overview

This video explains the **core theory behind thermistors**, focusing on their nonlinear behavior, the **Steinhart–Hart equation**, and practical considerations for **measuring temperature with firmware**. It also explores **circuit design trade-offs** for accurate resistance measurement.

---

## 🔹 Resistance vs. Temperature

- Thermistors (NTC type) exhibit **strong nonlinear behavior**.
- Example: A **10 kΩ thermistor** at 25 °C can drop by **four orders of magnitude** over a 100 °C increase.
- The **resistance–temperature curve** is smooth but steep.

---

## 🧮 Steinhart–Hart Equation

- Describes the **nonlinear resistance–temperature** relationship.
- Developed in **1968** by Steinhart and Hart (geophysicists).
- Involves:
  - Natural logarithm of resistance
  - Temperature in **Kelvin**
  - Three material constants (**A**, **B**, **C**) or simplified form with a single **β (beta)** parameter

### Simplified β-form:
- Easier to implement in firmware
- Requires only:
  - Two temperature-resistance points
  - One material constant (**β**)

---

## 🛠️ Practical Implementation

### 🔌 Thermistor Example

- **Type**: Through-hole (resembles a matchstick)
- **Accuracy**: ±0.1 °C to ±0.2 °C
- **Response time**: ~10 seconds in air
- **Power dissipation**: 30 mW
- **Base resistance**: 10 kΩ
- **β constant**: 3890 K
- Manufacturer often provides **resistance-vs-temperature tables** (e.g., Excel spreadsheets)

---

## 📟 Measuring Resistance

### ✅ Option 1: Voltage Divider

- Simple circuit using a fixed resistor and the thermistor
- Accuracy depends on:
  - Stability of the **voltage source**
  - Tolerance of the **fixed resistor**

### ✅ Option 2: ADC Measurement

- Use the **same ADC** to measure voltage across both thermistor and reference resistor
- Use a **precision resistor** to reduce error

---

## ⚡ Voltage Source Accuracy

### 🔧 What is VDAC?

- **VDAC** = Voltage Digital-to-Analog Converter
- Converts a digital value into an analog voltage.
- Used to provide a programmable voltage source for circuits like voltage dividers.
- In the PSoC, it can be controlled from firmware and is useful for powering sensor circuits.



- **PSoC reference voltage**: ~0.5% accuracy
- **Precision shunt reference** (e.g., Texas Instruments): ~0.2% accuracy (adds ~$0.96 cost)
- **Stackpole 0.25% 10 kΩ resistor**: ~$0.05 cost — better tradeoff
- **VDAC (Voltage DAC)** in PSoC:
  - Useful but has poor voltage accuracy (up to 5% gain error)
  - Needs an external op-amp for current drive

---

## 🧑‍💻 Firmware Considerations

- Set up and configure the **ADC**
- **Sequence inputs**, measure voltage/current
- Use either:
  - **Steinhart–Hart calculation** (logarithmic, CPU-heavy)
  - **Table lookup** (less CPU, more memory)
    - Requires storing data from thermistor datasheet (e.g., Excel table)

---

## ✅ Recap

- Covered **thermistor theory**, **Steinhart–Hart equation**, and practical implementation.
- Discussed **circuit design choices** and **firmware strategies** for temperature measurement.
- Next up: exploring **RTDs** — their accuracy, range, and application differences.

