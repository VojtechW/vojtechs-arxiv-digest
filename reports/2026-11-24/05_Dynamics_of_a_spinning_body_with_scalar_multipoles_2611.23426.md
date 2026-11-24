# 🌀 Dynamics of a spinning body with scalar multipoles

🌟 **Must-Read** · 🔬 Quality 6/10 · 🎯 Relevance 7/10

📎 **Citation:** Jacopo Lestingi, Thomas P. Sotiriou, Andrew Spiers, Andrea Maselli, *Dynamics of a spinning body with scalar multipoles*, arXiv:[2611.23426](https://arxiv.org/abs/2611.23426) [gr-qc, astro-ph.HE, hep-th], submitted 17 Nov 2026.

> 💡 For a small spinning body that carries a scalar charge and spirals into a much heavier black hole, the paper derives the complete equations of motion needed for next-to-leading-order waveforms, and finds that only the body's mass, spin, scalar charge and one extra constant matter, while a parity-odd (axion-like) scalar leaves the motion identical to general relativity at that order.

## 🔍 Executive Summary

The authors build a worldline action for a spinning compact body coupled to a massless scalar, extending the Porto-style spinning-particle action by letting the Lagrangian depend on the scalar field and its gradient, and read off the body's scalar monopole and dipole from it. Varying the action gives modified Mathisson-Papapetrou-Dixon equations with a scalar force and a spin torque driven by the scalar gradient, plus the sourced scalar and Einstein equations. They then power-count everything in the mass ratio for extreme-mass-ratio inspirals and keep terms through first post-adiabatic order. For an ordinary (parity-even) scalar, the 1PA dynamics needs only the scalar charge Q0 and a quadratic self-coupling constant; the scalar dipole only enters at 2PA. The only genuinely new 1PA pieces are spin-scalar couplings proportional to Q0, entering the spin precession and the acceleration. For a pseudoscalar (dynamical Chern-Simons-like), symmetry forbids a monopole, the dipole is proportional to spin, the field comes out at order mass ratio squared, and the dynamics matches GR through 1PA.

## 📣 Claimed Contribution

A systematic action-based skeletonization of a spinning body dressed with scalar multipoles (a generalization of Eardley's field-dependent mass), from which modified MPD equations and field equations are derived for both scalars and pseudoscalars. Applied to EMRIs, this gives the complete 1PA equations of motion and self-force equations for a spinning, scalar-charged secondary, extending and completing the 0PA and nonspinning 1PA framework of Maselli et al. 2020 and Spiers et al. 2023. It also shows from symmetry alone that pseudoscalar effects first enter at 2PA.

## ✅ Strengths

- Fills a real gap in the modular scalar-charge EMRI program. The existing 1PA scalar framework (Spiers et al. 2023) was nonspinning, and secondary spin is a 1PA effect, so a consistent spinning extension is needed for 1PA beyond-GR waveforms.
- Clean symmetry argument: building the charge and dipole from contractions of u and the angular velocity Omega (Cayley-Hamilton) shows the parity-even dipole is irrelevant at 1PA, and the pseudoscalar has no monopole and a dipole proportional to spin.
- Sensible limit checks: the GR limit reproduces Mathews et al. 2021, the nonspinning limit reproduces the first- and second-order scalar forces of Spiers et al. 2023, and setting Q=0 with a spin-aligned dipole recovers the dynamical Chern-Simons MPD equations of Loutrel, Tanaka and Yunes 2018.
- Gives explicit self-force-ready acceleration terms, split into gravitational, spin, scalar and spin-times-scalar parts, written in terms of regularized fields, so a waveform code could actually use them.

## ⚠️ Weaknesses

- There are no numbers anywhere. The paper never estimates how big the new spin-scalar 1PA terms are (for example the dephasing they cause, or the bias if they are left out), so we cannot tell whether they matter for LISA.
- Much of the formal machinery is not new. Modified MPD equations with scalar monopole and dipole terms already exist (Obukhov and Puetzfeld 2014, which the paper itself says has a similar structure; Loutrel et al. 2018 for Chern-Simons), and Brax et al. 2021 already built a spinning point-particle action coupled to a scalar and showed that a scalar coupling to mass forces a coupling to spin. That is the physics behind the Q0-spin terms here.
- The pseudoscalar 'identical to GR through 1PA' result depends on the EFT power counting, with the coupling constant set to order (secondary mass)^2 so that primary hair is pushed to O(epsilon^4). It confirms the earlier dipole-flux suppression result of Lestingi, Cannizzaro and Pani 2024 rather than being a surprise.
- Spin-spin terms are dropped, and the claim that the setup is 'complete' through 1PA rests on dimensional power counting (for example dipole ~ mu^2) rather than on an explicit matched-expansion derivation of the scalar multipoles.
- The mapping of the new constants onto specific theories, such as scalar-Gauss-Bonnet, is left for future work, so Q_phichi is just a free parameter.
- The LaTeX source has a leftover author note flagging that the mapping to the earlier paper's second-order mass coefficient still needs checking, and that the earlier paper has typos. Anyone implementing these equations should check the coefficient conventions themselves.

## 🤔 Skeptic's Cross-Examination

This is Brax et al.'s spinning scalar-tensor point-particle action, re-run with EMRI power counting instead of post-Newtonian counting, and checked against equations already in the literature. The only new physical terms are Q0-proportional spin-scalar couplings at 1PA, and the paper never shows they are large enough to matter for LISA compared with the already-known scalar-charge and GR spin effects. The 'pseudoscalar equals GR' headline follows directly from the assumed size of the coupling constant.

## 🆕 Novelty in Context

The introduction positions the paper as generalizing the point-particle scalar-charge framework of Maselli et al. 2020 and Spiers et al. 2023 to spinning bodies, using the worldline EFT approach that Loutrel, Tanaka and Yunes 2018 applied to dynamical Chern-Simons gravity and Brax, Davis, Melville and Wong 2021 applied to scalar-tensor theories. Checking those abstracts: Brax et al. 2021 already build an effective action for a generic spinning body coupled conformally and disformally to a scalar, and show that a scalar coupled to the mass must also couple to the spin, though they apply it only in post-Newtonian theory. Guo et al. 2023 already added secondary spin to scalar-charged EMRIs at the equation-of-motion level, though not systematically. Lestingi, Cannizzaro and Pani 2024 already showed that a scalar dipole's flux is suppressed by the mass ratio squared. The paper itself notes that its modified MPD equations look like those of Obukhov and Puetzfeld 2014. So the honest novelty is narrower than 'a new skeletonization': the paper carries the spinning scalar worldline EFT through a consistent EMRI mass-ratio power counting to 1PA. It identifies exactly which parameters survive (Q0 and Q_phichi), shows the parity-even dipole drops out, and writes down self-force-ready 1PA equations. The pseudoscalar result is a symmetry-based confirmation of the earlier dipole suppression. This is a worthwhile, incremental closing of a gap, not a conceptual advance.

## 🎯 Relevance to Your Research

This is directly relevant to anyone working on 1PA EMRI modelling or beyond-GR self-force. It is the spinning-secondary completion of the scalar-charge framework (Maselli et al. 2020, Spiers et al. 2023, Barsanti et al.) that feeds LISA tests of GR. The result to take away is the 1PA equation set: the spin precession equation with the Q0 scalar-gradient torque, the four-velocity equation, and the self-force split. The pseudoscalar null result is also useful for anyone thinking about Chern-Simons constraints from EMRIs. The paper is pure formalism, with no waveforms or estimates.

📖 **Where to start:** Sec. 6 (Scalar vs pseudoscalar: the symmetry-based structure of the charges and dipole); Sec. 7.2 (the final 1PA MPD equations, including the new spin precession term); Sec. 7.4.1 (scalar self-force equations, with the explicit spin-times-scalar acceleration); Sec. 8 (pseudoscalar case, where it reduces to GR through 1PA). Skim the end of the Introduction for how the paper positions itself.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 7/10
- 🌟 **Reading priority:** Must-Read (weighted score 6.5/10)

## 🚧 Caveats

- Formalism only: there are no waveforms, dephasing estimates or numerical results, so we do not know how large the new spin-scalar terms are.
- The modified MPD structure and the spin-scalar coupling are not new in themselves (Obukhov and Puetzfeld 2014, Loutrel et al. 2018, Brax et al. 2021). What is new is the EMRI mass-ratio power counting through 1PA.
- The pseudoscalar 'same as GR at 1PA' conclusion assumes the coupling is set by the secondary's scale; if the coupling is larger, the primary's hair and background corrections would not be negligible.
- Spin-spin terms are neglected; the scalar self-coupling constant is left unmapped to any concrete theory.
- Check the coefficient conventions against Spiers et al. 2023 before implementing; the authors' own source notes possible typos there.

## In Network

- 🚩 Thomas Sotiriou — notable author
- 🚩 Andrew Spiers — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-11-24)
