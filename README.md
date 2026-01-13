# Explainable Sustainability Assessment and Optimization Framework for Toluene HDA Process
Overview

<img width="1193" height="712" alt="image" src="https://github.com/user-attachments/assets/ae1d8f72-0d16-40ca-917c-ac6057f7beee" />

This project presents a data-driven and explainable framework for the sustainability assessment and optimization of a full toluene hydrodealkylation (HDA) flowsheet, integrating global sensitivity analysis (GSA), surrogate modeling, and Bayesian optimization (BO) within a composite Life-Cycle Sustainability Index (LCSI) framework.

The methodology is designed to address the intrinsically coupled and multi-objective nature of process-level sustainability, simultaneously considering economic, environmental, social, and technological performance metrics, while maintaining high computational efficiency.

Methodology

A high-fidelity HDA flowsheet producing 100 kt/yr of ultra-high-purity benzene (99.99 wt%) was developed in Aspen HYSYS and systematically analyzed.

Key methodological components include:

Composite LCSI formulation integrating 7 sustainability indicators
(economic: TOC, ACC; environmental: CO₂, SO₂, NOₓ; social: process risk index; technological: exergy efficiency)

Perturbation-based global sensitivity analysis to reduce the decision space from 14 variables to a compact set of critical operating parameters using only 106 converged simulations

ANN-based surrogate models trained on the reduced parameter space with high predictive accuracy

Explainable AI (SHAP) analysis to identify dominant sustainability drivers and nonlinear trade-offs

GSA-enhanced ANN-assisted Bayesian optimization for efficient multi-objective decision-making

Key Results

ANN surrogate models achieved MAPE below 1.0% for all sustainability indicators, with R² exceeding 0.995 for most outputs

<img width="958" height="845" alt="image" src="https://github.com/user-attachments/assets/ea3844ef-9049-43c6-999a-083d3558ac60" />

SHAP analysis revealed that purge ratio, reactor operation mode, and feed temperature dominate sustainability performance, while separation-related parameters play secondary roles

<img width="850" height="819" alt="image" src="https://github.com/user-attachments/assets/bf70826e-1554-4ed3-9fd7-e7e4aa1dd317" />

Surrogate-assisted Bayesian optimization improved the composite LCSI by 17.1% relative to nominal operation

Compared with simulation-based optimization, the proposed framework achieved a ~99% reduction in computational cost, while maintaining solution deviations within a few percent

Robustness Analysis

The optimized operating conditions were further evaluated under time-varying electricity prices and grid emission factors in Singapore (2005–2024). Results demonstrate that the improved sustainability performance remains relatively stable across evolving energy-system conditions, indicating that the LCSI framework effectively reconciles competing economic and environmental drivers.


Significance

This work demonstrates that explainable, surrogate-assisted sustainability optimization can provide mechanistically consistent insights beyond black-box optimization while dramatically reducing computational burden. The proposed GSA–ANN–BO framework offers a scalable and reliable tool for:

Process-level sustainability assessment

Energy- and emission-aware operation optimization

Decision support in chemical reaction engineering systems

Future Work

Future extensions will focus on:

Structural process modifications and process intensification

Energy-intensive separation units using mechanical and fluid vapor recompression (MVR/FVR)

Exploiting peak–off-peak electricity price and emission variability

Evaluating thermal energy storage–integrated FVR configurations

These developments aim to further enhance the industrial relevance of computationally efficient and explainable sustainability optimization.
