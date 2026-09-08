# ♻️ Charged black-hole binary radiation at second post-Newtonian order

🔦 **Worth-Skimming** · 🔬 Quality 6.5/10 · 🎯 Relevance 4/10

📎 **Citation:** Andrea Placidi, Elisa Grilli, Matteo Pegorin, Marta Orselli, *Charged black-hole binary radiation at second post-Newtonian order*, arXiv:[2609.02825](https://arxiv.org/abs/2609.02825) [gr-qc], submitted 02 Sep 2026.

> 💡 For two black holes that carry electric charge and spiral together on nearly circular orbits, this paper works out the emitted gravitational and electromagnetic waves to a substantially higher order of accuracy than before, and finds that like-sign charges weaken the gravitational-wave power while opposite-sign charges strengthen it.

## 🔍 Executive Summary

Building on the same group's earlier derivation of the conservative two-body dynamics of an electrically charged, non-spinning binary at second post-Newtonian (2PN) order, this paper completes the radiation sector: the electric and magnetic source and radiative multipole moments of the vector field, the charge-dependent corrections to the gravitational mass- and current-type moments, the spin-weighted spherical-harmonic waveform modes, and the total energy flux for quasi-circular inspirals. The calculation is done twice for the instantaneous pieces, once by extending the matched multipolar post-Minkowskian post-Newtonian formalism to Einstein-Maxwell theory and once in an effective field theory formulation with background-field gauge fixing, with agreement between the two. New ingredients beyond a straightforward charge decoration of known results include the leading tail of the radiative electric dipole, Coulomb-radiative nonlinearities involving the total charge, and an oscillatory nonlinear memory in the gravitational radiative moments sourced by the stress-energy of the electromagnetic radiation (it appears in the dominant waveform mode at relative 1.5PN as a purely imaginary, i.e. phase-shifting, term and drops out of the flux at this order). Numerically, the tensor flux is suppressed relative to the neutral case for same-sign (repulsive) charges and enhanced for opposite-sign (attractive) charges, with the effect only becoming visible for charge-to-mass ratios of order a few tenths or larger.

## 📣 Claimed Contribution

Extension of both the matched multipolar post-Minkowskian post-Newtonian formalism and the effective field theory approach to the radiation sector of charged binaries in Einstein-Maxwell theory; derivation of the 2PN radiative electric/magnetic and mass/current multipole moments, the 2PN charge-dependent spherical waveform modes, and the 2PN total energy flux for quasi-circular orbits, including a new memory contribution sourced by the electromagnetic radiation stress-energy tensor, with the instantaneous sector verified independently in two formalisms.

## ✅ Strengths

- Genuine new calculation, not a repackaging: the 2PN radiation sector for charged binaries did not exist; prior charged/Einstein-Maxwell-dilaton radiation results (Julie 2018) stop at 1PN, and the 2PN work available before this series (Gupta, PRD 112, 104047) was conservative dynamics only.
- Two independent derivations of the instantaneous sector (matched multipolar post-Minkowskian post-Newtonian versus effective field theory, the latter with background-covariant gauge fixing and an explicit Ward-identity check) agree exactly, which is a meaningful internal control on a long algebraic computation.
- Non-trivial limit checks that actually work: setting the charges to zero recovers the standard neutral 2PN flux and the standard neutral (2,2) mode coefficients including the tail term, and the 1PN charged limit reproduces Julie's result.
- The nonlinear-propagation bookkeeping is done carefully rather than assumed away: the electric-dipole tail, the Coulomb-radiative monopole-times-radiative-multipole terms and the oscillatory electromagnetic memory are separated and their instantaneous completions retained.
- Honest positioning: no 'first ever' language, prior 2PN conservative work and charged-binary numerical relativity are cited, and the paper explicitly states what it does not do (eccentricity, zero-frequency memory).
- Full expressions supplied in machine-readable Supplementary Material, which matters for anyone who wants to use rather than admire the result.

## ⚠️ Weaknesses

- Methodologically this is well-established machinery applied to a system with one extra U(1) field. Nothing in the technique is new; the difficulty is bookkeeping, and the conceptual payoff is limited.
- The independent cross-check is narrower than the headline suggests: the effective field theory reproduces only the instantaneous vector flux and the tensor flux at next-to-leading order. The next-to-next-to-leading-order instantaneous tensor sector and every hereditary term (tails, memory) are computed once, in one formalism, by one group.
- The waveform is not uniformly 2PN-complete: the zero-frequency (direct-current) memory is omitted, and the paper itself concedes these terms accumulate secularly over the radiation-reaction timescale and can contribute at leading order, so the m = 0 sector is not delivered.
- The argument that the new oscillatory memory does not contribute to the flux at this order is given verbally ('orthogonal in the STF contractions, or quadratic in the memory amplitude') rather than demonstrated; it is plausible and consistent with the imaginary form of the (2,2) memory term, but it is asserted.
- Numerical section is thin relative to the abstract's promise about 'assessing observational signatures': three figures at chosen charge values, no parameter-estimation, Fisher, or measurability estimate, and no comparison against the existing charged-binary numerical-relativity waveforms (Bozzola and Paschalidis) that the paper cites in the introduction.
- The total post-Newtonian flux series goes negative within the plotted range and is rescued by an ad hoc diagonal Pade resummation in sqrt(x) with no error control or independent validation; the choice is asserted to be 'more robust' rather than shown to be.
- Editorial sloppiness in v1: the instantaneous tensor flux equation and its introductory sentence are duplicated verbatim, with the same equation label used twice, in Sec. VI B. Minor, but it indicates the manuscript was not read through carefully.
- The physical regime where the charge corrections are visible in the figures (charge-to-mass ratio 0.8, and one body at extremality) is astrophysically excluded for genuine electric charge and speculative even as a dark-sector proxy; for the small charges that are actually observationally allowed, 2PN charge corrections are far below the leading dipole term that already sets the constraint.

## 🤔 Skeptic's Cross-Examination

Strip away the algebra and ask what changed. The answer is a set of higher-order coefficients in a regime nobody can currently probe: the observationally allowed charge-to-mass ratios are small enough that the leading dipole flux, known since the 1980s, dominates any constraint, while the 2PN charge corrections computed here only become numerically visible at charge-to-mass ratios near unity, which is precisely where the post-Newtonian expansion is also being asked to work hardest and where the paper's own untruncated series goes negative and has to be Pade-resummed by hand. The paper's response would be that this is groundwork for a dark-U(1) or beyond-general-relativity waveform model, which is fair, but the paper does not take the step that would test that claim: no phasing, no waveform model, no injection study, and no comparison to the charged-binary numerical-relativity waveforms it cites. A second, sharper objection: the 'independent confirmation' framing is doing more work than the checks support, since the effective field theory calculation covers only part of the result and both calculations come from the same group starting from the same action.

## 🆕 Novelty in Context

The novelty claim survives the check, at its stated (modest) size. Julie's 2018 Einstein-Maxwell-dilaton radiation work stops at 1PN and is exactly what this paper reproduces as a limit. Gupta (arXiv:2205.11591, PRD 112, 104047, 2025) obtained the 2PN conservative Einstein-Maxwell dynamics by effective field theory, but conservative only, and it is cited here. A targeted search turned up no prior 2PN radiation-sector or waveform-mode results for charged binaries; the closest structural analogue is the scalar-tensor programme (dipolar tails and dipolar memory, Bernard et al.), which the paper explicitly names as the analogue for its new electromagnetic memory term rather than claiming that idea as its own. Notably the paper contains no 'first time' or 'we are the first' language anywhere, and it cites the charged-binary numerical-relativity literature it does not compare to. So the real contribution is: known wave-generation machinery, honestly extended to Einstein-Maxwell, pushed from 1PN to 2PN, with one structurally new piece (electromagnetic-radiation-sourced memory in the gravitational radiative moments). That is worth having and is correctly advertised; it is not a conceptual advance.

## 🎯 Relevance to Your Research

Adjacent rather than central for a reader working on extreme-mass-ratio inspirals, self-force and black-hole perturbation theory. The overlap is in the wave-generation formalism itself: this is a clean worked example of extending matched multipolar post-Minkowskian post-Newtonian wave generation to a system with an additional long-range vector field, including how the extra field's radiation stress-energy feeds back into the gravitational radiative moments as memory. That structure recurs in scalar-tensor and dark-sector settings and is the transferable part. If the interest is in constraining black-hole charge or hidden-U(1) couplings with gravitational-wave data, this supplies the high-accuracy circular-orbit flux and modes needed to build the model. Read Sec. IV C for the electromagnetic memory construction, Sec. VI for the flux and its charge dependence, and Sec. II D for the effective field theory cross-check setup; the multipole-moment sections are reference material best consulted through the Supplementary Material.

📖 **Where to start:** Sec. I (positioning against Julie 2018 and the companion 2PN dynamics paper); Sec. II D (effective field theory setup and the harmonic-gauge contact transformation, Eq. for r_H vs r_EFT); Sec. IV C (the new electromagnetic-sourced memory in the radiative moments, and the statement of what the direct-current memory omission costs); Sec. V (the explicit (2,2) mode, where the neutral-limit checks are easiest to verify by eye); Sec. VI B-C (flux, cross-checks, and the charge-dependence figures plus the Pade discussion).

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 4/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4.0/10)

## 🚧 Caveats

- Second paper of a series: the 2PN conservative dynamics it stands on is the companion paper (arXiv:2509.20432, PRD 112, 124060), which has a published erratum. Check which version of the dynamics you are comparing against.
- Circular orbits only, non-spinning only. Eccentricity is left to future work.
- The zero-frequency (direct-current) memory is not included, so the waveform is not fully 2PN-complete in the m = 0 sector; the authors say so.
- The two-formalism agreement covers only the instantaneous vector flux and the next-to-leading-order tensor flux. The hereditary sector and the highest-order instantaneous tensor terms rest on a single calculation.
- The illustrative plots use charge-to-mass ratios of 0.8 and 1. Those values are not astrophysically realistic for electric charge; treat them as a dark-U(1) or parametrized-deviation proxy.
- No observability or parameter-estimation analysis, and no comparison with the existing charged-binary numerical-relativity simulations.

---

🔗 [Back to the weekly digest](../2026-09-08)
