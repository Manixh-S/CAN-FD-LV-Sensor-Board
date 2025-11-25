# LV Sensor Board  
### Precision Low-Voltage Acquisition & CAN FD Telemetry Module for FSAE

---

## 🚀 Overview  

The **LV Sensor Board** is a custom-designed, high-precision mixed-signal data acquisition module built for the FSAE E.  
It measures **unipolar (0–5V)** and **bipolar (−18 to 18V)** low-voltage signals across *eight independent channels* and transmits real-time telemetry over **CAN FD** to the car’s main ECU.

---

## 🔍 Core Features  

### 🧩 **Signal Acquisition**
- **8 total LV channels**
  - 4× **0–5V** channels via *MCP3204* (Microchip)
  - 4× **−18 to 18V** channels via *ADS114S06* (Texas Instruments)
- Precision voltage dividers + negative rail generation for safe bipolar sensing  
- Input isolation & screw-terminal connectors for robust field wiring  

### ⚙️ **Processing & Control**
- **TI MSPM0C1104** (ARM Cortex-M0+) for fast embedded control  
- Dual-SPI architecture for independent ADC + CAN FD communication  
- Full USB-UART programming capability via onboard converter  
- **XDS110-compatible debug testpoints** for hardware breakpoints & flash programming  

### 📡 **Telemetry**
- External **CAN FD controller** + high-speed CAN transceiver  
- SPI-based CAN command interface  
- Designed for low-latency EV telemetry streaming  

### 🔌 **Power Architecture**
- Powered from the vehicle’s **12V LV rail**  
- Multi-stage regulation:
  - 5V LDO  
  - 3.3V LDO  
  - 2.5V LDO  
- Additional **5V auxiliary output** for external sensors  

---


