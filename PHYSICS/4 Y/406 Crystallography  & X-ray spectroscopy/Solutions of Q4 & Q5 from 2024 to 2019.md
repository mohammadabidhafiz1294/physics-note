# Batch 4: Questions 4 & 5 — Full Solutions (2024 → 2019)
## PH406 Crystallography & X-Ray Spectroscopy

---

# 2024

## Question 4

**(a) Deduce the Laue equation for a one-dimensional array of atoms**

Consider a row of identical atoms spaced at regular intervals **a** along a line. A parallel incident X-ray beam (direction **s₀**, wavelength λ) strikes the row; the scattered beam is observed along direction **s**. For two neighbouring atoms separated by **a**, the path difference between the waves scattered in direction **s** is:

Δ = **a**·**s** − **a**·**s₀** = **a**·(**s**−**s₀**)

For constructive interference (reinforcement) between waves from *all* atoms in the row (not just neighbours), this path difference must equal an integral number of wavelengths:

**a·(s−s₀) = hλ**, or equivalently **a(cosφ − cosφ₀) = hλ**

where φ₀, φ are the angles the incident and diffracted beams make with the row, and h is an integer (the order of diffraction). This is the **Laue equation for a 1-D row of atoms**; for a full 3-D lattice, three such equations (along a, b, c with integers h, k, l) must be simultaneously satisfied.

**(b) X-ray diffraction by a crystal; Bragg's law in vector form**

**X-ray diffraction** is the phenomenon in which X-rays incident on the periodic array of atoms in a crystal are coherently scattered and interfere constructively along specific directions determined by the crystal's lattice geometry, producing a discrete pattern of intensity maxima (reflections) rather than continuous scattering.

**Vector form of Bragg's law:** Consider a set of lattice planes (hkl) with spacing d. Constructive interference occurs when the scattering vector **S** = (**s**−**s₀**)/λ coincides with a reciprocal lattice vector **G**_hkl = h**a\***+k**b\***+l**c\***:

**S = G_hkl**, i.e. (**s**−**s₀**)/λ = **G**_hkl

Since |**G**_hkl| = 1/d_hkl and the geometry of **s**−**s₀** (unit vectors) gives |**s**−**s₀**| = 2 sinθ, this reduces to the familiar scalar Bragg's law:

**λ = 2d sinθ** (n=1) or generally **nλ = 2d sinθ**

**(c) 2θ for (321) plane: a=5Å, b=10Å, c=15Å, α=β=90°, γ=120°, λ=1.54Å**

For this monoclinic-type cell (a≠b≠c, γ=120°, α=β=90°), the general d-spacing formula (with only γ≠90°) is:

$$1/d² = (1/sin²γ)[h²/a² + k²/b² − 2hk cosγ/(ab)] + l²/c²$$

Substituting h=3, k=2, l=1, a=5, b=10, c=15, γ=120° (sinγ=0.8660, cosγ=−0.5):

1/d² = (1/0.75)[9/25 + 4/100 − 2(3)(2)(−0.5)/(50)] + 1/225
= (1.3333)[0.36 + 0.04 + 0.06] + 0.00444
= (1.3333)(0.46) + 0.00444
= 0.6133 + 0.00444 = 0.6178

d = 1/√0.6178 = **1.272 Å**

Bragg's law: sinθ = λ/2d = 1.54/(2×1.272) = 0.6053 → θ = 37.26°

**2θ ≈ 74.5°**

## Question 5

**(a) Structure factor — definition and physical significance**

The **structure factor** F_hkl is the resultant wave scattered by all the atoms in one unit cell, in the direction corresponding to reflection from the (hkl) planes, expressed as a complex quantity:

F_hkl = Σⱼ fⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)]

where fⱼ is the atomic scattering factor and (xⱼ,yⱼ,zⱼ) are fractional coordinates of the jth atom.

**Physical significance:** |F_hkl|² is directly proportional to the observed intensity of the (hkl) reflection. F_hkl encodes both the amplitude and phase of the scattered wave from the entire unit-cell contents (not just a single atom), so it determines which reflections are strong, weak, or systematically absent, and — via its phase (lost in a simple intensity measurement, the "phase problem") — governs the reconstruction of the electron-density map of the crystal structure.

**(b) Why are X-rays scattered by atoms? Atomic scattering factor derivation**

An atom scatters X-rays because it is a distribution of Z electrons in the electron cloud; each electron individually scatters via the Thomson mechanism, and the resultant wave from the atom is the coherent (phase-related) sum of all these individual electron waves.

