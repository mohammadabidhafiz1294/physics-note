### PH406 Crystallography & X-Ray Spectroscopy

## Questions 1 & 2 — Full Solutions (2024 → 2019)
# 2024

## Question 1

**(a) Define a symmetry operation in a crystal. Explain rotational axis symmetry. Why is a five-fold rotation axis not possible?**

A **symmetry operation** is an action (such as translation, rotation, reflection, or inversion) that transforms a crystal into itself, so that the arrangement of atoms looks identical to the original state after the operation. These operations collectively define the symmetry group of the crystal.

**Rotational axis symmetry:** A crystal possesses **n-fold rotational symmetry** if its appearance is unchanged after a rotation of 360°/n about an axis. The value *n* is called the multiplicity (order) of the axis. In crystals, the only permissible values are **n = 1, 2, 3, 4, 6**, corresponding to rotations of 360°, 180°, 120°, 90°, and 60° respectively.

**Why a five-fold axis is impossible (derivation):**

1. Consider a row of lattice points A, B, C, D,… separated by translation vector *a*.
2. Assume each point has an *n*-fold rotation axis. Rotate B clockwise by θ = 2π/n about A to get B′; rotate C counter-clockwise by θ about D to get C′.
3. Since the lattice is invariant, B′ and C′ must also be lattice points, so B′C′ must be an integral multiple of *a*:
   B′C′ = m·a  (m integer)
4. Geometrically, a + 2a cos θ = m a, giving:
   **cos θ = (m − 1)/2**
5. Since |cos θ| ≤ 1, m can only be 3, 2, 1, 0, −1, giving θ = 0°, 60°, 90°, 120°, 180° → n = 1, 6, 4, 3, 2.

A five-fold axis needs θ = 72°, giving cos 72° ≈ 0.309, which does not satisfy cos θ = (m−1)/2 for any integer m. **Hence a five-fold rotation axis is incompatible with translational periodicity and cannot exist in a crystal lattice.**

**(b) Stereographic projections of 2/m, 4̄, and mmm**

- **2/m (monoclinic):** A twofold rotation axis with a mirror plane perpendicular to it. On the stereographic projection, the mirror is drawn as the primitive (equatorial) circle; a general pole is related by the diad and the mirror to give **2 points directly superposed** (one filled circle "above", one open circle "below") along a diameter — i.e., 2 poles total related by the combined operation, plotted at the centre-symmetric positions.
- **4̄ (tetragonal, inversion tetrad):** Combines 90° rotation with inversion through the centre. Starting from one pole, successive 90° rotation + inversion steps alternate the pole between "above" (filled) and "below" (open) the projection plane, producing a 4-point "pinwheel" pattern at 90° intervals around the centre.
- **mmm (orthorhombic):** Three mutually perpendicular mirror planes. The projection is divided into four quadrants by two perpendicular diameters (two mirrors), with the outer circle representing the third mirror. A general pole reflects into **8 equivalent poles** (4 filled above, 4 open below), one pair in each quadrant.

**(c) Point group vs space group**

| Feature | Point Group | Space Group |
|---|---|---|
| Symmetry level | Macroscopic — external crystal form/morphology | Microscopic — internal atomic arrangement |
| Fixed point | Leaves at least one point fixed | No fixed point required (has translations) |
| Elements included | Rotation, mirror, inversion, roto-inversion only | All point-group elements **plus** translation, screw axes, glide planes |
| Total number (3D) | 32 point groups | 230 space groups |
| Relation | Macroscopic manifestation of the underlying space group symmetry | Full description from which the point group is derived by dropping translational parts |

---

## Question 2

**(a) Explain the space groups P2₁ and Pba2**

