---
title: Estimating Distance and Time Period of the Vela Pulsar
date: 2025-11-02
links:
  - type: Notes
    url: https://drive.google.com/file/d/1pleV-f7lfQZPvxedJrRCzrQSsh2J5w8w/view?usp=sharing

---

# 🚀 **Estimating Distance and Time Period of the Vela Pulsar**

## 🌌 Overview
This was an interesting project at space-Astronomy course. I had Kaustav Roy, Krishnabh Dutta Nandy an Nishant Pradeep Deo in my group. This project explores how raw voltage data from the **Ooty Radio Telescope (ORT)** can be transformed into astrophysical insights about the **Vela Pulsar** — one of the brightest and closest pulsars to Earth. It was my first experience in extensive data handling and analysis techniques.


From noisy voltage samples to clean pulsar profiles, we went through every step: analyzing noise, detecting pulses, correcting for interstellar dispersion, and finally measuring the pulsar’s rotation period.

---

## ⚙️ Signal Statistics
We first studied the **voltage data** from the telescope’s North and South apertures.  
As each voltage sample is the sum of many independent signals, the distribution follows a **Gaussian** form:

$$
X_{\text{new}} = \frac{X - \mu}{\sigma}
$$

Squaring the voltage gives the **power signal**, which follows an **exponential** distribution — confirming that the data contains primarily random Gaussian noise with embedded pulsar signals.

---

## 🎵 Frequency Domain Analysis
Using **Fast Fourier Transform (FFT)**, we explored the signal in frequency space (16.5 MHz bandwidth).  
Peaks in the power spectrum revealed both legitimate features and **Radio Frequency Interference (RFI)**.  
After detrending and time-averaging, we constructed the **dynamic spectrum**, where pulse arrival times clearly depend on frequency — a direct signature of **interstellar dispersion**.

---

## 🌠 Estimating the Dispersion Measure (DM)
Because radio waves at lower frequencies travel slower through the ionized interstellar medium, their arrival time is delayed.  
The relationship between time delay and frequency is given by:

$$
\tau = 4.149 \times 10^3 \times \text{DM} \times (\nu_1^{-2} - \nu_2^{-2})
$$

By fitting the pulse arrival times across different frequency channels, we obtained:

$$
\text{DM} = 72.77 \pm 0.74 \ \text{pc cm}^{-3}
$$

Assuming an average electron density  
$$n_e = 0.033 \ \text{cm}^{-3},$$  
the estimated distance becomes:

$$
d = \frac{\text{DM}}{n_e} = 2.18 \pm 0.24 \ \text{kpc}
$$

---

## 🕒 Measuring the Pulsar’s Time Period
After applying **dedispersion** (to align the frequency channels), we stacked the pulses and fitted each with Gaussian profiles.  
Plotting arrival time versus pulse number yielded a linear fit whose slope corresponds to the pulsar’s rotation period:

$$
T = 76.29 \pm 0.74 \ \text{ms}
$$

This matches closely with literature values, validating our numerical data analysis routine.

---

## 📈 Summary of Results we achieved:
| Quantity | Estimated Value | Literature Value | Notes |
|-----------|----------------|------------------|-------|
| Dispersion Measure (DM) | 72.77 ± 0.74 pc/cm³ | 67 pc/cm³ | Slight deviation due to noise and short observation |
| Time Period (T) | 76.29 ± 0.74 ms | 89.33 ms | Within expected range |
| Distance (d) | 2.18 ± 0.24 kpc | ~1 kpc | Depends on assumed electron density |





<!--more-->
