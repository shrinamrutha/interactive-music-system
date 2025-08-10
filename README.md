# Interactive Music System – Embedded

[![C/C++](https://img.shields.io/badge/Language-C%2FC++-blue.svg)](https://isocpp.org/)
[![Microcontroller](https://img.shields.io/badge/Hardware-Microcontroller-green.svg)](https://en.wikipedia.org/wiki/Microcontroller)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Real-Time](https://img.shields.io/badge/Real--Time-Yes-brightgreen)](#features)

---

## 📌 Overview

The **Interactive Music System – Embedded** is a **real-time, microcontroller-based music creation and playback system**.
It enables users to **compose, record, and play music interactively** using hardware buttons, sensors, and digital audio synthesis techniques.
The design focuses on **low-latency, portability, and user-friendly operation**, making it suitable for hobbyists, music enthusiasts, and embedded system learners.

---

## ✨ Features

* 🎵 **Real-time audio synthesis** using PWM/DAC.
* 🎛 **Interactive control** via buttons, potentiometers, or touch inputs.
* 🎼 **Pre-programmed melodies** with composition and playback modes.
* 💾 **EEPROM/SD storage** for saving custom compositions.
* 🔋 **Low-power consumption** for portable use.

---

## 🏗 System Block Diagram

```
 ┌──────────────────┐
 │   User Inputs     │
 │  (Buttons, Pots,  │
 │   Touch Sensors)  │
 └─────────┬────────┘
           │
 ┌─────────▼────────┐
 │ Microcontroller   │
 │  - Input Handling │
 │  - Mode Control   │
 │  - Tone Synthesis │
 │  - DSP Processing │
 └─────────┬────────┘
           │
 ┌─────────▼────────┐
 │ Audio Output      │
 │ (Speaker / Jack)  │
 └──────────────────┘
           │
   ┌───────▼────────┐
   │ Storage Module │
   │ (EEPROM / SD)  │
   └────────────────┘
```

---

## 🛠 Technologies Used

### **Hardware**

* Microcontroller: **Arduino Uno / STM32**
* Audio Output: **Speaker or headphone jack**
* Input: **Push buttons, potentiometers, capacitive touch sensors**
* Storage: **EEPROM or SD card**
* Power: **Battery or USB**

### **Software**

* Embedded C / C++
* Arduino IDE / STM32CubeIDE
* DSP techniques for tone generation
* Timer interrupts for precise playback
* State machine for mode management

---

## 📂 Functional Modules

1. **Initialization** – Hardware setup for I/O, timers, and sound output.
2. **Input Processing** – Reads user actions in real-time.
3. **Tone Generation** – Produces notes using PWM or DAC.
4. **Mode Selection** – Switch between Play, Compose, and Record.
5. **Data Storage** – Saves compositions for later playback.
6. **Output** – Sends generated tones to audio hardware.

---

## 📊 Performance

| Parameter        | Description                |
| ---------------- | -------------------------- |
| Latency          | <10 ms (near real-time)    |
| Power Efficiency | Optimized for portable use |
| Scalability      | Supports MIDI integration  |

---

## 🚀 Installation & Usage

### **Setup**

```bash
# Clone the repository
git clone https://github.com/<your-username>/interactive-music-system.git
cd interactive-music-system
```

1. Connect hardware as per wiring diagram.
2. Open the code in Arduino IDE or STM32CubeIDE.
3. Install necessary libraries.
4. Upload to the microcontroller.

### **Operation**

* **Mode 1 – Play**: Plays built-in melodies.
* **Mode 2 – Compose**: Create custom sequences.
* **Mode 3 – Record & Playback**: Save and replay your music.

---

## 📄 Requirements

```
Arduino IDE / STM32CubeIDE
C / C++ Compiler
tone() or custom PWM/DAC libraries
EEPROM or SD library
```

---

## 📚 References

* Embedded Music Systems – Academic & Hobbyist Resources
* DSP for Embedded Devices – Technical References
* Arduino & STM32 Official Documentation

---

