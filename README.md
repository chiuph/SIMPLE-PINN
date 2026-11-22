# SIMPLE-PINN

[![python >3.8](https://img.shields.io/badge/python-3.8-brightgreen)](https://www.python.org/) 

## **Bridging Computational Fluid Dynamics Algorithm and Physics-Informed Learning: SIMPLE-PINN for Incompressible Navier-Stokes Equations**

__Chang Wei, Yuchen Fan, Chin Chun Ooi, Jian Cheng Wong, Heyang Wang, Pao-Hsiung Chiu__



_Physics-informed neural networks (PINNs) have shown promise for solving partial differential equations (PDEs) by directly embedding them into the loss function. Despite their notable success, existing PINNs often exhibit training instability and slow convergence when applied to strongly nonlinear fluid dynamics problems. To address these challenges, this paper proposes a novel PINN framework, named as SIMPLE-PINN, which incorporates velocity and pressure correction loss terms inspired by the semi-implicit pressure link equation. These correction terms, derived from the momentum and continuity residuals, are tailored for the PINN framework, ensuring velocity-pressure coupling and reinforcing the underlying physical constraints of the Navier-Stokes equations. Through this, the framework can effectively mitigate training instability and accelerate convergence to achieve accurate solution. Furthermore, a hybrid numerical-automatic differentiation strategy is employed to improve the model's generalizability in resolving flows involving complex geometries. The performance of SIMPLE-PINN is evaluated on a range of challenging benchmark cases, including strongly nonlinear flows, long-term flow prediction, and multiphysics coupling problems. The numerical results demonstrate SIMPLE-PINN's high accuracy and rapid convergence. Notably, SIMPLE-PINN achieves, for the first time, a fully data-free solution of lid-driven cavity flow at Re=20000 in just 448s, and successfully captures the onset and long-time evolution of vortex shedding in flow past a cylinder over t=0-100. These findings demonstrate SIMPLE-PINN's potential as a reliable and competitive neural solver for complex PDEs in intelligent scientific computing, with promising engineering applications in aerospace, civil engineering, and mechanical engineering._

# Install
[![jax-0.4.33](https://img.shields.io/badge/jax-0.4.33-yellowgreen)](https://github.com/google/jax) [![evojax-0.2.17](https://img.shields.io/badge/evojax-0.2.17-orange)](https://github.com/google/evojax) [![evosax-0.1.6](https://img.shields.io/badge/evosax-0.1.6-red)](https://github.com/RobertTLange/evosax) [![flax-0.9.0](https://img.shields.io/badge/flax-0.9.0-lightgrey)](https://github.com/google/flax) [![optax-0.2.3](https://img.shields.io/badge/optax-0.2.3-blue)](https://github.com/google-deepmind/optax) [![numpy-2.1.1](https://img.shields.io/badge/numpy-2.1.1-green)](https://github.com/numpy/numpy) [![pandas-2.2.3](https://img.shields.io/badge/pandas-2.2.3-yellow)](https://github.com/pandas-dev/pandas) [![matplotlib-3.9.2](https://img.shields.io/badge/matplotlib-3.9.2-purple)](https://github.com/matplotlib/matplotlib)


# Usage
You can download this repo and run the demo tasks on your computing machine.

# Time cost
Typical install time should be under 30min for all the above packages.

Expected time required for training in the provided scripts on a workstation with Intel Xeon W-2275 CPU and Nvidia Gefore RTX 3090 GPU is tabulated as follows:
| Problem | Time |
|:-----|-----:|
| 01. Lid-Driven Cavity | 450s|
| 02. Wavy Channel |  200s|
| 03. NACA0012_airfoil | 400s|
| 04. Flow past three squares | 340s|
| 05. Flow past cylinder | 7000s|
| 06. Rayleigh-Taylor instability | 6400s|


# Citation

Chang Wei, Yuchen Fan, Chin Chun Ooi, Jian Cheng Wong, Heyang Wang, Pao-Hsiung Chiu, _"Bridging Computational Fluid Dynamics Algorithm and Physics-Informed Learning: SIMPLE-PINN for Incompressible Navier-Stokes Equations"_. [https://arxiv.org/abs/2312.03243](https://arxiv.org/abs/2603.24013)
