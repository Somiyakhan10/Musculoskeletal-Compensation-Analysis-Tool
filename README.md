# 🦴 MuscleComp — Musculoskeletal Compensation Analysis Study

**Quantitative Analysis of Muscle Activation Changes Under Simulated Knee Weakness**

**By Somiya Khan**

---

⚠️ **Academic Disclaimer:**
This project is a computational simulation using a musculoskeletal model in OpenSim. It does not represent real patient data, and results should be interpreted within the limitations of the modeling framework.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Key Findings](#key-findings)
- [Screenshots](#screenshots)
- [Model Performance](#model-performance)
- [Dataset / Model Information](#dataset--model-information)
- [Muscles Analyzed](#muscles-analyzed)
- [Conclusion](#conclusion)
- [Future Work](#future-work)

---

## 🔬 Overview

**MuscleComp** is a computational biomechanics study that investigates how the musculoskeletal system adapts when a key lower extremity muscle is weakened.

Using **OpenSim 4.6**, a healthy model and a weakened model were developed by reducing the maximum isometric force of the Rectus Femoris by 50%. **Static Optimization** was then used to estimate muscle forces under both conditions.

The analysis focuses on identifying changes in muscle force distribution and observing trends in compensatory muscle activation.

---

## 📊 Key Findings

| Observation | Result |
|-------------|--------|
| **Soleus force change** | +67.8% |
| **Vastus Medialis force change** | +27.5% |
| **Tibialis Anterior force change** | +25.6% |
| **Rectus Femoris change** | +10.0% |
| **Semitendinosus change** | -0.3% |

👉 Results indicate increased contribution from certain muscles (particularly Soleus), suggesting compensatory activation behavior in response to reduced Rectus Femoris strength.

> ⚠️ Note: These values are derived from a single simulation and are presented as relative differences.

---

## 📸 Screenshots

### Muscle Force Comparison
<img width="767" height="477" alt="image" src="https://github.com/user-attachments/assets/dfeab50c-5de8-4fd0-aa2d-f3ca4dc7ce04" />


### Percent Change Visualization

<img width="653" height="472" alt="image" src="https://github.com/user-attachments/assets/357d920d-0c8b-45c0-aebc-a40ca485173b" />




---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| **Primary observed compensator** | Soleus |
| **Maximum observed change** | 67.8% |
| **Muscles analyzed** | 5 lower extremity muscles |
| **Simulation type** | Static Optimization |
| **Simulation cases** | 2 (Healthy, Weakened) |

### Compensation Summary Table

| Muscle | Healthy (N/kg) | Weakened (N/kg) | Δ (%) |
|--------|---------------|-----------------|-------|
| **Soleus** | 0.143 | 0.240 | **+67.8%** |
| Vastus Medialis | 0.207 | 0.264 | +27.5% |
| Tibialis Anterior | 0.550 | 0.691 | +25.6% |
| Rectus Femoris | 0.909 | 1.000 | +10.0% |
| Semitendinosus | 0.792 | 0.790 | -0.3% |

---

## 📁 Dataset / Model Information

| Property | Details |
|----------|---------|
| **Base Model** | Gait2392 (Delp et al., 1990; Thelen, 2003) |
| **Software** | OpenSim 4.6 |
| **Muscle Model** | Thelen2003Muscle |
| **Analysis Tool** | Static Optimization |
| **Simulation Cases** | Healthy vs Weakened |
| **Muscles Analyzed** | 5 lower extremity muscles |

---

## 💪 Muscles Analyzed

| Muscle | Function | Original Force (N) | Modified Force (N) |
|--------|----------|-------------------|-------------------|
| Rectus Femoris | Knee extensor / Hip flexor | 585 | 292 (50% reduction) |
| Soleus | Ankle plantarflexor | 1558 | 1558 |
| Vastus Medialis | Knee extensor | 647 | 647 |
| Tibialis Anterior | Ankle dorsiflexor | 905 | 905 |
| Semitendinosus | Knee flexor | 410 | 410 |

---

## 🧠 Conclusion

This study demonstrates how reducing the strength of a key muscle can alter force distribution across other muscles in the system. The observed increases in specific muscles highlight how the musculoskeletal model adapts under simulated weakness conditions.

These findings provide a foundation for further studies in:
- Rehabilitation biomechanics
- Muscle coordination analysis
- Assistive device simulation (future work)

---

## 🚀 Future Work

- Introduce assistive torque (exoskeleton simulation)
- Expand analysis to additional muscles and joints
- Incorporate multiple simulation trials for statistical analysis
- Explore energy expenditure and joint loading

---

## 👩‍🔬 Author

**Somiya Khan**

Biomechanics Researcher | Musculoskeletal Modeling

- **GitHub:** [github.com/somiya-khan01](https://github.com/somiya-khan01)




---

**Built with OpenSim 4.6**

⭐ If you find this project useful, please consider giving it a star!

---