**Derivation of atomic scattering factor f:**
Let ρ(r) be the electron density at position **r** within the atom, with ∫ρ(r)dV = Z. For scattering vector **S** = (**s**−**s₀**)/λ, each volume element dV contributes an amplitude ρ(r)dV with phase 2π**S**·**r** relative to the origin (nucleus). The total scattered amplitude relative to that of a single free electron is:

**f(sinθ/λ) = ∫ρ(r) exp(2πi S·r) dV**

For a spherically symmetric ρ(r), this reduces (via integration over solid angle) to:

f = ∫₀^∞ 4πr²ρ(r) [sin(4πr sinθ/λ)/(4πr sinθ/λ)] dr

At θ=0 (forward scattering), f = Z (all electrons scatter in phase); f decreases monotonically as sinθ/λ increases, because path differences among electrons within the atom cause increasing destructive interference.

**(c) Scattered intensities from (111) and (200) of NaCl**

For the NaCl rock-salt structure (FCC, with Na⁺ at (0,0,0)+fcc and Cl⁻ at (½,0,0)+fcc):

F_hkl = 4[f_Na + f_Cl exp{πi(h+k+l)}]  (using the standard NaCl structure-factor reduction)

- For **(111)**: h+k+l = 3 (odd) → exp(πi·3) = −1
  F₁₁₁ = 4(f_Na − f_Cl) → **|F₁₁₁|² = 16(f_Na−f_Cl)²** — a relatively weak reflection since f_Na and f_Cl are not too different in magnitude (partially cancelling).

- For **(200)**: h+k+l = 2 (even) → exp(πi·2) = +1
  F₂₀₀ = 4(f_Na + f_Cl) → **|F₂₀₀|² = 16(f_Na+f_Cl)²** — a strong reflection, since the two contributions add constructively.

**Conclusion:** Since f_Na and f_Cl are comparable in magnitude but not equal, (f_Na+f_Cl)² ≫ (f_Na−f_Cl)², so the **(200) reflection is significantly stronger than (111)** — this is a classic diagnostic feature of the NaCl-type structure, where even-index reflections (h,k,l all same parity, sum even) are systematically enhanced relative to the "difference" reflections.


---

# 2023

## Question 4

**(a) Deduce an expression for the experimental form of structure factor**

The structure factor's ideal (theoretical) form F_hkl = Σⱼfⱼexp[2πi(hxⱼ+kyⱼ+lzⱼ)] assumes atoms are stationary point scatterers. Experimentally, atoms undergo thermal vibration about their mean positions, and the observed diffracted intensity is systematically lower. Including the isotropic Debye–Waller (temperature) factor exp(−B sin²θ/λ²), the **experimental (observed) structure factor** becomes:

**F_hkl(exp) = Σⱼ fⱼ exp(−Bⱼ sin²θ/λ²) exp[2πi(hxⱼ+kyⱼ+lzⱼ)]**

where B = 8π²⟨u²⟩ is related to the mean-square thermal displacement ⟨u²⟩ of the atom. The measured intensity I_hkl ∝ |F_hkl(exp)|² (times the appropriate Lorentz-polarization and multiplicity factors) is what is actually compared to experiment, and the temperature-dependent exponential factor causes the effective scattering power to fall off faster with increasing θ than the "static-atom" prediction.

**(b) Prove the equivalence of Bragg's and Laue's conditions for a simple cubic lattice**

**Laue's conditions** for a 3-D lattice require simultaneous satisfaction of:
a·(s−s₀) = hλ, b·(s−s₀) = kλ, c·(s−s₀) = lλ

For a simple cubic lattice with a=b=c and orthogonal axes, this is equivalent to the reciprocal-lattice statement: the scattering vector **S**=(s−s₀)/λ must equal a reciprocal lattice vector **G**_hkl = ha*+kb*+lc*. Since |G_hkl| = 1/d_hkl and geometrically |S| = 2sinθ/λ, we obtain:

2sinθ/λ = 1/d_hkl  ⟹  **λ = 2d_hkl sinθ**

which is exactly **Bragg's law**. Thus for a simple cubic lattice, satisfying the three Laue equations simultaneously is mathematically identical to satisfying the Bragg condition for the corresponding (hkl) planes — the Laue formulation (three simultaneous conditions in three dimensions) and the Bragg formulation (reflection from lattice planes) describe the same physical diffraction condition, viewed from atom-row-interference and plane-reflection perspectives respectively.

