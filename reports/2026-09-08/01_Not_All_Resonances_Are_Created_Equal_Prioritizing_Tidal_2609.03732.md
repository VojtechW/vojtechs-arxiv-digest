# 💫 Not All Resonances Are Created Equal: Prioritizing Tidal Resonances in EMRIs

🌟 **Must-Read** · 🔬 Quality 6/10 · 🎯 Relevance 8/10

📎 **Citation:** Béatrice Bonga, Patrick Bourg, Bram ten Brink, H. A., Peters, *Not All Resonances Are Created Equal: Prioritizing Tidal Resonances in EMRIs*, arXiv:[2609.03732](https://arxiv.org/abs/2609.03732) [gr-qc], submitted 03 Sep 2026.

> 💡 A systematic survey of how a distant companion star or black hole shakes a small body spiralling into a giant black hole finds that, out of two dozen possible resonant kicks, only a handful are strong enough to matter for future space-based gravitational wave measurements.

## 🔍 Executive Summary

The paper maps out the transient resonances that a distant third body (a star or stellar-mass black hole) drives in an extreme-mass-ratio inspiral, in the regime of a weak, effectively frozen tidal field. Using symmetry and frequency-ordering arguments, the authors cut 405 candidate resonance triplets down to 24 physically admissible ones (12 prograde, 12 retrograde), then compute for each the location of the resonance surface in the semi-latus-rectum/eccentricity/inclination space, the resonance duration (using both the fifth-order post-Newtonian and the exact-Kerr flux modules of the FastEMRIWaveforms package), and the jumps in angular momentum and Carter constant. Combining jump size with duration into a phase-independent figure of merit, they rank the resonances: for prograde orbits (3,-1,-1) and (3,0,-2) dominate, with (3,-3,1) and the n=4 analogues roughly two orders of magnitude weaker, and everything else negligible; retrograde orbits mirror this with the sign of m flipped. All contour and jump data are released publicly with the stated aim of feeding them into the FastEMRIWaveforms code.

## 📣 Claimed Contribution

A systematic, parameter-space-wide survey of stationary tidal resonances for generic Kerr orbits: resonance contours in (p, e, x) for every low-order (n,k,m), the associated resonance durations, and the jump amplitudes in L_z and Q; a resulting practical ranking of which resonances matter for waveform modelling; an analytic transformation law giving the jump amplitudes for an arbitrary perturber sky location (stated in the appendix as the specific methodological novelty over earlier work); and a public data release intended for direct incorporation into the FastEMRIWaveforms framework.

## ✅ Strengths

- The enumeration is genuinely useful and analytically justified, not just numerical brute force: reflection symmetry (k+m even), the (n,k,m) versus (jn,jk,jm) degeneracy, the ordering omega_theta <= omega_phi from Lense-Thirring precession, and the near-separatrix stalling of omega_r together reduce 405 combinations to 24, and they also explain the observed organisation of contours into n=3 and n=4 groups ordered by k.
- Several independent internal checks: Delta E is verified to be consistent with numerical zero (as required by time-translation invariance of the frozen tide), the two-for-one relation of Gupta, Kakehi and Tanaka is used as a cross-check whenever m is nonzero, and the m=0 angular-momentum jump (which must vanish by axisymmetry) is used as a numerical error yardstick.
- The duration calculation is checked against two different flux prescriptions (fifth-order post-Newtonian versus exact Kerr, restricted to equatorial orbits where the Kerr module applies), and the disagreements are located and discussed rather than hidden.
- The paper is explicitly and repeatedly honest that its ranking is a heuristic efficiency guide rather than a truncation criterion, because a weak resonance can still shift the entry phase of a later strong one, and because a large jump close to the separatrix affects only the last few orbits.
- Concrete, actionable implementation advice for waveform codes (adaptive stepping plus event detection/root finding on the resonance condition, careful ordering of multiple kicks where contours cross), plus a public dataset of contours and jumps.

## ⚠️ Weaknesses

- No observability metric anywhere. The ranking rests on the proxy (jump amplitude) x (resonance duration); the paper never converts this into radians of accumulated gravitational-wave phase, mismatch, or parameter bias. Earlier work by an overlapping author group (Gupta et al. 2021, 2022) did compute dephasings and Fisher-matrix biases, so on the axis a data analyst actually cares about this paper is a step sideways rather than forward.
- The stationary-perturber approximation is weakest exactly where the paper's own ranking says the action is. The authors state it is accurate for short-duration, strong-field resonances, but the duration-weighted figure of merit is largest for low spin, high eccentricity and large semi-latus rectum, i.e. the longest-lived resonances, where the perturber's orbital phase changes appreciably during the crossing. No quantitative validity criterion (e.g. perturber orbital frequency times resonance duration much less than one) is given anywhere.
- The Discussion concedes that a moving perturber introduces an extra harmonic index s and can produce two resonances per (n,k,m,s) instead of one; that is a qualitative change of structure, so the present ranking may not survive the very generalisation the authors say is in preparation.
- The largest duration-weighted jumps occur as eccentricity approaches one, i.e. at large apoapsis, which is precisely where the leading-order (Newtonian, quadrupole) tidal expansion in orbital radius over perturber distance degrades. For the parameters the authors quote elsewhere (perturber at about ten astronomical units, roughly 250 central-black-hole masses for a Sagittarius A* mass), an orbit at p ~ 20 and e ~ 0.9 has apoapsis comparable to the perturber separation. No estimate of the neglected higher-multipole or post-Newtonian tidal corrections is given.
- Inconsistent hybrid model: the tidal metric perturbation is computed in Schwarzschild perturbation theory in lightcone gauge while the geodesics and frequencies are Kerr. The validation of this choice is thin, being a comparison for a single resonance, (3,0,-2), against the Yunes-Gonzalez construction (itself carrying a known factor-of-two erratum and lacking m=0 modes), quoted at below 0.1 percent generically and about 1 percent at high eccentricity.
- No error bars on the jump data. Numerical accuracy is only characterised qualitatively via the spurious nonzero m=0 angular-momentum jumps, which the authors admit degrade with increasing eccentricity and spin, and which they knowingly leave plotted. The 'negligible' classification is defined as below one part in a thousand of the largest jump, uncomfortably close to their own demonstrated noise floor.
- Several central features are reported as not understood: why jumps vanish for circular orbits ('we do not have a rigorous explanation'), why they diverge as eccentricity approaches one (only 'a possible explanation'), the spin dependence at low x ('not yet understood'), and the post-Newtonian duration spike for (4,0,-2) at spin 0.9 ('could not pin down its precise cause'). For a survey paper this leaves the physics thin relative to the plot count.
- The ranking omits the two ingredients that would make it a real priority ordering: the probability that a given inspiral actually crosses each contour, and how much inspiral remains after the crossing. The authors flag the second issue themselves but do not fold it in. The angular-momentum and Carter-constant orderings also disagree with each other, and no combined figure of merit is offered.
- Presentation is unpolished: leftover commented-out text and a commented figure block in the source, a garbled author list in the arXiv metadata, and an introduction that never states plainly what is new relative to Gupta et al. 2021/2022 (the reader must reach the appendix to learn that the methodological novelty is one orientation-transformation formula).

## 🤔 Skeptic's Cross-Examination

The single sharpest objection is that the paper's ranking may be an artefact of the approximation it is built on. The frozen-perturber assumption is admitted to fail for long-duration resonances, and the figure of merit is linear in duration, so the resonances that come out on top are systematically those for which the assumption is least defensible. Add that the highest-eccentricity region, where the duration-weighted jumps grow fastest, is also where the leading-order tidal multipole expansion in orbital radius over perturber distance is most suspect, and the two effects driving the headline ordering are both concentrated in the corner of parameter space the model handles worst. The authors' own Discussion, noting that a moving perturber adds an index s and can double the number of resonances per label, effectively concedes that the companion paper in preparation could rewrite the ordering. A skeptic would want the validity condition written down and the ranking recomputed with the resonance-crossing probability and the remaining inspiral time folded in before treating the shortlist as a modelling prescription.

## 🆕 Novelty in Context

The framework (forced geodesics, action-angle two-timescale jump formula, quadrupolar frozen tide) is inherited wholesale from Bonga, Yang and Hughes 2019 and Gupta, Bonga, Chua and Tanaka 2021, and the paper says so. The claim of a 'systematic survey across EMRI parameter space' overlaps substantially with prior work by an author group sharing a member: Gupta et al. 2021 already advertised 'a first study of how common and important such resonances are over the entire orbital parameter space' (stationary perturber, but restricted to the equatorial plane) and supplied fitting formulae for the jumps, while Gupta, Speri, Bonga, Chua and Tanaka 2022 extended to 'a more generic model for the tidal perturber with additional resonance combinations', implemented resonant kicks as step functions in an inspiral, and quantified dephasing and Fisher biases. My own searches for tidal-resonance work in 2023-2026 turned up no competing survey, so this is the same subfield being continued by the same community rather than a scooped result, but the increment is narrower than the abstract implies. The genuinely new items are: the complete low-order enumeration with explicit selection rules (405 to 82 to 24), the analytic law for arbitrary perturber orientation lifting the equatorial restriction of the 2021 study, the m=0 modes made accessible by the lightcone-gauge Schwarzschild tidal field, the systematic duration calculation with a post-Newtonian versus exact-Kerr comparison, and the duration-weighted ranking plus public dataset. To the paper's credit, it makes no explicit 'we are the first' claim in the abstract, and the appendix states the novelty accurately.

## 🎯 Relevance to Your Research

Squarely in the reader's territory: transient resonances in Kerr, action-angle and two-timescale formulation, Kerr fundamental frequencies and their evolution, and the interface between orbital dynamics and practical waveform generation. Anyone who has worked on self-force or tidal resonances will find the frequency-ordering and selection-rule arguments in Section 3 immediately usable, and the observation that only k+m even survives and that n=1 resonances are pinned to the separatrix is the kind of structural statement that generalises. The public dataset is directly reusable. It is also a useful reference point for anyone thinking about a Hamiltonian or canonical-perturbation treatment of the same problem, since the paper's unexplained features (vanishing jumps for circular orbits, divergence at high eccentricity) look like they have clean analytic explanations that this paper does not supply.

📖 **Where to start:** Section 3 up to Table I for the selection rules and the reduction from 405 to 24 resonances, and the contour-ordering argument in the prograde subsection; Section 4 for the resonance durations and the post-Newtonian versus exact-Kerr comparison; Section 5 for the duration-weighted jumps and the resulting rankings for angular momentum and Carter constant (including the two-for-one argument explaining why the (3,0,-2) angular-momentum jump does not vanish in the equatorial limit); Section 6 for the honest caveats and the sketch of what changes once the perturber is allowed to move. Appendix A is worth skimming for the orientation-transformation formula, which is the paper's stated methodological novelty.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 8/10
- 🌟 **Reading priority:** Must-Read (weighted score 7/10)

## 🚧 Caveats

- The importance ranking is built on the proxy (jump size) x (resonance duration); the paper never converts it into gravitational-wave dephasing, mismatch or parameter bias, unlike the earlier papers by an overlapping author group.
- The perturber is frozen during the resonance crossing. That assumption is weakest for the long-lived, low-spin, large-separation resonances that the ranking places at the top, and no quantitative validity condition is given.
- The largest jumps occur as eccentricity approaches one, where the leading-order quadrupolar tidal expansion in orbital radius over perturber distance is least reliable; no estimate of the neglected corrections is provided.
- The tidal field is computed in Schwarzschild while the orbits are Kerr; this hybrid is validated for only one resonance, at about 0.1 percent generically and about 1 percent at high eccentricity.
- Jump amplitudes come with no error bars; the 'negligible' cutoff of one part in a thousand sits close to the paper's own demonstrated numerical noise floor at high spin and high eccentricity.
- Several key trends (vanishing jumps for circular orbits, divergence at high eccentricity, spin dependence at high inclination) are reported as unexplained.
- Methodologically this continues Bonga-Yang-Hughes 2019 and Gupta et al. 2021/2022; the genuine increments are the complete low-order enumeration, the arbitrary perturber orientation law, the duration study and the public dataset.

## In Network

- 🚩 Beatrice Bonga — extended-network collaborator
- 🚩 Patrick Bourg — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-09-08)
