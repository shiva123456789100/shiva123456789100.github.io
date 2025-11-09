---
title: Quasi-normal modes of Black Holes in non-static environment
date: 2025-11-02
math: true
links:
  - type: site
    url: https://github.com/pandas-dev/pandas
tags:
  - Hugo
  - HugoBlox
  - Markdown
---

“When a black hole is struck, it starts to sing.  
Its dying echoes, are the purest notes in the symphony of spacetime.”

Perturbed black holes emit gravitational waves at very specific complex frequencies before being stabilized into ground state. These characteristics complex frequencies are known as **Quasi-Normal Modes** of black hole. The signal is called **Ringdown** signal. Ringdown signal is very important to extract information about the black hole mass, charge , angular momentum. 

Interestingly, not only black holes stars also show similar kind of modes. A relativistic star can be shown to have a plethora of modes(see [Review](https://arxiv.org/abs/gr-qc/9909058)).

1. **f-mode (fundamental mode):**
   This is a surface mode that exists even in the absence of buoyancy or compressibility effects. Its frequency depends mainly on the star’s mean density and roughly scales as
               $$\omega_f^2\approx \frac{GM}{R^3}$$
   which, for neutron stars, corresponds to frequencies around 1–3 kHz with damping times due to gravitational radiation of about 0.1–0.3 seconds. The f-mode represents large-scale oscillations of the stellar fluid and is an efficient emitter of gravitational waves.

2. **p-modes (pressure or acoustic modes):**
     Here, pressure acts as the restoring force. These modes have higher frequencies than the f-mode and are less efficiently      damped. The oscillations are primarily confined to the star’s interior, with nodes in the radial direction. The frequency increases with the order of the mode and with the stiffness of the equation of state.

3. **g-modes (gravity modes):**
     In these modes, buoyancy (or gravity) provides the restoring force. They generally occur in stably stratified regions         where density gradients exist. g-modes have lower frequencies and longer periods, typically associated with thermal or        compositional gradients within the star.
   
5. **r-modes(rotational modes):**
     The r-modes (rotational) in a non-rotating star are purely toroidal (axial) modes with vanishing frequency. In a rotating star, the displacement vector acquires spheroidal components and the frequency in the rotating frame, to first order in the rotational frequency $\Omega$ of the star, becomes
   \[\omega_{r}=\frac{2m\Omega}{\ell(\ell+1)}\]
   all r-modes with  $ \ell\geq 2$ are generically unstable to the emission of gravitational radiation,
due to the Chandrasekhar-Friedman-Schutz (CFS) mechanism.

7. **w-modes(spacetime modes)**
    The spacetime modes are perhaps the most crucial mode for all astrophysical application. These are modes are related to the spacetime curvature and exist for all relativistic star. They are higly damped modes. Damping rate is higly correlated with the compactness of star. Damping rate increases as compactness decreases. For nearly newtonian stars, it is very difficult to determine w-modes, as due to high damping numerical programs hit instability. These are very close to the quasi-normal modes.

  There are also **trapped modes** and **interference modes**. 

  The master equation is given by

\[
\frac{d^2 \Psi_{\ell}^{s}}{dr_*^2} + \left[ \omega^2 - V_s \right] \Psi_{\ell}^{s} = 0,
\]
where
\[
V_s = f \left( \frac{\ell(\ell + 1)}{r^2} + \frac{2M(1 - s^2)}{r^3} \right)
     = f \left( \frac{\Lambda}{r^2} + \frac{2\beta}{r^3} \right).
\]

   


<!--more-->
