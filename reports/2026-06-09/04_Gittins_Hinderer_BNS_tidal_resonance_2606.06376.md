# 〰️ Gittins, Narola, Wouters, Pang, Hinderer, Van Den Broeck — Detecting Tidal Resonances in Binary Neutron Stars

**arXiv:** [2606.06376](https://arxiv.org/abs/2606.06376)
**Categories:** gr-qc astro-ph.HE
**Length:** 6 pages, 3 figures
**Recommendation:** Should-Read · **Quality:** 7/10

## Summary

First fully Bayesian study (Bilby/dynesty on simulated ET data with IMRPhenomXAS_NRTidalv3 baseline) of whether resonantly excited oscillation modes are detectable in BNS GW signals. The headline numbers: ~32% detection efficiency among the 200 loudest events per year, and a minimum detectable phase shift ΔΦ ≈ 0.03 for favourable events — a vast improvement on the Balachandran–Flanagan (2007) Fisher threshold of ΔΦ ~ 2.

## Key Results

- "First fully Bayesian study of the capability of the Einstein Telescope to detect tidal resonances."
- Sensitive to GW phase shifts as small as ΔΦ ≈ 0.03 for favourable events; detection probability P_det ≈ 0.32 across 200 loudest sources, ≈ 0.4 for ΔΦ_max ≈ 0.22.
- Neglecting resonances biases inferred tidal deformabilities: Λ̃ biased high once ΔΦ_max ≳ 0.2 — a clean systematics result.
- Proper hypothesis test: builds a no-resonance background distribution from 200 injections to calibrate a 5σ Bayes-factor threshold (ln B_th ≈ 1.73).
- Uses realistic astrophysical rate (Iorio+ 2023) and current EOS set (Koehn+ 2025 Set A); relative-binning likelihood validated against exact.

## Strengths

- Genuine Bayesian PE with nested sampling, not Fisher.
- Honest scope: single resonance per star, positive ΔΦ only, instantaneous-resonance approximation valid only for f ≲ 150 Hz (controlled by ε ≪ 1).
- Connects detectable ΔΦ to specific mode classes (composition g-modes, inertial/r-modes, interface modes).
- Concrete EOS-inference-bias quantification — useful systematic independent of the detection claim.

## Weaknesses

- Underlying resonance model is the standard ~1990s Lai/Reisenegger–Goldreich SPA jump (Eq. 5). The Bayesian framing is the genuine novelty; the waveform correction is decades old.
- Restriction to positive ΔΦ explicitly excludes the most interesting r-mode case (ΔΦ < 0) — odd, since r-modes are highlighted in the discussion.
- Single EOS in injection and recovery; no marginalisation over EOS uncertainty.
- ΔΦ and f_res are sampled as free parameters with broad priors — measures detectability of generic phase jumps, not asteroseismic mode identification.
- Single triangular ET, no CE network; "200 loudest in one year" is a thin tail.
- Realistic g-mode shifts (~0.08) sit below the EOS-bias threshold ΔΦ ≳ 0.2 — bias may not matter for near-future analyses.

## Relevance to Vojtěch

Moderate. The physics — transient resonance crossings producing instantaneous phase/action jumps in an adiabatically inspiralling system — is structurally identical to the transient resonances Vojtěch studies in EMRIs (single-mode SPA jump, ε ≪ 1 from τ_res/τ_rr). The Bayesian detectability methodology (Bayes-factor with background calibration, prior on jump amplitude/frequency) ports naturally to EMRI transient-resonance detection with LISA — a useful methodological template. Hinderer authorship reinforces the cross-pollination with the LISA EMRI community.

## Honest Assessment

The right kind of paper: a careful Bayesian benchmark replacing a 20-year-old Fisher estimate, with a well-controlled background distribution. Does not claim new resonance physics; the contribution is the rigorous detectability number (ΔΦ ≈ 0.03 favourable, ~32% of loud events) plus the EOS-bias demonstration. Methodology and threshold-calibration approach are directly transferable to EMRI transient-resonance detectability problems — that's the main reason to read it carefully.
