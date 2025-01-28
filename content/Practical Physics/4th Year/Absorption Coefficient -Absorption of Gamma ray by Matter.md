### Absorption coefficient vs compton effect vs Photoelectric effect vs Pair production

These are three important interactions of electromagnetic radiation (e.g., X-rays or gamma rays) with matter:

---
#### 1. **Absorption Coefficient**

The absorption coefficient quantifies how much a material attenuates radiation. It depends on the material properties, the type of radiation, and the interaction mechanisms involved. It is commonly expressed as: $μ=1λ/mu = \frac{1}{\lambda}$ where $μ\mu$ is the linear absorption coefficient, and λ\lambda is the mean free path of the photons in the material.

---
#### 2. **Compton Effect**

The Compton effect describes the inelastic scattering of X-rays or gamma rays by electrons. When a photon collides with an electron, it transfers some of its energy to the electron, causing the photon to lose energy and change direction. The energy and wavelength change are given by:

$$Δλ=hmec(1−cos⁡θ)\Delta \lambda = \frac{h}{m_e c} (1 - \cos \theta)$$
where:
- h is Planck's constant,
- $m_e$ is the electron mass,
- $c$ is the speed of light,
- $\theta$ is the scattering angle.
This effect is significant for intermediate photon energies.

---
#### 3. **Photoelectric Effect**

In the photoelectric effect, a photon transfers all its energy to a bound electron, ejecting it from the atom. The photon's energy must exceed the electron's binding energy ($E_b$):

$$E_{photon}=hν=E_{\text{kinetic}}+E_{\text{photon}} = h \nu = E_{\text{kinetic}} + E_b$$
where:
- $E_{\text{kinetic}}$ is the kinetic energy of the ejected electron,
- $E_b$ is the binding energy of the electron.

This effect is dominant at low photon energies and depends on the atomic number ($Z$) of the material.

---
#### 4. **Pair Production**
Pair production occurs when a high-energy photon interacts with a nucleus and converts into an electron-positron pair. The photon energy must be greater than the combined rest mass energy of the electron and positron ($2m_e c^2$):

$$Ephoton>1.022 MeVE_{\text{photon}} > 1.022 \, \text{MeV}$$
This process is significant for very high photon energies, typically in the MeV range.

---
Each interaction dominates in a different photon energy range and has distinct applications in fields such as medical imaging, radiation therapy, and nuclear physics.
#### **Half Value Thickness (HVT)**

The **Half Value Thickness (HVT)**, also known as the **Half Value Layer (HVL)**, is a measure of the material's ability to attenuate or reduce the intensity of radiation. It represents the thickness of a material required to reduce the intensity of the radiation to **half** of its initial value.

The attenuation of radiation follows an exponential law:

$I=I0e−μxI = I_0 e^{-\mu x}$

where:

- II: Intensity of radiation after passing through the material
- $I_0$: Initial intensity of the radiation
- μ\mu: Linear absorption coefficient of the material
- xx: Thickness of the material

For half-value thickness, $I = \frac{I_0}{2}$, so:
$$\frac{I_0}{2} = I_0 e^{-\mu \, x_{\text{HVT}}}$$

Taking the natural logarithm:

$$x_{HVT}=ln⁡(2)μx_{\text{HVT}} = \frac{\ln(2)}{\mu}$$

where $ln⁡(2)≈0.693$.

---
#### **Key Points**

1. **Dependence on Material:** HVT depends on the type of material and its density. Denser materials (like lead) have a smaller HVT because they absorb radiation more effectively.
2. **Dependence on Radiation Energy:** HVT also depends on the energy of the radiation. Higher energy photons (e.g., gamma rays) require a greater thickness to achieve the same attenuation.
3. **Applications:**
    - **Radiation Shielding:** Used in designing protective barriers for X-ray and gamma-ray shielding.
    - **Medical Imaging and Therapy:** Helps determine the required shielding thickness in X-ray and radiation therapy rooms.
    - **Nuclear Physics:** Used to characterize materials for radiation attenuation.
---
For example:

- Lead may have a small HVT (a few millimeters) for X-rays or gamma rays due to its high density and atomic number.
- Concrete may require several centimeters for the same radiation attenuation.

#### **Components of a Gamma-Ray Schema**

1. **Energy Levels**:
    
    - Represented as horizontal lines.
    - The vertical position of each line corresponds to the energy of the nuclear state (in units of keV or MeV).
    - Energy levels are labeled by their excitation energy and, often, their quantum numbers (e.g., spin JJ and parity π\pi).
2. **Ground State**:
    
    - The lowest energy level, typically labeled as 0+0^+ or 0 keV0 \, \text{keV}.
3. **Excited States**:
    
    - Higher energy levels where the nucleus can exist temporarily after absorbing energy (e.g., from particle interactions).
    - These states are unstable and decay to lower states by emitting gamma rays.
4. **Gamma Transitions**:
    
    - Represented by vertical or diagonal arrows connecting energy levels.
    - Each arrow represents a gamma-ray photon emitted as the nucleus transitions from a higher energy state to a lower one.
    - The energy of the emitted gamma ray is equal to the energy difference between the two levels: $E_\gamma = E_{\text{higher}} - E_{\text{lower}}$
5. **Multipolarity and Transition Type**:
    
    - Gamma transitions can be of different types (e.g., E1, M1, E2), where E and M stand for electric and magnetic transitions, and the number indicates the multipolarity.
    - These determine the selection rules and likelihood of the transition.
6. **Lifetimes of States**:
    
    - Sometimes lifetimes of excited states (e.g., nanoseconds or picoseconds) are noted, indicating how quickly the nucleus decays.
7. **Branching Ratios**:
    
    - If an excited state decays via multiple gamma-ray pathways, the branching ratio (percentage of decays through each path) is often shown.

---

#### **Example of a Gamma-Ray Schema**

For a nucleus such as **Cobalt-60 (60Co^{60} \text{Co})**, the schema might look like this:

- Ground State: $0^+ \, (0 \, \text{keV})$
- First Excited State: $1173 \, \text{keV} \, (2^+)$
- Second Excited State: $1332 \, \text{keV} \, (2^+)$

Gamma Transitions:

- $1332 \, \text{keV} \to 1173 \, \text{keV}$: Emits a $159 \, \text{keV}$ gamma ray.
- $1173 \, \text{keV} \to 0 \, \text{keV}:$ Emits a $1173 \, \text{keV}$ gamma ray.

---
#### **Applications**

1. **Nuclear Spectroscopy**:
    - Analyzing gamma-ray spectra to identify nuclear energy levels and structure.
2. **Decay Analysis**:
    - Understanding radioactive decay chains and gamma emissions.
3. **Material Identification**:
    - Detecting gamma signatures to identify isotopes in nuclear reactors or security settings.
4. **Astrophysics**:
    - Studying gamma emissions from cosmic sources to understand stellar processes.
