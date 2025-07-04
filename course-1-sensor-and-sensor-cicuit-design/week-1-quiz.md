# Sensor and Sensor Circuit Design: Quiz Week 1

## Question 1

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

###❓ Question

What advantage does a thermocouple have over the NTC thermistor?  
(Select all that apply)

☑ It can measure higher temperatures than the NTC thermistor.  
☑ Its curve of temperature vs. voltage is more linear, and can be used without complex calibration.  
☐ It can measure lower temperatures than the NTC thermistor  
☐ It is more accurate than the NTC thermistors.

###📝 Solution

Let’s evaluate each statement:

-	✅ It can measure higher temperatures than the NTC thermistor  
Correct. Thermocouples (e.g., Type C) can measure up to 2300 °C, far beyond the range of typical NTC thermistors (up to ~200 °C).
-	✅ Its curve of temperature vs. voltage is more linear, and can be used without complex calibration  
Considered correct in quiz context. Thermocouples are less nonlinear than NTC thermistors and can be approximated as linear over small spans, requiring less complex calibration.
-	❌ It can measure lower temperatures than the NTC thermistor  
Incorrect. While some thermocouples (e.g., Type T) operate at cryogenic temperatures, NTCs also perform well at low temps. The "advantage" is ambiguous and likely not correct per quiz intent.
-	❌ It is more accurate than the NTC thermistors  
Incorrect. NTC thermistors can achieve high accuracy (±0.1 °C to ±0.2 °C). Thermocouples are typically accurate to about ±1% of reading and require periodic recalibration.

## 🎯 Answer

✅ It can measure higher temperatures than the NTC thermistor.  
✅ Its curve of temperature vs. voltage is more linear, and can be used without complex calibration.  

## Question 3

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

## Question 4

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

## Question 5

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

## Question 6

### ❓ Question

Suppose we include the lead resistance in the calculation of temperature for an RTD.  
If:  
- R₃ = 5000 Ω  
- Rₐ = 50 Ω  
- V₀ = 3 V  
- V = 6.5 V  

What is R?  
(Type in a one-decimal number.)

### 📝 Solution

We use the formula derived in the lecture slides:

    R = (R₃ + Rₐ) × (1 / (V₀ / V + 1/2) - 1) - Rₐ

Step-by-step:

1. V₀ / V = 3 / 6.5 ≈ 0.4615  
2. Add 0.5: 0.4615 + 0.5 = 0.9615  
3. Take the reciprocal: 1 / 0.9615 ≈ 1.04  
4. Subtract 1: 1.04 - 1 = 0.04  
5. Multiply by (R₃ + Rₐ): 0.04 × (5000 + 50) = 0.04 × 5050 = 202  
6. Subtract Rₐ: 202 - 50 = **152 Ω**

### 🎯 Answer

152.0 Ω

## Question 7

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

## Question 8

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

## Question 9

### ❓ Question

In what temperature measurement applications are thermocouples used?  
*(Select all that apply)*

☐ When it is acceptable to do periodic calibration checks  
☐ When accuracy of worse than 1% is acceptable  
☐ Measuring temperatures above 1400 °C  
☐ Where a large number of measurement points are needed, and you need to keep the total cost of the sensors down  
☐ None of the above  

### 📝 Solution

Let’s examine each option:

- **✅ When it is acceptable to do periodic calibration checks**  
  Correct — thermocouples tend to drift over time and often require recalibration.

- **✅ When accuracy of worse than 1% is acceptable**  
  Correct — typical thermocouple accuracy is around 1% of the reading.

- **✅ Measuring temperatures above 1400 °C**  
  Correct — some thermocouples (e.g., Type C) can measure up to ~2300 °C.

- **✅ Where a large number of measurement points are needed, and you need to keep the total cost of the sensors down**  
  Correct — thermocouples are inexpensive, making them ideal for high-channel-count applications.

- **❌ None of the above**  
  Incorrect — thermocouples are widely used in several relevant applications.

### 🎯 Answer

- ✅ When it is acceptable to do periodic calibration checks  
- ✅ When accuracy of worse than 1% is acceptable  
- ✅ Measuring temperatures above 1400 °C  
- ✅ Where a large number of measurement points are needed, and you need to keep the total cost of the sensors down  

## Question 10

### ❓ Question

You are using a 2252 Ω thermistor, β = 3940, and you measure a resistance of 672.5 Ω.  
What is the temperature in °C that you are measuring?  
*(Type in a one-decimal number for your answer)*

### 📝 Solution

We use the **Beta parameter equation**:

    1/T = 1/T₀ + (1/β) * ln(R/R₀)

Where:  
- `T` = temperature in Kelvin  
- `T₀` = 298.15 K (25 °C)  
- `R` = 672.5 Ω  
- `R₀` = 2252 Ω  
- `β` = 3940

**Step-by-step:**

1. Compute the ratio:
    
       R / R₀ = 672.5 / 2252 ≈ 0.2986

2. Take the natural log:

       ln(R / R₀) ≈ ln(0.2986) ≈ –1.208

3. Plug into the equation:

       1/T = 1/298.15 + (1/3940) * (–1.208)
           ≈ 0.003354 + (–0.0003065)
           ≈ 0.0030475

4. Invert to find temperature:

       T ≈ 1 / 0.0030475 ≈ 328.1 K

5. Convert to °C:

       T(°C) = 328.1 – 273.15 ≈ **55 °C**

### 🎯 Answer

55 °C

