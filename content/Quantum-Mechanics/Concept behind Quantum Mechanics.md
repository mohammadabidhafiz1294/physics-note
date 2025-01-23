---
tags: [Hermitian-operators, concept-quantum-mechanics, quantum-mechanics/concept]
---

### Eigen-values and Eigen-functions
*Definition:* In quantum mechanics, #eigen-values and #eigen-functions arise from the study of operators, particularly Hermitian operators, which represent physical observables.

**Eigenvalue:** A scalar value associated with an operator that indicates the measurable quantity of a physical observable.

**Eigenfunction:** A non-zero function that, when acted upon by an operator, yields the same function multiplied by the eigenvalue.

*Mathematical Formulation*:
For an operator $\hat{A}$, the eigenvalue equation is given by:
$$
\hat{A} \psi_n(x) = a_n \psi_n(x)
$$

Where: $\hat{A}$ is the operator (e.g., position, momentum, Hamiltonian).$\psi_n(x)$ is the eigen-function corresponding to the eigenvalue $a_n$.

*Properties*

- **Real Eigenvalues:** For Hermitian operators, the eigenvalues are real numbers.
- **Orthogonal Eigenfunctions:** Eigenfunctions corresponding to different eigenvalues are orthogonal.

*Examples*

- **Position Operator:**
   The position operator $\hat{x}$ acts on a wave function $\psi(x)$ as follows:<br/>
   $$\hat{x} \psi(x) = x \psi(x)$$
   Here, the eigenvalue is the position $x$, and the eigen-function is $\psi(x)$ itself.

- **Momentum Operator:**
   The momentum operator $$\hat{p} = -i\hbar \frac{d}{dx}$$ has eigen-functions of the form:$$\hat{p} \psi_p(x) = p \psi_p(x)$$ where $$\psi_p(x) = e^{ipx/\hbar}$$ is the eigen-function and $p$ is the eigenvalue (momentum).

- **Hamiltonian Operator (for a particle in a one-dimensional infinite potential well)**:
   The Hamiltonian operator $\hat{H}$ is given by:
   $$
   \hat{H} = -\frac{\hbar^2}{2m} \frac{d^2}{dx^2}
   $$
   The eigenvalue equation becomes:$$\hat{H} \psi_n(x) = E_n \psi_n(x)$$
   The solutions (eigen-functions) are:$$\psi_n(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{n\pi x}{L}\right), \quad n = 1, 2, 3, \ldots$$
   The corresponding eigenvalues (energy levels) are:$$E_n = \frac{n^2 \hbar^2 \pi^2}{2mL^2}$$
### Hermitian Operators

*Definition:* #Hermitian-operators are linear operators that satisfy the condition:
$$
A = A^\dagger
$$
where $A^\dagger$ is the adjoint (or conjugate transpose) of the operator $A$. This means that the inner product of two states is preserved under the action of the operator.

*Properties:*

- **Real Eigenvalues:** The eigenvalues of a Hermitian operator are always real.
- **Orthogonal Eigenfunctions:** The eigenfunctions corresponding to different eigenvalues are orthogonal.

*Example:* The position operator $\hat{x}$ and the momentum operator $$\hat{p} = -i\hbar \frac{d}{dx}$$ are both Hermitian operators.
### Projection Operators

*Definition:* A #projection-operator $P$ is a Hermitian operator that satisfies:
$$P^2 = P$$
This means that applying the operator twice is the same as applying it once.

*Properties:*

- Idempotent: $$P^2 = P$$
- Hermitian: $$P = P^\dagger$$

*Example:*

- Consider a projection operator that projects a vector onto a subspace spanned by a normalized vector $|\phi\rangle$:$$P = |\phi\rangle \langle \phi|$$If you apply this operator to any state $|\psi\rangle$, it projects $|\psi\rangle$ onto the direction of $|\phi\rangle$.

- Consider a three-dimensional vector A, which can be expressed in terms of its components along three orthonormal basis vectors,$ε₁, ε₂, and ε₃$:$$|A⟩ = A₁|ε₁⟩ + A₂|ε₂⟩ + A₃|ε₃⟩$$The projection operator that projects A onto the direction of $ε₁$ is $P̂₁ = |ε₁⟩⟨ε₁|$. Applying $P̂₁ to |A⟩$ gives:$$P̂₁|A⟩ = (|ε₁⟩⟨ε₁|)(A₁|ε₁⟩ + A₂|ε₂⟩ + A₃|ε₃⟩) = A₁|ε₁⟩.$$The result is a vector that lies entirely along the direction of $ε₁$ and has a magnitude equal to the component of A in that direction.
### Expectation Values

Definition: The #expectation-value of an observable represented by a Hermitian operator $A$ in a state described by the wave function $\psi$ is given by:

$$
\langle A \rangle = \int \psi^*(x) A \psi(x) \, dx
$$

where $\psi^*(x)$ is the complex conjugate of the wave function.

*Properties:*

- The expectation value is a real number since $A$ is Hermitian.
- It represents the average value of the observable over many measurements.

Example:

- For the momentum operator $\hat{p}$, the expectation value is:
$$
\langle \hat{p} \rangle = \int \psi^*(x) \left(-i\hbar \frac{d}{dx}\right) \psi(x) \, dx
$$
- Suppose, you want to find the expectation value of the position of a particle in a state described by the wave-function $ψ(x)$. The expectation value of the position operator $\hat{x}$ is:$$⟨\hat{x}⟩ = ⟨\psi^*| \hat{x} |ψ⟩ = ∫\psi^*(x) x ψ(x) dx*$$This integral calculates the weighted average of the position $x$, where the weight is given by the probability density $|ψ(x)|²$.

==Summary==

**Hermitian Operators**: Operators with real eigenvalues and orthogonal eigen functions.<br/>
**Projection Operators**: Special Hermitian operators that project states onto subspaces.<br/>
**Expectation Values**: Average values of observables calculated using Hermitian operators.<br/>
**Eigen values:** represent measurable quantities in quantum mechanics.<br/>
**Eigen functions:** describe the state of a system corresponding to those measurements.

---
#### Reference
> These concepts are foundational in quantum mechanics and are discussed in detail in the documents you've tagged, such as "Principles of Quantum Mechanics" by R. Shankar, "A Student's Guide to the Schrödinger Equation" by Daniel A. Fleisch & "Introduction to Quantum Mechanics" by David J. Griffiths.