# Fully Differential Folded-Cascode OTA

## Overview
A fully differential folded-cascode OTA with capacitive feedback, designed using the gm/ID methodology in Cadence Virtuoso. Includes both behavioral and transistor-level CMFB.

## Specifications
| Parameter | Specification | Achieved |
|-----------|---------------|----------|
| Supply Voltage | 2.5 V | 2.5 V |
| Closed Loop Gain | 2 V/V | 1.998 V/V |
| Phase Margin (Diff) | ≥ 70° | 87.5° |
| Phase Margin (CM) | - | 65.66° |
| CMIR Low | ≤ 0 V | -0.15 V |
| CMIR High | ≥ 1 V | 1.06 V |
| Output Swing | ≥ 1.2 Vpk-pk | 1.4 Vpk-pk |
| DC Loop Gain | ≥ 60 dB | 61.96 dB |
| Settling Time (1%) | ≤ 100 ns | 98.63 ns |

## Design Approach
- **Input Stage:** PMOS differential pair (folded)
- **Cascode Stage:** NMOS and PMOS cascode devices
- **Load:** PMOS current source loads
- **CMFB:** Behavioral CMFB (verified), then actual transistor-level CMFB
- **Feedback:** Capacitive divider (CIN = 2 pF, CF = 1 pF, β = 1/3)

## Tools
- Cadence Virtuoso
- ADT (Analog Design Tool)

## Key Techniques
- Folded cascode topology for high gain
- Common-mode feedback (CMFB) design
- STB analysis for loop stability
- Capacitive feedback network
- Output swing optimization

---
*Mini Project 2 of the CMOS Analog IC Design course at the Information Technology Institute (ITI), instructed by Dr. Hesham Omran.*

*Part of the [CMOS Analog IC Design Projects](../) portfolio.*
