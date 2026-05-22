# 4-Bit SAR ADC Design Using Custom CMOS Logic in Cadence

## Overview

This project presents the design and simulation of a 4-bit Successive Approximation Register (SAR) Analog-to-Digital Converter implemented using custom CMOS logic in Cadence Virtuoso.

The complete ADC was designed from transistor level using basic NMOS and PMOS transistors without using predefined digital blocks. The project includes the design of SAR logic, D flip-flops, comparator, R-2R DAC, clock synchronization, and analog-digital interfacing.

Transient analysis was performed to verify successful analog-to-digital conversion.

---

## Project Objectives

- Design a fully custom 4-bit SAR ADC
- Implement SAR logic using D flip-flops
- Design transistor-level digital and analog blocks
- Integrate R-2R DAC with comparator and SAR control logic
- Perform transient simulations for ADC verification
- Understand timing synchronization between analog and digital sections

---

## Tools Used

- Cadence Virtuoso

---

## ADC Architecture

The SAR ADC consists of the following blocks:

1. Sample and Hold
2. Comparator
3. SAR Logic
4. D Flip-Flops
5. R-2R DAC
6. Clock and Control Logic

---

## Key Features

- Fully custom transistor-level implementation
- Built using basic NMOS and PMOS devices
- 4-bit SAR conversion logic
- R-2R ladder DAC architecture
- Positive-edge triggered SAR logic
- Negative-edge triggered comparator operation
- Mixed-signal integration in Cadence
- Functional verification using transient analysis

---

## Working Principle

1. The analog input signal is sampled.
2. SAR logic starts conversion from MSB to LSB.
3. The R-2R DAC generates reference voltages based on SAR output.
4. Comparator compares DAC output with sampled input.
5. Comparator output updates SAR register bit-by-bit.
6. Final 4-bit digital output represents the analog input value.

---

## Comparator Timing

- Comparator operates on negative clock edge
- SAR register updates on positive clock edge

This timing separation helps avoid logic conflicts during conversion.

---

## Simulation Results

Transient analysis was performed to verify:

- SAR bit-by-bit approximation
- Comparator operation
- DAC voltage generation
- Correct digital output generation

The ADC successfully converts analog input signals into corresponding 4-bit digital outputs.

---

## Learning Outcomes

Through this project, the following concepts were understood practically:

- SAR ADC architecture
- CMOS digital design
- Clock synchronization
- DAC operation
- Comparator behavior
- Mixed-signal circuit integration
- Timing analysis in ADC systems

---

## Future Improvements

- Increase ADC resolution
- Reduce conversion delay
- Add asynchronous SAR logic
- Perform DNL/INL analysis
- Optimize power consumption
- Add layout design and post-layout simulations

---


---

## Author

Designed and simulated as a student mixed-signal VLSI project using Cadence Virtuoso.
