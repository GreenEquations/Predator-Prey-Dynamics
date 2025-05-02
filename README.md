# Predator-Prey Dynamics and Dynamic Carrying Capacity

## Overview
This repository contains a mathematical model extending the traditional Lotka-Volterra predator-prey model by introducing a **dynamically fluctuating carrying capacity**. The hypothesis is that instead of assuming a constant carrying capacity, fluctuations due to environmental factors (like seasonal changes or habitat shifts) influence the populations of predators and prey.

## Model Description
The dynamic predator-prey model incorporates a time-dependent carrying capacity \(K(t)\) that fluctuates according to the following equation:
\[
K(t) = K_0 \left( 1 + \lambda \cdot \sin(\omega t) + \varphi \cdot \cos(\omega t) \right)
\]
Where:
- \( K_0 \): Baseline carrying capacity
- \( \lambda \), \( \varphi \): Amplitude factors controlling the intensity of fluctuations
- \( \omega \): Frequency of oscillations (seasonal variations, etc.)

## Mathematical Model
The modified Lotka-Volterra equations are:
\[
\frac{dP}{dt} = \alpha P \left( 1 - \frac{P}{K(t)} \right) - \beta P Q
\]
\[
\frac{dQ}{dt} = \delta P Q - \gamma Q
\]
Where:
- \( P \): Prey population
- \( Q \): Predator population
- \( \alpha, \beta, \delta, \gamma \): Model parameters for growth and interaction rates

The modification with the dynamic carrying capacity \(K(t)\) adjusts the interaction terms based on the available resources, leading to the following equations:
\[
\frac{dP}{dt} = \alpha P \left( 1 - \frac{P}{K(t)} \right) - \beta P Q
\]
\[
\frac{dQ}{dt} = \delta P Q - \gamma Q
\]

## How to Use This Model
1. Clone the repository:
```bash
git clone https://github.com/your-username/predator-prey-dynamics.git