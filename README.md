<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a3a5c,100:0d1117&height=120&section=header&text=&animation=fadeIn" width="100%"/>

# Akhilesh Yadav

### Applied Mathematician · Numerical PDEs · Scientific Machine Learning

**`M.Sc. Applied Mathematics — IIEST Shibpur`**

[![Email](https://img.shields.io/badge/Email-akhileshyadav.maths%40gmail.com-0d6efd?style=flat-square&logo=gmail&logoColor=white)](mailto:akhileshyadav.maths@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-akhileshyadav1598-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akhileshyadav1598)
[![MathLumen](https://img.shields.io/badge/MathLumen-mathlumen.com-1a3a5c?style=flat-square&logo=academia&logoColor=white)](https://mathlumen.com)
[![arXiv](https://img.shields.io/badge/arXiv-Preprints-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org)

</div>

---

## Research Profile

Applied mathematician working at the intersection of **numerical analysis**, **reduced-order modelling**, and **scientific machine learning**.
Research focuses on structure-preserving model reduction for parametric PDEs, *a posteriori* error certification for neural PDE solvers, and Bayesian inverse problems with surrogate-accelerated uncertainty quantification.
Experienced in finite element methods, physics-informed neural networks, and computational fluid dynamics.
Seeking a **fully funded PhD** to develop mathematically rigorous, ML-enhanced numerical methods for complex physical systems.

---

## Preprints & Publications

> Two independent research preprints submitted to **arXiv:math.NA** (2026)

**[P1]** A. Yadav — *"Energy-Preserving POD-Galerkin Reduced-Order Models with Neural Closure Corrections for Parameterized Navier–Stokes Equations"* — arXiv:26XX.XXXXX, 2026
- Proved discrete energy inequality for ROM with neural closure; derived computable *a posteriori* error bounds for the coupled system
- Demonstrated long-time stability on lid-driven cavity (Re = 100–500) and flow past cylinder benchmarks

**[P2]** A. Yadav — *"Residual-Based A Posteriori Error Bounds for PINN Solutions of Elliptic PDEs in Sobolev Norms"* — arXiv:26XX.XXXXX, 2026
- Derived rigorous H¹ error bounds with explicit constants via Riesz representer approach
- Achieved near-optimal effectivity indices η ≈ 1.1–1.4 on Poisson, variable-coefficient, L-shaped domain, and convection-dominated benchmarks

---

## Research Interests

```
Structure-preserving reduced-order models for parametric PDEs
A posteriori error estimation and certification for neural PDE solvers
Bayesian inverse problems with learned surrogates and certified UQ
Hybrid FEM–neural operator methods with convergence guarantees
Neural operators on complex geometries with geometric priors (FEEC)
Computational fluid dynamics
```

---

## Research Projects

### [P1] Energy-Preserving POD-ROM with Neural Closures for Navier–Stokes
`2026` · `ArXiv Paper #1` · `FEniCS` · `PyTorch` · `POD/Galerkin`

Constructed POD-Galerkin ROM for parameterized incompressible Navier–Stokes with energy-constrained neural closure enforcing discrete energy inequality `dE/dt ≤ −ν‖∇uᵣ‖²`. Proved long-time boundedness theorem; derived *a posteriori* error bounds decomposing POD truncation and closure approximation errors. Validated on 2D benchmarks where standard POD-ROM diverges at T → ∞.

---

### [P2] A Posteriori Error Certification for Physics-Informed Neural Networks
`2026` · `ArXiv Paper #2` · `FEniCS` · `PyTorch` · `Functional Analysis`

Derived computable H¹ error bounds for PINN solutions of elliptic PDEs: `‖u − û‖₁ ≤ Cₚ‖r‖₋₁` with explicit Poincaré and coercivity constants. Implemented residual dual-norm evaluation via auxiliary FEM solve. Demonstrated that training loss is unreliable: PINN with low training loss had true error 10× larger than estimated bound predicted.

---

### [P3] Bayesian Inversion for Diffusion Coefficient via PINN Surrogates
`2026` · `emcee` · `PyMC` · `Bayesian UQ`

Formulated Bayesian inverse problem for spatially varying diffusion coefficient recovery from noisy observations. Implemented MCMC posterior sampling with PINN forward surrogate vs. FEM forward model. Quantified surrogate-induced posterior error via Wasserstein-2 distance.

---

### [P4] Finite Element Solver Suite with Convergence Verification
`2025–2026` · `NumPy` · `SciPy` · `FEM from scratch`

Implemented P1 and P2 Lagrange FEM from scratch on unstructured triangular meshes. Verified optimal convergence rates O(h), O(h²) for P1 and O(h²), O(h³) for P2, matching Brenner–Scott theory. Performed condition number analysis and mesh refinement studies.

---

### [P5] DeepONet and FNO Benchmarking on Non-Rectangular Domains
`2026` · `DeepONet` · `FNO` · `NumPy/SciPy` · `Non-trivial geometry`

Benchmarked DeepONet-RFF and FNO-POD on parametric elliptic PDEs on L-shaped, annular, and perforated domains. Identified systematic failure at re-entrant corner singularities (u ~ r²/³): DeepONet shows **7.4× error amplification** near the corner. Demonstrated FNO achieves 0.03–4.4% in-distribution L² error but degrades 7–17× OOD vs. DeepONet's 1.2–2.5×. Proposed domain decomposition preprocessing as mitigation.

| Domain | Model | Test L² | OOD L² | OOD Factor |
|---|---|---|---|---|
| L-shaped | DeepONet-RFF | 16.1% | 40.2% | 2.5× |
| L-shaped | FNO-POD | **0.03%** | 0.49% | 17× |
| Annular | DeepONet-RFF | 35.9% | 41.2% | **1.2×** |
| Annular | FNO-POD | **0.74%** | 8.2% | 11× |

---

## Technical Skills

#### Numerical Methods
`Finite Element Methods (FEniCS/Firedrake)` · `Finite Differences` · `Finite Volumes` · `POD/Galerkin ROM` · `Spectral Methods`

#### Scientific Machine Learning
`PINNs` · `DeepONet` · `FNO` · `Neural Closure Models` · `PyTorch` · `Automatic Differentiation` · `Loss Landscape Analysis`

#### Bayesian / Uncertainty Quantification
`MCMC (emcee, PyMC)` · `Polynomial Chaos Expansions` · `Gaussian Processes` · `Bayesian Optimization`

#### Scientific Computing
`Python (NumPy, SciPy, Matplotlib)` · `MATLAB` · `LaTeX` · `Git/GitHub` · `Jupyter`

#### Mathematical Foundations
`Sobolev Spaces` · `Weak Formulations` · `A Priori/A Posteriori Error Analysis` · `Functional Analysis` · `Measure Theory`

---

## Self-Directed Advanced Study

| Book | Author | Chapters Studied |
|---|---|---|
| *Partial Differential Equations* | L. C. Evans | Ch. 1–10: Sobolev spaces, elliptic/parabolic/hyperbolic theory |
| *The Mathematical Theory of Finite Element Methods* | Brenner & Scott | Ch. 1–8: FEM error analysis, Aubin–Nitsche |
| *Finite Volume Methods for Hyperbolic Problems* | R. J. LeVeque | Conservation laws, Riemann solvers |
| *Uncertainty Quantification* | R. C. Smith | Full text |
| *Approximation of Large-Scale Dynamical Systems* | A. C. Antoulas | Balanced truncation, Krylov, SVD-based ROM |
| *Inverse Problems: A Bayesian Perspective* | A. M. Stuart (Acta Numerica 2010) | Full survey |

---

## Education

**M.Sc. Applied Mathematics** · IIEST Shibpur · 2022–2024 · CGPA 8.15/10  
Specialization: Fluid Mechanics & Numerical Methods  
Coursework: Advanced Fluid Mechanics · PDEs · Numerical Analysis · Linear Algebra · Probability & Statistics · Functional Analysis  

**B.Sc. Mathematics & Physics** · VBSPU Jaunpur · 2018–2021

---

## MathLumen

I am building **[MathLumen](https://mathlumen.com)** — an academic platform bridging rigorous mathematical foundations with modern scientific machine learning, PINNs, and physics-informed modeling. The platform is aimed at researchers and graduate students working at the intersection of numerical analysis and deep learning.

---

## Open to Research Collaboration

I am open to academic collaboration in:
- Scientific Machine Learning & operator learning
- A posteriori error estimation for neural PDE solvers
- Structure-preserving reduced-order models
- Bayesian inverse problems and certified UQ
- Hybrid FEM–neural operator methods

📧 [akhileshyadav.maths@gmail.com](mailto:akhileshyadav.maths@gmail.com)

---

<div align="center">

*"The goal of numerical analysis is not merely to compute answers, but to understand when and why those answers are correct."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a3a5c,100:0d1117&height=80&section=footer" width="100%"/>

</div>
