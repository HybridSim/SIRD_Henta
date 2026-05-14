# HSML SEIRD Dashboard
## Interactive Cruise Ship Hantavirus Outbreak Simulation

![HSML Dashboard](preview.png)

---

# Overview

The HSML SEIRD Dashboard is an interactive epidemiological simulation platform developed by the **Hybrid Simulation Modelling Lab (HSML)** for modeling infectious disease transmission dynamics in confined populations such as cruise ships.

The dashboard implements a deterministic **SEIRD (Susceptible–Exposed–Infectious–Recovered–Dead)** compartmental model inspired by the following research study:

> Cui, J. (2026). *Modeling the Impact of Exposed Cases in a Hantavirus Outbreak on a Cruise Ship*. arXiv:2605.07498v1.

The application enables real-time exploration of outbreak dynamics through adjustable epidemiological parameters and animated system dynamics visualizations.

---

# Features

## Interactive Controls
The dashboard includes adjustable sliders for:

- Transmission Rate (β)
- Latency Period (Z)
- Infectious Period (D)
- Fatality Rate (δ)
- Total Population
- Initial Exposed Population
- Initial Infectious Population
- Simulation Duration

---

## Real-Time Simulation
The simulation dynamically updates outbreak trajectories using animated epidemic curves.

---

## Epidemiological Visualizations

### 1. SEIRD Population Dynamics
Tracks:
- Susceptible population
- Exposed population
- Infectious population
- Recovered population
- Dead population

---

### 2. Hidden vs Identified Cases
Compares:
- Exposed (hidden) infections
- Infectious (identified) infections

---

### 3. Daily New Infections
Displays daily incident infections over time.

---

### 4. Phase Space Dynamics
Plots:
- Exposed population vs Infectious population

Used for:
- nonlinear epidemic trajectory analysis
- dynamical systems interpretation

---

### 5. Cumulative Cases
Displays cumulative outbreak growth over time.

---

# Mathematical Model

The dashboard implements the SEIRD compartmental system:

\[
\frac{dS}{dt} = -\beta \frac{SI}{N}
\]

\[
\frac{dE}{dt} = \beta \frac{SI}{N} - \frac{E}{Z}
\]

\[
\frac{dI}{dt} = \frac{E}{Z} - \frac{I}{D}
\]

\[
\frac{dR}{dt} = (1-\delta)\frac{I}{D}
\]

\[
\frac{dD}{dt} = \delta\frac{I}{D}
\]

Where:

| Symbol | Description |
|---|---|
| S | Susceptible population |
| E | Exposed population |
| I | Infectious population |
| R | Recovered population |
| D | Dead population |
| β | Transmission rate |
| Z | Latency period |
| D | Infectious duration |
| δ | Fatality rate |
| N | Total population |

---

# System Dynamics Interpretation

This model exhibits several classical System Dynamics archetypes:

- Reinforcing epidemic growth loops
- Limits to growth
- Delay structures
- Overshoot and collapse dynamics
- Stock-and-flow epidemic behavior

---

# Technology Stack

- HTML5
- CSS3
- JavaScript
- Plotly.js

---

# Research Context

This dashboard was developed as an educational and research-oriented visualization platform based on:

> Cui, J. (2026). *Modeling the Impact of Exposed Cases in a Hantavirus Outbreak on a Cruise Ship*. arXiv:2605.07498v1.

The original paper explored:
- hidden exposed populations
- stochastic SEIRD dynamics
- outbreak inference
- transmission estimation
- epidemiological uncertainty

This implementation provides an interactive deterministic visualization layer for educational and analytical purposes.

---

# Intended Use

This software is intended for:

- educational demonstrations
- epidemiological visualization
- system dynamics teaching
- outbreak modeling research
- simulation experimentation

---

# Disclaimer

This software is provided solely for educational, research, and visualization purposes.

The dashboard:
- does not constitute medical advice
- is not a clinical decision-support tool
- should not be used for operational public health response
- simplifies real-world epidemiological dynamics

Simulation outputs are dependent on user-defined parameters and modeling assumptions.

The Hybrid Simulation Modelling Lab (HSML) makes no guarantees regarding predictive accuracy or suitability for real-world outbreak management.

---

# Copyright Notice

© Hybrid Simulation Modelling Lab (HSML)

All Rights Reserved.

This software, visualizations, source code, documentation, and associated materials are protected under international copyright law.

Unauthorized reproduction, redistribution, modification, or commercial use without explicit written permission from HSML is prohibited.

---

# Citation

If using this dashboard in academic or research work, please cite:

```text
Hybrid Simulation Modelling Lab (HSML).
HSML SEIRD Dashboard: Interactive Cruise Ship Outbreak System Dynamic Simulation.
2026.
