# Batch 3: Question 7 — Full Solutions (2024 → 2019)
## PH406 Crystallography & X-Ray Spectroscopy

---

# 2024 — Question 7

**(a) Define systematic absences. Deduce conditions of absences for (i) B-face centering, (ii) 2₁ screw axis ∥ c, (iii) c-glide ⊥ b**

**Systematic absences** (extinctions) are families of reflections (hkl) whose intensities are consistently and systematically zero — dictated strictly by the space-group symmetry, unlike "accidental" absences caused by a particular atomic arrangement. They occur whenever the unit cell is non-primitive (lattice centering) or contains symmetry elements with a translational component (screw axes, glide planes); the translation introduces a fixed phase difference between scattered waves that produces complete destructive interference for specific classes of reflections.

General structure factor: F_hkl = Σⱼ fⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)]

**(i) B-face centering:** extra lattice point at (x+½, y, z+½) for every atom at (x,y,z) (translation ½**a**+½**c**). Substituting the atom pair into F_hkl and factoring:
F_hkl = Σ fⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)] × [1 + exp{πi(h+l)}]
Since exp{πi(h+l)} = (−1)^(h+l): the bracket vanishes when h+l is odd.
**Condition: hkl absent for h+l = 2n+1.**

**(ii) 2₁ screw axis parallel to c:** relates (x,y,z) to (−x,−y,z+½). For axial reflections (h=k=0):
F_00l = Σ fⱼ exp(2πilzⱼ)[1+exp(πil)]
Vanishes when l is odd.
**Condition: 00l absent for l = 2n+1.**

**(iii) c-glide plane perpendicular to b:** relates (x,y,z) to (x,−y,z+½). For the h0l zone (k=0):
F_h0l = Σ fⱼ exp[2πi(hxⱼ+lzⱼ)][1+exp(πil)]
Vanishes when l is odd.
**Condition: h0l absent for l = 2n+1.**

**(b) Identify the space group from absences: hkl absent for h+k+l=2n+1; 0kl absent for k=2n+1; h0l absent for l=2n+1; h00 absent for h=2n+1 (orthorhombic)**

- **hkl absent for h+k+l = 2n+1** → **body-centred (I) lattice**.
- **0kl absent for k = 2n+1** → **b-glide plane perpendicular to a**.
- **h0l absent for l = 2n+1** → **c-glide plane perpendicular to b**.
- **h00 absent for h = 2n+1** → consistent with an **a-glide plane perpendicular to c** (which forces hk0 absent for h=2n+1, and thus its subset h00 absent for h=2n+1 too).

Combining I-centering with the b-glide ⊥ a, c-glide ⊥ b, and a-glide ⊥ c:

**Space group: Ibca (No. 73)**

**(c) Information from intensity statistics**

Intensity statistics analyse the distribution of measured |F| (or |F|²) across reciprocal space, using the central-limit theorem, to determine:

- **Presence/absence of a centre of symmetry** — the primary application. Centrosymmetric (centric) structures give a 1-D Gaussian distribution of structure factors with a higher proportion of very weak reflections and M = ⟨|F|⟩/⟨|F|²⟩^½ = 0.637; non-centrosymmetric (acentric) structures give a 2-D Gaussian distribution with fewer very weak reflections and M = 0.785. The cumulative **N(z) test** (fraction of reflections with intensity ≤ z times local average) distinguishes centric [N(z)=erf(√(z/2))] from acentric [N(z)=1−e⁻ᶻ] cases.
- **Detection of individual symmetry elements** — a mirror plane perpendicular to an axis causes atom overlap in projection, doubling the average intensity of the corresponding zone (e.g. |F_h0l|² ≈ 2Σ); a diad axis along b similarly raises |F_0k0|².
- **Presence of heavy atoms** — a single very heavy atom dominates scattering and makes the intensity distribution depart from the standard statistical curves; detected via the moments of the distribution.
- **Non-crystallographic (hypercentric) symmetry** — centrosymmetric molecules related by a non-crystallographic centre give an even higher proportion of weak intensities than the ordinary centric distribution, visible as a distinctive N(z) curve.


---

# 2023 — Question 7

