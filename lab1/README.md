# Laboratory Work 1

Modeling of a permanent-magnet synchronous motor for the Sensorless Control course, variant 3.

## Project Structure

```text
lab1/
├── README.md
├── report.pdf
├── artifacts/
│   ├── *.png
│   ├── *.json
│   └── *.npz
├── lab_1_screenshots/
│   └── *.png
└── matlab/
    ├── SC_Lab1_Variant3.slx
    ├── build_lab1_simulink_model.m
    └── lab1_params_v3.m
```

## Task

Build a PMSM model in the stationary alpha-beta frame, apply sinusoidal stator voltages and a step load torque, then analyze the transient responses of the motor variables during a 1-second simulation.

## Solution

The PMSM was modeled in Simulink and in the supporting numerical scripts. For variant 3, the voltages were set as `v_alpha = 52 cos(26 t)` and `v_beta = 52 sin(26 t)`, while the load torque changed from `0` to `0.35 N*m` at `t = 0.5 s`. The report contains the simulation scheme, real Simulink screenshots, calculated values, and transient plots for voltages, currents, speed, rotor position, and magnetic flux.
