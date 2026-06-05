# Two-Stage Miller-Compensated Operational Transconductance Amplifier (OTA)

## Overview

This project presents the design and simulation of a two-stage Miller-compensated Operational Transconductance Amplifier (OTA) implemented using a 180 nm CMOS process in LTspice.

The design employs an NMOS differential input stage with an active current mirror load, followed by a PMOS common-source gain stage. Frequency compensation is achieved using Miller compensation with a nulling resistor to ensure stable operation while driving capacitive loads.

## Design Objectives

* DC Gain ≥ 60 dB
* Gain-Bandwidth Product (GBW) ≈ 5 MHz
* Phase Margin ≥ 60°
* Slew Rate ≥ 10 V/µs
* Load Capacitance = 10 pF
* Supply Voltage = 1.8 V
* Low-Power Operation

## Architecture

### First Stage

* NMOS differential input pair
* PMOS current mirror active load
* Tail current source biasing

### Second Stage

* PMOS common-source amplifier
* Provides additional voltage gain and output swing

### Compensation Network

* Miller compensation capacitor
* Nulling resistor for pole-zero cancellation
* Improved stability under capacitive loading

## Design Methodology

1. Derived transistor dimensions from gain, GBW, slew rate, and ICMR requirements.
2. Sized differential pair and current mirrors to satisfy transconductance targets.
3. Designed the second gain stage for enhanced voltage gain.
4. Added Miller compensation and optimized the nulling resistor.
5. Validated performance through DC, AC, and transient simulations in LTspice.

## Simulation Results

| Parameter              | Achieved Value |
| ---------------------- | -------------- |
| Supply Voltage         | 1.8 V          |
| Open-Loop Gain         | ~70 dB         |
| Gain Bandwidth Product | ~4.8 MHz       |
| Phase Margin           | ~63.7°         |
| Load Capacitance       | 10 pF          |
| Power Consumption      | ~500 µW        |

## Tools Used

* LTspice
* CMOS 180 nm Technology Models
* Analog IC Design Principles
* Small-Signal Analysis

## Key Learnings

* CMOS analog amplifier design
* Differential amplifier design
* Frequency compensation techniques
* Stability and phase margin optimization
* Transistor sizing and biasing
* AC and transient simulation analysis

## Repository Contents

```text
├── OTA_Schematic.asc
├── Design_Report.pdf
├── AC_Response.png
├── Transient_Response.png
└── README.md
```

## Author

Charvit Rajani
B.Tech Electronics and Communication Engineering
Indian Institute of Technology Guwahati
