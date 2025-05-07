# 📘 Dynamic Predator-Prey Theorem: Fluctuating Carrying Capacity

## I. Theorem Statement

In predator-prey ecosystems, when the environmental carrying capacity becomes time-dependent, the system no longer stabilizes at fixed equilibrium points.

Let:

- K(t): Time-dependent carrying capacity
- P(t): Prey population
- Q(t): Predator population

Then, for a system with non-constant K(t), the equilibrium points become dynamic and shift over time, stabilizing below the traditional fixed carrying capacity.

---

## II. Model Equations

### Dynamic Carrying Capacity
A sinusoidal carrying capacity:

    K(t) = K₀ * (1 + λ * sin(ωt) + φ * cos(ωt))

Where:
- K₀: Baseline carrying capacity
- λ, φ: Amplitude parameters
- ω: Frequency of oscillation

### Modified Lotka-Volterra Equations

    dP/dt = αP * (1 - P / K(t)) - βPQ  
    dQ/dt = δPQ - γQ

Where:
- α: Prey growth rate
- β: Predation rate
- δ: Predator growth rate per consumed prey
- γ: Predator mortality rate

---

## III. Equilibrium Behavior

Given K(t) is fluctuating:

- Equilibrium prey population:

      P*(t) = (α * K(t)) / (β + γ)

- Equilibrium predator population:

      Q*(t) = (δ * α * K(t)) / (β(γ + δ))

Thus, both P*(t) and Q*(t) become **functions of time** and shift with K(t).

---

## IV. Predictions

1. Populations stabilize **below** fixed K₀ in environments with seasonal or fluctuating resources.
2. Oscillations in P and Q match the frequency ω of the carrying capacity K(t).
3. Empirical populations in dynamic environments match this model more closely than fixed-K models.

---

## V. Simulation Suggestions

- Simulate using numerical ODE solvers (e.g., Euler, Runge-Kutta)
- Track P(t) and Q(t) over time with sinusoidal K(t)
- Validate against real-world data (e.g., marine or wildlife ecosystems)

---

## VI. Applications

- **Ecology**: More realistic models of population fluctuation
- **Conservation**: Predicting collapse under environmental stress
- **Systems Biology**: Modeling coupled systems with time-dependent resources