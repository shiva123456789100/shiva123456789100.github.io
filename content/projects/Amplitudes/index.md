---
title: MS Thesis- Gravitational physics from amplitudes
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

"Have u heard the birthcry of cosmos?   
Not of light, but of trembling spacetime itself —  
the faint ripple of creation, echoing across eons,  
carrying the memory of colliding stars,  
of black holes entwined in their final dance.  "


First observation of **gravitational waves** from a binary black hole in 2015 and hundreds of observations since then has given us new ears tuned to the silent music of spacetime, the unsung sagas of cosmos.
![Merging black holes simulated by numerical relativity](image.png)
Accurate and precise modeling of the gravitational waves emitted during merger or scattering events are essential to detect the signal and infer properties of the compact object accurately. Theoretical modeling combines both analytical(fast but approximate) and numerical (slow but accurate) techniques to analyze Einstein's field equation.


In recent years, physicists have turned to Feynman-diagrammatic frameworks, bringing the ammunation of modern amplitude techniques, originally developed for precise collider scattering experiment - into the realm of gravitational physics.
[Nima Arkani Hamed et al](https://arxiv.org/abs/1906.10100) has showed that an interaction between a test particle and Kerr Black hole can be modeled from the scattering amplitude of minimally coupled spin-s field and a scalar field at $s\to\infty$ limit. The authors have computed the momentum kick first for electromagnetic analogue of Kerr ($\sqrt{\text{Kerr}}$ BH) and then used double copy relation to derive the impusle for gravitational interaction (Kerr BH). [Spin universality](https://arxiv.org/abs/2207.03947) allows us to compute the spin s-spin s field four point amplitude and five point amplitudes(at LO) for conservative and radiation sector computation and classical limit will give us desired classical observable upto $(\mathcal(O)^{2s})$. The coefficient of $(\mathcal(O)^{2s})$ for any $s\in\mathcal{N}$ doesn't depend on s.

![Merging black holes simulated by numerical relativity](BlackHole.png)

The machinary of computing classical limit from amplitude was already at our disposal, in form of [KMOC](https://arxiv.org/abs/1811.10950) formalism. [Nima Arkani Hamed et al](https://arxiv.org/pdf/1709.04891) equipped us with all possible massive-massive-graviton/photon three point functions. Thus, all the collider caculations have found a new hunting ground. 

In my MS thesis,with Prof. Arnab Rudra , IISER Bhopal,we are trying to address a few related queries and issues under this broad theme:  
1. Although computationally robust enough to be widely applicable, KMOC prescription has some conceptual pitfalls. Inconsistent restoration of $\hbar$ and lack of convincing arguments about cancellation of superclassical terms at higher order are two biggest issue.  
2. WQFT,EFT prescriptions have been able to model the neutron star-neutron star mergers in addition to BH mergers. But , classical limit of amplitudes only have focused on minimally copuled higher spin fields till now, which gives BH scattering. So, the natural question arises what can be done to extend the framework for any general spinning compact object?


**Want to know about amplitudes: I am creating an online course page for u, where you will carry the same journey with me**  
      [Scattering amplitudes](https://shiva123456789100.github.io/courses/hugo-blox/)



<!--more-->
