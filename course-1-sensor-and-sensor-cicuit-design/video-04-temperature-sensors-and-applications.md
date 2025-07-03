# 🧪 Temperature Sensors and Applications

The lecture introduces four major types of thermal sensors, describing their working principles, advantages, limitations, and typical applications.

## 1. Thermocouples

* **Principle**: Two dissimilar metal wires joined at one end. The voltage generated at the junction is proportional to temperature.
* **Range**: Up to **1800 °C**.
* **Applications**: Metal and semiconductor fabrication.
* **Pros**: High temperature range.
* **Cons**: Susceptible to **drift** over time; must be **recalibrated yearly**.

## 2. Resistance Temperature Detectors (RTDs)

* **Principle**: Resistance of metals (typically platinum) increases linearly with temperature.
* **Range**: Up to **800 °C**.
* **Applications**: Pharmaceutical and biotech industries.
* **Pros**:
  * High **accuracy** and **linearity**.
  * Very **stable**, no need for frequent recalibration.
* **Cons**:
  * Requires an **accurate current source**.
  * Limited to **3- or 4-wire** circuits to eliminate lead resistance effects.

## 3. Thermistors

* **Principle**: Semiconductor material with resistance that **decreases sharply** with increasing temperature (NTC type).
* **Range**: Up to **200 °C**.
* **Applications**: Smartphones, computers.
* **Pros**
  * **Accurate** and **stable**.
  * **Compact** and easy to integrate.
* **Cons**:
  * **Highly nonlinear**; requires extensive **firmware compensation**.

## 4. Infrared Sensors

* **Principle**: Measure emitted infrared energy to estimate **surface temperature**.
* **Range**: Very high surface temperatures (non-contact).
* **Applications**: Firefighting, hazardous environments.
* **Pros**:
  * **Non-contact**; safe for distant/hot objects.
* **Cons**:
  * Need accurate **emissivity values**.
  * Must ensure the object is **within the field of view**.
  * Cannot measure **internal temperature**.
  * Typically **not embedded** in systems; used in standalone tools.
---

## 🌟 Key Takeaways

* Choose **thermocouples** for extreme temperatures.
* Use **RTDs** when accuracy and long-term stability are important.
* Pick **thermistors** for compact, low-to-medium temperature needs, but be ready for nonlinear compensation.
* Use **infrared sensors** only when non-contact measurement is required, but they are limited in embedded integration.
