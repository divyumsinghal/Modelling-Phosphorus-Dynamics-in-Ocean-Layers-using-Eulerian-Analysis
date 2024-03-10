# Modelling-Phosphorus-Dynamics-in-Ocean-Layers-using-Eulerian-Analysis

# Short Summary
This Project involves modeling the exchange of phosphorus between the upper and lower ocean layers based on differential equations by using Euler's method to estimate the concentrations of phosphorus over time.


## Overview

This MATLAB project employs Eulerian analysis to model phosphorus dynamics in ocean layers. The simulation utilizes differential equations and Euler's method to estimate phosphorus concentrations in the lower and upper ocean layers over time. Additionally, the project explores the effects of a 1-degree Celsius temperature change on phosphorus dynamics.

## Prerequisites

- MATLAB

## Main Variables

- `k12`: Rate constant for phosphorus transfer from the lower to upper ocean.
- `k21`: Rate constant for phosphorus transfer from the upper to lower ocean.
- `M`: Total phosphorus mass in the ocean.
- `m1_initial`: Initial mass of phosphorus in the lower ocean.
- `m2_initial`: Initial mass of phosphorus in the upper ocean.

## Functions

### `lowerOcean` and `upperOcean`

These functions calculate the derivatives of phosphorus mass in the lower (`dm1dt`) and upper (`dm2dt`) ocean layers, respectively. Input parameters include the rate constants (`k12` and `k21`) and current masses of phosphorus in both layers (`m1` and `m2`).

## Simulation

### First Calculation

Solving for phosphorus concentrations over a time interval of 0 to 5 years in steps of 3 months using Euler's method. Output data is stored in variables `m1_e3` and `m2_e3`. Concentrations at 5 years are assigned to variables `m1pe` and `m2pe`.

### Repeating with Different Time Step

Solving for concentrations over a time interval of 0 to 5 years in steps of 1 month. Output data is stored in variables `m1_e1` and `m2_e1`.

### Comparing the Two Results

Plotting the estimates in Figure 1 and comparing the results for different time steps.

### Future Analysis

Assuming a 1-degree Celsius temperature change, the code calculates new estimates and plots them in Figure 2.

### Comparing Future with Present

Calculating the percentage change in phosphorus concentrations in the lower and upper ocean layers after 3 years with a 1-month time step.

## Euler's Algorithm

### `eulersMethod`

This function implements Euler's method for solving ordinary differential equations (ODEs). Input parameters include rate constants, initial masses, initial time, time step, and final time. The function returns concentrations of phosphorus in the lower (`m1`) and upper (`m2`) ocean layers over time.

## Numerical and Computational Concepts

The project employs numerical methods, specifically Euler's method, to solve ordinary differential equations governing phosphorus dynamics. Euler's method is a straightforward numerical integration technique that iteratively approximates solutions at discrete time steps. This approach allows for the simulation of complex dynamic systems, providing insights into the behavior of phosphorus concentrations in ocean layers over time.

## License

This project is licensed under the [GNU GPL-3.0 license](LICENSE).

