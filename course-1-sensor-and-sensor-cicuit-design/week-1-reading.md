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

## 📺 Video Reading: Thermocouple Tutorial (ControlEngTV)

### 🎓 Introduction

- Presented by Peter Wander, Process Industries Editor at *Control Engineering*.
- Thermocouples are a popular and sometimes debated topic in process instrumentation.
- Demonstrates how thermocouples can be made and used with simple materials.

---

### 🔧 Thermocouple Basics

- **Thermocouple construction**: Two dissimilar metals joined together form a junction that generates a voltage when heated.
- This voltage is **very small**, so sensitive instruments (e.g., digital multimeters with mV scale) are needed.

---

### 🔬 DIY Thermocouple Example

- **Materials**: Steel wire and copper wire twisted together.
- **Measurement**: Connected to a digital VOM (voltmeter) with a 0–300 mV range.
- **Heating**: A propane torch applied heat to the junction.
- **Observation**:
  - Voltage increased when heated.
  - Voltage dropped as the wire cooled — demonstrating the thermoelectric effect.

---

### 🧪 Type T Thermocouple Demonstration

- **Setup**: Real type T thermocouple wires in a crockpot of water.
  - Red wire: copper-nickel alloy.
  - Blue wire: copper.
- **Voltage increases** as the water heats (e.g., from 1.1 mV to 4.0 mV).
- Junction was in the crockpot, and the reference end in a **glass of ice water**.

---

### 🌡️ Cold Junction Compensation

- A thermocouple measures **temperature difference** between two junctions:
  - **Hot junction**: In the measurement zone (e.g., boiling water).
  - **Cold (reference) junction**: At known temperature (e.g., ice bath).
- To obtain **absolute temperature**, you must know the temperature at the reference junction.
- In field instruments, cold junction compensation is done using internal temperature sensors (e.g., thermistors).

---

### 🧾 Voltage vs. Temperature

- Example: With one junction in boiling water and the other in ice:
  - Expected: 4.253 mV for Type T at 100 °C.
  - Measured: ~4.0 mV → within expected range considering equipment limitations.
- As the hot junction cooled, voltage decreased — correlates with lower temperature.

---

### 🧠 Key Takeaways

- Thermocouples exploit the Seebeck effect — different metals generate different voltages when heated.
- You need **cold junction compensation** to interpret readings accurately.
- DIY setups are useful for learning but impractical for industrial use.
- Real-world systems use transmitters with built-in reference measurement and signal conditioning.

## 🔗 References

- RimstarOrg, *[Thermistors for measuring temperature](https://www.youtube.com/watch?v=9opuvLXAetI)*, YouTube video, (accessed 2025-07-04)
- Endress+Hauser, [*Temperature measurement in the process industry*](https://www.youtube.com/watch?v=yQvRqtozC6g ), YouTube video, (accessed 2025-07-04)
- ControlEngTV, *[Thermocouple Tutorial](https://www.youtube.com/watch?v=AubXDi6AD2M)*, YouTube video, (accessed 2025-07-04)
