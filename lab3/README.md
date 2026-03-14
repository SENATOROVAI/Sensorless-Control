# Laboratory Work 3

Adaptive observer and sensorless PMSM control for the Sensorless Control course, variant 3.

## Project Structure

```text
lab3/
├── README.md
├── report.pdf
├── artifacts/
│   ├── *.png
│   ├── *.json
│   └── *.npz
├── lab_3_screenshots/
│   └── *.png
└── matlab/
    ├── SC_Lab3_Variant3.slx
    └── build_lab3_simulink_model.m
```

## Task

Design an adaptive observer for PMSM, estimate the rotor position and speed without direct sensors, evaluate the observer in open-loop mode, and then use the estimated position inside the control loop to obtain a sensorless drive.

## Solution

The model combines PMSM dynamics, field-oriented control, a gradient-based adaptive observer, and a PLL-based speed estimator. First, the observer performance was checked using parameter, flux, position, and speed estimation errors. Then the measured rotor position was replaced by the estimated one, which produced a sensorless control scheme. The final report includes the Simulink implementation, screenshots, design parameters, transient plots, and the numerical verification of the observer accuracy.
