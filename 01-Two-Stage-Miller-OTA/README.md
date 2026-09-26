# Two-Stage Miller-Compensated OTA

## Overview
A two-stage Miller-compensated OTA designed using the gm/ID methodology in Cadence Virtuoso.

## Specifications
| Parameter | Specification | Achieved |
|-----------|---------------|----------|
| DC Gain | ≥ 66 dB | 73.84 dB |
| CMRR | ≥ 74 dB | 87.5 dB |
| Phase Margin | ≥ 70° | 73.19° |
| GBW | ≥ 5 MHz | 6.6 MHz |
| Slew Rate | ≥ 5 V/µs | 5.091 V/µs |
| Rise Time | ≤ 70 ns | 33.55 ns |
| Current | ≤ 60 µA | 60 µA |

## Design Approach
- **First Stage:** 5T OTA with PMOS input pair and PMOS current mirror load
- **Second Stage:** Common-source amplifier (M8) with PMOS current source load (M7)
- **Compensation:** Miller capacitor (CC = 1.8 pF) with nulling resistor (M9) for RHP zero cancellation

## Tools
- Cadence Virtuoso
- ADT (Analog Design Tool)

## Key Techniques
- gm/ID methodology for systematic transistor sizing
- Miller compensation
- RHP zero cancellation using nulling resistor
- Two-stage amplifier design

---

*Mini Project 1 of the CMOS Analog IC Design course at the Information Technology Institute (ITI), instructed by Dr. Hesham Omran.*
*Part of the [CMOS Analog IC Design Projects](../) portfolio.*

