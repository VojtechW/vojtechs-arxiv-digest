# 🎵 Perturbations of Kerr-Newman black holes: separation and mode stability

🌠 **Should-Read** · 🔬 Quality 7/10 · 🎯 Relevance 5/10

📎 **Citation:** Peter Hintz, *Perturbations of Kerr-Newman black holes: separation and mode stability*, arXiv:[2609.33661](https://arxiv.org/abs/2609.33661) [gr-qc, math.AP], submitted 27 Sep 2026.

> 💡 A mathematician claims to have found a way to split the tangled gravitational and electromagnetic vibrations of a spinning, charged black hole into separate angular and radial equations, a problem open for about forty years, and uses this to prove that no undamped vibrations exist at real frequencies.

## 🔍 Executive Summary

The paper studies linear perturbations of the subextremal Kerr-Newman black hole in Einstein-Maxwell theory, where gravitational and electromagnetic perturbations are coupled and have long been believed not to separate in Boyer-Lindquist-type coordinates. According to the abstract, the author rewrites the radiative degrees of freedom as suitably transformed first-order systems and uses a matrix-valued integrating factor to achieve separation of the angular dependence, leaving (coupled) radial ordinary differential equations. For these radial equations he proves mode stability on the real frequency axis, meaning there are no quasinormal modes with real frequency, using a generalisation of Whiting's integral transform. Mode stability in the upper half plane (exponentially growing modes) is not claimed in the abstract.

## 📣 Claimed Contribution

(i) A method that overcomes Chandrasekhar's 'apparent indissolubility of the coupling between the spin-1 and spin-2 fields' for Kerr-Newman, via a matrix integrating factor for transformed first-order systems, yielding angular separation of the coupled electromagnetic-gravitational perturbation equations; (ii) a proof of real-axis mode stability (no real-frequency quasinormal modes) for the resulting radial ODEs, via a Whiting-type transform.

## ✅ Strengths

- If the separation holds as stated, it resolves a long-standing structural obstruction: previous work either solved coupled 2D PDEs numerically (Dias-Godazgar-Santos 2015, Pombo 2026), used small-charge or slow-rotation expansions (Mark-Yang-Zimmerman-Chen 2015, Pani-Berti-Gualtieri 2013), used the uncontrolled Dudley-Finley approximation, or worked in physical space precisely because mode separation was thought impossible (Giorgi 2020 onward).
- Author is a leading figure in rigorous black-hole perturbation theory (Kerr-de Sitter and Kerr-Newman-de Sitter nonlinear stability, Kerr-de Sitter mode stability), so the result is very likely a genuine rigorous theorem rather than a formal manipulation.
- Real-axis mode stability is exactly the ingredient needed for the Kerr-style route to boundedness and decay (as Whiting/Shlapentokh-Rothman and Andersson-Ma-Paganini-Whiting supplied for Kerr), so the paper plugs into an established programme.
- A separated ODE formulation would make Kerr-Newman quasinormal modes, Green functions and potentially self-force-type computations accessible with ODE tools instead of 2D eigenvalue solvers.

## ⚠️ Weaknesses

- The full text could not be retrieved: the paper was not in local storage, the LaTeX outline tool returned no sections (only an unresolved bibliography include), and text search failed. This assessment rests on the abstract, the metadata and the literature check only; no equation, theorem statement or proof was inspected.
- Only real-axis mode stability is claimed. Absence of growing modes in the upper half plane, the physically decisive statement, is not claimed in the abstract and remains supported only by the numerical evidence of Dias-Godazgar-Santos.
- Separation via a matrix integrating factor is likely to give coupled matrix-valued (at least 2x2) radial and angular systems, not decoupled scalar Teukolsky-like equations for each spin. The word 'separation' should not be read as 'decoupling of spin-1 and spin-2'. This could not be checked in the text.
- It is unclear from the abstract whether the transformed first-order systems fully capture the gauge-invariant radiative content (how metric reconstruction or the low-frequency and stationary modes are handled), and whether the angular eigenvalue problem is self-adjoint or has a usable spectral theory.
- No numerical cross-check against known Kerr-Newman quasinormal-mode tables is mentioned in the abstract; for a mathematics-style paper this may be absent, so practical use for spectroscopy is untested.

## 🤔 Skeptic's Cross-Examination

A 'matrix integrating factor' separation may simply repackage the coupling into matrix-valued angular and radial operators. That is a genuine but more modest advance than decoupling, and it may not come with the spectral completeness, such as a complete set of angular eigenfunctions, needed to reconstruct general perturbations. Real-axis mode stability is also the easier half of mode stability, so the headline 'mode stability' falls well short of ruling out growing modes.

## 🆕 Novelty in Context

The literature check supports the novelty claim as far as it can be tested without the full text. Giorgi (arXiv:2002.07228) states explicitly that the stability of Kerr-Newman 'can not be obtained through standard decomposition in modes' because the gravitational and electromagnetic modes cannot be decoupled, and so develops physical-space generalised Regge-Wheeler equations. The follow-up boundedness and decay results (Giorgi 2023; Giorgi-Wan 2024) are restricted to small charge and rotation or to axisymmetry. Dias-Godazgar-Santos (arXiv:1501.04625) solved a coupled system of two partial differential equations numerically and found no unstable modes up to 99.999% of extremality. As recently as July 2026, Pombo (arXiv:2607.14216) still treats Kerr-Newman quasinormal modes as 'a genuinely coupled two-field problem' requiring a 2D solver. Other approaches rely on small-charge or slow-rotation expansions or on the Dudley-Finley approximation (Saha-Silva 2025). No prior paper claiming angular separation of the full coupled Kerr-Newman system was found. The real-axis mode-stability part follows the established Whiting-transform route used for Kerr (Whiting 1989; Shlapentokh-Rothman 2015; Andersson-Ma-Paganini-Whiting 2017), and Civin (2014) did the scalar-wave case on Kerr-Newman. That part is therefore a natural, though likely technically hard, extension, and the separation result is the real novelty. Whether the separation is as strong as the abstract suggests (decoupled versus matrix-coupled) could not be verified.

## 🎯 Relevance to Your Research

Moderately relevant to black-hole perturbation theory and self-force work: a separable Kerr-Newman formulation would be the charged analogue of the Teukolsky framework that underpins extreme-mass-ratio inspiral modelling, and the integrating-factor trick may interest anyone working on separability and hidden symmetries. Direct application to astrophysical inspirals is limited, since astrophysical black holes carry negligible charge; the main interest is structural and mathematical. Read the introduction for the positioning relative to Chandrasekhar and Giorgi, the section constructing the first-order systems and the matrix integrating factor, and the statement of the mode-stability theorem (section titles could not be retrieved).

📖 **Where to start:** Introduction (positioning against Chandrasekhar, Giorgi and Dias-Godazgar-Santos); the section introducing the transformed first-order systems and the matrix integrating factor (the core new idea); the statement of the main real-axis mode-stability theorem and the Whiting-type transform. Exact section numbers could not be retrieved.

## Scores

- 🔬 **Quality:** 7/10
- 🎯 **Relevance:** 5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.6/10)

## 🚧 Caveats

- This report is based on the abstract and a literature check only; the full text could not be accessed.
- Mode stability is proven only for real frequencies, not for exponentially growing modes.
- 'Separation' probably means separation into coupled matrix-valued ordinary differential equations, not scalar decoupled Teukolsky-type equations; check before relying on it.
- Rigorous mathematics-style paper; expect little or no quasinormal-mode numerics.

---

🔗 [Back to the weekly digest](../2026-09-29)