**(a) Define systematic absence. Deduce conditions of absences for (i) A-face centering, (ii) b-glide ⊥ a, (iii) 2₁ ∥ c**

**Systematic absence:** as defined above — reflections forced to zero intensity by translational symmetry (centering, screw axes, glides), independent of atomic positions.

**(i) A-face centering:** extra lattice point at (0,½,½). F_hkl ∝ [1+e^{2πi(k/2+l/2)}], vanishes unless k+l=2n.
**Condition: hkl absent when k+l = 2n+1; present when k+l = 2n.**

**(ii) b-glide plane perpendicular to a:** operation (x,y,z)→(−x,y+½,z), affects 0kl reflections: F_0kl ∝ [1+e^{2πi(k/2)}], vanishes unless k=2n.
**Condition: 0kl absent for k = 2n+1.**

**(iii) 2₁ screw axis parallel to c:** affects 00l reflections (as in 2024): **00l absent for l = 2n+1.**

**(b) Identify symmetry elements from absences: (i) h0l absent for h=2n+1; (ii) 0k0 absent for k=2n+1 and 0kl absent for k+l=2n+1**

- **h0l absent for h=2n+1** → indicates an **a-glide plane perpendicular to b** (glide translation ½ along a).
- **0k0 absent for k=2n+1** → indicates a **2₁ screw axis parallel to b**.
- **0kl absent for k+l=2n+1** → indicates an **n-glide plane perpendicular to a** (diagonal glide, translation ½(b+c)).

**(c) Selection rules for presence of reflections in cubic lattices**

- **Simple cubic (P):** all hkl present (no restriction).
- **Body-centred cubic (I):** reflections present only if h+k+l = 2n (even); i.e. h+k+l = odd → absent.
- **Face-centred cubic (F):** reflections present only if h,k,l are **all even or all odd** (unmixed parity); mixed-parity indices are absent.
- **Diamond cubic (Fd3m type, F-centring + glide):** in addition to the F-centring rule, h00-type reflections require h = 4n for presence (extra condition from the d-glide/diamond glide).

These selection rules allow the Bravais lattice type of a cubic crystal to be identified directly from which classes of reflections appear in the powder pattern.


---

# 2022 — Question 7

**(a) Define systematic absence. Deduce conditions of absences for (i) 2₁ ∥ a, (ii) a-glide ⊥ b**

Definition as above.

**(i) 2₁ screw axis parallel to a:** operation (x,y,z)→(x+½,−y,−z), affects h00 reflections:
F_h00 ∝ [1+e^{2πi(h/2)}], vanishes unless h=2n.
**Condition: h00 absent for h = 2n+1.**

**(ii) a-glide plane perpendicular to b:** operation (x,y,z)→(x+½,−y,z), affects h0l reflections:
F_h0l ∝ [1+e^{2πi(h/2)}], vanishes unless h=2n.
**Condition: h0l absent for h = 2n+1.**

**(b) Identify space group from absences: (i) hkl absent for h+k+l=2n+1, (ii) 0kl absent for k=2n+1, (iii) h0l absent for l=2n+1, (iv) h00 absent for h=2n+1 (orthorhombic)**

This is the identical absence set analysed in 2024 Q7(b): I-centering (from hkl condition) combined with a b-glide ⊥ a (from 0kl) and a c-glide ⊥ b (from h0l), consistent with h00 absences arising automatically from the centering. **Space group: Ibca (No. 73).**


---

# 2021 — Question 7

**(a) Define systematic absence. Deduce conditions of absences for (i) 2₁ ∥ c (00l absent for l=2n+1), (ii) b-glide ⊥ c (hk0 absent for k=2n+1)**

Definition as above.

**(i) 2₁ screw axis parallel to c:** as derived in 2024 Q7(a)(ii) — affects 00l reflections:
**Condition: 00l absent for l = 2n+1.**

**(ii) b-glide plane perpendicular to c:** operation (x,y,z)→(x,y+½,−z), affects hk0 reflections:
F_hk0 ∝ [1+e^{2πi(k/2)}], vanishes unless k=2n.
**Condition: hk0 absent for k = 2n+1.**

