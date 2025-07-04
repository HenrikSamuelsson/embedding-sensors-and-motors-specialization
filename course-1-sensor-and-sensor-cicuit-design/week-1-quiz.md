# Sensor and Sensor Circuit Design: Quiz Week 1

## Example question 1

### ❓ Question

Which of the following is not a type of sensor in your smartphone?

⚪ Gyroscope  
⚪ Capacitive Touch Screen  
⚪ Pressure  
⚪ GPS  
⚪ Temperature  

### 📝 Solution

All listed items appear in some form in smartphones:

  - **Gyroscope:** Detects rotation/motion.
  - **Capacitive Touch Screen:** Detects user input — technically a type of sensor.
  - **GPS:** Receives satellite signals to determine location — not a sensor in the traditional sense (i.e., not measuring a physical property of the phone’s environment).
  - **Temperature:** Used internally for CPU and battery monitoring — not for ambient sensing.
  - **Pressure (Barometer):** Present in some smartphones, but not universal.

The quiz most likely expects **Pressure** as the answer, since it’s less commonly included.

### 🎯 Answer

**Pressure** (as expected by quiz makers, though interpretation may vary)

## Example Question 2

### ❓ Question

What advantage does a thermocouple have over the NTC thermistor?  
*(Select all that apply)*

☐ It is more accurate than the NTC thermistors.  
☐ It can measure higher temperatures than the NTC thermistor.  
☐ Its curve of temperature vs. voltage is more linear, and can be used without complex calibration.  
☐ It can measure lower temperatures than the NTC thermistor.  

### 📝 Solution

Let’s evaluate each option:

- **❌ It is more accurate than the NTC thermistors.**  
  Incorrect. Thermistors can achieve accuracies of ±0.1 °C to ±0.2 °C. Thermocouples typically have ~1% accuracy unless individually calibrated.

- **✅ It can measure higher temperatures than the NTC thermistor.**  
  Correct. Thermocouples can operate well above 800 °C (even over 2000 °C in some cases), whereas thermistors are typically limited to 200 °C.

- **❌ Its curve of temperature vs. voltage is more linear, and can be used without complex calibration.**  
  Incorrect. Thermocouple output is **non-linear**, and lookup tables (e.g., ITS-90) or interpolation are required. 

- **❌ It can measure lower temperatures than the NTC thermistor.**  
  Unclear, but not generally true. Thermistors are often used for low-temperature applications (e.g., down to –50 °C). Some thermocouples can handle cryogenic ranges, but thermistors are more accurate and common at low temperatures.

### 🎯 Answer

✅ It can measure higher temperatures than the NTC thermistor.

## Example Question 3

### ❓ Question

Which of the following are true statements about an NTC thermistor?  
*(Select all that apply)*

☐ The range: -100° to 300°C    
☐ Common base resistances are 20,000 Ω and 100,000 Ω    
☐ It is made of transistors and memory circuits    
☐ It has an excellent accuracy of 0.1 °C – 0.2 °C  
☐ None of the above  

### 📝 Solution

Let’s analyze each option:

  - **❌ The range: -100° to 300°C**  
  Incorrect. Typical NTC thermistor range is around –50 °C to +200 °C. Some may go higher, but 300 °C is beyond normal limits.

  - **❌ Common base resistances are 20,000 Ω and 100,000 Ω**  
  Incorrect. Common base resistances are **2,252 Ω** and **10,000 Ω** .Higher resistances like 30 kΩ or 50 kΩ may be used for extended ranges, but 20 kΩ and 100 kΩ are not standard base resistances.

  - **❌ It is made of transistors and memory circuits**  
  Incorrect. NTC thermistors are made from **sintered metal oxides**, not active semiconductor components like transistors.

  - **✅ It has an excellent accuracy of 0.1 °C – 0.2 °C**  
  Correct. With proper calibration, thermistors can reach high accuracy in their operational range.

  - **❌ None of the Above**  
  Incorrect. One statement **is** true.

### 🎯 Answer

✅ It has an excellent accuracy of 0.1 °C – 0.2 °C

## Example Question 4

### ❓ Question

What is the Steinhart Hart Equation?  
*(Select all that apply)*

☐ A cubic polynomial equation that models the highly nonlinear behavior of thermistors  
☐ A highly nonlinear equation that models the behavior of thermistors    
☐ An equation that compares the thermistor voltage to the RTD voltage  
☐ An equation that compares the thermistor voltage to the thermocouple voltage  
☐ None of the above  

