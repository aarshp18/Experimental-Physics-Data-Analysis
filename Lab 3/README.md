# Experimental Determination of Gravitational Acceleration ($g$)

## Project Overview
This project utilizes computer vision techniques and statistical analysis to experimentally determine the acceleration due to gravity ($g$). By analyzing the kinematics of a free-falling projectile, I developed a Python pipeline to extract motion data and validate the theoretical model of uniformly accelerated motion.

## Methodology
The experiment consisted of three main phases:

1.  **Data Acquisition:** High-speed video recording of a free-falling spherical object.
2.  **Motion Tracking:** Utilized **Tracker Video Analysis** software to extract frame-by-frame position $(y)$ and velocity $(v_y)$ data, exporting the raw dataset to `.csv` format.
3.  **Computational Analysis:**
    * Ingested raw data using **Pandas**.
    * Modeled the motion using the kinematic equation: $v_y = v_{0y} + gt$.
    * Performed a **linear regression** on the Velocity vs. Time dataset to calculate the slope.

## Mathematical Model
According to Newtonian mechanics, the velocity of an object in free fall is given by:

$$v_y(t) = -gt + v_0$$

Where:
* $v_y(t)$ is the vertical velocity at time $t$.
* $g$ is the acceleration due to gravity (experimentally determined slope).
* $v_0$ is the initial velocity.

## Key Results
The analysis generated a linear fit for the velocity-time data:

> **Equation of Fit:** $v = -8.49t + 44.13$

From this regression, the experimental value of gravity was determined to be:
* **Experimental $g$:** $8.49 \pm 0.28 \, m/s^2$
* **Standard Error:** Factors contributing to the deviation from the theoretical value ($9.81 \, m/s^2$) included motion blur and camera parallax errors.

## Technologies Used
* **Python:** Data processing and automated analysis.
* **Libraries:** `pandas` (Dataframes), `matplotlib` (Visualization), `numpy` (Linear Algebra).
* **Tools:** Tracker Video Analysis, LaTeX (for reporting).

## Visualizations
*Figure 1: Velocity vs. Time scatter plot with linear regression fit.*
![Velocity vs Time Graph](velocity_vs_time.jpeg)
*Figure 2: Position vs. Time scatter plot with linear regression fit.*
![Position vs Time Graph](position_vs_time.jpeg)

