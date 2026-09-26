# Self-Biased Sub-1V Bandgap Reference (BGR)

## Overview
A sub-1V bandgap reference designed with a self-biased amplifier, startup circuit, and low-temperature-coefficient output. Designed using the gm/ID methodology in Cadence Virtuoso.

## Specifications
| Parameter | Specification | Achieved |
|-----------|---------------|----------|
| Output Voltage | 0.8 V | 0.803 V |
| Supply Voltage | 1.2 V | 1.2 V |
| Total Bias Current | < 10 µA | 5.42 µA |
| Phase Margin | > 60° | 63.46° |

## Design Approach
- **Core:** PTAT + CTAT summation (ΔVBE from BJT pair + VBE)
- **Amplifier:** Self-biased amplifier
  - Part 1: Behavioral VCVS
  - Part 2: Actual transistor-level amplifier
- **Startup Circuit:** Ensures BGR does not remain in the zero-current state
- **Passives:** Ideal resistors/capacitors replaced with PDK passives

## Tools
- Cadence Virtuoso
- ADT (Analog Design Tool)

## Key Techniques
- Bandgap reference design (PTAT + CTAT)
- Self-biased amplifier design
- Startup circuit design
- Temperature and process corner analysis
- Sub-1V supply operation

---
*Mini Project 1 of the CMOS Analog IC Design course at the Information Technology Institute (ITI), instructed by Dr. Hesham Omran.*

*Part of the [CMOS Analog IC Design Projects](../) portfolio.*