### 📝 Solution

Let’s analyze the options:

  - **❌ A cubic polynomial equation that models the highly nonlinear behavior of thermistors**  
  This is **not** the correct description. While the equation may be rearranged to appear polynomial-like, it is **not** a cubic polynomial in the traditional sense.

  - **✅ A highly nonlinear equation that models the behavior of thermistors**  
  Correct. The Steinhart–Hart equation models the **nonlinear relationship between temperature and resistance** of thermistors using logarithmic terms.

  - **❌ An equation that compares the thermistor voltage to the RTD voltage**  
  Incorrect. The Steinhart–Hart equation is unrelated to RTDs.

  - **❌ An equation that compares the thermistor voltage to the thermocouple voltage**  
  Incorrect. It deals only with thermistors.

  - **❌ None of the above**  
  Incorrect. One option is clearly true

### 🎯 Answer

✅ A highly nonlinear equation that models the behavior of thermistors

## Example Question 5

### ❓ Question

Which fact is **not true** about RTDs?  
*(Select one)*

⚪ They have a temperature coefficient of resistance (TCR) of 3.85 Ω/Ω/°C  
⚪ DIN/IEC 60751 is the global standard for RTDs  
⚪ They have a range of –200 °C to 800 °C  
⚪ The Class A resistance tolerance is smaller than the Class B resistance tolerance  
⚪ They have a nearly linear temperature vs. resistance curve  

### 📝 Solution

Let’s evaluate each statement:

- **❌ They have a TCR of 3.85 Ω/Ω/°C**  
  Not true. The standard **TCR is 0.00385 Ω/Ω/°C**, not 3.85. This value is often expressed as 3850 ppm/°C.

- ✅ DIN/IEC 60751 is indeed the international standard that defines RTD characteristics.

- ✅ RTDs typically operate in the range of –200 °C to 800 °C.

- ✅ Class A has **tighter** (smaller) tolerance than Class B — this is correct.

- ✅ RTDs have a **nearly linear** temperature vs. resistance characteristic, especially compared to thermistors.

### 🎯 Answer

It is **not true** that RTDs have a temperature coefficient of resistance (TCR) of 3.85 Ω/Ω/°C

## Example Question 7

### ❓ Question

What happens if you don’t perform cold junction compensation in a thermocouple circuit?  
*(Select one)*

⚪ The temperature reading will be inaccurate because you have no way to compensate the circuit for thermoelectric voltages created at the junctions of dissimilar metals.  
⚪ The accuracy will be improved because you are doing away with an unnecessary process measurement step  
⚪ Nothing. The reading will be accurate anyway  
⚪ The temperature reading will be inaccurate because the ice bath reference temperature will not be maintained  
⚪ The temperature reading will be inaccurate because the table lookup curve for thermoelectric voltage vs. temperature will be thrown off  

### 📝 Solution

- **✅ The temperature reading will be inaccurate because you have no way to compensate the circuit for thermoelectric voltages created at the junctions of dissimilar metals**. — Correct.
- **❌  The accuracy will be improved because you are doing away with an unnecessary process measurement step** — Incorrect. Thermocouples measure the **difference** in temperature between two junctions, so failing to compensate for the reference (cold) junction leads to incorrect results.
- **❌ Nothing. The reading will be accurate anyway** — Incorrect. Se discussion about accuracy above.
- **❌ Ice bath reference not maintained** — This is historically true, but not relevant if using modern **cold junction compensation (CJC)** methods.
- **❌ Table lookup curve being thrown off** — Not directly correct. The lookup table assumes **known reference junction temperature**, so the inaccuracy is more fundamental than the curve.

### 🎯 Answer

✅ The temperature reading will be inaccurate because you have no way to compensate the circuit for thermoelectric voltages created at the junctions of dissimilar metals.

## Example Question 8

### ❓ Question

Which is the most common thermocouple in use?  
*(Select one)*

⚪ Type J  
⚪ Type T  
⚪ Type E  
⚪ Type N  
⚪ Type K  

### 📝 Solution

- **Type K** is the most widely used thermocouple due to:
  - Its **wide temperature range** (up to ~1250 °C)
  - **Low cost**
  - **Good stability** and **availability**

Other types:
- **Type J** – Iron/Constantan, limited upper range.
- **Type T** – Excellent for very low temperatures.
- **Type E** – Higher voltage output, but less common.
- **Type N** – Better high-temp stability, used in specialized applications.

### 🎯 Answer

✅ Type K

