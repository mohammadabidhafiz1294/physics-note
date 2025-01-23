### Crystal Symmetry
**Crystal symmetry describes the ordered and repetitive arrangement of atoms or molecules within a crystal, resulting in a symmetrical pattern that extends in three dimensions.** This inherent order is evident in several aspects of a crystal's structure and properties:

### 1. External Manifestations of Symmetry

- **Crystal Habit**: Crystals of a given substance tend to develop similar shapes, implying that the chemical nature of the material influences its crystal habit, or the general form it takes. The flat surfaces, or facets, of well-formed crystals are remarkably planar and are a direct consequence of the regular arrangement of atoms within the crystal structure.
- **Cleavage**: The tendency of crystals to break along specific planes, called cleavage planes, also reflects their internal symmetry. Cleavage occurs along planes where the bonding forces between atoms are weaker, and these planes are determined by the underlying atomic arrangement.
- **Normals to Faces**: Analyzing the set of normals (lines perpendicular to the faces) of a crystal is crucial for understanding its symmetry. Even if a crystal lacks perfect external symmetry, the arrangement of these normals reveals the inherent symmetry of its internal structure. For instance, a collection of seemingly irregular plate-like crystals, when rearranged based on the parallelism of their faces, reveals an underlying hexagonal symmetry.

### 2. Unit Cell and Symmetry Elements

The concept of a **unit cell** is fundamental to understanding crystal symmetry. A **unit cell is the smallest repeating unit in a crystal lattice**. When stacked together in three dimensions, these unit cells create the entire crystal structure.

- **Crystal Systems**: The shape of the unit cell determines the crystal system to which a crystal belongs. There are seven crystal systems: triclinic, monoclinic, orthorhombic, tetragonal, trigonal, hexagonal, and cubic. Each system is defined by specific relationships between the lengths of the unit cell edges (a, b, c) and the angles between them (α, β, γ).
- **Symmetry Elements**: The symmetry of the unit cell, and consequently of the entire crystal, is described by specific symmetry elements. These elements include:
    - **Center of symmetry**: This exists when every point in the unit cell has an identical point located an equal distance but in the opposite direction from a central point.
    - **Mirror plane**: This is a plane that divides the unit cell into two mirror images.
    - **Rotation axes**: These axes define rotations (by 180°, 120°, 90°, or 60°) that leave the appearance of the unit cell unchanged.
    - **Inversion axes**: These axes involve a combination of rotation and inversion through a center point.
    - **Glide planes**: These involve reflection across a plane followed by a translation.
    - **Screw axes**: These combine rotation with a translation along the axis.

### 3. Crystal Classes and Space Groups

- **Crystal Classes**: The 32 crystal classes arise from the different possible arrangements of symmetry elements within the seven crystal systems. Each crystal class is represented by a unique stereographic projection. For example, the triclinic system has two crystal classes, 1 and \overline{1}, representing the absence of symmetry and the presence of a center of symmetry, respectively.
- **Space Groups**: The 230 space groups describe the complete set of symmetry operations that can be applied to a crystal structure, including those related to translational symmetry. Each space group is associated with a specific crystal class and lattice type. The International Tables for Crystallography provide a detailed description of all 230 space groups.

### 4. Significance of Crystal Symmetry

The understanding of crystal symmetry is essential in X-ray crystallography.

- **Diffraction Patterns**: The symmetrical arrangement of atoms in a crystal leads to the production of characteristic diffraction patterns when X-rays interact with the crystal. By analyzing these patterns, crystallographers can determine the positions of atoms within the unit cell, ultimately revealing the crystal structure.
- **Structure Determination**: The identification of systematic absences in diffraction patterns, which are specific reflections that are absent due to the presence of translational symmetry elements like screw axes and glide planes, helps in determining the space group of the crystal.
- **Structure Factor**: The structure factor, a mathematical expression that describes the amplitude and phase of the X-ray waves scattered by the atoms in a unit cell, is also influenced by the symmetry elements present within the unit cell. This simplifies the calculation of structure factors, which are crucial for determining the electron density distribution in the crystal.

