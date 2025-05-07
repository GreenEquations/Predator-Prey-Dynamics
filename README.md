# 📘 Dynamic Predator-Prey Theorem: Fluctuating Carrying Capacity

## I. Theorem Statement

In predator-prey ecosystems, when the environmental carrying capacity becomes time-dependent, the system no longer stabilizes at fixed equilibrium points.

Let:
- K(t): Time-dependent carrying capacity
- P(t): Prey population
- Q(t): Predator population

Then for a system with non-constant K(t), the equilibrium points become dynamic and shift over time, stabilizing below the traditional fixed carrying capacity.

---

## II. Model Equations

**Dynamic Carrying Capacity:**

    K(t) = K0 * [1 + λ * sin(ωt) + φ * cos(ωt)]

Where:
- K0: Baseline carrying capacity
- λ, φ: Amplitude parameters
- ω: Frequency of oscillation

**Modified Lotka-Volterra Equations:**

    dP/dt = α * P * (1 - P / K(t)) - β * P * Q  
    dQ/dt = δ * P * Q - γ * Q

Where:
- α: Prey growth rate
- β: Predation rate
- δ: Predator growth rate per consumed prey
- γ: Predator mortality rate

---

## III. Equilibrium Behavior

Given K(t) is fluctuating:

**Equilibrium Prey Population:**

    P*(t) = (α * K(t)) / (β + γ)

**Equilibrium Predator Population:**

    Q*(t) = (δ * α * K(t)) / [β * (γ + δ)]

Thus, both P*(t) and Q*(t) are functions of time and shift with K(t).

---

## IV. Predictions

1. Populations stabilize **below** fixed K0 in environments with seasonal or fluctuating resources.
2. Oscillations in P(t) and Q(t) will follow the frequency ω of K(t).
3. Real-world ecosystems with dynamic resources match this model more closely than static-K models.

---

## V. Simulation Suggestions

- Use numerical ODE solvers (Euler or Runge-Kutta)
- Simulate time series of P(t) and Q(t) using sinusoidal K(t)
- Compare with empirical ecological population data

---

## VI. Applications

- **Ecology**: Improved modeling of population cycles
- **Conservation**: Predicting population collapse under environmental stress
- **Biological Systems**: Modeling time-varying resource constraints