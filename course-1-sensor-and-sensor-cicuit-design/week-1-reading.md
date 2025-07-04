# 📚 Thermistors for Measuring Temperature (RimstarOrg)

## 🔧 What Is a Thermistor?

- A **thermistor** is a ceramic or polymer component with two wires.
- Its **resistance changes with temperature**:
  - **PTC (Positive Temperature Coefficient):** Resistance increases with temperature.
  - **NTC (Negative Temperature Coefficient):** Resistance decreases with temperature.
- Used for experiments, temperature monitoring, and basic control applications.

---

## 🚗 Thermistors in Practice

- **Automobile coolant temperature sensors** are thermistors in a protective case.
- In the example, one wire connects to the threaded part, another to the brass case.

### 📏 Measuring Resistance

- A multimeter set to resistance mode shows the **resistance drops** when the thermistor is warmed by touch → confirms **NTC type**.

---

## 🧪 Creating a Resistance-to-Temperature Table

- No datasheet available → user **built their own table**:
  - Submerged sensor in water alongside a kitchen thermometer.
  - Placed setup in the **freezer** (~0 °C), then heated on a stove to **boiling point (100 °C)**.
  - Recorded temperature and resistance at intervals.
- Result: A **non-linear curve** of resistance vs. temperature.

---

## 🔄 Example Application: PC Fan Control

### 🔌 Basic Fan Circuit

- Fan connected directly to power: spins when power is on.

### 🌡️ Fan with Thermistor

- Thermistor added in series with the fan.
- At **room temperature**, thermistor resistance is high → **fan does not spin**.
- When **heated** with a hair dryer:
  - Resistance drops → **current increases** → **fan turns on**.
  - Fan cools thermistor → resistance rises again → fan slows/stops.

---

## 🎥 Related Topics Mentioned

- **Experiment:** Does cold water boil faster than hot water?
- **Other videos by RimstarOrg**:
  - Powering a CFL with two AA batteries.
  - Making a solar panel from transistors.
  - Subscribe and explore more experiments.

---

## 📌 Summary

- Thermistors are simple, passive components used for temperature sensing.
- NTC thermistors decrease resistance with increasing temperature.
- Can be used in DIY control applications like temperature-based fan control.
- When no datasheet is available, you can build your own resistance-temperature lookup table.

---

## 🔗 References

- RimstarOrg, *Thermistors for measuring temperature*, YouTube video,  
  https://www.youtube.com/watch?v=9opuvLXAetI (accessed 2025-07-04)
