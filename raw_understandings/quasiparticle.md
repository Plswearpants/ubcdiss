# **Quasiparticles, Band Structure Renormalization, and Breakdown of Fermi Liquid Theory**

## **1. Introduction**
Quasiparticles form the foundation of our understanding of many-body systems in condensed matter physics. They provide an effective way to describe interacting electrons in terms of renormalized single-particle excitations. This document explores the role of quasiparticles in Fermi Liquid Theory (FLT), how they renormalize band structures, and why FLT fails in certain unconventional materials such as topological systems and strongly correlated materials.

---

## **2. Standard Quasiparticles in Fermi Liquid Theory (FLT)**
### **2.1 Quasiparticle Concept and Lifetime in FLT**
In Fermi liquids, quasiparticles are long-lived excitations that behave like renormalized free electrons. Their lifetime $\tau$ is determined by the imaginary part of the self-energy:

$$\tau^{-1} \sim \text{Im} \Sigma(\mathbf{k}, \omega) \sim (\omega - \mu)^2$$

#### **Why $\text{Im} \Sigma(\omega) \sim (\omega - \mu)^2$?**
1. **Phase Space Constraints**: The Pauli exclusion principle restricts electron-electron scattering, shrinking the phase space near the Fermi surface. The probability of scattering scales with the available density of states, which vanishes quadratically at the Fermi level.
2. **Fermi's Golden Rule**: The transition rate of electron-electron scattering is given by:

   $$\Gamma_{\mathbf{k}} \sim \sum_{\mathbf{k}',\mathbf{q}} |V_{\mathbf{k}, \mathbf{k}'}|^2 \delta(E_{\mathbf{k}} - E_{\mathbf{k}'})$$

   Since the density of available final states grows quadratically with energy above the Fermi surface, the imaginary part of the self-energy follows:

   $$\text{Im} \Sigma(\omega) \sim (\omega - \mu)^2$$

3. **Physical Consequence**: This ensures that quasiparticles remain well-defined near $E_F$, allowing a coherent metallic state to emerge. The quadratic decay rate guarantees that at sufficiently low energy, quasiparticles have long lifetimes.

### **2.2 Band Structure Renormalization**
The bare band structure $\epsilon_{\mathbf{k}}$ is modified by the self-energy:

$$\tilde{E}(\mathbf{k}) = \epsilon_{\mathbf{k}} + \text{Re} \Sigma(\mathbf{k}, \omega)$$

- The **quasiparticle weight** (or residue) is given by:

  $$Z_{\mathbf{k}} = \left( 1 - \frac{\partial \text{Re} \Sigma}{\partial \omega} \right)^{-1}$$

- **Methods like GW and DMFT correct Density Functional Theory (DFT) band structures** by incorporating these effects.

---

## **3. Breakdown of Fermi Liquid Theory (FLT)**
### **3.1 Why FLT Fails in Topological Materials**
FLT assumes adiabatic continuity, meaning interactions do not induce phase transitions. However, in **topological systems**, discrete, nontrivial band structures emerge, violating this assumption.

#### **(A) Weyl and Dirac Semimetals: Nontrivial Band Topology**
Weyl/Dirac quasiparticles obey a relativistic dispersion:

$$E(\mathbf{k}) = \pm v_F |\mathbf{k}|$$

- **Berry curvature** modifies their semiclassical motion:

  $$\frac{d \mathbf{k}}{dt} = -e \mathbf{E} - e \mathbf{v} \times \mathbf{B} + e \mathbf{E} \times \mathbf{\Omega}(\mathbf{k})$$

- **Chiral anomaly** leads to electron population imbalance between Weyl nodes:

  $$\nabla \cdot \mathbf{J}_5 = \frac{e^2}{h^2} \mathbf{E} \cdot \mathbf{B}$$

### **3.2 Breakdown of Semiclassical Motion Due to the Chiral Anomaly**
FLT assumes that quasiparticles follow a well-defined semiclassical equation of motion:

$$\frac{d \mathbf{k}}{dt} = -e \mathbf{E} - e \mathbf{v} \times \mathbf{B}$$

However, in Weyl semimetals, the chiral anomaly alters this equation by introducing a nonzero divergence in the chiral current:

$$\nabla \cdot \mathbf{J}_5 = \frac{e^2}{h^2} \mathbf{E} \cdot \mathbf{B}$$

This means that:
- The **Fermi surface itself changes dynamically** in the presence of external fields.
- **Berry curvature effects** introduce anomalous transport, making the standard Hamiltonian evolution incomplete.
- The quasiparticle decay rate deviates from the Fermi liquid behavior and follows:

  $$\text{Im} \Sigma(\omega) \sim \omega$$

This results in a **non-Fermi liquid state** where the concept of long-lived quasiparticles breaks down.

### **3.3 Strongly Correlated Systems and Mott Insulators**
- **Mott transition**: Interactions destroy the Fermi surface.
- **Hubbard model** as an example:
  - For weak interactions, system behaves as a **Fermi liquid**.
  - For strong interactions, system becomes a **Mott insulator**.
- Breakdown of quasiparticles: **Residue $Z_{\mathbf{k}} \to 0$, meaning no well-defined excitations.**

### **3.4 Non-Hermitian Topological Systems**
- **FLT assumes a Hermitian system**: $H^\dagger = H$.
- **Non-Hermitian systems violate this**, leading to:
  - **Exceptional points** and complex eigenvalues.
  - **Non-reciprocal transport** and new quasiparticle behavior.
  - Need for **non-Hermitian quantum mechanics**.

---

## **4. Summary Table**
| **Phenomenon** | **FLT Works?** | **Why or Why Not?** |
|----------------|----------------|---------------------|
| Standard Metals | ✅ Yes | Renormalized quasiparticles exist. |
| Superconductors | ✅ Yes | Bogoliubov quasiparticles behave like FLT states. |
| Weyl Semimetals | ❌ No | Nontrivial topology, Berry curvature, chiral anomalies. |
| Mott Insulators | ❌ No | Quasiparticles disappear, strong correlations dominate. |
| Non-Hermitian Systems | ❌ No | No conserved quasiparticle states. |

---

## **5. Final Takeaways**
- **FLT quasiparticles renormalize band structure, but breakdown occurs in topological and strongly correlated systems.**
- **Unconventional quasiparticles (e.g., Weyl fermions) exist, but they violate FLT assumptions.**
- **Alternative theories like DMFT, non-Fermi liquids, and non-Hermitian quantum mechanics are needed for these materials.**

This document serves as a structured reference for understanding quasiparticle behavior beyond FLT. 🚀

