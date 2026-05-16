# 🖥️ PIC16F877A-Microcontroller-Programming-with-mikroC-Proteus-Simulation


## 📌 Project Title
**Initiation to PIC16F877A Microcontroller Programming using mikroC and Simulation under Proteus**


## 🎯 1. Introduction

This practical work is part of the **Microprocessors and Microcontrollers** module.  
The main objective is to become familiar with:

- 🔹 **PIC16F877A** microcontroller
- 🔹 **mikroC** development environment
- 🔹 **Proteus** electronic circuit simulation

This TP represents the first step in understanding the **complete design chain**:  
`Code Writing → Compilation → .HEX Generation → Simulation`

---

## 📚 2. TP Objectives

- ✅ Master project creation under mikroC
- ✅ Understand configuration of **TRIS**, **PORT**, and **ADCON** registers
- ✅ Control an LED as a digital output
- ✅ Read the state of a push button
- ✅ Simulate a simple circuit in Proteus
- ✅ Program a basic LED chaser (Knight Rider effect)

---

## 🧱 3. Project Structure

The project is divided into four main parts:

### 🔷 Part A – Programming with mikroC
- Created a **Standard Project** in mikroC
- Selected **PIC16F877A** as microcontroller
- Configured clock frequency to **20 MHz**
- Test program to turn ON/OFF an LED connected to **RC0** with a **100ms delay**

<img width="294" height="158" alt="image" src="https://github.com/user-attachments/assets/7d79926e-7004-4a21-ba8b-37e1cb262fb0" />

 

### 🔷 Part B – Simulation with Proteus
- Created a new Proteus project including:
  - PIC16F877A
  - 1 LED
  - Current limiting resistor
- Loaded the `.hex` file (compiled in mikroC) into the microcontroller
- Successfully simulated LED blinking


<img width="196" height="158" alt="image" src="https://github.com/user-attachments/assets/10ad55a2-b553-4bab-8465-a71655e60592" />



### 🔷 Part C – Push Button Reading
- Push button connected to **RA0** with a **pull-down resistor**
- When pressed → RA0 = HIGH (1)
- When released → RA0 = LOW (0)
- Program turns LED ON when button is pressed, OFF otherwise

<img width="296" height="227" alt="image" src="https://github.com/user-attachments/assets/8add3f13-c3e9-4415-a2d1-5f7344d9ce31" />

\n

<img width="301" height="123" alt="image" src="https://github.com/user-attachments/assets/2e4481a1-15ff-460a-87e1-ea3bfa248387" />


### 🔷 Part D – LED Chaser (Knight Rider)

#### 📍 Version 1: Basic Chaser
- Used **8 lines of PORT C** (RC0 to RC7)
- `for` loop generates sequential lighting
- Each LED lights up one after another
- Fixed delay of **150ms** between transitions
- Runs continuously without user interaction

<img width="312" height="383" alt="image" src="https://github.com/user-attachments/assets/41e7257d-357e-42fa-b30e-d5d5834ca28a" />

\n


<img width="286" height="245" alt="image" src="https://github.com/user-attachments/assets/a3a4520a-aa4f-4c93-b67b-79cc30d13344" />

#### 📍 Version 2: Chaser with Start Button
- Added a push button (on **RB0**) to **start/stop** the chaser
- Button read as digital input
- When user presses the button → chaser starts
- When pressed again → chaser stops (toggle functionality)


<img width="304" height="328" alt="image" src="https://github.com/user-attachments/assets/f740ac6e-be7d-4978-9130-8288fdb13ab1" />


\n


<img width="298" height="220" alt="image" src="https://github.com/user-attachments/assets/9b3d389e-6253-40a9-bc39-b833291f64c1" />



## 🧰 4. Components Used

| Component | Reference / Details |
|-----------|---------------------|
| Microcontroller | PIC16F877A |
| IDE | mikroC Pro for PIC |
| Simulator | Proteus ISIS |
| LEDs | 8x (for chaser) |
| Resistors | 220Ω (for LEDs), 10kΩ (pull-down) |
| Push button | Normally open |
| Clock frequency | 20 MHz |



## 🚀 7. How to Run the Project

### 📍 In mikroC:
1. Open the project file (`.mcppi`)
2. Verify the configuration (PIC16F877A, 20 MHz)
3. Compile (F9) to generate the `.hex` file

### 📍 In Proteus:
1. Open the circuit schematic (`.pdsprj`)
2. Double-click the PIC16F877A component
3. Browse and load the generated `.hex` file
4. Click **Play** ▶️ to start simulation

---


## 📚 11. Key Learnings

- 🧠 Understanding of microcontroller registers (TRIS, PORT, ADCON)
- 🧠 Digital I/O configuration and usage
- 🧠 Difference between pull-up and pull-down resistors
- 🧠 Software debouncing (basic implementation)
- 🧠 Complete workflow from code to simulation

---

## ⚖️ 12. License

📚 This project is for **educational purposes only**.
