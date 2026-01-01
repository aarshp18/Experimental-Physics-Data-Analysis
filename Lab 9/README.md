# Advanced Spring Dynamics: Mass Determination

## Project Overview
Building on previous elasticity studies, this project utilized improved data acquisition methods (Video Analysis) to characterize a real spring and determine the mass of an unknown object[cite: 1029]. [cite_start]The experiment compared static force analysis (Hooke's Law) with dynamic oscillation modeling (Simple Harmonic Motion)[cite: 1029].

## Methodology
The experiment employed two physical models to characterize the system:

1.  **Static Characterization:**
    * [cite_start]Measured spring extension ($\Delta x$) under known loads ($F$)[cite: 1030, 1049].
    * [cite_start]Calculated the Spring Constant ($k$) via linear regression[cite: 1051].
2.  **Dynamic Mass Determination:**
    * [cite_start]Captured high-frame-rate video of the oscillating system[cite: 1053].
    * [cite_start]Extracted the period ($T$) of the unknown mass using **Tracker Video Analysis** software[cite: 1053].
    * [cite_start]Calculated the unknown mass by inverting the SHM equation[cite: 1054].

## Mathematical Models
### 1. Static Model (Hooke's Law)
$$F = k \Delta x$$
* [cite_start]**Slope:** Spring Constant ($k$)[cite: 1032].

### 2. Dynamic Model (SHM)
The mass ($m$) is derived from the oscillation period ($T$) and the previously determined stiffness ($k$):
$$m = \frac{k T^2}{4\pi^2} - \frac{m_s}{3}$$
[cite_start]Where $m_s$ is the effective mass of the spring correction[cite: 1037, 1086].

## Key Results
* [cite_start]**Spring Constant ($k$):** $44.40$ N/m[cite: 1081].
* [cite_start]**Unknown Mass Determination:** $0.535$ kg[cite: 1090].
* [cite_start]**Methodology Comparison:** The use of video analysis (Tracker) provided significantly cleaner period data compared to manual timing methods used in previous iterations (Lab 7)[cite: 1097, 1098].
* [cite_start]**Limitations:** Static analysis could not be used for the unknown mass validation as the specific extension data point was not captured during the trial[cite: 1092].

## Technologies Used
* **Data Analysis:** Python (Pandas for data ingestion, Matplotlib for regression).
* [cite_start]**Computer Vision:** Tracker Video Analysis (for precise period measurement)[cite: 1040].
* **Physics:** Classical Mechanics, Harmonic Oscillators.

## Visualizations

### 1. Static Stiffness Analysis
*Linear regression of Force vs. Extension. The slope ($44.4$) represents the spring constant $k$.*
![Hooke's Law Analysis](hookes_law_fit.png)
