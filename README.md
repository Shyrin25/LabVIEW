# LabVIEW Traffic Light Control

This project demonstrates a *traffic light control system* built using *LabVIEW* and *National Instruments DAQ (Data Acquisition) device*.  
The system controls three LEDs (Red, Yellow, Green) on a breadboard to simulate a standard traffic light sequence.

---

## 🎯 Objective
To simulate a working traffic light using LabVIEW software for control logic and an NI DAQ module to interface with physical LEDs.

---

## 🛠 Hardware Required
- NI DAQ (e.g., NI USB-6001 or similar)
- Breadboard
- Jumper wires (Male–Male)
- Red, Yellow, and Green LEDs
- Resistors (220Ω each)

---

## 💻 Software Required
- *LabVIEW* (any recent version)
- NI-DAQmx driver installed

---

## ⚙ Working Principle
1. LabVIEW controls the output channels of the NI DAQ device.
2. Each output pin is connected to an LED via a resistor.
3. The LabVIEW block diagram contains a sequence structure to turn LEDs on/off in the order:
   - *Green ON* → Delay → OFF  
   - *Yellow ON* → Delay → OFF  
   - *Red ON* → Delay → OFF
4. The sequence repeats to mimic real-world traffic light operation.

---

## 🔌 Circuit Connections
| NI DAQ Pin | LED Color | Resistor Value |
|------------|-----------|----------------|
| P0.0       | Green     | 220Ω           |
| P0.1       | Yellow    | 220Ω           |
| P0.2       | Red       | 220Ω           |
| GND        | Common Ground | —         |

---

## 📄 LabVIEW VI Description
- *Front Panel:* Contains three indicators representing the LEDs.
- *Block Diagram:* Uses a flat sequence structure with timed delays to control each LED.
- Digital Output nodes send HIGH (5V) or LOW (0V) signals to the NI DAQ pins.

---

## ▶ How to Run
1. Connect the LEDs to the NI DAQ pins as per the circuit table.
2. Open the .vi LabVIEW file.
3. Run the VI and observe the LEDs switching in the traffic light pattern.

---

## 📌 Future Improvements
- Add pedestrian crossing control.
- Add real-time control via sensors.
- Simulate using timers instead of fixed delays.

---

## 📜 License
This project is open-source under the MIT License.  
Feel free to modify and share.

---
