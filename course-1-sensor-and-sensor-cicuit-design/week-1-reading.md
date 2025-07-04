# Week 1 "Reading"

Three Youtube videos are recommended "reading" for week one of the course. This is notes based on the content of these videos.

## 📺 Video Reading: Thermistors for Measuring Temperature (RimstarOrg)

### 🔧 What Is a Thermistor?

- A **thermistor** is a ceramic or polymer component with two wires.
- Its **resistance changes with temperature**:
  - **PTC (Positive Temperature Coefficient):** Resistance increases with temperature.
  - **NTC (Negative Temperature Coefficient):** Resistance decreases with temperature.
- Used for experiments, temperature monitoring, and basic control applications.

---

### 🚗 Thermistors in Practice

- **Automobile coolant temperature sensors** are thermistors in a protective case.
- In the example, one wire connects to the threaded part, another to the brass case.

#### 📏 Measuring Resistance

- A multimeter set to resistance mode shows the **resistance drops** when the thermistor is warmed by touch → confirms **NTC type**.

---

### 🧪 Creating a Resistance-to-Temperature Table

- No datasheet available → user **built their own table**:
  - Submerged sensor in water alongside a kitchen thermometer.
  - Placed setup in the **freezer** (~0 °C), then heated on a stove to **boiling point (100 °C)**.
  - Recorded temperature and resistance at intervals.
- Result: A **non-linear curve** of resistance vs. temperature.

---

### 🔄 Example Application: PC Fan Control

#### 🔌 Basic Fan Circuit

- Fan connected directly to power: spins when power is on.

#### 🌡️ Fan with Thermistor

- Thermistor added in series with the fan.
- At **room temperature**, thermistor resistance is high → **fan does not spin**.
- When **heated** with a hair dryer:
  - Resistance drops → **current increases** → **fan turns on**.
  - Fan cools thermistor → resistance rises again → fan slows/stops.

---

### 🎥 Related Topics Mentioned

- **Experiment:** Does cold water boil faster than hot water?
- **Other videos by RimstarOrg**:
  - Powering a CFL with two AA batteries.
  - Making a solar panel from transistors.
  - Subscribe and explore more experiments.

---

### 📌 Summary

- Thermistors are simple, passive components used for temperature sensing.
- NTC thermistors decrease resistance with increasing temperature.
- Can be used in DIY control applications like temperature-based fan control.
- When no datasheet is available, you can build your own resistance-temperature lookup table.

---

## 📺 Video Reading: Temperature Measurement in the Process Industry (Endress+Hauser)

### ❓ Purpose

Explain how temperature is measured in industrial process systems and highlight the use of platinum resistance thermometers (RTDs), especially Pt100 sensors.

### 🔧 Key Concepts

- **Process Industry Media:** Includes liquids (e.g., milk, oil, water) and gases (e.g., natural gas, biogas).
- **Measurement Principle:** Resistance Temperature Measurement (RTM) is one of the most common methods.

### 📏 Temperature Scales

- **Celsius (°C):** Introduced by Anders Celsius in 1742.
- **Kelvin (K):** Introduced by William Thompson (Lord Kelvin) in thermodynamics.
- **ΔT Equivalence:** A difference of 1 K is equal to 1 °C.

### 🧪 RTD Sensor Design

- **Structure:**
  - Thermowell housing a rod-shaped **measuring insert**.
  - Sensor is fitted at the **tip** of the insert.
- **Common Sensor:** 
  - **Pt100**: A platinum resistor with exactly **100 Ω at 0 °C**.
  - Made with **thin-film technology**: Platinum trace on ceramic.
- **Working Principle:**
  - **Increased temperature → increased atomic vibrations → increased resistance**.
  - Current through platinum is impeded by thermal agitation.

### ⚙️ Signal Conversion

- The resistance value is passed to a **temperature transmitter**:
  - Converts resistance to a standardized, interference-resistant signal.
  - Performs **error checking** (e.g. wire break detection).
  - Can display the measurement locally.

### ✅ Advantages of RTD (Pt100)

- High accuracy.
- Excellent long-term stability.
- Usable over a wide temperature range.
- Reliable in:
  - Hygienic environments.
  - Vibrating installations.
  - High temperature applications.

### 🏭 Industrial Use

RTDs like Pt100 are widely used in process automation due to their robustness and precision. Solutions are available for standard and specialized applications.


### 🔗 References

- RimstarOrg, *Thermistors for measuring temperature*, YouTube video, https://www.youtube.com/watch?v=9opuvLXAetI (accessed 2025-07-04)
- Endress+Hauser *Temperature measurement in the process industry*, Youtube video, https://www.youtube.com/watch?v=yQvRqtozC6g, (Accessed2025-07-04)
