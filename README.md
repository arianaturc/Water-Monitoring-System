# 💧 Water Monitoring System (Arduino)

## 📖 Overview
The **Water Monitoring System** is an **Arduino-based project** designed to measure and monitor key water parameters.  
It provides real-time detection of **water level, water quality, temperature, and clarity** with visual and audio alerts.  

The system is ideal for applications in **water tanks or environmental monitoring**.  

---

## 🚀 Functionalities
- ✔️ **Water Level Detection**  
   Detects water levels and indicates them using LEDs + LCD.  

- ✔️ **Water Quality Assessment (TDS sensor)**  
   Measures **Total Dissolved Solids (TDS)** in water and triggers a **buzzer melody** when dangerous levels are detected.  

- ✔️ **Temperature Monitoring**  
   Reads water temperature in **Celsius and Fahrenheit** and displays it on the LCD.  

- ✔️ **Water Clarity Measurement (Turbidity sensor)**  
   Detects how clear or cloudy the water is and categorizes it as **clean, cloudy, or dirty**.  

---

## 🛠️ Components Used

### 🔹 Water Level
- Water level sensor 
- 3 LEDs (Low, Medium, High indicator)  
- LCD display  

### 🔹 Water Quality
- Analog **TDS sensor** (Total Dissolved Solids)  
- Buzzer for unsafe levels  

### 🔹 Water Temperature
- Temperature sensor 

### 🔹 Water Clarity
- Turbidity sensor 

---

## 📟 Hardware Setup
- Arduino Uno 
- Sensors connected to analog pins:  
  - `A0` → Water level sensor  
  - `A1` → Turbidity sensor  
  - `A2` → TDS sensor  
- Digital pins for LEDs:  
  - `D2` → Low-level LED  
  - `D3` → Medium-level LED  
  - `D4` → High-level LED  
- Digital pin `D8` → Buzzer  
- Digital pin `D9` → Temperature sensor 
- LCD display connected via **I2C module**  

---

## 🖥️ Features in Action
- **LEDs + LCD** indicate water level (Low / Medium / High).  
- **LCD + Serial Monitor** show TDS readings, with categories:  
  - Excellent  
  - Good  
  - Warning ("Are you sure?") with buzzer  
  - Not drinkable  
- **Turbidity sensor** calculates clarity % and classifies water.  
- **Temperature sensor** outputs Celsius + Fahrenheit values.  
