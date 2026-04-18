# MuscleComp — Musculoskeletal Compensation Analysis Tool

**Quantifying Compensatory Muscle Activation in Simulated Gait Pathology**

By [Somiya Khan]

---

**⚠️ Academic Disclaimer:** This simulation is a computational model and does not represent real patient data. Results should be interpreted within the context of model limitations.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Key Findings](#key-findings)
- [Screenshots](#screenshots)
- [Model Performance](#model-performance)
- [Dataset / Model Information](#dataset--model-information)

---

## 🔬 Overview

**MuscleComp** is a computational biomechanics project that investigates how the human neuromuscular system compensates when a major lower extremity muscle is weakened during gait.

Using **OpenSim 4.6** musculoskeletal simulation software, we created healthy and pathological gait models and performed **Static Optimization** to estimate muscle forces. The key finding reveals a **distal-to-proximal compensation strategy** where the Soleus muscle increases activation by **67.8%** when the Rectus Femoris is weakened.

---

## 📊 Key Findings

| Finding | Value |
|---------|-------|
| **Soleus compensation** | +67.8% increase (p < 0.01) |
| **Vastus Medialis compensation** | +27.5% increase (p < 0.01) |
| **Tibialis Anterior compensation** | +25.6% increase (p < 0.05) |
| **Compensation strategy** | Distal-to-proximal |
| **Statistical significance** | 3 muscles with p < 0.05 |

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
| **Primary compensator identified** | Soleus |
| **Maximum compensation magnitude** | 67.8% |
| **Statistically significant muscles** | 3/5 (p < 0.05) |
| **Muscles analyzed** | 5 major lower extremity muscles |
| **Gait cycle duration** | 1.0 second (100% cycle) |

### Compensation Summary Table

| Muscle | Healthy (N/kg) | Weakened (N/kg) | Δ (%) | p-value |
|--------|---------------|-----------------|-------|---------|
| **Soleus** | 0.143 | 0.240 | **+67.8%** | 0.003 *** |
| Vastus Medialis | 0.207 | 0.264 | +27.5% | 0.008 *** |
| Tibialis Anterior | 0.550 | 0.691 | +25.6% | 0.012 ** |
| Rectus Femoris | 0.909 | 1.000 | +10.0% | 0.089 |
| Semitendinosus | 0.792 | 0.790 | -0.3% | 0.782 |

***p < 0.01, **p < 0.05*

---

## 📁 Dataset / Model Information

| Property | Details |
|----------|---------|
| **Base Model** | Gait2392 (Delp et al., 1990; Thelen, 2003) |
| **Software** | OpenSim 4.6 |
| **Muscle Model** | Thelen2003Muscle |
| **Analysis Tool** | Static Optimization |
| **Total Simulations** | 2 (Healthy, Weakened) |
| **Muscles Analyzed** | 5 lower extremity muscles |
| **Gait Condition** | Normal walking |

### Muscles Analyzed

| Muscle | Function | Original Force (N) | Weakened Force (N) |
|--------|----------|-------------------|-------------------|
| Rectus Femoris | Knee extensor / Hip flexor | 585 | 292 (50% ↓) |
| Soleus | Ankle plantarflexor | 1558 | 1558 (unchanged) |
| Vastus Medialis | Knee extensor | 647 | 647 (unchanged) |
| Tibialis Anterior | Ankle dorsiflexor | 905 | 905 (unchanged) |
| Semitendinosus | Knee flexor | 410 | 410 (unchanged) |

---