The study of crystal symmetry is not just about understanding the aesthetic beauty of crystals; it is also about unraveling the fundamental principles that govern the structure and properties of materials at the atomic level. This knowledge has broad applications in fields such as materials science, chemistry, and biology.

### Centre of Symmetry ($\bar{1}$)

A **center of symmetry**, also called an inversion center, is a point within a crystal such that for any atom at vector position **r** relative to the center of symmetry, there is an equivalent atom located at **-r**. A crystal has a center of symmetry when, for every point within the crystal, **faces occur in parallel pairs of equal dimensions on opposite sides of the point and equidistant from it**. **Figure 1.5 (a) from source provides examples of centrosymmetric crystals**.

Even if a crystal does not possess a center of symmetry, the arrangement of **normals to its faces may still reveal the intrinsic presence of a center**. This is because the **normals to centrosymmetrically related faces occur in collinear pairs**. **Figure 1.5 (b) from source illustrates this concept on a stereographic projection.**
![[Centre of Symmetry.png | 700]]
The **presence of a center of symmetry** significantly **simplifies the analysis of a crystal structure and its diffraction pattern**. For instance:

- When the center of symmetry is chosen as the origin of the unit cell, the structure factor, which represents the scattering amplitude from a centrosymmetric arrangement of atoms, becomes real.
- Additionally, a phase-vector diagram for the structure factor of a centrosymmetric structure clearly shows that the structure factor is real.

The **International Tables for Crystallography always refer a centrosymmetric unit cell to a center of symmetry as the origin**. This convention was observed in the description of the space group $P21/c$. However, it's important to note that **Friedel's law** makes it challenging to **directly detect a center of symmetry from X-ray photographs**. This law states that the weighted reciprocal lattice always exhibits a center of symmetry, irrespective of the presence or absence of a center of symmetry in the actual crystal structure.

As a result, **statistical methods** are employed to differentiate between centrosymmetric and non-centrosymmetric structures based on the **distribution of intensities** in the diffraction data. These methods leverage the distinct intensity distributions exhibited by the two structural types. The **N(z) test**, for example, helps identify a center of symmetry by comparing the cumulative distribution of normalized intensities to theoretical distributions for centrosymmetric and non-centrosymmetric structures.
### Mirror Plane (m)

A **mirror plane**, also known as a plane of symmetry, is a plane that divides a crystal into two halves that are mirror images of each other. **Crystals with mirror planes exhibit this symmetry in their external morphology, and the arrangement of normals to their faces reflects this symmetry**.

**Figure 1.6(a) from source shows examples of crystals possessing mirror planes.**

**In stereographic projections, mirror planes are clearly visible when the projecting plane is either parallel or perpendicular to the mirror plane**. **Figure 1.6(b) from source illustrates these two cases:**

- **(i) Mirror Plane in the Plane of Projection**: When the mirror plane lies within the plane of projection, the stereographic projection shows the **mirror plane as a straight line**, with **poles (representing face normals) located symmetrically on either side**.
    
- **(ii) Mirror Plane Perpendicular to the Plane of Projection**: If the mirror plane is perpendicular to the plane of projection, it appears as a **great circle (a circle that divides the stereographic projection into two hemispheres)**. **Poles related by the mirror plane will be located at equal angular distances from the great circle but on opposite sides.**
![[Mirror plane.png| 700]]
The **presence of a mirror plane** in a crystal structure has several important consequences for the analysis of the structure and its diffraction pattern:

- **It imposes constraints on the arrangement of atoms within the unit cell**. Atoms must be located either on the mirror plane or in pairs symmetrically related to it.
    
- **It affects the structure factor**. When a mirror plane is present, certain terms in the structure factor equation will cancel out, leading to specific relationships between the structure factors of different reflections.
    
- **It can give rise to systematic absences in the diffraction pattern**. These absences are reflections that have zero intensity because of the destructive interference of X-rays scattered by symmetry-related atoms. For instance, a **c-glide plane perpendicular to the b axis will result in systematic absences for reflections with indices (h0l) where l is odd**. This is because the c-glide operation introduces a phase shift of π for these reflections, leading to complete cancellation of the scattered waves.

