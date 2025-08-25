# 🌌 Investigating Baryon Acoustic Oscillations with DES Galaxy Data

**Author:** Emilia Zabrzanska  
**Date:** April 2025  

This repository contains the analysis for my project *"Investigating how Baryon Acoustic Oscillations depend on Redshift in the Dark Energy Survey Galaxy Catalogue"* (S385 – TMA03).  
The work explores the detection and evolution of the **BAO signal** across multiple redshift bins using galaxy data from the **Dark Energy Survey (DES)**.  

---

## 📘 Project Overview

Baryon Acoustic Oscillations (BAOs) are relic sound waves from the early universe, imprinted in the large-scale structure of galaxies.  
They provide a **standard ruler** for measuring cosmic distances and probing the expansion history of the universe.  

This project measures the **two-point angular correlation function** ω(θ) across different redshift bins to identify the BAO "bump" and compare its angular scale θ<sub>BAO</sub> with theoretical predictions.  

---

## 🎯 Objectives

- Divide DES galaxy data into redshift bins (0.60 < z < 1.10).  
- Compute the **two-point angular correlation function** ω(θ).  
- Detect BAO signatures using the **Landy–Szalay estimator**.  
- Fit models combining a broken power law (background clustering) and a Gaussian component (BAO bump).  
- Extract the BAO angular scale θ<sub>BAO</sub> and compare with theoretical predictions.  
- Evaluate uncertainties and discuss limitations of the method.  

---

## 🧮 Methods

### 1. Two-point correlation function

The probability of finding galaxy pairs separated by angle θ:  

$$
\omega(\theta) = \frac{\langle P(\theta) \rangle}{R(\theta)} - 1
$$

where *P(θ)* is the probability of galaxy–galaxy separations, and *R(θ)* is the random distribution.

### 2. Landy–Szalay Estimator

For real surveys, the Landy–Szalay estimator was used:  

$$
\omega(\theta) = \frac{DD(\theta) - 2fDR(\theta) + f^2RR(\theta)}{f^2RR(\theta)}
$$

- **DD(θ):** data–data pairs  
- **DR(θ):** data–random pairs  
- **RR(θ):** random–random pairs  
- **f:** normalisation factor  

### 3. BAO Fitting

The correlation function was modelled as:  

$$
f_{\text{combined}}(\theta) = f_{\text{BPL}}(\theta) + f_{\text{BAO}}(\theta)
$$

- **Broken Power Law (BPL):** background clustering  
- **Gaussian (BAO):** models the "bump" feature  

### 4. Theoretical Angular BAO Scale

The physical BAO size at redshift *z*:  

$$
d_{p,\text{BAO}}(z) = \frac{d_{c,\text{BAO}}}{1+z}
$$  

Angular BAO size:  

$$
\theta_{\text{BAO}}(z) = \frac{d_{p,\text{BAO}}(z)}{d_A(z)}
$$

where *d<sub>A</sub>(z)* is the angular diameter distance.  

---

## 📊 Results

- Clear BAO signals detected in **0.75 < z < 1.10** bins.  
- Weak or absent signals in **z < 0.75** bins.  
- Extracted θ<sub>BAO</sub> values broadly followed theoretical expectations, decreasing with redshift.  
- Some deviations (e.g., 0.85 < z < 0.95 and 1.00 < z < 1.10 bins), likely due to noise and sample size.  
- Results support BAOs as a **reliable standard ruler**, consistent with the ΛCDM cosmological model.  

---

## ⚖️ Limitations & Future Work

- **Weak signals** at low redshift → need larger sample size.  
- **Noise** affected some fits, producing large uncertainties.  
- **Future improvements:**  
  - Analyse larger datasets (DESI, Euclid).  
  - Refine bin widths for optimal signal clarity.  
  - Include survey geometry and systematic errors.  

---

## 📂 Repository Contents

- `S385_TMA03_Report.pdf` – Full project report with analysis, figures, and discussion.  
- `README.md` – Project summary (this file).  
- *(Optional future additions: Python/Jupyter notebooks for correlation function calculation and model fitting.)*  

---

## 📚 References

- Dark Energy Survey (DES) galaxy catalogue.  
- Landy, S. D., & Szalay, A. S. (1993). *Bias and variance of angular correlation functions*. ApJ, 412, 64.  
- Open University S385 Cosmology module (Chapters 7, 9, 10, 11).  

---

## 📬 Contact

- 📧 [emiliazabrzanska02@gmail.com](mailto:emiliazabrzanska02@gmail.com)  
- 💼 [LinkedIn – Emilia Zabrzanska](https://www.linkedin.com/in/emilia-zabrzanska/)  

---

## 📜 License

This project is shared under the **MIT License**.  
You are free to use, adapt, and share the modelling approach with attribution.