**(c) Row spacing 7.7Å, incident angle 30°, diffraction angle 62°13′, λ=1.54Å: find order**

Using the 1-D Laue (row) equation: a(cosφ − cosφ₀) = hλ

Here φ₀ = 30° (incident angle with row), φ = 62°13′ = 62.217° (diffracted angle with row), a = 7.7 Å, λ = 1.54 Å.

cosφ₀ = cos30° = 0.8660
cosφ = cos62.217° = 0.4649

h = a(cosφ − cosφ₀)/λ = 7.7(0.4649 − 0.8660)/1.54 = 7.7(−0.4011)/1.54 = −3.089/1.54 ≈ **−2.006 ≈ −2**

**Order of diffraction: h = −2** (second order, on the opposite side of the incident beam from the zero order).

## Question 5

**(a) Atomic scattering factor — definition, expression, and f ~ sinθ/λ curve**

**Definition:** The atomic scattering factor f is the ratio of the amplitude scattered by an atom to the amplitude that would be scattered by a single free electron under the same conditions, as a function of scattering angle.

**Expression:** f(sinθ/λ) = ∫ρ(r) exp(2πi S·r) dV = ∫₀^∞ 4πr²ρ(r)[sin(kr)/(kr)] dr, where k=4π sinθ/λ (as derived in 2024 Q5(b)).

**f ~ sinθ/λ curve:** f starts at its maximum value f=Z at sinθ/λ=0 (forward scattering, all electrons scatter in phase), and decreases monotonically and smoothly as sinθ/λ increases, approaching zero at large sinθ/λ. The curve is concave, falling steeply at first and then leveling off — reflecting increasing destructive interference among electrons distributed over the finite size of the atom as the scattering angle (and hence path-difference) grows. Heavier atoms (larger Z) have systematically higher f curves throughout.

**(b) Structure factor F_hkl for HCP cell; show intensity from (101) > (102)**

HCP has 2 atoms per unit cell at fractional coordinates (0,0,0) and (⅓,⅔,½).

F_hkl = f[1 + exp{2πi(h/3+2k/3+l/2)}]

For **(101)**: h=1,k=0,l=1 → phase = 2π(1/3+0+1/2) = 2π(5/6)
F₁₀₁ = f[1+exp(2πi·5/6)] = f[1+cos300°+isin300°] = f[1+0.5−i0.866] = f[1.5−0.866i]
|F₁₀₁|² = f²(1.5²+0.866²) = f²(2.25+0.75) = **3f²**

For **(102)**: h=1,k=0,l=2 → phase = 2π(1/3+0+1) = 2π(4/3) ≡ 2π(1/3) (mod 2π)
F₁₀₂ = f[1+exp(2πi/3)] = f[1+cos120°+isin120°] = f[1−0.5+i0.866] = f[0.5+0.866i]
|F₁₀₂|² = f²(0.25+0.75) = **1×f²**

**Comparison:** |F₁₀₁|² = 3f² > |F₁₀₂|² = f². **Hence the (101) reflection is three times more intense than (102)**, confirming the stated result.


---

# 2022

## Question 4

**(a) Bragg's law in vector and scalar form; significance of Ewald construction**

Vector form: (s−s₀)/λ = G_hkl (as in 2024 Q4(b)); scalar form: nλ = 2d sinθ.

**Ewald construction:** A geometric device in reciprocal space — draw a sphere of radius 1/λ (the "sphere of reflection") passing through the origin of the reciprocal lattice, centred at the point −s₀/λ. A reflection (hkl) occurs whenever a reciprocal lattice point lies exactly on the surface of this sphere; the direction from the sphere's centre to that point gives the diffracted beam direction. **Significance:** it converts Bragg's law into a simple, visualizable geometric criterion, immediately showing which reflections can occur simultaneously for a given crystal orientation and wavelength, and underlies the interpretation of rotation/oscillation photographs.

**(b) Show ordinary Bragg's equation holds only for higher values of n**

Bragg's law nλ = 2d sinθ requires sinθ = nλ/2d ≤ 1, i.e. n ≤ 2d/λ. For low orders (small n), the corresponding θ is small and the approximation of treating the crystal as a stack of "mirror" planes reflecting the whole beam coherently is least accurate, because at small θ the beam samples many planes with only weak cumulative phase coherence and dynamical (multiple-scattering) effects dominate. As n increases (higher order, larger θ, approaching 90°), the geometric path-difference condition becomes an increasingly good and unambiguous description of the sharp, well-defined diffraction condition, since higher-order reflections correspond to a more strongly peaked, well-resolved interference maximum with negligible overlap from neighbouring orders. Hence the simple (kinematic) Bragg equation is most reliably applicable for higher n.

