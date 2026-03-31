
# 🚦 UltraSmart Traffic Camera ML (Verilog FPGA Project)

An AI-inspired smart traffic light controller implemented in Verilog that dynamically adjusts signal timing using camera input and priority-based decision logic. Designed for FPGA-based intelligent traffic systems.

---

## 📌 Overview

This project presents an adaptive traffic control system that replaces fixed-timing signals with a real-time decision engine. It analyzes vehicle density, congestion trends, pedestrian requests, and emergency signals to optimize traffic flow efficiently.

---

## 🧠 Key Features

* Camera-based vehicle density estimation (OV7670 interface)
* Priority-based traffic control (ML-inspired weighted model)
* Congestion prediction using gradient analysis
* Emergency vehicle override (highest priority handling)
* Pedestrian request integration
* Starvation prevention for fair lane access
* Adaptive signal timing (dynamic green duration)
* Night mode operation (blinking/yellow mode)

---

## ⚙️ Working Principle

The system captures pixel data from a camera and estimates vehicle density using brightness thresholding. Traffic congestion and trends are analyzed, and a weighted priority score is calculated for each lane:

**Priority = Vehicle + Pedestrian + Congestion + Starvation + Trend + Emergency**

The lane with the highest priority is selected, and traffic lights are controlled using a finite state machine (GREEN → YELLOW → REDALL) with adaptive timing.

---

## 🏗️ Architecture

Camera Input → Processing → Density Estimation →
Congestion Analysis → Priority Engine →
Lane Selection → Traffic Light FSM

---

## 🧪 Technologies

* Verilog HDL
* FPGA Design
* Digital System Design
* Basic Image Processing
* Heuristic ML Model

---

## ⚠️ Limitations

* Uses simple pixel thresholding (no real object detection)
* No lane-wise image segmentation
* Fixed weights (non-trainable model)

---

## 🚀 Future Scope

* CNN-based vehicle detection accelerator
* Lane-wise segmentation
* Adaptive/learning-based weights
* FPGA pipelined optimization
* Smart city integration (IoT)

---

## 👨‍💻 Author

**Benudhar Saikia**
B.Tech (ECE) | Interested in VLSI & Semiconductor Design

---

## ⭐

If you find this project useful, give it a star on GitHub!
