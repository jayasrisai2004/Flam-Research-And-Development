# Flam Research and Development Assignment

## Overview
This project implements a parametric curve fitting approach using Python, specifically leveraging libraries such as Pandas, NumPy, Matplotlib, and Scipy. The goal is to find the unknown parameter values Theta(θ), M, and X using the given parametric equation and dataset provided for 6<t<60.

## Features
- Upload and load dataset with two columns (`x` and `y`).
- Visualize observed curve points using scatter plots.
- Define a parametric curve model with parameters theta, M, and X.
- Calculate L1 distance as a metric for model fitting.
- Optimize parameters using differential evolution to minimize the L1 distance.
- Plot the fitted parametric curve against the observed data.

## Usage
1. Upload a CSV file containing the dataset with columns `x` and `y`.
2. Run the notebook cells to load and visualize the data.
3. The code will optimize the parametric curve fitting parameters.
4. Visualize the fitted curve compared to the original data points.

## Dependencies
- Python 3.x
- pandas
- numpy
- matplotlib
- scipy

## Mathematical Formulation
### Parametric equation of the curve:
$x = t\cos(\theta) - e^{M|t|}\sin(0.3t)\sin(\theta) + X$

$y = 42 + t\sin(\theta) + e^{M|t|}\sin(0.3t)\cos(\theta)$

where \(t\) is uniformly spaced, and \(\theta\), \(M\), and \(X\) are parameters optimized to best fit the observed \(x\) and \(y\) data.

## Final Outcomes
- Optimal parameters:
  - Theta (degrees): 28.12
  - M: 0.0214
  - X: 54.90
- Final L1 distance (mean absolute error) between predicted and observed data: 25.24

This parametric model with the above parameters provides the best fit to the observed data.

### Final Equation for Submission format
$$\left( t \cos(0.4908) - e^{ 0.0214 |t| } \sin(0.3 t) \sin(0.4908) + 54.8997 \right),\left( 42 + t \sin(0.4908) + e^{ 0.0214 |t| } \sin(0.3 t) \cos(0.4908) \right)$$

### Fitted Curve Plot
![plotting](https://github.com/jayasrisai2004/Flam-Research-And-Development/blob/main/Graph.png)

## License
This project is licensed under the Apache License, Version 2.0.