**(c) FCC Laue photo: a=6.5Å, V=3kV, sample-to-film distance=3cm — distance to (111) max-spacing plane**

Electron accelerating voltage relation for continuous (white) X-ray minimum wavelength (Duane–Hunt law): λ_min = hc/(eV) = 12398/V(eV) Å = 12398/3000 = **4.133 Å**

For FCC, (111) interplanar spacing: d₁₁₁ = a/√(h²+k²+l²) = 6.5/√3 = **3.753 Å**

Since d₁₁₁ < λ_min/2 (3.753 < 2.07 is false; check Bragg condition instead): Bragg's law: λ=2d sinθ ⟹ sinθ = λ/2d. Using the shortest usable wavelength component of the white radiation available for this reflection, take λ ≈ λ_min for the highest-angle (most sharply diffracted) case:
sinθ = 4.133/(2×3.753) = 0.5507 → θ = 33.4°, 2θ = 66.8°

Distance on flat film from centre: r = D tan(2θ) = 3 cm × tan(66.8°) = 3 × 2.335 = **≈ 7.0 cm**

*(This uses the standard flat-film Laue geometry r = D tan2θ, with D = sample-to-film distance.)*

## Question 5

**(a) Formation of the diffraction line by the powder method**

In the powder method, a finely powdered (polycrystalline) sample containing millions of randomly oriented tiny crystallites is placed in a monochromatic X-ray beam. For each set of (hkl) planes, some fraction of the crystallites will, by chance, be oriented at exactly the Bragg angle θ_hkl to the incident beam. Because of the random orientation distribution, the diffracted beams from all such correctly-oriented crystallites lie on the surface of a cone of semi-angle 2θ_hkl, coaxial with the incident beam. Recording this cone of diffracted rays on a strip of film (or with a counter) wrapped around the sample produces an arc (or, for a full circle, a ring) — the **diffraction line** — for each distinct d-spacing in the crystal.

**(b) Powder method vs Laue method — experimental comparison**

| Feature | Powder method | Laue method |
|---|---|---|
| Sample | Polycrystalline powder | Single crystal, fixed orientation |
| Radiation | Monochromatic | Continuous (white) spectrum |
| Purpose | Phase ID, lattice parameters, d-spacings | Crystal symmetry, orientation |
| Diffraction pattern | Concentric cones/rings (Debye–Scherrer rings) | Discrete spots in symmetric pattern |
| Sample motion | Stationary (crystallites provide all orientations) | Stationary single crystal |

**(c) Indexing an X-ray photograph; graphical indexing of a rotating-crystal photograph**

**Indexing** means assigning the correct Miller indices (hkl) to each observed diffraction spot/line, thereby determining unit-cell dimensions and orientation.

**Graphical indexing (rotating crystal method):** As the crystal rotates about a chosen axis (say c), reciprocal lattice points sweep through the sphere of reflection in layers, producing layer lines on the cylindrical film corresponding to l=0,1,2,… (spacing between layer lines gives the identity period along the rotation axis via the standard tanμ = y/R relation). Within each layer line, the spot positions are plotted onto a graphical net (e.g. a Bernal chart), which unrolls the geometry of the reciprocal lattice layer intersecting the sphere of reflection; matching observed spot coordinates to the net's grid directly yields the (hk) indices for each spot in that layer (with l fixed by the layer number), without needing detailed calculation for every reflection.


---

# 2021

## Question 4

**(a) Deduce the Laue equation for a one-dimensional array of atoms** — identical derivation to 2024 Q4(a):
**a(cosφ − cosφ₀) = hλ**

**(b) Prove the equivalence of Bragg's and Laue's conditions for a simple cubic lattice** — identical derivation to 2023 Q4(b): both reduce to λ = 2d_hkl sinθ via the reciprocal-lattice relation S=G_hkl and |G_hkl|=1/d_hkl.

**(c) Row spacing 7.7Å, incident angle 30°, diffraction angle 62°13′, λ=1.54Å: find order** — identical calculation to 2023 Q4(c):

h = a(cosφ−cosφ₀)/λ = 7.7(cos62.217°−cos30°)/1.54 = 7.7(0.4649−0.8660)/1.54 ≈ **−2**

