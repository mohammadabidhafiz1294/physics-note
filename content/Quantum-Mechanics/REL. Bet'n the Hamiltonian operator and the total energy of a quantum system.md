---
title: Hamiltonian Operator & Total Energy Relation of a Quantum System
tags:
  - physics/hamiltonian-Operator
  - quantum-mechanics/schrödinger-equation
---
#### The Hamiltonian: The Architect of Quantum Energy

The Hamiltonian-Operator (Ĥ) is the cornerstone of quantum mechanics when it comes to understanding the energy of a system. It acts as a mathematical representation of the **total energy**, encompassing both the kinetic and potential energy contributions. The sources illuminate the profound connection between the Hamiltonian operator and a system's total energy through the lens of the time-independent Schrödinger equation ( #TISE ).

- The TISE, written as **$Ĥψ(x) = Eψ(x)$**, is not just an equation; it's a declaration of the Hamiltonian's role as the arbiter of allowed energy levels.
    - The **eigenfunctions** of the Hamiltonian, denoted by ψ(x), represent the system's possible states, and their corresponding **eigenvalues (E)** reveal the quantized energy levels the system can occupy.
    - Solving the TISE is equivalent to unraveling the secrets of the Hamiltonian—finding its eigenfunctions and eigenvalues.

The sources provide explicit forms of the Hamiltonian operator, bridging the gap between classical and quantum realms:

- In one dimension: 
$$Ĥ = -(ħ²/2m) ∂²/∂x² + V$$
    - This mirrors the classical Hamiltonian 
    $$H(x, p) = (p²/2m) + V(x)$$, where the momentum (p) is replaced by its quantum operator counterpart **$-iħ ∂/∂x$**.
- In three dimensions: **$$Ĥ = -(ħ²/2m) ∇² + V$$
    - The Laplacian operator (∇²) steps in to account for the spatial complexity.

The sources further emphasize that:

- The **expectation value of the total energy** for a system in state ψ, denoted by **⟨H⟩**, is calculated using the inner product: $$⟨H⟩ = ∫ψ*Ĥψ dx = E$$.
    - For **stationary states**—states where the energy is precisely defined—the expectation value of the Hamiltonian elegantly matches the energy eigenvalue (E).
- The time-dependent Schrödinger equation, **$iħ ∂Ψ/∂t = ĤΨ,$ also underscores the Hamiltonian's dominion over energy.
    - It governs the wave-function's evolution in time, with the Hamiltonian acting as the driving force.

-> Illustrative Examples:

- **Harmonic Oscillator:**
    - The Hamiltonian for this system (in one dimension) is **$$Ĥ = -(ħ²/2m) ∂²/∂x² + (1/2)mω²x²$$**, leading to **quantized energy levels $E_n = (n + (1/2))ħω$**, where n is an integer.
- **Hydrogen Atom:**
    - The Hamiltonian embraces both the electron's kinetic energy and the Coulomb potential energy arising from the electron-proton interaction. The Schrödinger equation, armed with this Hamiltonian, unveils the hydrogen atom's quantized energy levels.
- **Multi-particle Systems:**
    - The Hamiltonian expands to accommodate the kinetic energy of each particle and the intricate dance of potential energy due to inter-particle interactions.

In essence, the Hamiltonian operator is the maestro of quantum energy. Its eigenvalues dictate the possible energies a #Quantum-system system can possess, making the Schrödinger equation the grand stage where the drama of quantum energy unfolds.