# Batch 2: Question 3 — Full Solutions (2024 → 2019)
## PH406 Crystallography & X-Ray Spectroscopy

---

# 2024 — Question 3

**(a) Why are X-rays scattered by electrons?**

X-rays interact with matter through their oscillating electric field. When an X-ray beam strikes a charged particle such as an electron, the alternating field imparts an alternating acceleration to it. By classical electromagnetic theory, an accelerating charged particle radiates secondary electromagnetic waves — the electron absorbs and re-emits energy at the same frequency as the incident wave (Thomson scattering).

The scattered intensity (Thomson formula):
I₂θ = [e²/(4πε₀c²m)]² × (1+cos²2θ)/2 × I₀/R²

The 1/m² factor shows why only **electrons** scatter appreciably — the proton (lightest nucleus) has ~1837× the electron's mass, so nuclear scattering is negligible. Hence the electron cloud around the nucleus is responsible for X-ray diffraction.

**(b) Rayleigh vs Compton scattering**

| Feature | Rayleigh (coherent) | Compton (incoherent) |
|---|---|---|
| Collision type | Elastic — no energy lost | Inelastic — energy/momentum shared |
| Wavelength | Unmodified (λ′=λ) | Modified, longer (λ′>λ) |
| Phase relation | Definite, fixed phase with incident beam | No fixed phase relation |
| Interference | Produces diffraction/interference | No interference; adds uniform background |
| Electron behaviour | Electron behaves as bound | Electron behaves as free, at rest |

**(c) Intensity of X-rays scattered by a pair of electrons (derivation)**

Consider two identical scatterers O₁, O₂ separated by vector **r**. Incident beam direction ŝ₀, scattered direction ŝ; define scattering vector **S** = (ŝ−ŝ₀)/λ.

Phase difference: δ = 2π **r**·**S**

Resultant amplitude at distant point P (single-electron amplitude A_φ):
E_P = A_φ e^{i(ωt+Δ)} + A_φ e^{i(ωt+Δ+δ)}
⇒ |A_P| = 2A_φ cos(δ/2)

Intensity I = |A_P|²:
**I_P = 4A_φ² cos²(δ/2) = 2I_e(1 + cos δ) = 2I_e[1 + cos(2π r·S)]**

where I_e = A_φ² is the intensity from a single free electron.

Averaging over random orientations (gas/liquid case):
**Ī_P = 2I_e(1 + sin x / x)**, where x = 2πr|S| = 4πr sinθ/λ

For x→0 (small angle), Ī_P → 4I_e; for large x, it oscillates about 2I_e.


---

# 2023 — Question 3

**(a) How does an atom scatter X-rays? Why do we use X-ray instead of visible light to analyze crystal structure?**

An atom scatters X-rays through its constituent electrons: each electron in the electron cloud independently scatters the incident wave (Thomson scattering), and the resultant scattered wave from the atom is the vector (phase) sum of the waves scattered by all Z electrons, weighted by the electron-density distribution ρ(r). This sum defines the **atomic scattering factor** f(sinθ/λ) = ∫ρ(r) e^{2πi(S·r)} dV.