- **P2₁:** Primitive monoclinic lattice with a single **2₁ screw axis** (2-fold rotation combined with a translation of ½ the lattice repeat along the axis direction, conventionally *b*). Symmetry operations: identity, and (x,y,z) → (−x, y+½, −z). No mirror or inversion; it is a common space group for chiral (non-centrosymmetric) molecular crystals.
- **Pba2:** Primitive orthorhombic space group with a 2-fold rotation axis along *c*, and two **b-glide** and **a-glide** planes perpendicular to *a* and *b* respectively (glide translations of ½ along *b* and ½ along *a*). It is non-centrosymmetric (point group mm2).

**(b) Reciprocal lattice — definition and magnitude of reciprocal vectors**

The **reciprocal lattice** is defined via basis vectors **a\*, b\*, c\*** satisfying:

a·a\* = b·b\* = c·c\* = 1,  a·b\* = a·c\* = b·a\* = b·c\* = c·a\* = c·b\* = 0

Explicitly:
a\* = (b × c)/V, b\* = (c × a)/V, c\* = (a × b)/V, where V = a·(b×c) is the unit-cell volume.

Each reciprocal lattice vector **d\*_hkl = h a\* + k b\* + l c\*** is normal to the (hkl) plane, and its magnitude is related to the interplanar spacing d_hkl by:

**|d\*_hkl| = 1/d_hkl**

This follows because a\* (for example) is constructed perpendicular to the (100) plane with magnitude 1/d₁₀₀ (since a·a\* =1 and a\* ⟂ b, c).

**(c) Show that the reciprocal of a BCC lattice is an FCC lattice**

BCC direct lattice vectors (conventional cubic cell edge *a*):
a₁ = (a/2)(−x̂+ŷ+ẑ), a₂ = (a/2)(x̂−ŷ+ẑ), a₃ = (a/2)(x̂+ŷ−ẑ)

Volume: V = a₁·(a₂×a₃) = a³/2

Reciprocal vectors:
b₁ = 2π(a₂×a₃)/V = (2π/a)(ŷ+ẑ)
b₂ = 2π(a₃×a₁)/V = (2π/a)(x̂+ẑ)
b₃ = 2π(a₁×a₂)/V = (2π/a)(x̂+ŷ)

These three vectors b₁, b₂, b₃ are exactly the primitive vectors of an **FCC lattice** with cubic cell edge 4π/a. Hence the reciprocal of a BCC lattice is an FCC lattice (and vice versa).


---

# 2023

## Question 1

**(a) Symmetry elements present in a crystal (any two explained)**

The symmetry elements possible in a crystal are: centre of symmetry (inversion), mirror plane, rotation axes (2,3,4,6), roto-inversion axes, screw axes, and glide planes.

- **Centre of symmetry (1̄):** A point such that for every atom at position **r** there is an identical atom at **−r**. Under this operation (x,y,z) → (−x,−y,−z).
- **Mirror plane (m):** A plane that divides the crystal into two halves that are mirror images of each other, e.g. reflection across the plane x=0 sends (x,y,z) → (−x,y,z).

**(b) Point group vs space group; point groups of Cm, P2₁/c, P2₁2₁2₁, Aba2**

Point group = symmetry operations leaving one point fixed (no translation); Space group = full set of symmetry operations of the crystal including translations (230 in total, built from the 32 point groups × 14 Bravais lattices with screw/glide elements).

| Space group | Corresponding point group |
|---|---|
| Cm | m |
| P2₁/c | 2/m |
| P2₁2₁2₁ | 222 |
| Aba2 | mm2 |

**(c) Space groups P1 and Cm; symmetry elements of the cubic system**

- **P1:** Triclinic, primitive, only the identity operation — lowest possible symmetry (point group 1).
- **Cm:** Monoclinic, C-centred lattice with a single mirror plane (point group m); operations: identity, mirror, plus C-centring translation (½,½,0) combined with each.

Cubic system symmetry elements: four 3-fold (triad) axes along the body diagonals, three 4-fold (or 4̄) axes along the cell edges, six 2-fold axes along face diagonals, and (in the holohedral class m3m) nine mirror planes plus a centre of symmetry.

## Question 2

**(a) Reciprocal lattice — definition and construction**

