# Fuel Cell Monitoring System

A real-time monitoring solution for a 500W PEM fuel cell, designed using **ESP32-S3** microcontroller and a **custom PCB** created in **KiCad**. The system provides accurate voltage, current, and temperature measurements with SPI-based data acquisition.

---

## 📌 Features
- **Custom PCB Design** for reliable analog front-end and minimal noise interference.
- **High-Precision Signal Conditioning** using operational amplifiers.
- **Real-Time Data Logging** via SPI communication.
- **Scalable Firmware** developed in C using **PlatformIO** for ESP32-S3.
- **Low Power Consumption** optimization for energy-efficient operation.

---

## 🛠 Tech Stack
- **Microcontroller:** ESP32-S3
- **Hardware Design:** KiCad (Schematics & PCB Layout)
- **Programming Languages:** C, Embedded C
- **Communication Protocols:** SPI, UART
- **Tools:** PlatformIO, VS Code

---

## 🔍 System Overview
The system continuously monitors:
- **Voltage**
- **Current**
- **Temperature**

The measurements are processed through an **analog signal conditioning circuit** and transmitted to the ESP32-S3 for further logging and analysis.

---

## 📂 Project Structure
fuel-cell-monitoring-system/
│
├──> hardware/
│   ──> ProjectSeminar_2025.kicad_pcb        # PCB layout
│   ── Projec>Seminar_2025.kicad_sch        # Main schematic
│   ──> Voltage measurement.kicad_sch        # Voltage sensing circuit
│   ──> current_measurement.kicad_sch        # Current sensing circuit
│
├──> firmware/
│   ──> platformio.ini                       # PlatformIO configuration
│   ──> src/
│      ──> DAQ.c                            # Data acquisition firmware
│
├──> docs/
│   ──> pcb_preview.png                      # PCB design image
│
└──> README.md

✅ Results

Achieved <2% error margin in voltage and current measurements.

Reduced signal noise using precision op-amp-based conditioning circuits.

Successfully implemented low-power, real-time monitoring for a 500W PEM fuel cell.
