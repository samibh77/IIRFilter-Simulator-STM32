# STM32 Digital Filter Prototyping

## 📌 Overview
This project demonstrates the implementation of an **IIR digital filter** on an STM32 microcontroller.  
Instead of physically building an analog filter, we prototype and validate its behavior in firmware.  
This approach helps **save time and cost**: you can test a filter’s performance digitally before buying analog components.

## 🎯 Objectives
- Convert an analog filter design into digital form using the **bilinear transform**.
- Compute filter coefficients for a given cutoff frequency.
- Implement the **difference equation** in STM32 firmware.
- Test the filter in real time on microcontroller inputs.

## 🛠️ Features
- Implementation of a **1st-order Low-Pass Filter (LPF)**.
- Real-time update of output based on past inputs and outputs.
- Easily extendable to higher-order or other filter types (HPF, BPF).
- Lightweight and optimized for embedded applications.

## 🚀 Workflow
1. Design the filter in analog domain.
2. Apply the **bilinear transform** to obtain digital coefficients.
3. Implement the difference equation in STM32 firmware.
4. Feed test signals and observe filtered output.

## 📂 Repository Structure

