# Development of Quasiparticle Theory

Below is a **condensed overview** of how each major theory in the development of quasiparticle concepts **extends or generalizes** our ability to describe interacting fermion systems, along with **examples** of materials where each theory **makes accurate predictions**.

---

## 1. Landau Fermi Liquid Theory (1956–1957)
- **Original Quasiparticle Picture**:  
  - Postulates that an interacting fermion system can be mapped **adiabatically** to a non‐interacting Fermi gas, with **long‐lived quasiparticles** near the Fermi surface.
- **Regime**:  
  - **Weak to moderate correlations**; sufficiently low temperatures ($T \ll E_F$).  
  - Metals with well-defined Fermi surfaces and no strong localization.
- **Example Materials**:  
  - **Simple metals** (alkali metals like sodium, potassium) and **noble metals** (like copper at low $T$).  
  - **Liquid $^3\text{He}$** is also an excellent Fermi liquid that matches Landau's predictions.

**Key Expansion**:  
1. **Introduces** "quasiparticle" with renormalized mass $m^*$ and a finite lifetime.  
2. Explains **low-temperature thermodynamic properties** (heat capacity, susceptibility) via Landau parameters.

---

## 2. Hartree-Fock (1930s onward, widely used mid-20th century)
- **Mean-Field Exchange**:  
  - Treats electron-electron **exchange** exactly but **ignores dynamic correlation** (fluctuations).
- **Regime**:  
  - **Weak correlations, wide conduction bands**.  
  - Typically used as a **starting point** for more accurate post-HF methods.
- **Example Materials**:  
  - **Free-electron-like metals** with small effective mass and minimal localization (e.g., aluminum).  
  - Often a base method in atomic/molecular quantum chemistry, not the best for strongly correlated solids but can be decent for **simple sp-bonded metals**.

**Key Expansion**:
1. **First step** beyond a purely free-electron model, introduces self-consistency in a single-particle framework.  
2. Lays groundwork for **diagrammatic expansions** (as HF is the zeroth-order approximation in many-body perturbation).

---

## 3. Random Phase Approximation (RPA) (1950s)
- **Collective Screened Interactions**:  
  - Summation of "bubble" diagrams to capture **screening** of the Coulomb interaction and collective modes (plasmons).
- **Regime**:  
  - **Moderate correlations** where **long-range screening** is crucial.  
  - Good for describing **collective excitations** (plasmons, screening) in electron gases.
- **Example Materials**:  
  - **Aluminum** (free-electron–like metal) where plasmons are well described by RPA.  
  - **Simple semiconductors** (Si, GaAs) for screening properties in doping contexts.

**Key Expansion**:  
1. Improves HF by including **dynamical screening**.  
2. Explains **plasmon dispersion** and optical properties in metals/semiconductors.

---

## 4. GW Approximation (Hedin, 1965)
- **Self-Energy with Dynamic Screening**:  
  - Uses $\Sigma = i G W$ to incorporate frequency-dependent Coulomb screening more accurately than RPA alone.
- **Regime**:  
  - **Weak to moderate correlation** but significantly better than HF for band-gap corrections, quasiparticle energies.  
  - Fills the gap between simple Fermi liquids and strongly correlated systems.
- **Example Materials**:  
  - **Semiconductors** (Si, GaAs) and **insulators** (e.g., MgO, LiF) for **accurate band-gap predictions**.  
  - **Simple metals** for refining Fermi surface details, effective masses.
  
**Key Expansion**:
1. **Systematically corrects HF** by adding dynamic screening in the self-energy.  
2. **One-shot $G_0W_0$ to fully self-consistent GW** are used in real materials codes.

---

## 5. Dynamical Mean-Field Theory (DMFT) (1990s)
- **Local Correlations, Mott Physics**:  
  - Focuses on the **local** self-energy by mapping lattice sites to an **Anderson impurity model**.  
  - Captures **Mott transitions**, heavy-fermion behavior, etc.
- **Regime**:  
  - **Strong local correlations** (e.g., transition metal oxides, f-electron materials).  
  - Retains the idea of quasiparticles but can show their **destruction** near Mott transitions.
- **Example Materials**:  
  - **$V_2O_3$** near the Mott transition.  
  - **NiO**, **La$_{1-x}$Sr$_x$TiO$_3$** (doped transition-metal oxides).
  
**Key Expansion**:
1. Extends quasiparticle concept to cases where HF, RPA, or GW fail due to **strong correlation**.  
2. Introduces a **three-peak structure** in spectral function (Hubbard bands + quasiparticle peak).

---

## 6. GW+DMFT (2000s)
- **Combining Nonlocal Screening (GW) + Local Strong Correlation (DMFT)**:  
  - Merges the best of **GW** (dynamic, nonlocal screening) with **DMFT** (local but exact correlation).
- **Regime**:  
  - **Intermediate to strong correlation** with significant screening effects.  
  - e.g., f-electron heavy fermions, transition-metal oxides with conduction band screening + local d-electron interactions.
- **Example Materials**:
  - **SrVO$_3$**, **Ce-based** heavy fermion compounds.  
  - Key to describing **simultaneous Mott + band gap** phenomena.

**Key Expansion**:
1. Resolves shortcomings of pure DMFT (no long-range screening) or pure GW (no strong local correlation).  
2. Achieves more **quantitatively accurate** spectral functions in correlated metals/oxides.

---

## 7. Non-Fermi Liquid Theories & Beyond (Late 20th Century–Present)
- **Strange Metals, Quantum Critical Systems**:  
  - Where quasiparticles may not be well-defined, e.g., $\text{Im}\Sigma(\omega) \sim \omega$.  
  - Requires new frameworks (AdS/CFT, functional RG, etc.).
- **Regime**:  
  - **Quantum critical points**, high-$T_c$ cuprates, heavy-fermion quantum phase transitions.
- **Example Materials**:  
  - **Cuprate superconductors** above $T_c$, **heavy fermion systems** near critical doping.
  
**Key Expansion**:
1. Illustrates **breakdown** of conventional quasiparticle picture.  
2. Motivates new theories that do not rely on Landau's FLT assumptions.

---

## Conclusion
Each theoretical advancement **extends or refines** the quasiparticle picture to new regimes of interaction strength and complexity:

1. **Fermi Liquid Theory** (Landau) → Foundational quasiparticle idea for weakly correlated metals.  
2. **Hartree-Fock** → Mean-field exchange for moderate correlation; baseline for perturbation expansions.  
3. **RPA** → Collective modes (plasmons) & screening in electron gas.  
4. **GW** → More accurate band energies and quasiparticle properties beyond HF, good for moderate correlations.  
5. **DMFT** → Local strong correlations, Mott physics, heavy fermions.  
6. **GW+DMFT** → Nonlocal screening + local strong correlation.  
7. **Non-Fermi Liquid & Beyond** → Strange metals, quantum critical points, breakdown of the quasiparticle concept.

Each approach works best in the **regime** for which it was designed, and many real materials require **hybrid or advanced** methods to accurately capture their quasiparticle excitations.
