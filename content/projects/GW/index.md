---
title: "Topology and geometry in QM and Anomalies in QFT"
date: 2025-11-02
math: true
links:
  - type: site
    name: "Notes (Incomplete)"
    url: https://drive.google.com/file/d/1O4Da5GUWpglPMasa7263h4OKIPWp_9S2/view?usp=sharing
  - type: site
    name: "Slides for Anomaly"
    url:  https://drive.google.com/file/d/1xiNKNd4Z7bbfSs3cH8g9xQcQdW9kaCxP/view?usp=sharing
---

Geometry and Physics are like inseparable couple of Romeo and Juliet. Classical mechanics begins from the geomtry of the phase space and goe on to general relativity , which connects the geometry of spacetime with dynamics of heavenly bodies.  

The relation between quantum mechanics and geometry are not generally explored in a typical undergrad curriculum. But, with the advent of quantum information theory , the geometry has given us a new perspective to look at the quantum mechanical entanglement. The geometry of Hilbert space, is very mathematically elegant. It connects differential geometry, symplectic geometry , group extension and what not!


The story starts with the space of density matrix and Dirac-Von Neumann axioms of QM.  
1.Physical states are identified with trace-class positive operators $\rho$ of trace one.(known as density matrices)  
2.Physical observables are identified with self-adjoint operators. We denote the set of self-adjoint operators by $\mathbb{O}$.  
3.**Born rule:** When measuring the observable $\mathbb{O}$ in a state $\rho$ the probability of measuring value $e\in E \in \mathbb{R} $,  where E is a Borel-measurable subset of $\mathbb{R}$ is  
   $$P_{\rho,O}(E)=Tr P_{O}(E)\rho$$  
Here PO is the projection-valued-measure associated to the self-adjoint operator O by the spectral theorem.

   Every quantum state can be effectively represented by a density operator and the space of pure states $\rho^2=\rho$ can be shown to be isomorphic to $\mathcal{CP}^{N-1}$. This projective space can be shown to support an inetersting metric **Fubini-Study metric**. This metric also can be shown to be equivalent to overlap functions we used in quantum mechanics. This $\mathcal{CP}^{N}$ is Kahler and symplectic manifold.  

   
   The Fubini-study metric can be shown to be equivalent to **Fisher-Rao metric** in statistical probability theory. The distance between two density operators $\rho_1$ and $\rho_2$ can be written as  
   $$D(1,2) = \frac{1}{2} Tr(\rho_1-\rho_2)^2 $$  

   
  Now, the power of this approach lies in the analysis of entangled states. $\mathcal{CP}^{N}\bigotimes\mathcal{CP}^{M}$ can be shown (I independently was able to do the proof, click on the link on top of the page to see notes) as **Segre embedded** manifold of $\mathcal{CP}^{N+M-1}$.  


  Symmetry groups are another interesting hunting ground of geoemtry in physics. Weinberg QFT vol-I's 2nd chapter is a **MUST** for anyone who wants to understand the power of symmetry. We, in this project started our exploration with the difference between classical symmetry group and quantum symmetry group.  

  The symmetry group of lagrnagian is called classical symmetry group and when that symmetry trnasformations are represented by unitary operator , that gives birth to quantum symmetry group. For example, Dirac lagrangian and Dirac equation is invariant of classical rotation. The classical symmetry group related to rotation is just $SO(3)$. But, when rotation is represented by unitary operator parametrized by $\theta$, then the quantum symmetry group becomes $SU(2)$. This can be studied by **group extensions**.(see notes for more).


The group extension becomes an important tool analyze anomolies in QFT. There are two types of anomalies in QFT  
1. **ABJ anomaly:** This happens when classical symmetry group after quantisation  no more remains as a symmetry .For classical EM field coupled with massless Dirac spinors, $$U_V(1)\times U_A(1)$$ is the global
symmetry group or symmetry group of the lagrangian as there are two expected to be conserved current i.e. axial current and vector current. But , in quantum symmetry group, we  observe that $U_A(1)$ is no more a symmetry after quantisation.

2.**'t Hooft Anomaly:** ’t Hooft anomaly is said to be the obstruction that doesnot allow the global symmetry G to be realised as the local gauge transformation. Consider a QFT theory $\mathbf{T}$ with Global Symmetry(Symmetry of lagrangian) group G coupled with background G-gauge field A.  
Now, we say that $\mathbf{T}$ has a ’t Hooft anomaly if and only if
$$\mathbf{Z}[A^g]=\mathbf{Z}[A]\exp{i\mathbf{A}(\alpha,A})$$  
where $A \to A^g$ is G-gauge transformation and $\mathbf{A}$ cannot be countered by another terms.


We explore the 't Hooft anomaly in the context of charged scalar in the ring coupled with a background U(1)gauge field. The analysis invoke's Witten's topological-$\theta$ term, Chern-Simons theory, symmetry breaking and what not!! Please take alook at the **SLIDES**(at the top of the page) of my presentation if you find the topic interesting.

  


<!--more-->
