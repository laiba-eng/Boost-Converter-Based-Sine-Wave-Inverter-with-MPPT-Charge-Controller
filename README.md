# Boost-Converter-Based-Sine-Wave-Inverter-with-MPPT-Charge-Controller
A compact, high-efficiency solar power system that converts 12V DC to 240V AC using a custom-designed boost converter, SPWM-based H-bridge inverter, and MPPT algorithm for optimal energy extraction.
# Key Features
Boost Converter (12V DC → 240V DC)

SPWM-based Inverter (Pure Sine Wave Output)

MPPT using Incremental Conductance Algorithm

PCB-based modular design

Controlled via Arduino (50kHz switching)
# Architecture Overview
The system consists of three main power stages integrated through custom PCBs and controlled by an Arduino microcontroller:
-MPPT Buck Converter: Extracts maximum power from a variable 12V solar input using the Incremental Conductance algorithm.

-Boost Converter: Steps up the buck converter output to 233V DC using a 10μH inductor and high-frequency PWM (50kHz) controlled by Arduino.

-SPWM Inverter: Converts 233V DC to 220V AC sine wave using a 4-leg H-bridge configuration with 16 IRFP250N MOSFETs, driven by IR2101 gate drivers and Arduino-generated SPWM signals.

The coordination between these stages ensures efficient, stable, and clean power output suitable for sensitive AC loads.

# Performance Highlights
Boost Output: 240V from 12V input

Inverter Output: 220V AC (low THD)

Efficiency: >85%

Load Support: Up to 100W

Modular PCBs with JST headers

# Simulations & Hardware
<img width="1047" height="403" alt="image" src="https://github.com/user-attachments/assets/ecfd8235-9e62-4776-b842-4ffc3613f2d4" />
Boost Converter Simulation

<img width="800" height="320" alt="image" src="https://github.com/user-attachments/assets/47041aea-b367-4fbc-9542-4909bb99235c" />
Boost Converter PCB

<img width="593" height="334" alt="image" src="https://github.com/user-attachments/assets/edc9c60a-c620-41fc-961c-03eb4cbce569" />
Boost Converter Hardware


