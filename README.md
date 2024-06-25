# Two-Stage Miller-Compensated Op-Amp Design

## Introduction

This document outlines the design and simulation results of a two-stage Miller-compensated operational amplifier (op-amp) designed to meet specific performance specifications.

### Specifications

- *DC Gain*: 2000
- *Input Common Mode Range*: 0.7 V to 1.6 V
- *Phase Margin*: > 60 degrees
- *Capacitive Load (CL)*: 5 pF
- *Gain-Bandwidth (GBW) Product*: 50 MHz

## Design Overview

### Design Procedure

1. *Miller Compensation Design*:
   - Calculate the compensating capacitor \( Cc \) to achieve a phase margin of 60°.
   - \( Cc \geq 0.22 \times CL \)

2. *Transconductance and Current Calculations*:
   - Evaluate drain current \( ID5 \) from the slew rate requirement.
   - Determine transconductance \( gm1 \) and \( gm4 \).
   - Calculate widths \( (w/l)1,2 \), \( (w/l)3,4 \), \( (w/l)5,8 \), \( (w/l)6 \), \( (w/l)7 \).

3. *Simulation and Optimization*:
   - Perform LTSpice simulations to verify design parameters.
   - Adjust \( Cc \) to achieve desired GBW product while maintaining phase margin.

### Important Formulas and Considerations

- GBW = \( gm1 / Cc \)
- Phase Margin Calculation
- Slew Rate Calculation
- Transconductance Calculations

## Simulation Results

### Circuit Diagram

Include the circuit diagram here or refer to the design schematic used in LTSpice.

### DC Operating Point

- *Bode Plot Analysis*:
  - *At Input Common DC Voltage 0.7V*:
    - DC Gain: 66.01 dB
    - Phase Margin: 70.05°
    - Gain Bandwidth Product: 50.35 MHz
  - *At Input Common DC Voltage 1.6V*:
    - DC Gain: 65.408 dB
    - Phase Margin: 70.74°
    - Gain Bandwidth Product: 50.83 MHz

### Error Analysis

- *Comparison with Specifications*:
  - *DC Gain (Simulation)*:
    - 0.7V: 1997.56 (Measured) vs 2000 (Spec)
    - 1.6V: 1862.08 (Measured) vs 2000 (Spec)
  - *Phase Margin*: > 60° (Achieved)
  - *Gain Bandwidth Product*: 50 MHz (Achieved)

### Conclusion

The designed two-stage Miller-compensated op-amp meets the required specifications with minor adjustments in \( Cc \) to optimize the Gain-Bandwidth Product. Further optimizations may be explored to fine-tune DC gain while maintaining stability and phase margin.

*The Two Stage op-amp*

![The Two Stage op-amp](https://github.com/Aryansh-kr/Commnet-24-PS1/assets/127012188/6428d521-5518-4080-ba08-725ba77fdf7a)

# Result
### Final Schematic
![image](https://github.com/Aditya24jar/Two-Stage-Opamp-Design/assets/126892937/6b088c56-f13b-49b9-95b0-ea1f8e628759)

### Calculated (w/l) ratois and current value
![image](https://github.com/Aryansh-kr/Commnet-24-PS1/assets/127012188/eebda71e-9529-490e-abe9-cd8a179bc997)

### Final Parameters value
![Screenshot 2024-06-25 160027](https://github.com/Aditya24jar/Two-Stage-Opamp-Design/assets/126892937/3f8a7966-2930-4629-9840-a3d752e26f76)

