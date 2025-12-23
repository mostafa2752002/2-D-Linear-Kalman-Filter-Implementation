# 2D Linear Kalman Filter Tracking

This repository contains my implementation of a 2D Linear Kalman Filter (LKF) designed to track an object's position and velocity using a Constant Velocity (CV) motion model.

## 🎓 Origin
This project was completed as an assignment for the Udemy course:
**"Data Fusion and Linear Kalman Filter"** by **Steven Dumble**.

## 🚀 Learning Objectives
The project is divided into three progressive scripts to demonstrate the core mechanics of the Kalman Filter:
1. **Prediction Only**: Demonstrates dead-reckoning drift without sensor updates.
2. **Standard Update**: Integrates noisy measurements to correct the state estimate.
3. **Robust Initialization**: Proves filter convergence even when the initial state estimate is highly uncertain ($P_0 = 100^2$).

## 🛠️ Technical Details
* **State Vector ($x$):** $[p_x, p_y, v_x, v_y]^T$
* **Motion Model:** Constant Velocity (CV) Transition Matrix $F$.
* **Sensor Model:** Position-only measurement matrix $H$.
* **Environment:** Developed on Ubuntu 22.04 using NumPy and Matplotlib.

## 📈 Results
The simulation provides real-time visualization of:
* **State vs. Truth**: Comparing estimated position/velocity against actual values.
* **Innovation**: Monitoring the measurement residual to ensure filter health.
* **2D Path**: Tracking the trajectory in a Cartesian plane.

![Simulation Results](docs/simulation_results.png)