**(b) What information from absences: (i) h+k=2n+1, (ii) hk0 for h+k=2n+1, (iii) h0l for l=2n+1**

- **(i) General hk (all reflections) absent for h+k=2n+1** → indicates a **C-face centering** (extra lattice point at (½,½,0)).
- **(ii) hk0 absent for h+k=2n+1** → consistent with the same C-centering projected onto the hk0 zone (no additional independent symmetry element beyond the centering already identified).
- **(iii) h0l absent for l=2n+1** → indicates a **c-glide plane perpendicular to b**.

**(c) Identify symmetry element from absence: (i) 0k0 for k=2n+1, (ii) h0l for h=2n+1, (iii) none**

- **(i) 0k0 absent for k=2n+1** → **2₁ screw axis parallel to b**.
- **(ii) h0l absent for h=2n+1** → **a-glide plane perpendicular to b**.
- **(iii) No absences** → indicates the corresponding axis/plane in that zone is a **simple (non-translational) symmetry element** — i.e., an ordinary rotation axis or mirror plane with no associated glide/screw component.


---

# 2020 — Question 7

**(a) Define systematic absences. Deduce selection rules for presence of reflections in cubic lattices**

Definition as above. Selection rules (as derived in 2023 Q7(c)):
- **P (simple cubic):** all hkl present.
- **I (body-centred):** present only if h+k+l = 2n.
- **F (face-centred):** present only if h,k,l all even or all odd (unmixed parity).

**(b) Deduce conditions of absences for (i) 2₁ screw axis ∥ a, (ii) a-glide ⊥ b**

Identical derivations to 2022 Q7(a):
**(i)** 2₁ ∥ a → **h00 absent for h = 2n+1.**
**(ii)** a-glide ⊥ b → **h0l absent for h = 2n+1.**

**(c) Information from absences: (i) h+k+l=2n+1, (ii) h+k=2n+1, (iii) 00l for l=2n+1, (iv) hk0 for h=2n+1**

- **(i) hkl absent for h+k+l=2n+1** → **I (body-centred) lattice.**
- **(ii) hkl absent for h+k=2n+1 (all l)** → **C-face centering** (extra point at (½,½,0)).
- **(iii) 00l absent for l=2n+1** → **2₁ screw axis parallel to c** (or c-glide, if accompanied by a mirror; here indicates the screw axis).
- **(iv) hk0 absent for h=2n+1** → **a-glide plane perpendicular to c** (glide translation ½ along a, reflection plane normal to c).


---

# 2019 — Question 7

**(a) Define systematic absences. Deduce condition of absence for (i) 2₁ screw axis parallel to b, (ii) b-glide plane perpendicular to c**

Definition as above.

**(i) 2₁ screw axis parallel to b:** relates (x,y,z) to (−x, y+½, −z). For axial reflections 0k0 (h=l=0):
F_0k0 = Σ fⱼ exp(2πikyⱼ)[1+exp(πik)]
Vanishes when k is odd.
**Condition: 0k0 absent for k = 2n+1.**

**(ii) b-glide plane perpendicular to c:** relates (x,y,z) to (x, y+½, −z). For the hk0 zone (l=0):
F_hk0 = Σ fⱼ exp[2πi(hxⱼ+kyⱼ)][1+exp(πik)]
Vanishes when k is odd.
**Condition: hk0 absent for k = 2n+1.**

**(b) Identify the space group from absences in an orthorhombic lattice: (i) hkl absent for h+k+l=2n+1, (ii) 0kl absent for k=2n+1, (iii) h0l absent for l=2n+1, (iv) hk0 absent for h=2n+1**

- **(i) hkl absent for h+k+l=2n+1** → **I (body-centred) lattice**.
- **(ii) 0kl absent for k=2n+1** → **b-glide plane perpendicular to a**.
- **(iii) h0l absent for l=2n+1** → **c-glide plane perpendicular to b**.
- **(iv) hk0 absent for h=2n+1** → **a-glide plane perpendicular to c**.

Combining the I-centring with the b-glide ⊥ a, c-glide ⊥ b, and a-glide ⊥ c (the same combination identified in the 2024 and 2022 papers):

**Space group: Ibca (No. 73)**