Similar to the case with a center of symmetry, **identifying mirror planes from X-ray photographs alone can be difficult** due to Friedel’s law. Statistical tests based on the distribution of intensities are often needed to confirm the presence of a mirror plane. One such test involves comparing the average intensity of reflections related by the suspected mirror plane to the average intensity of general reflections. **For example, the presence of a mirror plane perpendicular to the b axis is indicated if the average intensity of ($h0l$) reflections is twice the average intensity of general reflections**. This arises because the mirror plane effectively doubles the number of atoms contributing to these specific reflections in the projected structure.
### Rotation Axes (2,3,4,6)

A **rotation axis** is an imaginary line that passes through a crystal such that a rotation of the crystal about this line by an angle of $2π/n$ leaves the appearance of the crystal unchanged. The integer **n** is called the **order of the rotation axis**. Allowed values of n in a crystal are **1, 2, 3, 4, and 6**, corresponding to **monad, diad, triad, tetrad, and hexad axes**, respectively.

- A **diad axis (n=2)** implies that a rotation of 180° leaves the crystal unchanged.
- A **triad axis (n=3)** implies that rotations of 120° leave the crystal unchanged.
- **Tetrad (n=4)** and **hexad (n=6) axes** imply rotational symmetries of 90° and 60°, respectively.

**Figure 1.7(a) from source illustrates crystals possessing various rotation axes, with perspective views and views down the axis, while Figure 1.7(b) shows their corresponding stereographic projections.**
![[Rotation axes.png | 700]]
**The existence of rotation axes is reflected in the arrangement of faces and edges of the crystal, and consequently, in the set of normals to the faces**. For instance, if a **crystal possesses a tetrad axis**, there will be **four faces or edges symmetrically arranged around the axis, and the normals to these faces will also exhibit fourfold symmetry**.

**Rotation axes** are crucial symmetry elements that have several **important implications for crystal structure analysis and diffraction patterns**:

- They impose restrictions on the arrangement of atoms within the unit cell. Atoms must be located either on the rotation axis or in sets of symmetry-related positions around the axis.
    
- They introduce relationships between the structure factors of different reflections. This is because the scattering contributions from atoms related by the rotation axis are related in a specific way.
    
- They can lead to systematic absences in the diffraction pattern. These absences occur when the scattering contributions from symmetry-related atoms interfere destructively, resulting in zero intensity for certain reflections.

The identification of rotation axes from the diffraction pattern is often aided by considering the symmetry of the diffraction spots. **For example, a Laue photograph taken down a triad axis will exhibit a threefold symmetry in the arrangement of the diffraction spots.** However, Friedel’s law complicates the direct identification of rotation axes solely from diffraction data, as it dictates that the weighted reciprocal lattice always possesses inversion symmetry. Consequently, careful analysis and consideration of systematic absences are often required to unambiguously determine the presence and order of rotation axes in a crystal structure.
### Inversion axes

**Inversion axes** are symmetry elements that relate crystal planes by a **combination of rotation and inversion through a centre**. The operation of an **inversion axis**, denoted by the symbol **\overline{n}**, involves the following steps:

1. **Rotation:** Rotate a point about the axis by an angle of 2π/n.
2. **Inversion:** Invert the point through a centre that lies on the inversion axis.

**Figure 1.8(a) from source provides a perspective view of the operation of a $\overline{4}$ (inverse tetrad) axis.** Starting with face A, a rotation of 90° about the $\overline{4}$ axis brings it to position A'. Subsequent inversion through the centre O results in face B. Repeating this operation on B yields C, and then D.

**The possible inversion axes in a crystal, along with their written and graphical symbols, are:**

- **$\overline{1}$**: Equivalent to a centre of symmetry. Graphical symbol: _o_
    
- **$\overline{2}$**: Equivalent to a mirror plane. Graphical symbol: _m_ (more commonly used than the \overline{2} symbol)
    
- **$\overline{3}$**: Inverse triad axis. Graphical symbol: _Δ_
    
- **$\overline{4}$**: Inverse tetrad axis. Graphical symbol: _□_
    
- **$\overline{6}$**: Inverse hexad axis. Graphical symbol: _$_

**Figure 1.8(b) from source presents the stereographic projections for all the inversion axes.**