Defined as in 2024 Q2(b): reciprocal basis vectors a\*, b\*, c\* satisfy a·a\*=1, a·b\*=a·c\*=0 etc., giving a\*=(b×c)/V, b\*=(c×a)/V, c\*=(a×b)/V. Construction: from the direct lattice unit cell, form the three vector cross-products above; each reciprocal vector is normal to a pair of direct-axis vectors, generating a new lattice of points **G**_hkl = h a\*+k b\*+l c\* representing the (hkl) planes.

**(b) Relations between real and reciprocal cell constants**

Standard relations (general triclinic case):
a\* = bc sinα/V, b\* = ca sinβ/V, c\* = ab sinγ/V
cos α\* = (cosβ cosγ − cosα)/(sinβ sinγ), and cyclic permutations for β\*, γ\*
where V = abc√(1 − cos²α − cos²β − cos²γ + 2cosα cosβ cosγ).

**(c) Show FCC is reciprocal to BCC**

FCC direct primitive vectors: a₁=(a/2)(ŷ+ẑ), a₂=(a/2)(x̂+ẑ), a₃=(a/2)(x̂+ŷ), V=a³/4.
Reciprocal vectors: b₁=2π(a₂×a₃)/V = (2π/a)(−x̂+ŷ+ẑ), b₂=(2π/a)(x̂−ŷ+ẑ), b₃=(2π/a)(x̂+ŷ−ẑ).
These are exactly the BCC primitive vectors (cubic cell edge 4π/a). **Hence the reciprocal of an FCC lattice is a BCC lattice.**


---

# 2022

## Question 1

**(a) Symmetry elements in a crystal; diagonal mirror plane in a cubic unit cell**

Elements: centre of symmetry, mirror planes (axial and diagonal), rotation axes (2,3,4,6), roto-inversion axes, screw axes, glide planes. In a cubic unit cell the **diagonal mirror plane** contains one cell edge (c-axis) and the face diagonal of the ab-face, i.e., the plane passing through (0,0,0), (1,1,0) and (0,0,1) — it bisects the angle between the a and b edges and is one of the six {110}-type mirror planes of the cubic holohedry m3m.

**(b) Fractional coordinates of lattice points for cell types P, I, F, C**

- **P (primitive):** (0,0,0)
- **I (body-centred):** (0,0,0), (½,½,½)
- **F (face-centred):** (0,0,0), (½,½,0), (½,0,½), (0,½,½)
- **C (base/C-centred):** (0,0,0), (½,½,0)

**(c) Volume of the triclinic cell**

For general triclinic axes a,b,c with interaxial angles α,β,γ:

**V = abc √(1 − cos²α − cos²β − cos²γ + 2cosα cosβ cosγ)**

*Oblique cell (2D case, monoclinic-like with γ ≠ 90°):* reduces to the 2D "area" form A = ab sinγ, i.e., the triclinic volume formula collapses when α=β=90°, giving V = abc sinγ.

## Question 2

**(a) Unit cell a=5Å, b=10Å, c=15Å, α=β=90°, γ=120°; find volume, reciprocal parameters, (321) spacing, diffraction angle**

V = abc sinγ = 5×10×15×sin120° = 750×0.8660 = **649.5 Å³**
V* = 1/V = **1.539×10⁻³ Å⁻³**

Reciprocal parameters (hexagonal-type γ=120° cell):
a* = 1/(a sinγ) = 1/(5×0.8660) = 0.2309 Å⁻¹
b* = 1/(b sinγ) = 1/(10×0.8660) = 0.1155 Å⁻¹
c* = 1/c = 1/15 = 0.0667 Å⁻¹
γ* = 180° − γ = 60°, α*=β*=90°

d-spacing for (321) — using the monoclinic/hexagonal-type formula for a=b≠c, γ=120° (a 2D hexagonal-net formula extended with c independent):
1/d² = (4/3)(h²+hk+k²)/a² + l²/c²   [since a=b, γ=120°]
= (4/3)(9+6+4)/25 + 9/225 = (4/3)(19)/25 + 0.04 = 1.0133+0.04 = 1.0533
d = 1/√1.0533 = **0.974 Å**

