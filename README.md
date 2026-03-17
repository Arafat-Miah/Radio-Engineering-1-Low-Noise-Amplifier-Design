# Radio Engineering I — Low-Noise Amplifier Design

This repository contains our **Radio Engineering I** design project on the **design and simulation of a low-noise amplifier (LNA)** using the **BFP450 transistor** in **QUCS-S**.

## Project Overview

The objective of this work was to design a **1.8–1.9 GHz low-noise preamplifier** that satisfies gain, noise figure, and stability requirements. The project included:

- bias-network design
- Smith-chart and noise-circle analysis
- stability analysis
- input matching for minimum noise figure
- full-band RF performance verification

## Design Specifications

Using the **BFP450** transistor at **VCE = 3 V** and **IC = 40 mA**, the amplifier was required to satisfy:

- **Noise Figure (NF):** not greater than **1.9 dB**
- **Gain |S21|:** not smaller than **13 dB**
- **Stability:** unconditionally stable over **1.8–1.9 GHz**

The design was carried out in **QUCS-S**, following the Radio Engineering I design exercise manual.

## Design Flow

1. Import transistor S-parameter data for BFP450
2. Simulate the transistor without bias networks
3. Design input and output bias networks using fan-shaped open stubs and quarter-wave microstrip lines
4. Compare RF behavior with and without bias networks
5. Analyze constant noise circles, S11, S22, Sopt, NFmin, and gain
6. Perform stability analysis using μ and K factors
7. Match the input using lumped components to approach minimum noise figure
8. Simulate the complete amplifier over the largest available bandwidth

## Key Results

The final amplifier achieved:

- **Noise Figure:** approximately **1.6 dB at 1.85 GHz**
- **Gain:** approximately **14–15 dB**
- **Stability:** unconditionally stable across the operating band

The results showed that proper input matching significantly improved both noise figure and gain, while the stabilization trade-off remained minimal.

## Technical Highlights

- BFP450 transistor-based LNA design
- QUCS-S simulation and RF data-display analysis
- Smith chart and constant noise-circle interpretation
- Bias-network design using radial stub + quarter-wave microstrip line
- Stability-factor evaluation using **μ**, **μ′**, and **Rollett K**
- Hand-calculated lumped matching network for low-noise operation

## Repository Contents

- `report/` — final accepted project report
- `assignment/` — original course design brief
- `images/` — schematics, Smith charts, and result plots
- `notes/` — optional hand calculations and supporting notes

## Tool Used

- **QUCS-S**

## Notes

This was a **group project**, and the work was shared among team members in design, simulation, analysis, and reporting.

## Authors

- **Mounir Lakhdari**
- **Arafat Miah**
- **Mohammadmahdi Ghanbari**

## Supervisor

- **Kimmo Rasilainen**

**Arafat Miah**  
MSc Electronics, University of Oulu
