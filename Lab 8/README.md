# Advanced Spring Dynamics: Mass Determination

## Project Overview
Building on previous elasticity studies, this project utilized improved data acquisition methods (Video Analysis) to characterize a real spring and determine the mass of an unknown object. The experiment compared static force analysis (Hooke's Law) with dynamic oscillation modeling (Simple Harmonic Motion).

## Methodology
The experiment employed two physical models to characterize the system:

1.  **Static Characterization:**
    * [cite_start]Measured spring extension ($\Delta x$) under known loads ($F$)[cite: 1110, 1111].
    * Calculated the Spring Constant ($k$) via linear regression.
2.  **Dynamic Mass Determination:**
    * Captured high-frame-rate video of the oscillating system.
    * [cite_start]Extracted the period ($T$) of the unknown mass using **Tracker Video Analysis** software[cite: 1114].
    * Calculated the unknown mass by inverting the SHM equation.

## Mathematical Models
### 1. Static Model (Hooke's Law)
$$F = k \Delta x$$
* **Slope:** Spring Constant ($k$).

### 2. Dynamic Model (SHM)
The mass ($m$) is derived from the oscillation period ($T$) and the previously determined stiffness ($k$):
$$m = \frac{k T^2}{4\pi^2} - \frac{m_s}{3}$$
Where $m_s$ is the effective mass of the spring correction.

## Key Results
* [cite_start]**Spring Constant ($k$):** $44.40$ N/m[cite: 1142].
* [cite_start]**Unknown Mass Determination:** $0.535$ kg[cite: 1151].
* [cite_start]**Methodology Comparison:** The use of video analysis (Tracker) provided significantly cleaner period data compared to manual timing methods used in previous iterations (Lab 7)[cite: 1158, 1159].
* [cite_start]**Limitations:** Static analysis could not be used for the unknown mass validation as the specific extension data point was not captured during the trial.

## Technologies Used
* **Data Analysis:** Python (Pandas for data ingestion, Matplotlib for regression).
* **Computer Vision:** Tracker Video Analysis (for precise period measurement).
* **Physics:** Classical Mechanics, Harmonic Oscillators.

## Visualizations

### 1. Static Stiffness Analysis
*Linear regression of Force vs. Extension. The slope ($44.4$) represents the spring constant $k$.*
![Hooke's Law Analysis](lab08.jpeg)