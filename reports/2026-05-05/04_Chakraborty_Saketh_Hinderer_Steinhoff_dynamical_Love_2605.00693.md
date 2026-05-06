# 🌊 Dynamical tidal Love numbers of black holes under generic perturbations

**Authors:** Sumanta Chakraborty, M.V.S Saketh, Tanja Hinderer, Jan Steinhoff  
**arXiv:** [2605.00693](https://arxiv.org/abs/2605.00693) [gr-qc]  
**Date:** May 2026  
**Categories:** gr-qc

---

## Summary

The paper builds an explicit bridge between black-hole perturbation theory (BHPT) on the Kerr background and an effective worldline action with frequency-dependent (i.e. dynamical) tidal response. To linear order in the perturbing frequency ω, they extract the *non-static* parts of the tidal response of a spinning black hole to scalar and gravitational perturbations, dealing carefully with multipole mixing induced by the rotation. The take-home message: while *static* Love numbers vanish for Schwarzschild and Kerr (Charalambous, Dubovsky, Ivanov; Hui et al.), *dynamical* O(ω) Love coefficients are non-zero and non-trivial — and the EFT/BHPT match makes those coefficients explicit and useable in PN/EOB models.

## Strengths

- **EFT–BHPT bridge.** The paper is one of the more careful efforts at this matching since Saketh-Hinderer-Steinhoff (2210.…). It treats both dissipative and conservative pieces transparently.
- **Multipole-mode mixing handled, not avoided.** Rotation mixes ℓ-multipoles in the response, which previous static-Love-vanishing arguments side-stepped. Doing this honestly at O(ω) is the technically interesting work.
- **Strong author lineup.** Hinderer (Tier 3) and Steinhoff (Tier 2) are sophisticated EFT practitioners; their imprimatur is real.
- **Direct usability.** The Wilson coefficients can be plugged into TEOB / SEOB-type models for tidal heating / dissipation.

## Weaknesses

- **Matching scheme dependence not exhausted.** Worldline-EFT matching at O(ω) has known scheme/gauge ambiguities — these need to be cleanly separated from physical predictions. The paper makes some claims here, but a fully transparent scheme-independence statement is lacking.
- **No numerical cross-validation.** A direct numerical Teukolsky comparison (e.g. via BHPToolkit or pybhpt) at intermediate ω would solidify the claims. This is not yet shown.
- **Power-counting at higher ω is implicit.** The reader cannot directly read off the regime of validity (in dimensionless ωM) from the paper.
- **Conservation/time-reversal argument for separating dissipative vs conservative parts is somewhat opaque.**

## Relevance to Vojtěch

**Strong.** Dynamical tidal response of BHs feeds directly into EMRI waveform precision, comparable-mass tidal heating in EOB, and PN-Kerr matching of compact-body multipoles. This is the kind of paper whose results Skoupý / Piovano / Tanay-style work needs as input.

## Quality / Verdict

- **Quality:** 7.5/10
- **Relevance:** 8.5/10
- **Survives critical review:** **Yes, provisionally** — pending an independent numerical Teukolsky check of the linear-ω response against the EFT prediction at moderate orbital frequencies. The framework looks solid; the cross-validation is the natural follow-up.
