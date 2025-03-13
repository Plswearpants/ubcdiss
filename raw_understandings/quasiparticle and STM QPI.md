# Quasiparticles and Quasiparticle Interference (QPI) in Scanning Tunneling Microscopy (STM)

## 1. Introduction
Quasiparticle interference (QPI) is a powerful technique in scanning tunneling microscopy (STM) that provides insight into the electronic structure of materials. It arises when quasiparticles scatter off impurities or defects, leading to interference patterns in the local density of states (LDOS). This document explores the nature of quasiparticles in QPI, their relation to band structure, and how QPI patterns can be used to infer key electronic properties of a material.

---

## 2. Quasiparticles in the Context of QPI
### 2.1 Standard Quasiparticles and Band Structure
- In a clean material, quasiparticles are well-defined excitations that renormalize the band structure via the self-energy:
  
  $$\tilde{E}(\mathbf{k}) = \epsilon_{\mathbf{k}} + \text{Re} \Sigma(\mathbf{k}, \omega)$$
  
- The **quasiparticle residue**:
  
  $$Z_{\mathbf{k}} = \left( 1 - \frac{\partial \text{Re} \Sigma}{\partial \omega} \right)^{-1}$$
  
  characterizes how strongly the bare electron states are modified by interactions.
- In STM, the tunneling current depends on the **local density of states (LDOS)**, given by the spectral function:
  
  $$A(\mathbf{k}, \omega) = -\frac{1}{\pi} \text{Im} G(\mathbf{k}, \omega)$$
  
  STM directly probes these quasiparticle-modified electronic states.

### 2.2 Quasiparticle Interference and Impurity Scattering
- In the presence of impurities, quasiparticles undergo elastic scattering:
  
  $$E(\mathbf{k}) = E(\mathbf{k} + \mathbf{q})$$
  
  leading to a set of characteristic **scattering wavevectors** $\mathbf{q}$, which correspond to QPI patterns in STM measurements.
- The Fourier transform of the real-space STM conductance image reveals **QPI wavevectors**, which can be mapped onto the band structure of the material.

---

## 3. Relation Between QPI and Band Structure
### 3.1 QPI as a Probe of Quasiparticle Band Structure
- QPI **traces the energy contours** in the band structure through scattering wavevectors:
  
  $$\mathbf{q} = \mathbf{k}_1 - \mathbf{k}_2$$
  
- The resulting QPI pattern in STM is given by the **joint density of states (JDOS)**:
  
  $$\text{JDOS}(\mathbf{q}, \omega) = \sum_{\mathbf{k}} A(\mathbf{k}, \omega) A(\mathbf{k} + \mathbf{q}, \omega)$$
  
- This allows experimentalists to **extract the band dispersion** by tracking QPI peaks at different energies.

### 3.2 Role of Impurities in QPI
- **No impurities → No QPI**, as scattering events are necessary to generate interference patterns.
- However, even in the absence of QPI, a material still possesses a well-defined **quasiparticle band structure**, which can be accessed using ARPES.
- In strongly correlated systems, QPI can be used to detect **interaction-driven band renormalization**, including **flat bands or pseudogaps**.

---

## 4. Breakdown of Standard QPI Interpretation
### 4.1 Non-Fermi Liquid Effects in QPI
- In **Fermi liquids**, QPI patterns can be directly related to well-defined quasiparticles with a quadratic lifetime scaling:
  
  $$\text{Im} \Sigma(\omega) \sim (\omega - \mu)^2$$
  
- In **non-Fermi liquids**, QPI signals may be broadened or missing due to shorter quasiparticle lifetimes:
  
  $$\text{Im} \Sigma(\omega) \sim \omega$$
  
  which leads to enhanced decoherence and smearing of QPI features.

### 4.2 Topological Materials and QPI
- **Weyl semimetals**: QPI is suppressed when scattering between different Weyl nodes is forbidden by **chiral protection**.
- **Topological insulators**: Surface state QPI can be analyzed to detect **spin-momentum locking**, where only specific backscattering processes are allowed.
- **Non-Hermitian systems**: QPI may reveal new spectral features beyond conventional band theory predictions.

---

## 5. Summary Table
| **Phenomenon** | **QPI Present?** | **Why or Why Not?** |
|----------------|------------------|---------------------|
| Clean Metals | ❌ No | No impurities to induce QPI. |
| Metals with Impurities | ✅ Yes | Elastic scattering generates QPI patterns. |
| Fermi Liquids | ✅ Yes | Well-defined quasiparticles lead to clear QPI wavevectors. |
| Non-Fermi Liquids | ⚠️ Sometimes | Short-lived quasiparticles may suppress QPI. |
| Topological Insulators | ⚠️ Weak | Spin-momentum locking limits scattering channels. |
| Weyl Semimetals | ❌ No | Chiral protection suppresses QPI. |

---

## 6. Final Takeaways
- **QPI reveals quasiparticle band structure through impurity scattering**.
- **The absence of QPI does not mean the absence of quasiparticles**, but rather the absence of scattering.
- **Non-Fermi liquids and topological materials modify QPI patterns in ways that can diagnose new physics.**
- **STM-based QPI analysis complements ARPES in studying electronic structure, especially in correlated or topological materials.**

This document serves as a structured reference for understanding the relationship between quasiparticles, QPI, and their role in STM studies. 🚀

