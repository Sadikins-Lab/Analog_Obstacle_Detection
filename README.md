# Op-Amp Based IR Obstacle Detection Sensor

A basic **analog obstacle detection sensor** built using an **operational amplifier (op-amp)** as a comparator.  
The circuit uses an **IR transmitter** and **IR receiver** to detect nearby obstacles by comparing the received signal voltage with a reference voltage set using a **potentiometer**.

This project demonstrates the fundamentals of **op-amp voltage comparison**, **IR sensing**, and **analog electronics**.

---

## 🔧 Components Used

- Operational Amplifier (LM358)
- IR Transmitter (IR LED)
- IR Receiver (Photodiode)
- Potentiometer (10kΩ)
- Resistors (220Ω, 10kΩ)
- LED (for indication)
- Power Supply (5V–12V DC)
- Breadboard / PCB
- Connecting wires

---

## 🧠 Operational Amplifier (Op-Amp) Overview

An **operational amplifier (op-amp)** is a high-gain electronic amplifier used to amplify and process analog signals.  
It has **two inputs** and **one output**:

- **Non-inverting input (+)**  
- **Inverting input (−)**  
- **Output**

An op-amp amplifies the **difference between the two input voltages**.  
Due to its very high gain, even a small voltage difference causes a significant change at the output.

### Reference Diagram
<img width="1036" height="667" alt="image" src="https://github.com/user-attachments/assets/2ed3f26d-3b7c-4db7-ae27-bc53f81ff500" />



### Key Characteristics of an Op-Amp
- Very high voltage gain
- High input impedance
- Low output impedance
- Widely used in:
  - Comparators
  - Amplifiers
  - Filters
  - Signal conditioning circuits

---

## ⚙️ How the Op-Amp Works in This Project

In this obstacle detection system, the op-amp is configured in **comparator mode**.

- The **non-inverting input (+)** is connected to the **IR receiver output**, which generates a voltage based on reflected infrared light.
- The **inverting input (−)** is connected to a **reference voltage** set using a potentiometer.

### Operation:
- When **no obstacle** is present:
  - The IR receiver voltage is **lower** than the reference voltage
  - The op-amp output remains **LOW**
  - The output LED stays **OFF**

- When an **obstacle is detected**:
  - Reflected IR light increases the sensor voltage
  - Sensor voltage becomes **greater than the reference voltage**
  - The op-amp output switches **HIGH**
  - The LED turns **ON**, indicating obstacle detection

The potentiometer allows **adjustment of the reference voltage**, enabling control over the sensor’s **sensitivity and detection range**.

Because of the op-amp’s **high gain**, the output transition is sharp and reliable, making it suitable for basic analog comparison applications.

---

## ⚙️ Working Principle

1. The **IR LED** continuously emits infrared light.
2. When an obstacle is placed in front of the sensor:
   - IR light reflects back and is received by the **IR receiver**.
3. The IR receiver produces a voltage proportional to the reflected IR light.
4. The **op-amp is configured as a comparator**:
   - One input receives the IR sensor voltage.
   - The other input receives a **reference voltage** set by the potentiometer.
5. When the sensor voltage exceeds the reference voltage:
   - The op-amp output goes **HIGH**
   - The output LED turns ON, indicating obstacle detection.

---

## 🔁 Circuit Diagram

<img width="1210" height="805" alt="Screenshot 2026-01-14 220053" src="https://github.com/user-attachments/assets/d180448c-9dea-4035-a8f6-8ea826f64038" />



---

## 🎛️ Sensitivity Adjustment

- The **potentiometer** allows adjustment of the reference voltage.
- This controls:
  - Detection range
  - Sensitivity to reflected IR light
- Turning the potentiometer clockwise increases sensitivity (depending on wiring).

---

## 📸 Project Images

![IMG_20260111_093348_426](https://github.com/user-attachments/assets/f9ec8714-0d09-4658-a7cf-9cfdfb7efb33)


- Breadboard setup
- Final assembled circuit
- Output LED ON/OFF states

---

## 🧪 Applications

- Obstacle detection systems
- Line-following robots
- Proximity sensing
- Basic robotics projects
- Analog electronics learning

---

## 📚 Concepts Covered

- Operational amplifier as comparator
- Infrared sensing
- Voltage comparison
- Analog signal processing
- Potentiometer-based reference control

---

## 🚀 Future Improvements

- Add hysteresis using a feedback resistor (Schmitt trigger)
- Replace op-amp with comparator IC (LM393)
- Interface with a microcontroller
- Improve detection range and noise immunity

---

## 👤 Author


**Mohammad Sadikin Naser Araf**  
GitHub: [https://github.com/Araf773](https://github.com/Araf773)

---