Similar to other symmetry elements, inversion axes impose constraints on the arrangement of atoms within the unit cell. The presence of inversion axes can also lead to systematic absences in the diffraction pattern. For example, a **21 screw axis**, which combines a 180° rotation with a translation of half the unit cell length, **gives rise to systematic absences for reflections ($0k0$) with k odd**.

**It is important to note that inversion axes cannot be directly observed in the external morphology of crystals, as they involve an inversion operation that cannot be physically performed on a macroscopic object.** However, their presence can be inferred from the symmetry of the arrangement of normals to the faces and from the systematic absences in the diffraction pattern.

![[Inversion Axes.png | 700]]

### Symmetry Elements Present in a Crystal

A **symmetry element** is a geometrical entity, like a point, line, or plane, that describes an operation that can be performed on the crystal to leave its appearance unchanged. The sources describe multiple symmetry elements, present either in the external form of the crystal, or revealed by studying the set of normals to the crystal faces:

- **Center of Symmetry (\overline{1})**: For any point within the crystal, faces occur in parallel pairs of equal dimensions on opposite sides of the point, and equidistant from it. An equivalent definition is: for any atom at vector position **r** within the unit cell, there is an equivalent atom at **-r**. Represented by the symbol _o_.
- **Mirror Plane (m)**: A plane in the crystal such that the halves on opposite sides of the plane are mirror images of each other. Represented graphically by a thick solid line.
- **Rotation Axes (n):** Rotation through 2π/n about the axis leaves the appearance of the crystal unchanged. The possible values of _n_ are 1, 2, 3, 4, and 6, referred to as monad, diad, triad, tetrad, and hexad axes, respectively. These are represented by the following graphical symbols:
    - **2 (diad):** A filled black circle.
    - **3 (triad):** A filled black triangle.
    - **4 (tetrad):** A filled black square.
    - **6 (hexad):** A filled black hexagon.
- **Inversion Axes (\overline{n})**: These relate crystal planes by a combination of rotation and inversion through a center. The operation of an inversion axis involves a rotation of 2π/n about the axis, followed by an inversion through a center on the axis. They are represented by the following graphical symbols:
    - **$\overline{1}$:** _o_. Equivalent to a center of symmetry.
    - **$\overline{2}$:** None. Equivalent to a mirror plane (symbol _m_ is commonly used).
    - **$\overline{3}$:** _Δ_.
    - **$\overline{4}$:** _□_.
    - **$\overline{6}$:** _$._

The **external form** of a crystal often displays a high degree of symmetry, like the alum crystal shown in source, which has the shape of an octahedron. However, some crystals may lack obvious symmetry in their external form, yet still possess underlying symmetry revealed through analysis of the **normals to the crystal faces**. For instance, the platy crystals in source appear irregular at first glance. However, upon closer examination, the normals to their sides form an identical set from crystal to crystal, revealing an underlying hexagonal symmetry that is not immediately apparent in the crystal shapes themselves.

The symmetry elements mentioned above describe symmetry in the **macroscopic structure** of a crystal. However, when considering the **arrangement of atoms within the unit cell** (the smallest repeating unit of a crystal), additional symmetry elements become possible due to the periodic repeat pattern. These are called **microscopic symmetry elements**, and they include:

- **Glide Planes** (a,b,c,n,d): Combine mirror reflection with a translation. They are represented by dashed lines.
- **Screw Axes** (2<sub>1</sub>,3<sub>1</sub>,3<sub>2</sub>,4<sub>1</sub>,4<sub>2</sub>,4<sub>3</sub>,6<sub>1</sub>,6<sub>2</sub>,6<sub>3</sub>,6<sub>4</sub>,6<sub>5</sub>): Combine rotation about an axis with a translation parallel to the axis. The subscript number in the graphical symbol indicates the fraction of the unit cell length by which a point is translated after the rotation.

**The specific symmetry elements present in a crystal's unit cell determine its space group, which is a crucial piece of information for understanding its structure and properties.** There are 230 possible space groups, each with a unique combination of symmetry elements.

It is important to note that:

- Screw axes and glide planes do not influence the **macroscopic symmetry** of the crystal. The translational component of their operation is only relevant on the atomic scale, and the external appearance of the crystal reflects only the rotational or reflectional component.
- **Friedel's law** states that the diffraction pattern of a crystal is always centrosymmetric, even if the crystal structure itself lacks a center of symmetry. Therefore, determining the presence or absence of a center of symmetry requires methods beyond simply analyzing the diffraction pattern.

==> **Draw the diagonal plane of symmetry in the cubic unit cell**
![[symmetry element diagonal unit cell.png|700]]

==> **List of symmetry elements & the graphical symbols**
![[List S.E. table.png | 700]]
### Point Groups and Space Groups

**Point Groups**
- A point group encompasses all the symmetry elements that converge at a single point within the crystal structure. This point is often chosen as the origin of the unit cell.
    
- The point group determines the **crystal class**, dictating the possible shapes a crystal can adopt and influencing its physical properties.
    
- There are **32 possible crystal classes** (and corresponding point groups), each belonging to one of the seven crystal systems. Each crystal system is characterized by a specific type of unit cell, defined by the lengths of its edges (a, b, c) and the angles between them (α, β, γ).
    
    - For instance, the **triclinic system** has no restrictions on the unit cell dimensions and possesses the lowest symmetry. A triclinic crystal can have either no symmetry (crystal class 1) or only a center of symmetry (crystal class $\overline{1}$).
    - The **monoclinic system** has one unique axis (conventionally the b-axis) perpendicular to the other two, with the angle $β ≠ 90°$. This system has three crystal classes: 2, m, and 2/m.
    - The **cubic system** exhibits the highest symmetry, with all unit cell edges equal $(a = b = c)$ and all angles equal to 90° ($α = β = γ = 90°$). A key characteristic of the cubic system is the presence of four triad axes.
- **Stereographic projections**, which map the three-dimensional symmetry of a crystal onto a two-dimensional plane, provide a convenient way to visualize and represent crystal classes.

- Examples of point groups and their corresponding stereographic projections from the sources include:
    - **Class 1**: No symmetry. A general crystal face generates a single point in the stereographic projection.
    - **Class $\overline{1}**$: Center of symmetry only. Two points are generated from a general face, representing the face and its inversion through the center.
    - **Class 2**: A single diad axis. The projection shows two points related by a 180° rotation.
    - **Class m**: A single mirror plane. Two points appear in the projection, related by reflection across the mirror plane.
    - **Class 2/m**: A diad axis and a mirror plane perpendicular to it. Four points are generated.

**Space Groups**

- A space group incorporates the point group symmetry and combines it with the **translational symmetry** of the crystal lattice. It provides a complete description of the arrangement of atoms and symmetry elements within the unit cell.
    
- There are **230 possible space groups**, each with a unique combination of symmetry elements. The International Tables for Crystallography catalog and describe these in detail.
    
- The choice of origin for the unit cell can influence the apparent complexity of the space group description. Shifting the origin can sometimes reveal additional symmetry elements, leading to a more concise representation.
    
- **Two-dimensional space groups (plane groups)** provide a simpler way to understand space group concepts. There are 17 plane groups, arising from the combinations of four crystal systems, two lattice types, and a limited set of symmetry elements.
    
- When describing space groups, a shorthand notation is used to indicate the type of lattice (P for primitive, C for C-face centered, etc.) and the symmetry elements present.

    - For example, **$P212121$** signifies a primitive orthorhombic cell with 2<sub>1</sub> screw axes along each of the three cell edges.
    - The space group **Cm** indicates a C-face centered monoclinic unit cell with a mirror plane perpendicular to the b-axis.
- Space groups play a crucial role in **X-ray structure determination**, as they constrain the possible positions of atoms within the unit cell. Understanding the space group symmetry simplifies the interpretation of diffraction data and aids in the calculation of electron density maps.

##### Difference & relation of Point & space groups

