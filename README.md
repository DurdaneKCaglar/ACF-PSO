# Advanced Composite Fitness Particle Swarm Optimization: Achieving Theoretical Maximum Nonlinearity for S-box Design

## 📋 Table of Contents
- [Overview](#overview)
- [Data Structure](#data-structure)
- [Experiment Types](#experiment-types)

## 🔍 Overview

This repository contains experimental results for [brief description of your project]. The repository includes 4 distinct categories of experiments designed to evaluate [your research goal].

## 📁 Data Structure
```
experiments
├── main_experiments/     # Main experiments (30 cases × 3 files)
├── weight_sensitivity/   # Weight sensitivity analysis (3 weights × 3 initals × 5 runs × 3 files)
├── ablation/             # Ablation study (5 stages × 5 runs × 3 files)
├── multiple_runs/        # Multiple run tests (5 cases × 10 iterations × 3 files)
├── README.md
└── LICENSE
```

## 1. Main Experiments (`main_experiments/`)
- **Total Runs:** 30
<!--- **Purpose:** [Purpose of your main experiments]-->

<!--#### File Naming Convention
```
run_001/
  ├── output_1.txt  # [Description of content]
  ├── output_2.txt  # [Description of content]
  └── output_3.txt  # [Description of content]
```-->

#### Description
The main experiments evaluate. Each run represents an independent trial with multiply initials.

## 2. Weight Sensitivity Analysis (`weight_sensitivity/`)
- **Weight Values:** 3 different values
  - **1 - NL Dominant Values:** w_nl = 0.70, w_sac = 0.20, w_ddt = 0.10 
  - **2 - SAC Dominant Values:** w_nl = 0.15, w_sac = 0.70, w_ddt = 0.15 
  - **3 - DDT Dominant Values:** w_nl = 0.10, w_sac = 0.20, w_ddt = 0.70 
- **Runs per Weight:** 5
- **Total Runs:** 45
- **Purpose:** Analyze the impact of different weight parameters on model performance

<!--#### Folder Structure
```
weight_0.1/
  ├── run_001/
  │   ├── output_1.txt
  │   ├── output_2.txt
  │   └── output_3.txt
  └── ... (up to run_005)
weight_0.5/
  └── ... (same structure)
weight_1.0/
  └── ... (same structure)
```-->


## 3. Ablation Study (`ablation/`)
- **Number of Stages:** 5
- **Runs per Stage:** 5 different runs for 5 diffrent initials
- **Total Runs:** 116
- **Purpose:** Systematically evaluate the contribution of individual model components

#### Stages
- **V1:** Baseline model
- **V2:** Without Composite Fitness
- **V3:** Without Triple Swap
- **V4:** Without Perturbation
- **V5:** Without Guided Swap

<!--#### Folder Structure
```
stage_1/
  ├── run_001/
  │   ├── output_1.txt  # Training metrics
  │   ├── output_2.txt  # Validation metrics
  │   └── output_3.txt  # Test metrics
  └── ... (up to run_005)
```-->

## 4. Multiple Run Tests (`multiple_runs/`)
- **Execution Method:** 5 differebt run is executed 10 consecutive times
- **Purpose:** Test model stability and reproducibility across repeated executions


## 🔧 Requirements
```
Julia v1.11.2

ProgressMeter v1.11.0
Random v1.11.0
Statistics v1.11.1
Distributed v1.11.0
Dates v1.11.0
Printf v1.11.0
Base.Threads (Julia core)
```

## 📧 Contact

[Durdane (Kocacoban) Caglar] - [dk796@alumni.york.ac.uk]

[Ibrahim Caglar] - [ibrahimcaglar@alumni.york.ac.uk]
