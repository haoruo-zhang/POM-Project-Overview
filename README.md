# Product-of-Measures (POM) Project — Code Overview

This repository serves as the **master index** for the research code associated with the *Product-of-Measures (POM)* framework for high-dimensional polynomial optimization.  
It links to the **public components** of the project, including the augmented Lagrangian baseline solver and the Nullstellensatz certificate verification used in the theoretical analysis.

Due to ongoing manuscript preparation, the implementation of the **full POM–Projected Gradient Descent (POM-PGD)** algorithm is **not publicly available**, but can be shared privately with faculty upon request.

---

## 🔹 1. Polynomial Optimization via Product Measure  
### *Augmented Lagrangian + Burer–Monteiro Moment Solver*  
👉 **https://github.com/haoruo-zhang/Polynomial-Optimization-via-Product-Measure**

This repository implements the **classical benchmark solver** used to validate moment relaxations:

- Multivariate polynomial utilities  
- Moment matrix and Hankel structure construction  
- Burer–Monteiro factorization  
  $$M_d = R R^\top$$
- Augmented Lagrangian constraint enforcement  
- Hand-written gradients for SciPy L-BFGS-B  
- PSD + Hankel projection via Dykstra  
- Serves as a baseline comparison for the POM-PGD algorithm (private)

This solver is fully self-contained and reproduces baseline behavior for polynomial optimization over the hypercube.

---

## 🔹 2. Nullstellensatz Certificate Verification  
### *Symbolic and Numerical Algebraic Verification*  
👉 **https://github.com/haoruo-zhang/Nullstellensatz-certificate**

This repository contains the tools used to verify **Nullstellensatz certificates** for polynomial systems arising in the POM framework:

- Construction of polynomial ideals  
- Gröbner basis–based certificate discovery  
- Symbolic consistency checks (SymPy)  
- Numerical evaluation on sampled grids  
- Verification of birank (2,1) and high-rank critical-point structures  
- Algebraic investigation of the incidence variety  

These routines support the theoretical part of the project by validating the algebraic structure of high-rank stationary points.

---

## 🔒 Private Repository (Available Upon Request)  
### **POM-PGD: Product-of-Measures Projected Gradient Descent Algorithm**

The core algorithm developed in the manuscript—including:

- Projected gradient dynamics on moment variables  
- Rank-one manifold geometry  
- Strict-saddle escape conditions  
- High-dimensional experiments and scaling laws  
- Chebyshev-type and random polynomial benchmarks  

is currently **private** due to ongoing manuscript preparation.  
Faculty may request access by email.

---

## 📄 Research Context

Together, these repositories support the computational and algebraic components of my work on:

- Moment relaxations for multivariate polynomials  
- Product-measure reformulation  
- Active rank-one moment manifolds  
- Strict-saddle avoidance in high-dimensional settings  
- Algebraic characterization of high-rank critical points  
- Nullstellensatz-based incidence variety analysis  

These codes reproduce the theoretical and numerical results used in the manuscript.

---

## 📬 Contact

If you would like access to the private POM-PGD implementation or have questions about the computational setup, feel free to contact me.

