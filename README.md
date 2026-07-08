# Assignment 2: Beeping Countdown Timer
**Course:** Programming C++ for Engineers Using Arduino  
**Institution:** Ghana Communication Technology University

---

## Project Overview
This project implements a synchronized countdown timer utilizing an Arduino Uno. The system drives a single-digit 7-segment display to count down sequentially from 9 to 0. Each numerical step is synchronized with a brief, audible "tick" from a passive buzzer. Once the countdown hits zero, the system emits a sustained tone to clearly signal completion.

---

## Hardware Requirements
* **Microcontroller:** Arduino Uno
* **Display:** 1x Single-digit 7-segment display (Common Cathode)
* **Audio:** 1x Passive piezo buzzer
* **Current Limiting:** 1x 220 ohm resistor (allocated to the COM pin)
* **Prototyping:** Breadboard and premium jumper wires

---

## Core Concepts Demonstrated
* **Frequency Control:** Utilizing the `tone()` and `noTone()` functions for dynamic audio generation.
* **Hardware Architecture:** Identifying the operational distinctions between passive and active buzzers, alongside common cathode configurations.
* **Data Structures:** Designing a 2D array lookup table to map binary states directly to visual digit patterns.
* **Modular Programming:** Implementing parameterized functions to isolate and handle display logic independently.
* **Control Flow:** Managing execution using finite `while` loops, conditional logic, and initialization `for` loops.
* **System Diagnostics:** Outputting real-time status tracking via the Serial Monitor.

---

## Step-by-Step Installation & Deployment

### 1. Hardware Wiring
* Connect the positive terminal of the **buzzer** to Arduino **Pin 8**.
* Route the **7-segment display segment pins (a–g)** directly to Arduino **Pins 2, 3, 4, 5, 6, 7, and 9**.
* Connect the display’s **COM pin** to the Arduino **GND** rail through the **220 ohm resistor**.

### 2. Software Execution
* Launch the Arduino IDE and open the project's `.ino` file.
* Navigate to **Tools > Board** and verify that **Arduino Uno** is selected.
* Go to **Tools > Port** and select the active port associated with your microcontroller.
* Click the **Upload** button to flash the program.
* Open the **Serial Monitor** (set to 9600 baud) to observe the live numeric tracking logs.

---

## Author Info
* **Student Name:** Judah Ekow Affadu-Mensah
* **Index Number:** 2526402221
