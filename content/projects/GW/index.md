---
title: QNM of BH in environment
date: 2025-11-02
math: true
links:
  - type: site
    url: https://shiva123456789100.github.io/projects/gw/
tags:
  - Hugo
  - HugoBlox
  - Markdown
---

“When a black hole is struck, it starts to sing.  
Its dying echoes, are the purest notes in the symphony of spacetime.”

Perturbed black holes emit gravitational waves at very specific complex frequencies before being stabilized into ground state. These characteristics complex frequencies are known as **Quasi-Normal Modes** of black hole. The signal is called **Ringdown** signal. Ringdown signal is very important to extract information about the black hole mass, charge , angular momentum. 

# **Black Hole Perturbation Theory(BHPT)**  

## **1. Introduction**  

 A perturbed black hole emits gravitational waves carrying information about its internal geometry. The mathematical description of these perturbations can be formulated with as set of master equations — the **Regge–Wheeler**, **Zerilli**, and **Teukolsky** equations — which govern the evolution of such perturbations in Schwarzschild and Kerr solution of Einstein field equation.



### **2. Regge–Wheeler Equation (Axial Perturbations)**  

For a static (Schwarzschild) black hole, metric perturbations can be decomposed into **odd-parity (axial)** and **even-parity (polar)** parts based on their property under spatial inversion.  
The **Regge–Wheeler equation**, derived by T. Regge and J. A. Wheeler (1957), describes the axial perturbations.  

The expression for the Regge–Wheeler function $Q_\ell(t, r)$ is  

$$
\frac{\partial^2 Q_\ell}{\partial t^2} - \frac{\partial^2 Q_\ell}{\partial r_*^2} + V_{\text{RW}}(r) Q_\ell = 0,
$$

where the **tortoise coordinate** $r_*$ is defined by  

$$
\frac{dr_*}{dr} = \frac{1}{1 - \frac{2M}{r}},
$$

and the **Regge–Wheeler potential** can be written as   

$$
V_{\text{RW}}(r) = \left(1 - \frac{2M}{r}\right)
\left[\frac{\ell(\ell+1)}{r^2} - \frac{6M}{r^3}\right].
$$

This potential acts as a scattering barrier for gravitational waves near the black hole. The solutions represent oscillations that decay over time, known as **quasinormal modes (QNMs)**.  



### **3. Zerilli Equation (Polar Perturbations)**  

The **Zerilli equation**, derived by Frank Zerilli (1970), governs the **even-parity (polar)** perturbations of a Schwarzschild black hole. Despite being derived independently, the Zerilli and Regge–Wheeler equations are **isospectral**, meaning they share the same quasinormal mode frequencies.  

The equation for the Zerilli function \( \Psi_\ell(t, r) \) is

$$
\frac{\partial^2 \Psi_\ell}{\partial t^2} - \frac{\partial^2 \Psi_\ell}{\partial r_*^2} + V_Z(r)\Psi_\ell = 0,  
$$

where the **Zerilli potential** is  

$$
V_Z(r) = \frac{2(1 - 2M/r)}{r^3 (n r + 3M)^2}
\left[ n^2(n+1) r^3 + 3Mn^2 r^2 + 9M^2n r + 9M^3 \right],  
$$

with

$$
n = \frac{1}{2}(\ell - 1)(\ell + 2).
$$

Both \( Q_\ell \) and \( \Psi_\ell \) contain gauge-invariant information about gravitational perturbations and are essential for modeling gravitational wave emission from Schwarzschild black holes.  

---

### **4. Chandrasekhar Transformation**     

S. Chandrasekhar (1975) discovered a remarkable transformation connecting the Regge–Wheeler and Zerilli functions, demonstrating that the two equations are **physically equivalent**. This implies that both describe the same spectrum of quasinormal modes and contribute complementary perspectives on the same physical process — the oscillations of spacetime geometry.  
![QNM plots](plot.png)  



