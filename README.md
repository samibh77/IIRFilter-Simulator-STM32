# STM32 Digital Filter Prototyping

## 📌 Overview
This project focuses on the **implementation of an Infinite Impulse Response (IIR) digital filter** on an STM32 microcontroller.  
The main goal is to create a low-cost and flexible environment for **digital prototyping of analog filters** directly on embedded hardware.  

The workflow begins with the design of an analog prototype filter. The design is then transformed into its discrete-time equivalent using the **bilinear transform (Tustin’s method)**, which preserves the frequency response characteristics by mapping the analog s-plane into the digital z-plane.  

Once the filter’s digital transfer function is obtained, the corresponding **difference equation** is derived and implemented in firmware. The STM32 executes this recursive equation in real time, updating the output sample `y[n]` using both present and past input values `x[n]`, as well as past outputs.  

This approach enables embedded developers and researchers to:
- Validate the filter’s performance in real-time applications.
- Analyze stability, transient response, and steady-state characteristics.
- Rapidly iterate between different filter designs without the need for physical RC or op-amp based circuits.  

Ultimately, this method provides a **practical and cost-effective testbench** for evaluating analog filter behavior in the digital domain before committing to hardware implementation.


## 🎯 Objectives
- Convert an analog filter design into digital form using the **bilinear transform**.
- Compute filter coefficients for a given cutoff frequency.
- Implement the **recursive equation** in STM32 firmware.
- Test the filter in real time on microcontroller inputs.

## 🛠️ Features
- Implementation of a **1st-order Low-Pass Filter (LPF)**.
- Real-time update of output based on past inputs and outputs.
- Easily extendable to higher-order or other filter types (HPF, BPF).
- Lightweight and optimized for embedded applications.

## 📖 Detailed Documentation
The complete mathematical derivations, STM32CubeIDE setup, and CubeMonitor test results  
are provided in the documentation: 
[IIRF.pdf](https://github.com/user-attachments/files/21950361/IIRF.pdf)


