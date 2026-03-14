# Laboratory Work 2

Field-oriented control of PMSM for the Sensorless Control course, variant 3.

## Project Structure

```text
lab2/
├── README.md
├── report.pdf
├── artifacts/
│   ├── *.png
│   ├── *.json
│   └── *.npz
├── lab_2_screenshots/
│   └── *.png
└── matlab/
    ├── SC_Lab2_Variant3.slx
    └── build_lab2_simulink_model.m
```

## Task

Develop a field-oriented control system for the PMSM model from Lab 1, generate the reference speed profile, tune PI controllers, and verify that the drive tracks the required speed with low overshoot and small steady-state error.

## Solution

The PMSM was controlled in the rotating dq frame using cascade PI regulation: the outer speed loop generated the reference `i_q`, while the inner current loops controlled `i_d` and `i_q`. For variant 3, the speed reference increased linearly up to `106 rad/s` and then remained constant. The selected controller gains provided stable operation, very small overshoot, and accurate steady-state tracking. The report includes the Simulink scheme, real screenshots, controller parameters, and the main transient responses.
