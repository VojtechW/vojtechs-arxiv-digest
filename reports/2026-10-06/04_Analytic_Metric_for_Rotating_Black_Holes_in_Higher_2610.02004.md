# 🕳️ Analytic Metric for Rotating Black Holes in Higher-Derivative Gravity

🌠 **Should-Read** · 🔬 Quality 7/10 · 🎯 Relevance 6/10

📎 **Citation:** Jierui Hu, Dongjun Li, Nicolás Yunes, *Analytic Metric for Rotating Black Holes in Higher-Derivative Gravity*, arXiv:[2610.02004](https://arxiv.org/abs/2610.02004) [gr-qc], submitted 01 Oct 2026.

> 💡 By rebuilding the spacetime from a curvature perturbation rather than solving the full field equations, the authors get a rotating black hole in a gravity theory with curvature-cubed corrections, written in closed form at every spin, where earlier results were either expansions in small spin or purely numerical.

## 🔍 Executive Summary

The paper treats the first-order correction to Kerr in parity-even cubic (Riemann-cubed) gravity as a sourced linear perturbation problem. It solves a stationary sourced Teukolsky equation for Psi_0 mode by mode, with each angular mode written in closed form using rational functions, three logarithms and two dilogarithm pairs. It then gets the full metric through the authors' traceful-radiation-gauge reconstruction hierarchy, using an integral-free potential obtained from the Teukolsky modes by differentiation. Psi_4 follows from Psi_0 through a t-phi reflection isometry. The remaining Einstein equations are shown to close, and the truncated metric's Einstein residual is proven to be controlled only by the omitted source multipoles, decaying exponentially in the angular cutoff. The result reduces to the known static solution and reportedly matches independent analytic horizon predictions.

## 📣 Claimed Contribution

Turning metric reconstruction into an analytic solver for rotating black holes in modified gravity, bypassing direct solution of the coupled field equations. As a demonstration, the first analytic spinning black-hole metric in parity-even cubic gravity at linear order in the coupling, with no small-spin or weak-field expansion, validated against the field equations and against independent horizon predictions.

## ✅ Strengths

- Removes the small-spin expansion that limits the Cano-Ruiperez-type metrics, which in practice matters most at high spin where those series converge poorly.
- Careful closure argument: the reconstruction uses only part of the Newman-Penrose equations, and the paper shows the remaining Ricci/Bianchi residuals obey homogeneous equations whose solutions are excluded by the falloff conditions.
- Clean truncation-error identity: the Einstein residual of the ell-truncated metric equals a fixed second-order operator acting on the omitted source multipoles, so the error is computable and decays like rho(r)^(-ell_max) with an explicit rate.
- Neat structural results, notably Psi_4 = Delta^2 Psi_0 / (4 conj(Gm)^4) from the t-phi reflection isometry of Kerr, and an integral-free formula for the Hertz-like potential from the Teukolsky modes.
- Explicit horizon regularity (ingoing coordinates) and axis regularity arguments; mass and angular momentum fixed unambiguously by falloff; reduces exactly to the known static solution.

## ⚠️ Weaknesses

- 'Analytic metric' means an infinite sum over angular modes, each closed form, truncated at a finite cutoff. It is not a single closed-form expression. The convergence rate at the horizon degrades to (1+sqrt 2)^(-ell) as spin goes to extremality, which is exactly the regime where higher-derivative corrections are most interesting (Horowitz-Kolanowski-Remmen-Santos 2023).
- Only one example: parity-even cubic gravity, where the source is pure gravity, built from Kerr curvature and rational. Theories with extra scalar fields (scalar Gauss-Bonnet, dynamical Chern-Simons), parity-odd or quartic terms would need the scalar solved first, or have messier sources, so the 'general solver' framing is not yet demonstrated.
- The method rests on the traceful radiation gauge introduced five months earlier by two of the same authors (arXiv:2605.11080), so the methodological novelty is shared with that paper. This one is mainly the first nontrivial rotating application.
- Linear in the coupling and stationary only. Nothing on dynamics, perturbations or quasinormal modes of the new background yet.
- I could only access the supplemental-material sections of the LaTeX source, not the main body of the Letter. The comparison to independent horizon predictions, the numerical residual plots and the novelty discussion in the main text could not be checked directly.

## 🤔 Skeptic's Cross-Examination

The selling point is 'analytic, without spin expansion', yet the deliverable is an infinite angular sum that has to be truncated and checked numerically, much like a spectral solution, and it converges slowest near extremality, where the physics is most interesting. Cubic gravity is also the friendliest test case: the source is a rational function on Kerr and no extra fields appear. Until the method handles scalar Gauss-Bonnet or dynamical Chern-Simons, where the scalar profile is itself only known as a sum, the 'general solver' claim is a promise, not a result.

## 🆕 Novelty in Context

Prior work on rotating black holes in this theory is of two kinds. Cano and Ruiperez (2019) and the follow-ups by Cano, Fransen, Hertog and Maenaut on ringdown give analytic metrics as high-order expansions in spin. Horowitz, Kolanowski, Remmen and Santos (2023) solved the higher-derivative corrections at arbitrary spin numerically. Reall and Santos (2019) already obtained exact-in-spin corrections to thermodynamic and horizon quantities without solving for the metric, which is presumably the 'independent analytic prediction' used for validation. The reconstruction machinery, the traceful radiation gauge with transport equations for the trace, was introduced by Li and Yunes in arXiv:2605.11080 and only illustrated there on a static Schwarzschild shell. Calling this the 'first analytic spinning metric without spin expansion' is defensible only if a convergent sum of closed-form angular modes counts as analytic. The honest claim is a semi-analytic, exponentially convergent, exact-in-spin representation, and a first nontrivial Kerr application of the authors' own reconstruction scheme. That is still a genuine and useful step. My literature queries turned up no earlier analytic exact-in-spin metric for this theory.

## 🎯 Relevance to Your Research

This connects directly to Kerr perturbation theory and metric reconstruction from the Teukolsky equation with sources: a radiation-gauge-like reconstruction with a corrector, Wald's adjoint structure, and closure of the remaining Newman-Penrose equations. It is a useful template for sourced stationary reconstruction, for example for second-order or environmental sources on Kerr, and it supplies a background usable for modeling extreme-mass-ratio inspirals and tests of GR beyond Kerr at arbitrary spin. Read the supplemental sections on closed-form radial modes, the integral-free potential equation, and the finite-cutoff Einstein identity.

📖 **Where to start:** Supplement: 'Closed-form radial modes' (function class of each mode), 'The potential equation and its integral-free solution' (the trick that avoids extra radial integrals), 'Explicit metric' (final components and horizon shift), 'Closure of the remaining Einstein equations', and 'Finite-cutoff Einstein identity' plus 'Angular convergence rate' (error control). The Psi_0 to Psi_4 reflection argument is short and worth a look.

## Scores

- 🔬 **Quality:** 7/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.7/10)

## 🚧 Caveats

- 'Analytic' means a mode sum with closed-form terms, truncated in ell; convergence slows near extremal spin.
- Only demonstrated for parity-even Riemann-cubed gravity at linear order in the coupling; no scalar-field theories.
- The reconstruction method itself comes from the same group's May 2026 paper; this is its first rotating application.
- Stationary background only; no perturbations or ringdown of the corrected black hole.

## In Network

- 🚩 Nicolas Yunes — notable author

---

🔗 [Back to the weekly digest](../2026-10-06)
