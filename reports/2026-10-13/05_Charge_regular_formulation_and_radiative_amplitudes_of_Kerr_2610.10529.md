# 🎵 Charge-regular formulation and radiative amplitudes of Kerr-Newman perturbations

🌠 **Should-Read** · 🔬 Quality 6/10 · 🎯 Relevance 5.5/10

📎 **Citation:** Hayato Motohashi, *Charge-regular formulation and radiative amplitudes of Kerr-Newman perturbations*, arXiv:[2610.10529](https://arxiv.org/abs/2610.10529) [gr-qc, hep-th], submitted 07 Oct 2026.

> 💡 Building on last month's exact separation of the coupled gravitational and electromagnetic perturbations of a rotating charged black hole, this paper rewrites the separated equations so they turn smoothly into the familiar uncharged (Teukolsky) equations as the charge goes to zero, and gives explicit formulas for the gravitational and electromagnetic waves and energy each separated mode sends out to infinity.

## 🔍 Executive Summary

Hintz's recent separation of Kerr-Newman gravito-electromagnetic perturbations (arXiv:2609.33661) uses variables in which the angular eigenvalue and several coefficients diverge as Q -> 0. This paper rescales branch by branch to obtain angular and radial first-order systems, and second-order 'deformed Teukolsky' equations for s = +-1, +-2, that reduce exactly to the four Kerr Teukolsky equations at Q = 0. It then builds the inverse map from master variables to the physical Weyl and Maxwell scalars, fixes the horizon and infinity normalizations (taking care of a far zone at r ~ M^2/(omega Q^2) where the Q -> 0 limit is not uniform), and derives the outgoing gravitational and electromagnetic amplitudes and energy fluxes. The headline consequence is that the electromagnetic-to-gravitational power ratio of a single outgoing mode is an exact angular-only quantity, (Q^2/9M^2) N_zeta/N_chi, with a closed-form small-charge limit in terms of the Kerr eigenvalue and <cos theta>. That ratio reproduces the known Reissner-Nordstrom channel mixing exactly.

## 📣 Claimed Contribution

A charge-regular formulation of the separated Kerr-Newman system with a smooth Kerr limit, together with an explicit, normalized map from master solutions to the physical radiative fields. This yields boundary bases and a connection matrix that reduce to standard Kerr conventions, and closed-form outgoing gravitational and electromagnetic amplitudes, energy fluxes and exact finite-charge radiation-composition ratios at nonzero real frequency.

## ✅ Strengths

- Addresses a real and timely gap: Hintz's separation is not directly usable for flux or scattering calculations because its variables are singular as Q -> 0 and are not tied to normalized physical fields. This paper supplies that dictionary.
- Table I collects every equation needed for use (regular first-order systems, deformed Teukolsky equations, reconstruction, boundary bases, connection-to-amplitude map, power formulas), which makes the paper practical.
- Handles the boundary carefully: it identifies the far zone r ~ M^2/(omega Q^2), where fixed-radius convergence in Q fails, and builds normalized bases that are analytic in Q^2 instead of naively substituting Q = 0.
- Gives a nontrivial independent check: at a = 0 the composition ratio (L-1)/(L+1) matches the Reissner-Nordstrom channel-mixing angle of Ould El Hadj et al., which tests the relative gravitational and electromagnetic normalization and the sign of the Bianchi-identity subtraction.
- The small-charge composition formula needs only the Kerr eigenvalue and one angular moment, with no derivatives of the eigenfunction or of the finite-charge eigenvalue, so it is immediately computable.
- States its scope honestly: real frequency only for the flux formulas, no horizon flux, no full metric reconstruction, and the regular-limit overlap with Destounis-Cardoso-Hintz is acknowledged.

## ⚠️ Weaknesses

- No numerical results at all. The deformed Teukolsky equations are never solved for a rotating charged case, and no flux, composition ratio or connection coefficient is evaluated for a > 0, Q > 0. Apart from the Reissner-Nordstrom limit, every claim is unchecked in practice.
- Part of the main new content, the charge-regular angular and radial systems with their Kerr limits (Secs. III-IV), was obtained independently and published days earlier in Appendix B of Destounis, Cardoso and Hintz (arXiv:2610.07142). The genuinely unique part is the physical-field and flux normalization of Secs. V-VII.
- Fluxes are given only at infinity for outgoing modes. Horizon absorption, scattering conversion and sourced (e.g. point-particle) problems are explicitly left out, and these are what an inspiral or scattering calculation would actually need.
- The 'exact radiation composition' result follows almost directly from the reconstruction map (the radial amplitude cancels by construction), so it is less of a physics result than the abstract implies.
- The paper is heavy on notation (several sign and branch labels sigma, epsilon, tau and multiple rescalings) and the main text often defers proofs to appendices. Verification is laborious, and the author states that AI assistants were used for the symbolic calculations.
- The Kerr-Newman background is astrophysically marginal, so practical impact depends on theoretical interest (tests of Einstein-Maxwell, charged-black-hole ringdown, analogue models) rather than observational need.

## 🤔 Skeptic's Cross-Examination

This is bookkeeping on top of Hintz's breakthrough, written within two weeks and partly scooped by Hintz's own collaborators. A formalism paper whose only test is the a = 0 limit, already known since Chandrasekhar and Moncrief, has not shown that its rotating-charged normalizations are right. One numerically computed Kerr-Newman flux, compared against the two-dimensional coupled-equation codes of Dias-Godazgar-Santos, would have been worth more than the pages of analyticity arguments. Without horizon fluxes or a source term, it does not yet enable the calculations (scattering, inspirals, excitation factors) that motivate it.

## 🆕 Novelty in Context

The paper positions itself as a direct follow-up to Hintz (arXiv:2609.33661, Sept 2026), which achieved the separation and proved real-axis mode stability but in charge-adapted 'phantom-gauge' variables that are singular as Q -> 0. My literature check found the companion Destounis-Cardoso-Hintz paper (arXiv:2610.07142, two days earlier). Its Appendix B, 'The vanishing charge limit', builds regular angular generalized eigenproblems and regular radial first-order and second-order systems with Kerr limits by rescaling with powers of Q/M, essentially the same construction as Secs. III-IV here. The author acknowledges this in a 'Note added' and gives the parameter map mu = 3 lambda-tilde + (Q^2/M^2) lambda-tilde^2. The 'charge-regular formulation' half of the title is therefore not unique. The added value is the explicit deformed-Teukolsky second-order form in Kerr-like notation, plus the physical-field reconstruction, boundary normalization and outgoing flux and composition formulas, which I did not find elsewhere for Kerr-Newman. Earlier coupled-system work (Pani et al. slow rotation; Mark et al. small charge; Dias-Godazgar-Santos two-dimensional quasinormal modes and gauge-invariant radiative fields; Giorgi's coupled Teukolsky systems) is cited fairly. For Reissner-Nordstrom the composition result reduces to known channel mixing. The honest novelty is the normalization and radiation dictionary for the newly separated system, not the regularization itself.

## 🎯 Relevance to Your Research

Moderately relevant to a Kerr perturbation-theory and self-force reader. If the newly separated Kerr-Newman system is to be used for Teukolsky-style flux calculations (charged-black-hole extreme-mass-ratio inspirals, testing frequency-domain codes, Einstein-Maxwell response), this is the paper that ties the master functions to Psi_4/phi_2-type physical amplitudes with Kerr conventions at Q = 0. The deformed Teukolsky radial equation in Table I has the same structure as the standard Kerr one plus explicit order-Q^2 terms, so it could be added to an existing Teukolsky solver. It is not needed for vacuum Kerr work and is not astrophysically pressing.

📖 **Where to start:** Table I in the Introduction (all usable formulas in one place); Sec. VI.A (the nonuniform far zone, the key subtlety for anyone trying a small-Q expansion); Sec. VII.A-VII.D (Maxwell extraction via the Bianchi identity, flux formulas and the small-charge composition ratio); Sec. VII.E (Reissner-Nordstrom check). Skip Secs. III-IV if you have read Appendix B of arXiv:2610.07142.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 5.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.5/10)

## 🚧 Caveats

- Purely analytic: no Kerr-Newman flux or ratio is computed numerically for a rotating charged hole.
- The charge-regular separated equations overlap with Appendix B of Destounis, Cardoso and Hintz (arXiv:2610.07142); the new part is the physical normalization and flux map.
- Outgoing flux at infinity only, at real nonzero frequency; no horizon absorption, no source terms, no metric reconstruction.
- The only independent validation is the nonrotating Reissner-Nordstrom limit.

---

🔗 [Back to the weekly digest](../2026-10-13)
