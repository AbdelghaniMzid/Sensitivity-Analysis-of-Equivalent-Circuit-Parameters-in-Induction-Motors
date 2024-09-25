# Sensitivity Analysis of Equivalent Circuit Parameters in Induction Motors

## Project Overview
This project conducts a comprehensive sensitivity analysis of various equivalent circuit parameters in squirrel-cage induction motors. The study investigates how parameter variations, such as changes in resistance and reactance, impact the performance of the motors. The goal is to evaluate both the transient behavior, such as responses to short-circuit events, and steady-state conditions, particularly focusing on torque-speed characteristics.

## Key Components:
- **Simulation Tools:** MATLAB & Simulink
- **Motors Studied:** Two squirrel-cage induction motors with different power ratings:
  - **Motor 1:** 1.1 kW
  - **Motor 2:** 6.3 MW
- **Analysis Focus:**
  - **Torque-Speed Curve Analysis:** Examining how motor torque changes with speed under varying parameter conditions.
  - **Sensitivity Analysis:** 
    - **Screening (One-at-a-Time)**: Investigating the impact of individual parameters.
    - **Local Sensitivity Methods**: Evaluating sensitivity across multiple parameters.
  - **Parameter Variations:**
    - Stator Resistance (R1)
    - Rotor Resistance (R’2)
    - Stator and Rotor Leakage Reactances (Xσ1, Xσ2)
    - Main Reactance (Xh1)

## Tools and Software:
- **MATLAB:** Used for implementing the sensitivity analysis and steady-state simulations.
- **Simulink:** Employed to simulate dynamic behaviors such as short circuits and transient responses.
- **CSV Output:** Simulation results are stored in CSV files for further analysis and visualization.
- **Data Visualization Tools:** MATLAB's plotting capabilities are used to create detailed graphs of motor performance under different conditions.

## Setup Instructions:
1. **Clone the repository:** Download the project from the GitHub repository.
2. **Ensure Software Installation:** Verify that MATLAB and Simulink are installed and configured on your computer.
3. **Run the Simulations:** Navigate to the `/src` directory, where the simulation files are located, and execute the `.m` scripts or open the Simulink model for short-circuit analysis.

## Results:
The sensitivity analysis yields several important insights:
- **Rotor Resistance (R’2):** The variation of rotor resistance has a significant impact on the motor's startup torque.
- **Leakage Reactances (Xσ1, Xσ2):** These parameters notably affect the motor's behavior during short-circuit conditions, influencing current and torque responses.
- **Main Reactance (Xh1):** Slight variations in this parameter can affect overall efficiency but are less impactful on transient events.

### Example Outputs:
- **Torque-Speed Characteristics:** Graphs demonstrating the impact of varying stator and rotor resistances on motor performance.
- **Current and Torque under Short-Circuit Conditions:** Plots that show the transient behavior of the motor during electrical faults.
  
## Visual Documentation:

### Torque-Speed Curves:
![Torque-Speed Curve](Drehmoment.jpg)
*Figure 1: Torque-speed curve for Motor 1 with varying R1 values.*

### Short-Circuit Current Response:
![Short Circuit Current](Stoßstrom.jpg)
*Figure 2: Current response during a short circuit event, showing variations with different parameters.*

### Current Phasor Representation:
![Stromortskurve](stromsrtskurve.jpg)
*Figure 3: Phasor diagram showing real and imaginary parts of current under different R1 conditions.*

### Sensitivity Map:
![Widerstand Einfluss](Widerstand_Einfluss.jpg)
*Figure 4: Heatmap showing the sensitivity of rotor resistance (R'2) and main reactance (Xh1) on motor current.*

## Conclusion:
This sensitivity analysis provides valuable insights into how parameter variations affect the performance of induction motors. The results can be used to optimize motor design and predict behavior under fault conditions, enhancing overall motor efficiency and reliability. The findings highlight the importance of rotor resistance and leakage reactances in both steady-state and transient operations.
