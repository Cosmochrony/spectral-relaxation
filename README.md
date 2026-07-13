This repository contains the source of the **Spectral Relaxation** Cosmochrony paper  
*Asymptotic Saturation of Projective Resolution: Expander Relaxation Graphs*.

This work extends the **spectral admissibility programme** by deriving a
dynamical law for the **projective resolution** governing the accessibility
of spectral modes along the relaxation cascade.

While **Spectral Stratigraphy** identifies discrete spectral levels
capable of stabilisation, the present work investigates **how the projective
cut-off evolves along the cascade** and how this evolution controls
the emergence of particle mass hierarchies.

The analysis shows that, for expander relaxation graphs, the admissibility
threshold is governed by the **spectral connectivity of the relational graph**.

# Core Result

The projective resolution at cascade rank \(n\)

$\Lambda_{\mathrm{proj}}(n)$

is determined by the global projective flux bound $c_{\mathrm{BI}}(n)$.

Under the **projective coherence closure**

$c_{\mathrm{BI}}(n) \asymp h(G(n))$

where $h(G)$ is the Cheeger constant of the relaxation graph, the
projective resolution satisfies

$\Lambda_{\mathrm{proj}}(n) \asymp h(G(n))^2$.

Using the Cheeger inequality

$\frac{\lambda_2(n)}{2} \le h(G(n)) \le \sqrt{2\lambda_2(n)}$

this yields the spectral enclosure

$\lambda_2(n)^2 \lesssim \Lambda_{\mathrm{proj}}(n) \lesssim \lambda_2(n)$.

For expander families satisfying spectral–isoperimetric saturation,

$h(G(n))^2 \asymp \lambda_2(n)$,

the projective resolution follows the **linear spectral law**

$\Lambda_{\mathrm{proj}}(n) \asymp \lambda_2(n)$.

Thus the maximal projectable eigenvalue is controlled by the
**algebraic connectivity of the relaxation graph**.

# Relaxation Graph Model

To obtain an explicit realisation of the relaxation cascade, the paper
introduces a family of **expander relaxation graphs**.

The analysis focuses on the **Lubotzky–Phillips–Sarnak (LPS) Ramanujan graphs**

$X_{p,q} = \mathrm{Cayley}\!\left( PSL(2,\mathbb{F}_q), S_p \right)$

which satisfy:

- vertex transitivity
- bounded degree
- explicit spectral gap
- constructive infinite families

These graphs provide an analytically controlled model for the
evolution of relational connectivity along the cascade.

# Asymptotic Saturation

For fixed prime $p$, the algebraic connectivity of LPS graphs satisfies

$\lambda_2(n) \to \lambda_2^*(p)$

as the graph size increases.

Consequently

$\Lambda_{\mathrm{proj}}(n) \to \Lambda_0(p)$

and the admissibility threshold becomes **asymptotically static**.

In this regime, stabilisation of spectral modes is governed not by the
motion of the admissibility cut-off but by the **growth of the cumulative
spectral count**.

# Spectral Counting Dynamics

For large graphs the Laplacian spectrum follows the
**Kesten–McKay distribution**

$\rho_{KM}(\lambda)$.

The cumulative spectral count satisfies

$N(\lambda;n) \sim F_{KM}(\lambda)\, n$

where $F_{KM}$ is the cumulative Kesten–McKay distribution.

Stabilisation occurs when the number of projectable modes reaches the
dimension of the corresponding representation block:

$N(\lambda_i;n) \sim k\,\dim\rho_i$.

This yields the mass relation

$M_i \propto \frac{F_{KM}(\lambda_i)}{\dim\rho_i}$.

# Limitation of the Single-Level Mechanism

Numerical evaluation shows that the LPS–KM mechanism produces

- well-defined stratigraphic levels
- mass ratios of order unity

but fails to reproduce the observed **inter-generation hierarchy**.

Two limitations are identified:

- inversion of the admissibility ordering
- insufficient amplification of mass ratios.

These limitations arise from the **asymptotic constancy of the projective
resolution** in the fixed-$p$ model.

# Conceptual Structure

Spectral Relaxation connects several components of the Cosmochrony framework:

1. Projective admissibility from bounded relational flux
2. Global coherence constraints of the relational substrate
3. Spectral geometry of expander graphs
4. Kesten–McKay spectral statistics
5. Representation-theoretic stratification from Spectral Stratigraphy

The resulting framework establishes the **dynamical control of projective
resolution by spectral connectivity**.

# Separation of Physical Mechanisms

The combined analysis of Stratigraphy and Relaxation reveals a
clear separation of roles:

**Group topology**

→ determines the number of spectral levels  
→ fixes the number of particle generations

**Spectral connectivity**

→ determines the admissibility resolution  
→ governs accessibility of spectral sectors

**Cascade saturation**

→ determines the stabilisation rank  
→ generates mass relations.

# Open Direction

The analysis identifies a structural limitation of fixed-valence
relaxation graphs.

If the graph degree grows along the cascade,

$p(n) \to \infty$,

the Kesten–McKay support shrinks toward $\lambda=1$,
causing ADE spectral levels to leave the support in a
rank-dependent order.

This mechanism restores the admissibility ordering and provides a
natural candidate for generating realistic mass hierarchies.

This regime will be investigated in the next paper of the
**spectral admissibility programme**.

# Status

This framework is:

- spectral-geometric
- analytically tractable
- numerically testable
- compatible with spectral admissibility, spectral capacity,
  and spectral stratigraphy.

It does not assume:

- particle fields
- quantum statistics
- specific microscopic dynamics beyond bounded relational flux.

# Repository Structure
```
paper/
├── pdf/ # Compiled Spectral Relaxation PDF
├── tex/ # LaTeX sources
└── README.md
```

# Citation

If you reference this work, please cite:

> J. Beau, *Asymptotic Saturation of Projective Resolution: Expander Relaxation Graphs*, Zenodo, 2026.

# Acknowledgements

Portions of the derivations, numerical verification, and editorial
refinement benefited from iterative interactions with large language
models used as analytical assistants.  
All theoretical results and interpretations remain the sole responsibility
of the author.

# Contributions

This repository is intended as a research reference.

Critical feedback, independent spectral analyses, and alternative
expander constructions are welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
