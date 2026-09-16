# 〰️ NRHJSur3dq8: a spectral numerical-relativity surrogate family for non-eccentric aligned-spin binary-black-hole waveforms

🌠 **Should-Read** · 🔬 Quality 7.5/10 · 🎯 Relevance 6/10

📎 **Citation:** Vaishak Prasad, *NRHJSur3dq8: a spectral numerical-relativity surrogate family for non-eccentric aligned-spin binary-black-hole waveforms*, arXiv:[2609.09088](https://arxiv.org/abs/2609.09088) [gr-qc, astro-ph.HE, astro-ph.IM], submitted 08 Sep 2026.

> 💡 A new fast model of the gravitational waves from merging black holes reproduces full numerical simulations about five times more closely than the standard model of its class, and additionally hands the user exact derivatives of the wave with respect to the source parameters and an honest estimate of its own error.

## 🔍 Executive Summary

The paper builds a surrogate model for aligned-spin, quasi-circular binary-black-hole waveforms trained on 260 simulations from the SXS catalog, organised around an action-angle-inspired conditioning: waveform modes are demodulated by the orbital phase read from the (2,2) mode and every surrogated quantity (the co-orbital modes, the time-of-phase 'clock', the flux-integrated azimuthal action and energy) is carried as a slow function of that phase on shared hp-adaptive Chebyshev elements, with Gaussian-process regression across (log q, chi_1z, chi_2z). A separate time-parameterised merger-ringdown block is attached where adiabaticity fails, and low starting frequencies are reached by a call-time 4PN extension stitched in the action variable rather than in the waveform. Strict leave-one-out validation gives median unweighted mismatches of 1.3e-6 on the (2,2) and 2.3e-6 all-mode over the full inspiral-merger-ringdown span, roughly 5-6 times better per simulation than NRHybSur3dq8 on the identical measurement. Beyond accuracy, the model exposes closed-form analytic parameter derivatives (validated against Richardson-extrapolated finite differences), a calibrated Gaussian-process predictive uncertainty, exact exchange (mass-swap) symmetry by construction, and is released as a pip-installable package with model files on Zenodo.

## 📣 Claimed Contribution

First numerical-relativity surrogate organised around an action-angle / adiabatic-angle parameterization, in which the fast orbital phase is the abscissa and the surrogated content is what survives its removal; and the only waveform surrogate that simultaneously provides analytic (non-autodiff) device-native parameter derivatives, a calibrated and propagated per-evaluation uncertainty envelope, and exactly exchange-symmetric modes, at accuracy claimed to exceed NRHybSur3dq8 while evaluating 2-9 times faster.

## ✅ Strengths

- Validation is unusually disciplined: a full leave-one-out retrain on all 260 simulations (inspiral and merger-ringdown arms both refit), one fixed mismatch definition stated explicitly and reused for every comparison, and mode content matched before comparing against external models.
- The paper repeatedly identifies which floor limits each number: the (4,3) is representation-limited, the q~1 (4,4) and (5,5) training data are unresolved so quoted errors there are catalog-limited, and edge-on accuracy is set by the seven-mode truncation floor rather than by the fit. Very few waveform papers do this bookkeeping.
- Exact exchange symmetry via parity-restricted trend and symmetrized kernel is a genuine structural improvement: the model returns bitwise-mirrored modes where coordinates round-trip exactly, against residuals of 7e-5 to 2e-4 (NRHybSur3dq8) and 1e-3 to 2e-3 (NRSur7dq4).
- The action-native hybridization is more than framing: stitching the 4PN arm by value continuity of J_phi leaves the NR span structurally untouched, and the seam mismatch drops from 4.1e-7 to 2.3e-10 (all-mode) relative to a conventional waveform splice on the same simulation; the first-law residual |(dE/dJ)/omega - 1| is then used as a genuine acceptance test, including at held-out parameters where it isolates regression error (1.4e-4 versus 2.9e-6 on stitched NR data).
- Gradients are validated properly, against Richardson-extrapolated central differences with the finite-difference resolution itself measured, and the residual 3e-5 plateau is explained (native-grid versus resampled evaluation route) rather than hidden.
- The paper states, without prompting, that its comparison against NRHybSur3dq8 is conservative in the wrong direction for itself (LOO versus partially in-sample) and that NRSur7dq4 simply cannot cover the comparison span.

## ⚠️ Weaknesses

- The headline accuracy advantage over NRHybSur3dq8 is confounded by training data: this model uses 260 simulations from the current SXS catalog, NRHybSur3dq8 used roughly 100 from a 2019 catalog. The paper never attempts to separate the gain from the action-angle representation from the gain from 2.5x more and better-resolved simulations, which is the single most important control missing from the comparison.
- The detector-relevant numbers are in-sample. The sky-averaged, SNR-weighted, PSD-weighted full-IMR mismatches (8.9e-7 to 2.8e-5 over 40-120 solar masses) quoted in the abstract are evaluated with the released model against its own training simulations; the strict leave-one-out numbers are unweighted mode-space mismatches. The two are quoted adjacently and are easy to conflate.
- The action-angle conceptual apparatus does not cover the part that limits the model. The merger-ringdown arm, whose leave-one-out mismatch (1.2e-5 all-mode) is an order of magnitude above the inspiral arm, is explicitly time-parameterised and attached, i.e. handled outside the advertised framework.
- Much of the Hamilton-Jacobi framing reduces in practice to demodulating by the (2,2) phase and using orbital phase as the abscissa, which is a conditioning choice rather than a canonical transformation of the two-body dynamics; J_phi and E are flux integrals with a 4PN integration constant, not computed actions. The physics packaging is grander than the mechanism, even though the mechanism works.
- Novelty on uncertainty is overstated (see novelty_context): Sec. 2 asserts that among surrogates only surfinBH emits a per-evaluation uncertainty, which is not true of Doctor et al. 2017 or Williams et al. 2020, both cited elsewhere in the paper.
- The argument against JaxNRSur's automatic differentiation is weak. Autodiff of a deterministic differentiable pipeline is exact to machine precision, and implicit differentiation through root finds is standard in the JAX ecosystem; 'not guaranteed to yield gradients that are accurate, well-behaved, and physical' is asserted, not demonstrated against JaxNRSur.
- Only the evaluation code is released; the training code is not. Every central claim (LOO retraining, calibration of the GP envelope, the exchange-symmetric kernel construction) is therefore not independently reproducible, and this is a single-author paper with no external validation.
- Scope is narrow: aligned spin only, non-eccentric only, seven multipoles, and a native span of only about 18 orbits, so the minimum usable total mass at 20 Hz is 43-96 solar masses unless one accepts the PN extension arm.

## 🤔 Skeptic's Cross-Examination

Strip out the framing and ask what caused the 5x accuracy gain over NRHybSur3dq8. The candidate causes are (i) the phase-domain conditioning, (ii) the hp-adaptive spectral representation, (iii) the GP regression, and (iv) 260 modern simulations instead of about 100 older ones. The paper runs no ablation isolating any of these, and (iv) alone could plausibly account for most of the difference. A cheaper experiment settles it: retrain the same machinery on the NRHybSur3dq8 training set, or retrain an NRHybSur-style empirical-interpolation surrogate on these 260 simulations. Neither is done, so the strongest claim actually supported is 'a new, carefully built, well-validated surrogate trained on more data is more accurate', not 'the action-angle parameterization is what buys the accuracy'.

## 🆕 Novelty in Context

Two of the three advertised capabilities have closer precedent than the paper's Table I admits. Doctor, Farr, Holz and Puerrer (arXiv:1706.05408) built a GPR waveform model that produces 'interpolated waveforms along with uncertainties across the parameter space' and used exactly those errors in a greedy algorithm to decide where to place the next simulation, which is the same idea the present paper offers as an extension in Sec. 13 without attributing it there. Williams, Heng, Gair, Clark and Khamesra (arXiv:1903.09204) built a GPR NR surrogate that 'returns not just a single interpolated value for the waveform at a new point, but a full posterior probability distribution'. Both are cited in this paper's introduction as examples of GPR regression, yet Sec. 2 still states that among surrogates only surfinBH emits a per-evaluation uncertainty. The defensible, smaller claim is that this is the first production-accuracy NR surrogate whose GP uncertainty is explicitly calibrated against leave-one-out realisations, propagated through the full reconstruction, and exposed alongside analytic derivatives. On differentiability the positioning is fair: JaxNRSur and the recent neural-network emulators (Puerrer et al. arXiv:2607.24960, Modrekiladze arXiv:2608.09978, Gramaxo Freitas et al. arXiv:2412.06946) are all cited and none pairs derivatives with an error envelope. The phase-domain conditioning and the exchange-symmetric kernel appear genuinely new for NR surrogates; the action-stitched hybridization is a real methodological advance over the MacDonald-style waveform splice used in NRHybSur3dq8.

## 🎯 Relevance to Your Research

This is a data-analysis and waveform-modelling paper, but its spine is dynamics language a self-force or EMRI person owns: action-angle variables, adiabatic invariance, the Delaunay Hamiltonian, and the first law of binary mechanics used as a live numerical test. The genuinely interesting object for that reader is the flux-integrated azimuthal action J_phi(Phi) and energy E(Phi) extracted from comparable-mass NR simulations and fitted across parameter space, with the first-law residual measured at 8 parts per million on NR data and 1.4e-4 at regression-predicted points. That is an NR-measured circular-orbit Delaunay-like Hamiltonian function, directly comparable to the Le Tiec / Fujita first-law and self-force literature, and it is released. The merger-ringdown handling and the Kokkos/performance material are skippable.

📖 **Where to start:** Sec. 4.1-4.2 for the action-angle conditioning and what J_phi, E and the clock actually are; Sec. 6 for the action-native hybridization and the first-law residual used as an acceptance test (the most physically substantive part); Sec. 9.2 for the leave-one-out numbers and the honest per-mode floors; Sec. 2 and Table I for the self-positioning, read against the caveats above. Sec. 7 (performance) and Sec. 5 (numerical construction) can be skimmed.

## Scores

- 🔬 **Quality:** 7.5/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- The 5x accuracy advantage over NRHybSur3dq8 is not controlled for training-set size: 260 modern SXS simulations here against roughly 100 older ones there, and no ablation separates representation from data.
- The PSD-weighted, sky-averaged mismatches quoted in the abstract are in-sample; the strict leave-one-out numbers are unweighted mode-space mismatches. Do not read the two as the same measurement.
- The native NR span is only about 18 orbits (minimum total mass 43-96 solar masses at 20 Hz). Below that the waveform is a 4PN extension, accumulating up to 1.4 radians of dephasing over 46-129 added orbits; the quoted accuracy does not apply there.
- The claim that only surfinBH among surrogates exposes a per-evaluation uncertainty is inaccurate: Doctor et al. 2017 and Williams et al. 2020 both do, and the former also pioneered using that uncertainty to place the next simulation.
- Aligned spin, no eccentricity, seven multipoles, single author, evaluation code released but training code not.

---

🔗 [Back to the weekly digest](../2026-09-15)