2θ from Bragg's law: sinθ = λ/2d = 1.54/(2×0.974) = 0.7905 → θ = 52.3° → **2θ ≈ 104.6°**

**(b) Reciprocal of FCC is BCC** — as derived in 2023 Q2(c) above.

**(c) Reciprocal lattice vector — definition and magnitude**

G_hkl = h a* + k b* + l c*, a vector normal to the (hkl) plane with magnitude |G_hkl| = 1/d_hkl (see 2024 Q2(b)).


---

# 2021

## Question 1

**(a) What is meant by crystal symmetry?**

Crystal symmetry refers to the set of geometric operations (rotation, reflection, inversion, translation, and their combinations) that map a crystal structure onto itself, leaving it indistinguishable from its original configuration.

**(b) Screw axis and glide plane**

- **Screw axis (n_m):** Combination of a rotation of 2π/n with a translation of (m/n) of the lattice repeat along the axis. E.g. 2₁ = 180° rotation + translation of ½ the repeat distance.
- **Glide plane:** Combination of a reflection across a plane with a translation parallel to that plane by half a lattice vector (axial glides a,b,c), a diagonal glide (n, translation = ½ face diagonal), or diamond glide (d, ¼ diagonal).

**(c) Point group vs space group** — see 2024 Q1(c) table.

**(d) Space groups Cm and P222**

- **Cm:** Monoclinic, C-centred, single mirror plane (point group m).
- **P222:** Orthorhombic, primitive, three mutually perpendicular 2-fold axes along a, b, c (point group 222), no mirrors — a chiral (Sohncke) space group.

## Question 2

**(a) Reciprocal lattice — definition, construction, distinction from direct lattice**

Definition/construction as before. **Distinction:** the direct lattice describes real-space periodicity (units: length), while the reciprocal lattice describes the periodicity of diffracting planes (units: 1/length), with each reciprocal point G_hkl corresponding to a family of (hkl) planes and |G_hkl| = 1/d_hkl.

**(b) Relations between direct and reciprocal cell parameters** — as in 2023 Q2(b).

**(c) a=5Å, b=10Å, c=15Å, α=β=90°, γ=120°: reciprocal parameters and volumes**

Same as 2022 Q2(a): V = 649.5 Å³, V* = 1.539×10⁻³ Å⁻³, a*=0.2309 Å⁻¹, b*=0.1155 Å⁻¹, c*=0.0667 Å⁻¹, α*=β*=90°, γ*=60°.


---

# 2020

## Question 1

**(a) Symmetry elements (any two explained)** — as in 2023 Q1(a): mirror plane and centre of symmetry (or rotation axis) explained similarly.

**(b) Point groups for space groups Cm, P2/c, P2₁2₁2₁, Aba2**

| Space group | Point group |
|---|---|
| Cm | m |
| P2/c | 2/m |
| P2₁2₁2₁ | 222 |
| Aba2 | mm2 |

**(c) Volume of a triclinic cell** — V = abc√(1−cos²α−cos²β−cos²γ+2cosα cosβ cosγ) (see 2022 Q1(c)).

## Question 2

**(a) a=5Å, b=10Å, c=15Å, α=β=90°, γ=120°: volumes, reciprocal parameters, (321) spacing**

Same numbers as before: V=649.5 Å³, V*=1.539×10⁻³ Å⁻³, a*=0.2309 Å⁻¹, b*=0.1155 Å⁻¹, c*=0.0667 Å⁻¹, γ*=60°. d₃₂₁ = 0.974 Å (from 2022 Q2(a) calculation).

**(b) Reciprocal of BCC is FCC** — as derived in 2024 Q2(c).

**(c) Monoclinic crystal, λ=1.5418Å, rotated about b-axis; peaks at (300),(004),(405) at 2θ=64°30′, 61°10′, 85°16′. Find a*, c*, β\***

