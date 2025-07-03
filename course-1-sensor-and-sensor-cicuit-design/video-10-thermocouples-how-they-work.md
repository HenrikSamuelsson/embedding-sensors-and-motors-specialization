# 🔌 Video 10 – Thermocouples: How They Work

## 🧪 Cold Junction Compensation (CJC)

- Measuring thermoelectric voltage from a thermocouple seems simple but introduces unintended junctions:
  - Ex: Copper–Constantan connection introduces unwanted back-EMF at a second junction (J2).

- Historical method:
  - Use an **ice bath** at J2 to fix temperature at 0 °C → known reference.

- Kirchhoff’s Law tells us:  
  `V = V₁ − V₂`

- Linear approximation:  
  `V = b × (T₁ − T₂)`  
  (with b = local slope of the thermoelectric curve)

---

## 🧊 Modern Cold Junction Compensation

- Ice baths are replaced with **isothermal metal blocks** + **thermistors**.
- Process:
  1. Measure isothermal block temperature (T₂) using a thermistor.
  2. Convert T₂ to equivalent thermoelectric voltage (V₂) using lookup table.
  3. Measure V using ADC.
  4. Compute V₁ = V + V₂.
  5. Use ITS-90 tables to find temperature T₁.

- This is how CJC is implemented in embedded systems and data loggers.

  Example: **GRAPHTEC Model 840**
  - Terminal block = isothermal block
  - Internal thermistor handles CJC

---

## 📏 Thermocouple Probe Selection

- Example: Probe from Automation Direct
  - Probe types: **Type J** (up to ~720 °C), **Type K** (up to ~1249 °C)
  - Materials:
    - **316 Stainless Steel**: Suitable for lower temps.
    - **Inconel**: Required for high temps / corrosive environments.

- Other specs:
  - **Ungrounded junction**: no electrical connection to sheath
  - **Insulation**: magnesium oxide for thermal protection
  - **Bend radius**: ≥ 12 mm
  - **Minimum insertion depth**: 76 mm

- Accuracy governed by **ASTM spec 230**:
  - Max error is higher of ±2.2 °C or ±0.75% of reading

---

## ✅ Recap

- Cold junction compensation corrects for reference junctions in thermocouple circuits
- Modern embedded systems use thermistors and isothermal blocks
- Thermocouples are chosen based on mechanical needs, accuracy, and temperature range

> End of the thermo sensors module. Next up: TBD

