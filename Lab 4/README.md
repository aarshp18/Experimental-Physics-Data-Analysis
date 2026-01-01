# Dynamics of Atwood's Pulley System

## Project Overview
This project investigates the validity of Newton's Second Law of Motion using an Atwood's Pulley system. By systematically varying the unbalanced force acting on the system while keeping the total mass constant, I modeled the relationship between mass difference and system acceleration to experimentally determine the effective mass of the pulley ($m_p$).

## Methodology
The experiment involved precise data collection and computational modelling:

1.  **Data Collection:** Utilized a **Smart Pulley** sensor and **LoggerPro** interface to capture real-time kinematic data.
2.  **Experimental Design:** Maintained a constant total system mass while transferring weight between hangers to vary the driving force.
3.  **Computational Analysis:**
    * Processed experimental data using **Python (Pandas)**.
    * Performed a **Linear Regression** (using `numpy.polyfit`) to correlate the Mass Difference ($m_1 - m_2$) with Acceleration ($a$).
    * Calculated the effective mass of the pulley from the regression slope.

## Mathematical Model
The system was modelled using Newton's Second Law, rearranged into a linear form ($y = mx + b$):

$$(m_1 - m_2) = \left[ \frac{M_{total} + m_p}{g} \right] a + m_f$$

Where:
* $(m_1 - m_2)$: The mass difference (Driving Force proxy).
* $a$: System acceleration.
* $m_p$: Effective mass of the pulley (derived from the slope).
* $m_f$: Frictional losses (derived from the intercept).

## Key Results
* **Linear Model:** The data showed a strong linear correlation, validating Newton's Second Law.
* **Experimental Pulley Mass ($m_p$):** $23.56 \pm 1.28$ g.
* **Discrepancy Analysis:** The experimental mass was significantly higher than the manufacturer's specification (5.5 g). This discrepancy was attributed to rotational inertia and unmodeled frictional forces in the bearing system.

## Technologies Used
* **Analysis:** Python (Pandas, NumPy).
* **Visualization:** Matplotlib (Error bars, Linear Fit).
* **Hardware:** Vernier Smart Pulley, Photogates.

## Visualizations
*Figure 1: Linear regression of Mass Difference vs. Acceleration.*
![Atwood Regression Plot](lab_04.jpeg)