| **Feature**           | **Point Group**                                                                                      | **Space Group**                                                                                                     | **Relationship**                                                                                                                  |
| --------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Definition**        | Describes the **symmetry of a single object or the external form of a crystal**.                     | Describes the **complete symmetry of the internal structure of a crystal**, including translational symmetry.       | Space groups incorporate point group symmetry and add translational symmetry elements.                                            |
| **Symmetry Elements** | Includes macroscopic symmetry elements like **rotation axes, mirror planes, and inversion centers.** | Includes both macroscopic symmetry elements and microscopic elements like **screw axes and glide planes.**          | Microscopic elements in a space group manifest as their macroscopic counterparts in the crystal's external form (point group).    |
| **Number**            | **32** possible point groups.                                                                        | **230** possible space groups.                                                                                      | Each space group is associated with a specific point group.                                                                       |
| **Crystal Systems**   | Categorized into **seven crystal systems**.                                                          | Also classified into the **same seven crystal systems** based on unit cell geometry.                                | Both schemes use the same seven crystal systems to organize symmetry.                                                             |
| **Notation**          | Represented by symbols like **1, $\overline{1}$, 2, m, $2/m$, $4/mmm$, m$\overline{3}$m**.           | Represented by symbols like **P1, P21/c, C2/m, P4mm, Fd$\overline{3}$m**.                                           | Point group symbols are incorporated into space group symbols.                                                                    |
| **Determination**     | Determined by examining **crystal morphology** and **optical properties**.                           | Determined by analyzing **X-ray diffraction patterns** and identifying **systematic absences**.                     | Diffraction data provides information about both the point group (Laue group) and the specific space group.                       |
| **Applications**      | Predicts possible crystal shapes, influences physical properties, determines Laue group.             | Essential for solving crystal structures, constrains atom positions, simplifies diffraction pattern interpretation. | Point groups provide initial insights into a crystal's symmetry, while space groups are crucial for detailed structural analysis. |
| **Examples**          | Class 2/m, Class 4/mmm, Class m$\overline{3}$m                                                       | P2<sub>1</sub>/c, P4mm, Fd$\overline{3}$m                                                                           | $P21/c$ has a point group of $2/m$. $P4mm$ has a point group of $4/mmm$, Fd$\overline{3}$m has a point group of m$\overline{3}$m. |

**Key Difference:**
The fundamental difference lies in the scope of symmetry they describe. **Point groups focus on the symmetry of a single, isolated object, neglecting translational repetition.** **Space groups, on the other hand, encompass the full symmetry of the infinitely repeating crystal lattice, including translational symmetry operations.**

#### 32 point groups in seven crystal systems

| Crystal System   | Essential Symmetry of Crystal                     | Point Groups                                                      | No. of Point Groups |
| :--------------- | :------------------------------------------------ | :---------------------------------------------------------------- | :------------------ |
| **Triclinic**    | **None**                                          | **1, $\overline{1}$**                                             | **2**               |
| **Monoclinic**   | **Diad axis or mirror plane (inverse diad axis)** | **2, m, 2/m**                                                     | **3**               |
| **Orthorhombic** | **Three orthogonal diad or inverse diad axes**    | **222, $mm2$, mmm**                                               | **3**               |
| **Tetragonal**   | **One tetrad or inverse tetrad axis**             | **4,$\overline{4}$, 4/m, 422, 4mm, $\overline{4}$ 2m, 4/mmm**     | **7**               |
| **Trigonal**     | **One triad or inverse triad axis**               | **3, $\overline{3}$, 32, 3m, $\overline{3}$m**                    | **5**               |
| **Hexagonal**    | **One hexad or inverse hexad axis**               | **6, $\overline{6}$, 6/m, 622, 6mm, $\overline{6}$m2, 6/mmm**     | **7**               |
| **Cubic**        | **Four triad axes**                               | **23, m$\overline{3}$, 432, $\overline{4}$ 3m, m$\overline{3}$m** | **5**               |

**Total:** 32 point groups
**Notes:**

- This table summarizes the 32 point groups (crystal classes) distributed among the seven crystal systems.
- Each crystal system is characterized by a specific set of symmetry elements.
- The "Essential Symmetry" column lists the minimum symmetry requirements for each system.
- The "Point Groups" column enumerates the specific point group symbols within each system.
---
**Additional Points:**
- While the crystal system is determined by the general shape of the unit cell, the point group specifies the additional symmetry elements present within that unit cell.
- Stereographic projections offer a visual representation of these point groups, illustrating the symmetry relationships between crystal faces.
- For each point group, multiple space groups are possible, as space groups incorporate translational symmetry elements in addition to point group symmetry.
----
### Reciprocal Lattice Vector