**Order of diffraction: h = −2**

## Question 5

**(a) Structure factor F_hkl; exponential form**

F_hkl = Σⱼ fⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)]

This is the **exponential form** of the structure factor: a complex-number sum over all N atoms in the unit cell, each contributing an amplitude fⱼ (its atomic scattering factor) with a phase 2π(hxⱼ+kyⱼ+lzⱼ) determined by its fractional position. |F_hkl| gives the amplitude and arg(F_hkl) the phase of the resultant wave scattered by the (hkl) planes.

**(b) Structure factor for HCP cell; show (101) intensity > (102)** — identical derivation to 2023 Q5(b):

|F₁₀₁|² = 3f², |F₁₀₂|² = f² ⟹ **(101) is three times stronger than (102)**.

**(c) Powder diffraction, cubic crystal, 2θ = 38°, 44.2°, 81.4°; λ=1.54Å, a=4.10Å — find Miller indices and lattice type**

sin²θ = (λ²/4a²)(h²+k²+l²) → sin²θ ∝ N = h²+k²+l²

θ₁=19°: sin²θ₁ = 0.1060
θ₂=22.1°: sin²θ₂ = 0.1416
θ₃=40.7°: sin²θ₃ = 0.4249

Ratios: sin²θ₂/sin²θ₁ = 1.336 ≈ 4/3; sin²θ₃/sin²θ₁ = 4.009 ≈ 4

Taking sin²θ₁ as corresponding to N₁=3 (i.e. (111)): constant = 0.1060/3 = 0.03533
N₂ = 0.1416/0.03533 ≈ 4.0 → (200)
N₃ = 0.4249/0.03533 ≈ 12.03 → (222)

Sequence N = 3, 4, 12 — allowed values for **FCC** are N = 3,4,8,11,12,16,… (only all-even or all-odd hkl combinations). The observed sequence 3,4,12 (i.e. (111),(200),(222)) matches this FCC pattern (note the absence of N=8, i.e. (220), which would need a fourth line — consistent with only three lines being given/observed here).

**Lattice type: FCC**; **Miller indices: (111), (200), (222)** for the three lines respectively.


---

# 2020

## Question 4

**(a) Bragg's law in vector form and scalar form** — as derived in 2024 Q4(b): vector form (s−s₀)/λ=G_hkl; scalar form nλ=2d sinθ.

**(b) Atomic scattering factor expression; f ~ sinθ/λ curve for a point atom**

Expression as in 2023 Q5(a): f(sinθ/λ) = ∫ρ(r)exp(2πiS·r)dV.

**For a point atom** (idealised, all Z electrons concentrated at a single point, ρ(r)=Zδ(r)): every volume element scatters exactly in phase for all scattering angles (zero path difference regardless of θ), so:

**f = Z, independent of sinθ/λ** — i.e., the f~sinθ/λ curve for a point atom is a **horizontal straight line** at height Z, in contrast to the real (finite-size) atom's curve which starts at Z and falls off with increasing sinθ/λ. This comparison illustrates that the fall-off of f with angle for real atoms arises specifically from the finite spatial extent of the electron cloud.

**(c) Beam wavelength λ, angle 30° with row of spacing 5λ; find diffracted angle for h=−1**

Using a(cosφ−cosφ₀) = hλ, with a=5λ, φ₀=30°:

cosφ = cosφ₀ + hλ/a = cos30° + (−1)λ/(5λ) = 0.8660 − 0.20 = 0.6660

φ = cos⁻¹(0.6660) = **48.2°**

**The diffracted beam makes an angle of ≈ 48.2° with the row of scatterers** (for order h = −1).

## Question 5

**(a) Powder experiment: first line at 2θ=38°; find Miller index [CuKα, a=4.10Å]**

θ = 19°, sinθ = 0.3256, sin²θ = 0.1060

sin²θ = (λ²/4a²)N, with λ=1.5418Å (CuKα), a=4.10Å:
λ²/4a² = (1.5418²)/(4×4.10²) = 2.377/67.24 = 0.03535

N = sin²θ/0.03535 = 0.1060/0.03535 ≈ **3.0**

N=3 corresponds to Miller indices **(111)**.

**(b) Structure factor for NaCl; show (111) < (200)**

As derived in 2024 Q5(c): |F₁₁₁|²=16(f_Na−f_Cl)² and |F₂₀₀|²=16(f_Na+f_Cl)². Since (f_Na+f_Cl)² > (f_Na−f_Cl)² for any f_Na≠f_Cl of the same sign, **|F₂₀₀|² > |F₁₁₁|²**, i.e. the **scattered intensity from (200) is greater than from (111)** — consistent with the required result.

