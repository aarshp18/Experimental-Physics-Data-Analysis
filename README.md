# Experimental Physics & Computational Data Analysis

## 📌 Repository Overview
This repository contains a collection of experimental research projects conducted for **PHYS 144** at the **University of Alberta**.

The primary focus of this work is the intersection of **Experimental Physics** and **Scientific Computing**. Each project involves collecting real-world data (via sensors, video analysis, or oscilloscopes) and building computational pipelines in **Python** to model physical phenomena, calculate error propagation, and visualize complex datasets.

## 🛠 Tech Stack & Skills
* **Languages:** Python (3.x), $\LaTeX$
* **Data Science:** Pandas, NumPy
* **Visualization:** Matplotlib
* **Software & Tools:** Tracker Video Analysis, LoggerPro
* **Instrumentation:** Digital Oscilloscopes, Photodiodes, Smart Pulleys
* **Methods:** Linear Regression, Differential Equation Modelling, Signal Processing, Error Propagation

## 📂 Project Directory

| Project | Physics Domain | Computational Focus |
| :--- | :--- | :--- |
| **[Lab 3: Gravitational Acceleration](./Lab%203)** | Kinematics | Linear regression modeling of $v-t$ data to derive physical constants ($g$). |
| **[Lab 4: Atwood's Machine](./Lab%204)** | Dynamics (Newton's Laws) | Modelling multi-body systems and analyzing friction/rotational inertia discrepancies. |
| **[Lab 5: Optical Spectroscopy](./Lab%205)** | Wave Optics & Quantum | Calibrating pixel-to-wavelength pipelines and analyzing discrete emission spectra. |
| **[Lab 6: Damping & Energy](./Lab%206)** | Thermodynamics / Mechanics | Modeling exponential decay of energy in non-conservative systems. |
| **[Lab 7: Elasticity & Hysteresis](./Lab%207)** | Materials Science | Comparative analysis of Static (Hooke's Law) vs. Dynamic (SHM) elastic moduli in non-ideal polymers. |
| **[Lab 8: Iterative System Design](./Lab%208)** | Harmonic Motion | Optimizing measurement precision using Computer Vision (Tracker) to determine unknown masses. |
| **[Lab 9: Signal Instrumentation](./Lab%209)** | AC Circuits / Optics | Hardware-level waveform analysis, signal rectification, and frequency doubling using Oscilloscopes. |

## 📊 Sample Visualizations
*Below are examples of the data analysis pipelines built for these experiments.*

| Damping Analysis (Lab 6) | Spectroscopy (Lab 5) |
| :---: | :---: |
| <img src="Lab 6/linear_fit.jpeg" width="400"> | <img src="Lab 5/helium_spectrum.png" width="400"> |
| *Linearization of exponential energy decay* | *Discrete emission lines of Helium* |

## 🚀 How to Run the Analysis
The analysis for these projects is written in Python. To reproduce the graphs or calculations:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/aarshp18/Experimental-Physics-Data-Analysis.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib
    ```
3.  **Navigate to a lab and run the notebook/script:**
    ```bash
    cd "Lab 3"
    jupyter notebook
    ```

## 👨‍💻 Author
**Aarsh Patel**
* University of Alberta
* Major: Bsc Honors in Computing Science, intended Double Major in Physics 
* *Focus: Scientific Computing, Data Analysis, and Physical Modelling.*

---
*This repository serves as a portfolio of laboratory skills, demonstrating the application of computing science principles to experimental physics.*