**Why X-rays, not visible light:** To resolve atomic structure via diffraction, the wavelength of the radiation must be comparable to the interatomic spacing (~1–3 Å). Visible light (λ ≈ 4000–7000 Å) is roughly 1000× too long to diffract from such small spacings (per Bragg's law, nλ = 2d sinθ requires λ ≲ 2d). X-rays (λ ≈ 0.5–2.5 Å) match the interatomic scale, enabling measurable diffraction angles and structural resolution at the atomic level.

**(b) Intensity of X-rays scattered by an electron; behaviour at φ=0° and 180°**

From the Thomson scattering derivation, an electron under the oscillating field of an incident unpolarized X-ray beam re-radiates with intensity (at distance R, scattering angle φ measured from the propagation direction):

I_φ = I₀ [e⁴/(m²c⁴R²)] × (1+cos²φ)/2

(This is the classical Thomson formula; e, m are electron charge and mass, c is the speed of light.)

**Angular dependence:**
- At **φ = 0°**: cos²φ = 1 → I_φ = I₀ e⁴/(m²c⁴R²) — **maximum** intensity (forward scattering).
- At **φ = 180°**: cos²φ = 1 also → I_φ is again **equal to the forward-scattering maximum** (backscattering).
- At **φ = 90°**: cos²φ = 0 → I_φ is **minimum**, exactly half the forward/backward value.

So the polarization factor (1+cos²φ)/2 produces a symmetric intensity pattern about φ=90°, with equal maxima in the forward and backward directions and a minimum at 90°.

**(c) Carbon bar: mass scattering coefficient σ/ρ = 0.20; find (i) atoms/gram, (ii) electrons/atom**

Classical Thomson scattering cross-section per electron:
σ_e = (8π/3)(e²/4πε₀mc²)² = 0.665×10⁻²⁴ cm² (Thomson cross-section, standard value)

The mass scattering coefficient is related to the number of electrons per gram (N_e) by:
σ/ρ = σ_e × N_e  ⟹ N_e = (σ/ρ)/σ_e = 0.20/(0.665×10⁻²⁴) = **3.008×10²³ electrons/gram**

**(i) Number of carbon atoms per gram:**
N_atoms = Avogadro's number/atomic weight = 6.022×10²³/12 = **5.02×10²² atoms/gram**

**(ii) Number of electrons per carbon atom:**
Z_eff = N_e/N_atoms = 3.008×10²³/5.02×10²² ≈ **5.99 ≈ 6 electrons/atom**

This matches the known atomic number of carbon (Z=6), confirming the scattering coefficient corresponds to essentially all 6 electrons acting as independent Thomson scatterers.


---

# 2022 — Question 3

**(a) Define scattering of X-rays. Discuss the scattering mechanism of an X-ray beam.**

**Scattering** is the process by which an X-ray photon incident on matter changes direction (with or without a change in energy) due to interaction with the electrons of the material, without being absorbed.

**Mechanism:** When the oscillating electric field of an X-ray wave encounters a free or loosely-bound electron, the field exerts a periodic force on the electron, driving it into oscillation at the same frequency as the incident wave. This oscillating (accelerating) charge itself becomes a source of secondary electromagnetic radiation, re-emitted in all directions — this is **Thomson (coherent/Rayleigh) scattering**. If instead the photon transfers part of its energy and momentum to the electron (treated relativistically as a particle collision), the scattered photon emerges with reduced energy (longer wavelength) — this is **Compton (incoherent) scattering**. In a crystal, coherent scattering from the periodic array of atoms interferes constructively along specific directions, producing the diffraction pattern; incoherent scattering merely adds a smooth background.

**(b) Intensity of X-rays scattered at an angle by a single electron (derivation)**

Consider an unpolarized X-ray beam of intensity I₀ incident on a free electron. The electric field induces oscillation, and the electron radiates as an oscillating dipole. Using classical electrodynamics (Larmor's formula) for the power radiated by an accelerating charge, and averaging over the two orthogonal polarization components of unpolarized radiation, the intensity observed at distance R and scattering angle φ is:

**I_φ = I₀ [e⁴/(m²c⁴R²)] × (1+cos²φ)/2**

Derivation outline:
1. Field E = E₀ e^{iωt} exerts force F = eE on the electron, giving acceleration a = eE/m.
2. An accelerating charge radiates power per unit solid angle: dP/dΩ = (e²a²sin²ψ)/(4πε₀ 4πc³), where ψ is the angle between the acceleration vector and the observation direction.
3. Averaging over the two polarization states of unpolarized incident radiation (electric vector components parallel and perpendicular to the scattering plane) introduces the factor (1+cos²φ)/2, known as the **polarization factor**.
4. Combining gives the Thomson scattering formula above — showing intensity falls off as 1/R² and depends on scattering angle only through the polarization factor, being maximal at φ=0° and 180°, minimal at φ=90°.


---

# 2021 — Question 3

**(a) Define the scattering of X-rays.**

Scattering of X-rays is the phenomenon in which an incident X-ray photon interacts with the electrons of a material and is re-emitted in a different direction, either with the same energy (coherent/elastic) or with reduced energy (incoherent/inelastic), without being permanently absorbed.

**(b) Discuss the scattering mechanism of an X-ray beam.**

Same mechanism as described in 2022 Q3(a): the alternating electric field of the incident X-ray forces the atomic electrons into oscillation, and each oscillating electron re-radiates energy at the same frequency (Thomson/coherent scattering) — this is the process responsible for diffraction. A smaller fraction of photons undergo Compton (incoherent) scattering, transferring some energy/momentum to the electron and emerging with a longer wavelength, contributing only to background.

**(c) Deduce an expression for the intensity of X-rays scattered by a pair of electrons.**

(Same derivation as 2024 Q3(c) and 2019 Q3(b) below.) For two electrons O₁, O₂ separated by vector **r**, with scattering vector **S** = (ŝ−ŝ₀)/λ, the phase difference is δ = 2π**r**·**S**. The resultant intensity at a distant point P is:

**I_P = 2I_e(1 + cos δ) = 2I_e[1 + cos(2π r·S)]**

where I_e is the intensity scattered by a single electron. For random orientation (isotropic averaging), this reduces to:

**Ī_P = 2I_e(1 + sin x/x)**, with x = 4πr sinθ/λ

showing the scattered intensity from a pair of electrons depends on both the separation r and the scattering angle θ, oscillating between the coherent limits 4I_e (small x) and asymptotically 2I_e (large x).


---

# 2020 — Question 3

**(a) Why are X-rays scattered by electrons and atoms? Applications of XRD.**

X-rays are scattered by **electrons** because the alternating electric field of the X-ray wave accelerates each charged electron, and (per classical electrodynamics) an accelerating charge radiates electromagnetic energy at the same frequency — this re-radiation constitutes scattering. Nuclei scatter negligibly because scattered intensity ∝ 1/m², and nuclei are thousands of times more massive than electrons.

An **atom** scatters X-rays as the coherent superposition of the waves scattered independently by all its electrons; the resultant amplitude (the atomic scattering factor f) depends on the spatial distribution of electron density and on sinθ/λ, decreasing as θ increases due to increasing path-difference-induced destructive interference among electrons within the same atom.

**Applications of XRD:** Determination of crystal structure (unit cell, atomic positions), phase identification of crystalline materials, measurement of lattice parameters and strain, grain size and crystallite size analysis, texture/preferred-orientation studies, quality control in pharmaceuticals and metallurgy, and study of thin films and nanomaterials.

**(b) Deduce an expression for the intensity of X-rays scattered at an angle by a single electron.**

Identical derivation to 2022 Q3(b): using the classical dipole-radiation (Larmor) approach and averaging over unpolarized incident radiation gives the Thomson formula:

**I_φ = I₀ [e⁴/(m²c⁴R²)] × (1+cos²φ)/2**

with maxima at φ = 0° and 180°, and a minimum (half the maximum value) at φ = 90°.


---

# 2019 — Question 3

**(a) Define scattering of X-rays. Discuss the scattering mechanism of an X-ray beam.**

Same definition and mechanism as given in 2022 Q3(a) / 2021 Q3(a)–(b): scattering is the redirection of an incident X-ray photon by interaction with atomic electrons — coherently (Thomson/Rayleigh, same wavelength, capable of interference and hence diffraction) or incoherently (Compton, longer wavelength, no fixed phase, contributes to background).

**(b) Deduce an expression for the intensity of X-rays scattered by a pair of electrons.**

Full derivation as given in 2024 Q3(c):

For two identical scatterers O₁, O₂ separated by **r**, with incident/scattered unit vectors ŝ₀, ŝ and scattering vector **S**=(ŝ−ŝ₀)/λ, the phase difference between the waves scattered from the two electrons is:

δ = 2π **r**·**S**

Summing the two waves of equal amplitude A_φ with this phase difference:

|A_P| = 2A_φ cos(δ/2)  ⟹  I_P = |A_P|² = 4A_φ²cos²(δ/2) = 2I_e(1+cos δ)

**I_P = 2I_e[1 + cos(2π r·S)]**

where I_e = A_φ² is the intensity scattered by one electron. For a randomly oriented pair (isotropic average over all directions of **r**):

**Ī_P = 2I_e(1 + sin x/x)**, x = 4πr sinθ/λ

This shows the scattered intensity depends on the electron separation r and scattering angle θ, varying between 4I_e (θ→0, in-phase limit) and oscillating about 2I_e at larger angles as the two waves progressively lose coherence.

