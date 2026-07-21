# 🎯 High-order gravitational late-time tails in Kerr spacetime

**arXiv:** [2607.12151](https://arxiv.org/abs/2607.12151)
**Authors:** Marc Casals, Chris Kavanagh, Jakob Neef, Adrian Ottewill
**Category:** gr-qc (+ hep-th)
**Submitted:** 2026-07-13

## TL;DR
Third-order (leading + two sub-leading) late-time tails of the retarded Teukolsky Green function on subextremal Kerr for gravitational perturbations (s=−2), at fixed spheroidal (ℓ,m), obtained at finite radius (Boyer-Lindquist t), on H⁺ (Eddington-Finkelstein v), and on I⁺ (u). Log-in-time corrections appear at NLO on I⁺ and at NNLO in the other two cases, with an additional ln² u term on I⁺. Small-frequency (MST) expansions of every scattering-theory building block are provided as ancillary Mathematica notebooks, and analytic tails are validated against numerical Fourier IFT at r = r′ = 10 M and 3 M for a = 0.9 M.

## Summary
The paper closes a well-defined gap: prior Kerr-tail literature (Hod 1999; Barack 1999; Barack & Ori 1999) delivered only *leading-order* tails, and only for spherical (not spheroidal) modes with r, r′ ≫ M; Casals & Ottewill (2015) had done high-order Schwarzschild tails; Casals, Kavanagh & Ottewill (2016) had done high-order scalar Kerr tails. Here the same MST-based small-frequency / branch-cut-on-NIA machinery is pushed to the physical case of gravitational perturbations, at generic r ∈ (r₊, ∞), for arbitrary integer ℓ, m. Full-Green-function decay powers are inferred for generic integer spin s and coefficients are tabulated for s = −2. Two ancillary notebooks are shipped: one with generic-ℓ expressions for BC strength Q, scattering amplitudes B^{inc/ref/tra}, BC modes δ𝒢_{ℓm} and the radial in-solution to low PN; the other allowing arbitrary-order computation for specific ℓ (feasible to ~15 PN, with 8 PN sufficient down to r = 3 M).

## Strengths
- Concrete new analytic result: gravitational (s=−2) tails in Kerr at NNLO, in three physically distinct asymptotic regions, including all log-in-time and ln²-in-time corrections.
- Technique transferability is explicit: the small-frequency scattering-quantity expansions "are useful, not only for the late-time tail, but for other problems as well… tidal deformability and Love numbers of Kerr black holes … analytic weak-field self-force calculations describing small mass-ratio binaries," and even for interior/Cauchy-horizon problems (Alberti et al. 2026).
- Ancillary Mathematica notebooks integrate with the Black Hole Perturbation Toolkit — reusable infrastructure, not one-shot output.
- Numerical validation: real-frequency IFT compared against analytic series with successive-subtraction residual test; 8 PN with 17 terms reaches noise floor at r = 3 M.
- Reduces cleanly to Casals & Ottewill (2015) Schwarzschild limit.
- Clean, precise scholarly writing (Casals/Ottewill house style).

## Weaknesses
- The extension from scalar (2016) to gravitational (2026) is technically substantial but methodologically incremental — the machinery is inherited from Casals-Kavanagh-Ottewill 2016 and Casals-Ottewill 2015.
- Restricted to *linear* Teukolsky perturbations; no nonlinear/second-order tail structure (topical elsewhere).
- Restricted to subextremal Kerr; extremal Kerr tails (Casals-Gralla-Zimmerman lineage) not covered.
- The result is at *fixed* (ℓ, m); reconstructing the full metric perturbation tail needs one more step of mode summation (which is what the "full retarded GF" claim in the abstract effectively does for the decay powers, but coefficient-wise it's mode-by-mode).

## Novelty Cross-Check
Self-assessment (verbatim): *"Even though Casals et al. (2016b) carried out the explicit expansions in the scalar case only, it also laid out the whole high-order tail formalism … for the Teukolsky equation for generic integer field spin s. In this paper, we use this formalism in order to derive late-time asymptotics up to third leading order of the gravitational GF for Teukolsky spin s=−2 for fixed, arbitrary ℓ and m in all three cases."* And from the conclusions: *"The main novel result … is showing that logarithmic-in-time terms first appear at next-to-leading order in case (c) [I⁺] and at next-to-next-to-leading order in cases (a) and (b). In case (c), at next-to-next-to-leading order a quadratic logarithmic term also appears."*

Cross-checked against Casals & Ottewill 2015 (1509.04702, high-order Schwarzschild), Casals-Kavanagh-Ottewill 2016 (1608.05392, high-order Kerr scalar), and Hod 1999 (leading Kerr). The gravitational-spin, spheroidal-mode, arbitrary-radius extension is the actual delta and is genuinely new.

## Relevance to Witzany
High direct hit. This is Teukolsky-adjacent BH perturbation theory in exactly the analytic small-frequency / branch-cut sector that overlaps self-force, quasinormal-mode completeness, and EMRI-waveform late-time behaviour. The MST small-frequency expansions and the ancillary BHPT-integrated notebooks are precisely the sort of reusable analytic infrastructure Witzany's group would want to import into self-force or waveform-tail investigations. The paper's own transferability list names "analytic weak-field self-force calculations describing small mass-ratio binaries" — direct EMRI relevance. Kavanagh is a Tier-2 collaborator, which further motivates keeping close attention. Should be read carefully, in particular §VI–VII and the notebook contents.

## Quality Score
- Overall: 8.5/10
- Direct relevance: 8/10
- Novelty: 7/10
- Technical rigor: 9/10

**Tier:** Must-Read

**Collaborator flags:** Tier 2 (Chris Kavanagh). Casals & Ottewill are long-standing BH perturbation theorists in the wider self-force / QNM community.