The **reciprocal lattice vector, _s_**, is a concept in X-ray crystallography that helps explain the **relationship between the diffraction angle, wavelength, and the spacing of lattice planes** in a crystal. It is defined as **s = ha* + kb* + lc***, where h, k, and l are integers representing the Miller indices, and **a*, b*, and c* are the primitive vectors of the reciprocal lattice**. The reciprocal lattice itself is a mathematical construct that is **fixed relative to the real space lattice of the crystal**.

For a given set of Miller indices (hkl), there is a corresponding reciprocal lattice point defined by _s_. This reciprocal lattice point can be used to determine the **scattering vector**, which is the **vector that describes the change in wavevector of the X-ray beam during diffraction**. The scattering vector has a **magnitude of (2 sin θ)/λ**, where θ is the Bragg angle and λ is the wavelength of the incident beam. It also points in a **direction perpendicular to the reflecting planes**.

The **relationship between the real and reciprocal lattices** is defined by the following equations:

- **$a · a* = 1, a · b* = 0, a · c* = 0$**
- **$b · a* = 0, b · b* = 1, b · c* = 0$**
- **$c · a* = 0, c · b* = 0, c · c* = 1$**

These equations demonstrate that **any reciprocal lattice vector is perpendicular to two of the real space lattice vectors**. For example, **a* is perpendicular to b and c**, meaning it is perpendicular to the plane defined by these vectors. The scalar product of **a* and a** fixes the magnitude of **a***. The same logic can be applied to the other reciprocal lattice vectors.

The **reciprocal nature of these lattices** can be seen in the fact that the **volume of the real space unit cell (V) and the volume of the reciprocal lattice unit cell (V*) are multiplicative inverses**, i.e., $VV* = 1$.

The reciprocal lattice is a **unique mathematical construct** for each real space lattice, regardless of the choice of primitive vectors used to define the real space lattice. This means that while different choices of primitive vectors will result in different reciprocal lattice vectors, **the overall reciprocal lattice will remain unchanged**.

The **concept of the reciprocal lattice** is important for **understanding diffraction patterns** from crystals. The reciprocal lattice can be used to **predict the direction of diffracted beams** and to **index reflections in a diffraction pattern**. This information can then be used to **determine the crystal structure** of a material.

##### Distinguish reciprocal lattice from a direct lattice
The **direct lattice** and the **reciprocal lattice** are two important concepts in solid-state physics, particularly in the study of crystallography and diffraction. They are related by a mathematical transformation, and each lattice provides a different perspective on the structure of a crystal. Here's a table that distinguishes between the two:

| Feature                 | Direct Lattice                                                                                                 | Reciprocal Lattice                                                                                                                                                                                                                                                 |
| ----------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Definition**          | A lattice in **real space** that represents the periodic arrangement of atoms or molecules in a crystal.       | A lattice in **reciprocal space**, a mathematical construct where distances have units of inverse length, that is related to the direct lattice by a Fourier transform. Each point in the reciprocal lattice represents a set of planes in the real space lattice. |
| **Units**               | **Length** (e.g., Angstroms, Å)                                                                                | **Inverse length** (e.g., inverse Angstroms, Å⁻¹)                                                                                                                                                                                                                  |
| **Primitive Vectors**   | **a, b, c** - define the edges of the unit cell in real space.                                                 | **a*, b*, c*** - defined by the equations **a · a* = 1, a · b* = 0, a · c* = 0**; **b · a* = 0, b · b* = 1, b · c* = 0**; **c · a* = 0, c · b* = 0, c · c* = 1**                                                                                                   |
| **Relationship**        | **Reciprocal to each other.** The reciprocal lattice of the reciprocal lattice is the original direct lattice. | **Reciprocal to each other.** The reciprocal lattice of the reciprocal lattice is the original direct lattice.                                                                                                                                                     |
| **Volume of Unit Cell** | $V = \|a · (b × c)\|$                                                                                          | $V* = (2π)³/V$                                                                                                                                                                                                                                                     |
| **Significance**        | Defines the **physical structure** of the crystal and its symmetry.                                            | Used to understand **diffraction patterns** from crystals. Each point corresponds to a set of planes in the direct lattice that can diffract X-rays. Also used to describe the **behavior of electrons in a periodic potential** (Brillouin zones).                |