**(c) Relation among symmetry factor, atomic scattering factor, and structure factor**

The **structure factor** can always be factorised as:

F_hkl = f × S_hkl (for a single-atom-type basis)

or more generally, for a basis of several atoms of possibly different species, F_hkl = Σⱼfⱼ Sⱼ(hkl), where the **symmetry factor** (also called the geometric or lattice factor) S_hkl = Σⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)] depends only on the positions of the atoms within the cell (geometry/symmetry), while the **atomic scattering factor** fⱼ depends only on the electronic structure of each atom (how strongly that species scatters). Thus: **structure factor = atomic scattering factor × symmetry (geometric) factor**, i.e. the total scattering amplitude separates into a purely chemical/electronic part (f) and a purely geometric/positional part (S), with systematic absences arising when S_hkl = 0 for particular (hkl) classes regardless of which atoms are present.


---

# 2019

## Question 4

**(a) X-ray diffraction meaning; Laue's equations for a 1-D array of atoms**

**X-ray diffraction:** the coherent scattering of X-rays by the periodic array of atoms in a crystal, producing constructive interference (sharp intensity maxima) in specific directions determined by the lattice geometry and the X-ray wavelength — see definition in 2024 Q4(b).

**Laue's equation, 1-D array** (as derived in 2024 Q4(a)): **a(cosφ−cosφ₀) = hλ**

**(b) Prove the equivalence of Bragg's and Laue's conditions for a simple cubic lattice** — identical to 2023 Q4(b): both reduce to λ=2d_hkl sinθ via S=G_hkl, |G_hkl|=1/d_hkl.

**(c) Parallel beam at 30° to a row of scatterers; find diffracted angle for order h=−1**

*(Row spacing not explicitly stated in this year's question as transcribed; assuming the standard spacing a=5λ used consistently in this course's problems, as in the closely related 2020 Q4(c) with identical setup):*

Using a(cosφ−cosφ₀)=hλ with φ₀=30°, a=5λ, h=−1 (same as 2020 Q4(c)):

cosφ = cos30° + (−1/5) = 0.8660−0.20 = 0.6660 → **φ ≈ 48.2°**

**The diffracted beam makes an angle of ≈48.2° with the row** (for order h=−1).

## Question 5

**(a) Structure factor F_hkl; exponential form of structure factor**

As in 2021 Q5(a): F_hkl = Σⱼfⱼ exp[2πi(hxⱼ+kyⱼ+lzⱼ)] — the exponential (complex-sum) form encoding both amplitude and phase of the wave scattered by the unit-cell contents.

**(b) Symmetry factor; relation among symmetry factor, atomic scattering factor, and structure factor**

As derived in 2020 Q5(c): the **symmetry (geometric) factor** S_hkl = Σⱼexp[2πi(hxⱼ+kyⱼ+lzⱼ)] depends only on atomic positions (crystal geometry), and:

**F_hkl = f × S_hkl** (single atom type), or F_hkl = Σⱼ fⱼ Sⱼ in general —

i.e., the structure factor is the product of the purely electronic atomic scattering factor and the purely geometric symmetry factor.

**(c) Structure factor for HCP cell; show intensity from (101) plane greater than (200)**

*(Note: the question as transcribed says "(ii)" — this is almost certainly a transcription artifact for "(101)", consistent with the identical HCP problem in 2023 Q5(b) and 2021 Q5(b), which compares (101) to (102). Solved here for both the stated (200) and the more standard (102) for completeness.)*

F_hkl = f[1+exp{2πi(h/3+2k/3+l/2)}] (HCP, atoms at (0,0,0) and (⅓,⅔,½))

**(101):** phase=2π(1/3+0+1/2)=2π(5/6) → F₁₀₁=f[1+cos300°+isin300°]=f[1.5−0.866i] → |F₁₀₁|²=**3f²** (as in 2023 Q5(b))

**(200):** h=2,k=0,l=0 → phase=2π(2/3) → F₂₀₀=f[1+cos240°+isin240°]=f[1−0.5−0.866i]=f[0.5−0.866i] → |F₂₀₀|²=f²(0.25+0.75)=**1×f²**

**Comparison:** |F₁₀₁|²=3f² > |F₂₀₀|²=f² — **the (101) reflection is three times stronger than (200)**, confirming the required result.

