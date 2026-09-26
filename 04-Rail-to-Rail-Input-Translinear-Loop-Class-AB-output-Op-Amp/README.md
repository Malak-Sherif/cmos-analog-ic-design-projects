# Rail-to-Rail Input Translinear-Loop Class-AB Output Op-Amp

## Overview
A rail-to-rail input op-amp with a Monticelli translinear-loop Class-AB output stage, designed in Cadence Virtuoso.

## Specifications
| Parameter | Specification | Achieved |
|-----------|---------------|----------|
| Peak Output Current | 3 mA | 3.1 mA |
| Quiescent Current | 180 µA | 180 µA |
| Supply Voltage | 2.5 V | 2.5 V |
| Phase Margin | > 60° | 65° |
| Input CM Range | Rail-to-Rail | 0 to 2.5 V |

## Design Approach
- **Input Stage:** Complementary NMOS and PMOS differential pairs for rail-to-rail input
- **Folded Cascode Stage:** For high gain
- **Output Stage:** Monticelli translinear-loop Class-AB biasing with 3 mA peak output
- **Bias Circuitry:** Practical transistor-level current sources

## Testbenches
- **TB1:** Unity-gain buffer (β = 1) — worst case for PM
- **TB2:** Non-inverting (G = +2, β = 0.5)
- **TB3:** Inverting (G = −1)

## Tools
- Cadence Virtuoso

## Key Techniques
- Rail-to-rail input stage design
- Monticelli translinear-loop Class-AB biasing
- High-current output stage design
- Quiescent current control (180 µA)
- Peak output current delivery (3 mA)
- Unity-gain buffer, non-inverting, and inverting testbenches

---
*Design Challenge 2 of the CMOS Analog IC Design course at the Information Technology Institute (ITI), instructed by Dr. Hesham Omran.*

*Part of the [CMOS Analog IC Design Projects](../) portfolio.*