The direct lattice represents the real, physical arrangement of atoms or molecules within a crystal structure. It provides information about the distances between atoms, the angles between lattice vectors, and the symmetry of the crystal. The reciprocal lattice, on the other hand, is a mathematical construct that exists in a space with units of inverse length. It's used to analyze the diffraction of waves, such as X-rays, by crystals. Each point in the reciprocal lattice corresponds to a particular set of planes in the direct lattice that can diffract X-rays, and the spacing between points in the reciprocal lattice is inversely proportional to the spacing between planes in the direct lattice.

The **Brillouin zone** is the Wigner-Seitz cell of the reciprocal lattice and is an important concept in solid state physics. It can be used to visualize the behavior of electrons in a periodic potential.

==>**Why needed reciprocal lattice??**
The concept of the **reciprocal lattice** is crucial in X-ray crystallography because it provides a powerful tool for understanding and analyzing the **diffraction of X-rays by crystals**. It simplifies the complex geometry of diffraction and provides a framework for interpreting diffraction patterns and determining crystal structures. Here's why the reciprocal lattice is needed:

- **Simplification of Diffraction Geometry:** The Laue equations, which describe the conditions for constructive interference of diffracted X-rays, involve complex relationships between the incident beam direction, diffracted beam direction, wavelength, and lattice plane spacings. The reciprocal lattice simplifies these equations by providing a direct geometric interpretation of the diffraction conditions.
    
- **Visualization of Diffraction:** Each point in the reciprocal lattice corresponds to a specific set of parallel planes in the real space lattice. When the **scattering vector**, which is the difference between the incident and diffracted wave vectors, matches a reciprocal lattice vector, constructive interference occurs and a diffracted beam is observed. This allows one to visualize the direction of diffracted beams and relate them to specific lattice planes.
    
- **Indexing of Diffraction Peaks:** Diffraction patterns from crystals, such as those obtained from X-ray diffraction experiments, consist of a series of spots or peaks. These peaks correspond to the reciprocal lattice points that satisfy the diffraction conditions. By analyzing the positions of these peaks, one can index them (assign Miller indices) and determine the size and shape of the unit cell in reciprocal space, which is directly related to the unit cell in real space.
    
- **Determination of Crystal Structure:** The reciprocal lattice plays a central role in determining the crystal structure of a material. By analyzing the diffraction pattern and using the reciprocal lattice to index reflections, one can determine the arrangement of atoms within the unit cell. This information, along with intensity data, can be used to solve the crystal structure.
    
- **Understanding Electron Behavior in Solids:** The reciprocal lattice is essential for understanding the behavior of electrons in a periodic potential, such as that found in a crystal. The **Brillouin zone**, which is the Wigner-Seitz cell of the reciprocal lattice, is fundamental in describing electronic band structure, Fermi surfaces, and other electronic properties of solids.
    
- **Analysis of Lattice Vibrations:** The reciprocal lattice also simplifies the analysis of lattice vibrations (phonons) in crystals. Dispersion relations for phonons are typically plotted in reciprocal space, and the periodicity of the reciprocal lattice dictates the allowed wave vectors and frequencies for lattice vibrations.
    
In summary, the reciprocal lattice provides a powerful and convenient framework for:
- analyzing diffraction patterns,
- determining crystal structures, and
- understanding the electronic and vibrational properties of crystals.
It simplifies the complex geometry of diffraction, allowing for a clearer visualization of diffraction phenomena and a more straightforward interpretation of experimental data.

--------------
==> **Monoclinic Cm**:










---------------------------------
==> **Monoclinic P<sub>21/c</sub>**:










----
==> **Orthorhombic P<sub>212121</sub>:**










--------------------------------------
==>**Orthorohombic $Aba2$ :**










