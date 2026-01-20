# CMOS-AFE-Pulse-Oximeter
Low-noise, low-power CMOS analog front-end for biomedical optical sensing, featuring a regulated-cascode TIA and full signal-chain simulation in Cadence Virtuoso.

## Overview
This project presents the design and simulation of a low-noise, low-power CMOS analog front-end (AFE) for biomedical optical sensing applications such as pulse oximetry. The AFE interfaces directly with a photodiode and operates under low-voltage (≈1 V) constraints.

The design was implemented and simulated in Cadence Virtuoso using a semiconductor CMOS process.

---

## Architecture
The complete signal chain includes:
- Regulated-cascode Transimpedance Amplifier (TIA)
- Post-amplification stage
- 50 Ω output buffer

The architecture was optimized for low photodiode current operation while maintaining high bandwidth and low noise.

Block-level architecture:
- Photodiode interface → Regulated-cascode TIA → Post Amplifier → Output Buffer

(See `/schematics` for exported topology diagrams.)

---

## Key Design Goals
- Low input-referred noise for weak optical signals
- Low power operation under ~1 V supply
- High transimpedance gain
- Wide bandwidth to support fast photodiode response

---

## Simulation Results
| Metric | Achieved Performance |
|------|----------------------|
| Transimpedance Gain | ~36 dBΩ |
| Bandwidth | Multi-GHz |
| Input-Referred Noise | Sub-nV/√Hz |
| Supply Voltage | ~1 V |

Validation was performed using:
- AC analysis
- Noise analysis
- Transient simulations

Simulation plots are available in `/simulations`.

---

## Tools & Methods
- Cadence Virtuoso (schematic & simulation)
- AC / Noise / Transient analyses
- Analog biasing and stability optimization
- Low-voltage analog design techniques

---

## Notes
Due to licensing restrictions, proprietary PDKs and Cadence design files are not included. This repository focuses on design methodology, architecture, and verified simulation results.
