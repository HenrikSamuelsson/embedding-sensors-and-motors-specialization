# 📐 Video 8 – RTDs: How They Work

## 📘 Overview

This video explores how RTDs work from a circuit and calibration standpoint. It covers key challenges in achieving measurement accuracy, the role of lead wire resistance, bridge configurations, and the use of polynomial equations to linearize RTDs.

---

## ⚠️ Measurement Challenges

- RTDs must connect to embedded systems using **lead wires**.
- **Lead wire resistance** (typically 1–10 Ω) introduces error in measurements.
  - Example: 1 Ω extra resistance → ~2.6 °C temperature error (using slope of 0.385 Ω/°C)

---

## 🔁 Wheatstone Bridge Approaches

- **Simple circuit**: Measures resistance directly but is inaccurate due to unaccounted lead wire resistance.

- **First Wheatstone bridge**: Fixed resistors have their own temperature coefficients and drift.

- **Remote resistors**: Better thermal stability but reintroduces lead length problems.

- **3-wire Wheatstone bridge**:
  - Use equal-length wires (A & B) on opposite sides → resistance cancels out.
  - Third wire (C) is dead-ended → no current.
  - Allows better error cancellation but sacrifices linearity.

- **Final refinement**:
  - Insert known resistor values (R₁ = R₂, Rₐ = R_b)
  - Derive equations to solve for RTD resistance, with or without accounting for lead resistance.
  - Still sensitive to wire variability unless fully characterized or constant.

- **Best accuracy**: Use a **4-wire RTD** where calculations can fully isolate the sensor element.

---

## 📏 RTD Linearity and Polynomial Calibration

- RTDs are **not perfectly linear** over their full temperature range.
- Error curve:
  - **Negative deviation** below ~200 °C
  - **Positive deviation** above that

### 📈 Linearization Method

- Use **polynomial fitting** based on calibration data:

  - **Below 0 °C**: Use a **third-order polynomial**, calibrated at 3 points (solve for A, B, C)
  - **Above 0 °C**: Use a **second-order polynomial**, calibrated at 2 points (solve for A, B)

---

## 🛒 RTD Selection Example

- Example: **Vishay PTS 0603 chip**
  - 100 Ω at 0 °C
  - TCR: 0.385 Ω/°C or 3850 ppm/°K
  - Range: –55 °C to 155 °C
  - **2-second response** in air stream (but slower when mounted on PCB)
  - Very low **long-term drift**

- Other options:
  - **PTS 0805**: 100 Ω or 500 Ω versions
  - **PTS 1206**: 1000 Ω version

### Why higher resistance?
- **IEC 60751** defines 100 Ω standard, but some sensors use 500 Ω or 1000 Ω.
- Higher nominal resistance → lead resistance is a smaller percentage of total → improved accuracy with 3-wire setups.

---

## ✅ Recap

- Discussed core RTD circuitry and the need to account for **lead wire resistance**.
- Covered use of **Wheatstone bridges** and 3-wire/4-wire configurations.
- Introduced **polynomial linearization techniques**.
- Showed how higher resistance RTDs can mitigate lead wire error.
- Next up: thermocouples — their accuracy, range, and usage.