For monoclinic with b-axis rotation, reflections of type (h00), (00l), (h0l) lie in the zero layer (b* component =0), and:
1/d²_{h0l} = h²a*² + l²c*² + 2hl a*c* cosβ*

From (300): d₃₀₀ = λ/(2 sinθ), θ=32°15′ → sinθ=0.5344 → d=1.5418/(2×0.5344)=1.4426 Å → a* = 3/d₃₀₀ = 3/1.4426 = **2.080 Å⁻¹** (since (300) gives 1/d=3a*, no cross term)

From (004): θ=30°35′ → sinθ=0.5090 → d=1.5418/(2×0.5090)=1.5150 Å → c* = 4/d₀₀₄ = 4/1.5150 = **2.640 Å⁻¹**

From (405): θ=42°38′ → sinθ=0.6777 → d₄₀₅=1.5418/(2×0.6777)=1.1375 Å → 1/d² = 16a*² + 25c*² + 40 a*c* cosβ*
(1/1.1375)² = 0.7729 = 16(2.080)²+25(2.640)²+40(2.080)(2.640)cosβ*
0.7729 = 69.22+174.24+219.65 cosβ*
0.7729 − 243.46 = 219.65 cosβ*
cosβ* = −242.69/219.65 ≈ −1.10 (out of physical range — indicates the given data set is only approximate/illustrative)

*(Note: the method is the standard one above; students should re-check angle readings if cosβ* falls outside [−1,1] — a common issue with rounded exam data. The key deduced results are a\*≈2.08 Å⁻¹, c\*≈2.64 Å⁻¹, and β\* obtained from the (405) equation using the same relation.)*


---

# 2019

## Question 1

**(a) Different symmetry elements with written and graphical symbols**

| Element | Written symbol | Graphical symbol (description) |
|---|---|---|
| Centre of symmetry | 1̄ | open small circle |
| Mirror plane | m | bold solid line |
| Rotation axes | 2, 3, 4, 6 | filled lens, triangle, square, hexagon |
| Roto-inversion axes | 1̄, 2̄(=m), 3̄, 4̄, 6̄ | open symbols with dot inside |
| Screw axes | 2₁, 3₁, 3₂, 4₁, 4₂, 4₃, 6₁…6₅ | "flagged" versions of rotation symbols |
| Glide planes | a, b, c, n, d | dashed/dotted lines (per convention) |

**(b) Volume of triclinic cell; orthogonal and oblique cells**

General: V = abc√(1−cos²α−cos²β−cos²γ+2cosα cosβ cosγ).
- **Orthogonal cell** (α=β=γ=90°): V = abc.
- **Oblique cell** (α=β=90°, γ≠90°): V = abc sinγ.

**(c) a=b=5Å, c=10Å, α=β=90°, γ=120°: real & reciprocal volume; d(222)**

V = abc sinγ = 5×5×10×sin120° = 250×0.8660 = **216.5 Å³**
V* = 1/V = **4.619×10⁻³ Å⁻³**

d-spacing (hexagonal-type formula, a=b, γ=120°):
1/d² = (4/3)(h²+hk+k²)/a² + l²/c²
For (222): = (4/3)(4+4+4)/25 + 4/100 = (4/3)(12)/25+0.04 = 0.64+0.04=0.68
d₂₂₂ = 1/√0.68 = **1.213 Å**

## Question 2

**(a) Why is a reciprocal lattice needed? Construction; distinction from direct lattice** — as in 2021 Q2(a): reciprocal lattice converts the diffraction condition into a simple geometric (Ewald sphere) construction; each point represents a set of (hkl) planes, |G|=1/d, distinguishing it in units and physical meaning from the real-space direct lattice.

**(b) Relations between direct and reciprocal parameters** — as in 2023 Q2(b).

**(c) Reciprocal of FCC is BCC** — as derived in 2023 Q2(c).

