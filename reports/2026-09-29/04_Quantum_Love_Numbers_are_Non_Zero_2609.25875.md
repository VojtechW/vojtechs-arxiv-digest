# 🕳️ Quantum Love Numbers are Non-Zero

🌠 **Should-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 4.5/10

📎 **Citation:** Asaad Elkhidir, Godwin Martin, Julio Parra-Martinez, M. V. S. Saketh, *Quantum Love Numbers are Non-Zero*, arXiv:[2609.25875](https://arxiv.org/abs/2609.25875) [hep-th, gr-qc], submitted 22 Sep 2026.

> 💡 A one-loop quantum-gravity calculation shows that the tidal deformability of a non-rotating black hole, which is exactly zero in classical general relativity, cannot stay zero once quantum effects are included, because it changes logarithmically with the length scale at which it is probed, by an amount set by the square of the Planck length divided by the square of the horizon radius.

## 🔍 Executive Summary

The authors work in worldline effective field theory and compute the one-loop quantum correction, at linear order in the black-hole mass, to the scattering of massless scalars and photons off a Schwarzschild worldline. After subtracting infrared poles, which they cross-check against an independent soft-graviton emission calculation, the leftover ultraviolet poles have exactly the structure of the leading tidal operators and cannot be absorbed by any lower-order counterterm. This gives nonzero, tidal-coupling-independent beta functions for the scalar static dipole Love number (-1/(40 pi) l_pl^2/r_h^2), the scalar dynamical monopole coefficient (3/(2 pi) l_pl^2/r_h^2), and the electric and magnetic photon Love numbers (equal, 39/(40 pi) l_pl^2/r_h^2, as electric-magnetic duality requires). They recover the scalar beta functions from the soft-region expansion of one-loop massless-massive scalar scattering, and show that naively taking the heavy-mass limit of the fully integrated relativistic amplitude gives different, wrong numbers because of hard-region contributions. The gravitational quadrupole case is not computed; it is only estimated by power counting.

## 📣 Claimed Contribution

The authors say this is the first demonstration that the classical vanishing of Schwarzschild static Love numbers does not survive quantization. Graviton loops produce an inhomogeneous renormalization-group flow for the scalar and electromagnetic Love numbers, so 'zero' cannot hold at more than one scale. This fits the view that the classical vanishing comes from an accidental symmetry of static general relativity that quantum loops break. By extrapolation, they claim gravitational quadrupole Love numbers of size lambda ~ M r_h^2 l_pl^2.

## ✅ Strengths

- A concrete, explicit one-loop calculation, not an argument. It gives closed-form ultraviolet residues and beta functions for four tidal couplings (scalar static dipole, scalar dynamical monopole, photon electric and magnetic).
- Two independent internal checks. The infrared logarithm matches a separate soft-emission calculation, and the worldline beta functions are recovered from the soft-region expansion of a full relativistic massive-scalar amplitude.
- The explanation of why the naive heavy-mass limit of the integrated relativistic amplitude gives different beta functions (hard-region loop momenta of order M, and closed massive loops) is a useful methodological point for anyone matching amplitudes to worldline theories.
- The authors carefully rule out absorption into lower-order counterterms (graviton and scalar self-energies, the vertex, the worldline mass). This is what makes the running a statement about the Love numbers specifically.
- The equal electric and magnetic photon beta functions act as a built-in duality consistency check.
- Compact, clearly written, and honest in the Discussion that finite values need a one-loop matching calculation in the black-hole background, which is not done.

## ⚠️ Weaknesses

- The title and abstract overstate the result. The paper computes running (logarithms), not a finite Love number at any scale. 'Non-zero' means only that a zero value is not scale-invariant. The actual value at a reference scale is explicitly left for future work.
- The headline gravitational claim, lambda ~ M r_h^2 l_pl^2 for the quadrupolar Love number, is pure dimensional analysis plus a count of loops (Section 3.3). No diagram is computed, and it is not shown that the relevant logarithm has a nonzero coefficient. Yet it appears in the abstract.
- At first post-Minkowskian order the 'Schwarzschild black hole' is just a point mass on a worldline. Nothing in the calculation is specific to black holes or to the classical ladder or accidental symmetry. The same beta functions hold for any compact object, including a neutron star or a planet. The claim that this is 'consistent with' an accidental symmetry being broken by loops is an interpretation, not something the computation tests.
- The physical effect is suppressed by (l_pl/r_h)^2, about 10^-76 for a solar-mass black hole. It has no observational consequence for gravitational waves and is purely a matter of principle.
- The one-loop amplitudes for massless particles scattering off a massive scalar at this order were already computed by Bjerrum-Bohr, Donoghue, Holstein, Plante and Vanhove (2014-2016). The new step is interpreting the local ultraviolet counterterms as worldline Love-number running and separating soft from hard regions. That is smaller than a new calculation from scratch.
- What sets the scale mu in the static limit, and how the running tidal coefficient would show up in an observable (logarithms of frequency or momentum transfer in the Compton amplitude), is only sketched.

## 🤔 Skeptic's Cross-Examination

You computed ultraviolet logarithms of a point mass coupled to quantum gravity and relabelled the counterterms 'Love numbers'. Any massive body gets the same running at this order, so this says nothing about black holes or about breaking their special symmetry. It is the expected statement that a coupling set to zero is not protected once loops break the symmetry, confirmed for spin 0 and 1. The gravitational claim that would actually matter, and the finite value, are both absent. The paper survives because the calculation is explicit and cross-checked, and the question has been open since 2016, but it should be read as 'quantum running of scalar and photon tidal couplings of a point mass' rather than 'Schwarzschild has quantum Love numbers of a known size'.

## 🆕 Novelty in Context

The paper places itself as answering an open question raised by Porto (1606.08895, 'The Tune of Love'), namely whether vanishing Love numbers are a naturalness puzzle, and by Parra-Martinez and Podo (2510.20694). The latter proved classical vanishing and non-renormalization of static Love numbers to all nonlinear orders from a symmetry realised both in full general relativity and in the worldline theory. The present paper, sharing an author, shows that quantum graviton loops at finite frequency get around that non-renormalization. My InspireHEP and ADS searches found no earlier explicit calculation of quantum running of black-hole Love numbers, so the 'first' claim for the scalar and photon running looks sound. The underlying one-loop amplitudes, however, are close to the massless-on-massive scattering amplitudes of Bjerrum-Bohr, Donoghue, Holstein, Plante and Vanhove (1609.07477 and earlier), which focused on the non-analytic long-range terms. The paper cites them in Section 4. The real contribution is therefore a worldline-theory reinterpretation and a careful soft-region extraction of the local ultraviolet poles as Love-number beta functions. That is a clean and useful but modest step. The gravitational statement in the title and abstract goes beyond what is computed.

## 🎯 Relevance to Your Research

This is a conceptual result about black-hole tidal response, not something usable for EMRI modelling, self-force or waveforms. It matters to anyone who cites 'black-hole Love numbers vanish' as a sharp, protected statement, or who follows the hidden-symmetry and ladder-symmetry literature (Charalambous-Dubovsky-Ivanov, Hui et al., Parra-Martinez and Podo). It shows the protection is classical only. For a reader working on black-hole perturbation theory and integrability, the useful parts are the scalar calculation and the counterterm-exclusion argument (Section 3.1.2), the gravitational power counting (Section 3.3, to see how weak the extrapolation is), and Section 4 on soft versus hard regions if you ever match amplitudes to a worldline.

📖 **Where to start:** Introduction (1 page) for the positioning; Section 3.1.2 for the scalar ultraviolet residue, the counterterm exclusion and the beta functions; Section 3.2.1 for the photon result; Section 3.3 to judge how thin the gravitational extrapolation is; the end of Section 4 for the soft-region versus naive heavy-mass comparison. The appendices on master integrals are only for anyone reproducing the calculation.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 4.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.8/10)

## 🚧 Caveats

- Only the running (logarithms) is computed; the finite quantum Love number is left for future work.
- The gravitational quadrupole estimate in the abstract comes from dimensional analysis, not a calculation.
- At this order the source is a point mass, so nothing in the calculation is specific to black holes.
- The effect is suppressed by (Planck length / horizon radius)^2, about 10^-76 for a solar-mass black hole; it is of conceptual interest only.

## In Network

- 🚩 Julio Parra-Martinez — notable author

---

🔗 [Back to the weekly digest](../2026-09-29)
