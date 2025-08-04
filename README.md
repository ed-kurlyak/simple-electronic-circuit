# 7-Segment Display Counter Circuit

This project demonstrates a simple digital counter using Soviet TTL logic ICs and a single-digit 7-segment display.

![Circuit Diagram](schematic.jpg)

## 💡 Overview
The circuit acts as a manual counter that increments each time a button is pressed. It uses binary counting and BCD-to-7-segment decoding to display numbers from 0 to 9.

## 🧩 Components
- **КМ155ИЕ2** – Binary counter (Soviet TTL, 74192/74190 equivalent)
- **КР514ИД2** – BCD to 7-segment decoder/driver (7447 equivalent)
- **7-Segment Display** – Common anode type
- **Resistors (R1–R7)** – Current limiting resistors for each segment
- **R8** – Debounce or pull-down resistor for the button input
- **S1** – Manual push button (for incrementing the counter)

## ⚙️ Working Principle
1. Pressing **S1** generates a pulse that triggers the **КМ155ИЕ2** counter.
2. The counter outputs a binary number (0–9).
3. This binary number is fed into **КР514ИД2**, which converts it to a 7-segment display signal.
4. Resistors R1–R7 limit current to each display segment, showing the corresponding digit.

## 🔌 Power Supply
- **+U**: +5V typical TTL logic voltage
- **-U**: Ground

## 🧪 Possible Uses
- Educational purposes
- Hardware logic demonstrations
- Button press counter
- Basis for microcontroller-free display systems