These equations can be solved [Leaver's method of continued fraction](https://arxiv.org/abs/1509.04260) or [WKB approximation](https://arxiv.org/abs/2503.17245).  

### **5. Teukolsky Equation (Kerr Perturbations)**  

For **rotating (Kerr)** black holes, due to reduced symmetry , the separation into even and odd parity mode doesn't remain possible. Instead, **Teukolsky (1973)** developed a unified formalism using the **Newman–Penrose (NP)** approach, which represents gravitational fields via complex scalar quantities.  

The **Teukolsky master equation** governs perturbations of fields with arbitrary spin \( s \) (scalar \( s=0 \), electromagnetic \( s=\pm1 \), and gravitational \( s=\pm2 \)) in the Kerr geometry.  

In Boyer–Lindquist coordinates, the equation reads:  

$$
\left[\frac{(r^2 + a^2)^2}{\Delta} - a^2 \sin^2\theta\right]\frac{\partial^2 \psi_s}{\partial t^2}+ \frac{4Mar}{\Delta}\frac{\partial^2 \psi_s}{\partial t \partial \phi}+ \left(\frac{a^2}{\Delta} - \frac{1}{\sin^2\theta}\right)\frac{\partial^2 \psi_s}{\partial \phi^2}- \Delta^{-s}\frac{\partial}{\partial r}\left(\Delta^{s+1}\frac{\partial \psi_s}{\partial r}\right)- \frac{1}{\sin\theta}\frac{\partial}{\partial \theta}\left(\sin\theta \frac{\partial \psi_s}{\partial \theta}\right)- 2s\left[\frac{a(r - M)}{\Delta} + \frac{i\cos\theta}{\sin^2\theta}\right]\frac{\partial \psi_s}{\partial \phi}- 2s\left[\frac{M(r^2 - a^2)}{\Delta} - r - i a \cos\theta \right]\frac{\partial \psi_s}{\partial t}+ (s^2 \cot^2\theta - s)\psi_s = 0
$$

where $\Delta = r^2 - 2Mr + a^2$, $a$ is the black hole spin parameter, and $\psi_s$ denotes the spin-weighted NP scalar (e.g., $\psi_0,\psi_4$ for gravitational waves).  

The Teukolsky equation can be **separated** into radial and angular parts, leading to **spin-weighted spheroidal harmonics**. It provides the theoretical foundation for modeling gravitational waves from Kerr black holes and underpins modern black hole perturbation codes used in numerical relativity.  

Interestingly, not only black holes stars also show similar kind of modes. A relativistic star can be shown to have a plethora of modes(see [Review](https://arxiv.org/abs/gr-qc/9909058)).  

## **Oscillation modes of star:**

### **1.f-mode (fundamental mode):**
   This is a surface mode that exists even in the absence of buoyancy or compressibility effects. Its frequency depends mainly on the star’s mean density and roughly scales as
               $$\omega_f^2\approx \frac{GM}{R^3}$$
   which, for neutron stars, corresponds to frequencies around 1–3 kHz with damping times due to gravitational radiation of about 0.1–0.3 seconds. The f-mode represents large-scale oscillations of the stellar fluid and is an efficient emitter of gravitational waves.

### **2.p-mode (pressure mode or acoustic mode):**  
 Here, pressure acts as the restoring force. These modes have higher frequencies than the f-mode and are less efficiently      damped. The oscillations are primarily  
  confined to the star’s interior, with nodes in the radial direction. The frequency increases with the order of the mode and with the stiffness of the equation of state
     
    

### **3.g-modes (gravity modes):**
  In these modes, buoyancy (or gravity) provides the restoring force. They generally occur in stably stratified regions         where density gradients exist. g-modes have lower frequencies and longer periods, typically associated with thermal or        compositional gradients within the star.


![QNM plots2](plot2.png)
   

### **4.r-modes(rotational modes):**
   The r-modes (rotational) in a non-rotating star are purely toroidal (axial) modes with vanishing frequency. In a rotating star, the displacement vector acquires spheroidal components and the frequency in the rotating frame, to first order in the rotational frequency $\Omega$ of the star, becomes
   $$\omega_{r}=\frac{2m\Omega}{\ell(\ell+1)}$$
   all r-modes with  $\ell\geq 2$ are generically unstable to the emission of gravitational radiation,
due to the Chandrasekhar-Friedman-Schutz (CFS) mechanism.

### **5.w-modes(spacetime modes)**
   The spacetime modes are perhaps the most crucial mode for all astrophysical application. These are modes are related to the spacetime curvature and exist for all relativistic star. They are higly damped modes. Damping rate is higly correlated with the compactness of star. Damping rate increases as compactness decreases. For nearly newtonian stars, it is very difficult to determine w-modes, as due to high damping numerical programs hit instability. These are very close to the quasi-normal modes.

  There are also trapped modes and interference modes. 

The anlysis of w-modes in relativistic stars start with analyzing spacetime through Tolman–Oppenheimer–Volkoff (TOV) equation.
The TOV equation governs hydrostatic equilibrium in a static, spherically symmetric relativistic star:

$$
\frac{dP(r)}{dr} = -\frac{G \left[\rho(r)c^2 + P(r)\right] \left[m(r) + 4\pi r^3 P(r)/c^2\right]}{r^2 \left[1 - \frac{2Gm(r)}{r c^2}\right]},
$$

with the mass continuity relation:

$$
\frac{dm(r)}{dr} = 4\pi r^2 \rho(r)
$$

and the total gravitational mass of the star:

$$
M = m(R) = 4\pi \int_0^R \rho(r) r^2 dr
$$

## Problem I have worked on:

I, with [Prof. Rajesh Kumble Nayak](https://www.iiserkol.ac.in/~rajesh/), have focused on an interesting problem.

1. If instead of considering an isolated BH, we consider a black hole embedded in a stationary spacetime background (In real world, there is isolated black hole, every black hole is in a environment) how the behavior of QNM spectra will change? Interestingly , we find one interesting application of our study in Primordial Black Hole(PBH) capture by neutron stars.
To describe , the captured PBH in background of NS , our study can be useful.


   


<!--more-->
