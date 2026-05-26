# 💫 Gravitational Wave Hyperbolic Catalog: Reanalyzing High-Mass Gravitational Wave Signals Using Hyperbolic Waveforms

**arxiv:** [2605.21640](https://arxiv.org/abs/2605.21640)
**Authors:** Jacob Lange, Danilo Chiaramello, Peter Lott, Chad Henshaw, Alessandro Nagar, Richard O'Shaughnessy, Laura Cadonati
**Categories:** gr-qc

## TL;DR
🎯 First systematic LVK-catalog reanalysis with a hyperbolic-encounter EOB waveform: 38 pair-instability-mass-gap events run through `TEOBResumS-Dalí` in its unbound configuration vs. the quasi-circular precessing (QC-prec) configuration. **Only GW190521 prefers the hyperbolic hypothesis** (ln B^hyp/prec = 3.71 ± 0.11, i.e. BF ≈ 41 — far below Gamba+2023's 4300:1, and the authors say so). GW231123, despite its morphological similarity to GW190521, **strongly rejects** the hyperbolic interpretation (ln B = -15.80). Injection studies show GW190521-like hyperbolic and QC-precessing signals are nearly degenerate at that SNR — the headline result is not as robust as it looks.

## Summary
- 38 events with at least one median component mass ≥ 50 M☉ pulled from GWTC; reanalyzed under hyperbolic (non-precessing spins, modes (2,±2),(2,±1),(3,±3),(4,±4)) and QC-precessing `TEOBResumS-Dalí` using the RIFT PE code.
- Hyperbolic prior: E₀/M ∈ [1.002, ≤1.2], p_φ ∈ [2, 7–25] depending on event; NQC corrections disabled to avoid plunge-ringdown pathologies; ringdown is still the **QC ringdown** (a major model limitation flagged repeatedly).
- 37 of 38 events favor QC-precessing. GW190521 is the lone outlier (ln B ≈ +3.71), with E₀ railing to its lower bound and p_φ⁰ → 2 (direct-plunge region).
- GW190521 cross-checked against QC-non-prec, eccentric non-prec, eccentric prec (all TEOB), plus `NRSur7dq4` QC-prec — hyperbolic still wins in every comparison, but the surrogate margin shrinks to ln B = 2.01.
- GW231123 (highest-mass LVK event to date) yields ln B^hyp/prec = -15.80; precession (not eccentricity) is the dominant factor, but unbound + precessing is not modeled.
- Injection-recovery on max-likelihood waveforms of both events: GW231123-like signals are clearly distinguishable (ln B = 13.14 vs -21.73), but **GW190521-like injections are only marginally distinguishable** (ln B = 1.83 hyp-into-hyp, -0.75 prec-into-hyp). The real-event BF is anomalously *larger* than the synthetic one.
- Pompili et al. (parallel, `SEOBNRv6EHM`) agrees on GW190521 and GW231123 but disagrees on GW191109_010717 (they prefer plunge, this paper does not).

## Strengths
- 🚀 First *catalog-scale* (38 events) systematic LVK reanalysis with a hyperbolic EOB template — a clear advance over Gamba+2023 (GW190521 only).
- Multi-hypothesis ladder for the two headline events (hyp / QC-align / ecc / ecc+prec / NRSur) is good practice; rare to see five different model configurations on one event.
- Honest about model limitations: explicitly flags the QC ringdown contamination at high E₀, NQC failures, EOB/NR separatrix divergence, and missing unbound+precessing physics — does **not** oversell GW190521.
- Synthetic injection sanity check is the right thing to do, and the authors openly report that GW190521-like signals are only marginally separable, which undercuts their own headline.
- The downward revision from Gamba+2023's 4300:1 to ≈41:1 is healthy: explicitly attributed to (i) higher-order modes, (ii) non-prec spins, (iii) wider E₀,p_φ prior, (iv) updated TEOB model. This is methodological maturation, not new physics.

## Weaknesses / Skeptic's Attack
- 💥 The lone "detection" (GW190521) sits in the **least-trustworthy corner of the waveform model**: low p_φ⁰ (direct-plunge), where EOB/NR scattering-angle comparisons (Albanesi+2025) show the largest discrepancies, and where NQC corrections had to be turned off entirely. The authors say so but do not quantify the systematic floor.
- The hyperbolic configuration uses a **quasi-circular ringdown** — for direct plunges the signal is ringdown-dominated, so the BF is essentially measuring "QC ringdown + arbitrary inspiral free parameters" vs "QC-prec inspiral+merger+ringdown". This is not really comparing physical hypotheses cleanly.
- **No unbound + precessing model exists.** GW190521 has substantial χ_p support in the QC-prec analysis. The comparison is therefore: precessing-with-circular-orbit vs aligned-spin-with-hyperbolic-orbit. Selecting the latter is not the same as evidence for a hyperbolic encounter.
- Injection study is **anecdotal by the authors' own admission** (single max-likelihood point per scenario, no noise realizations, no parameter-space scan). The GW190521-like injection gives ln B = 1.83, the real event gives ln B = 3.71 — a real systematic injection campaign is deferred to a "forthcoming follow-up".
- Selection bias: only m* ≥ 50 M☉ events. Justified by dynamical-formation astrophysics, but means there's no proper null test on lower-mass events that should clearly *not* be hyperbolic.
- Disagreement with Pompili+2026 (`SEOBNRv6EHM`) on GW191109_010717 is glossed over in one sentence. This is exactly the kind of waveform-systematics disagreement that should be the front-page result.
- No comparison with Bini-Damour-Geralico PM scattering predictions; no explicit faithfulness check against NR hyperbolic encounters at the parameters favored by GW190521.

## Relevance to Vojtěch's Research
Direct overlap on multiple axes: (i) unconventional GW signals and hyperbolic encounters as a science target; (ii) waveform-model systematics in LVK PE; (iii) reaffirms that EMRI-adjacent topics like plunge dynamics and non-circular ringdown modeling are the actual bottleneck. The Pompili+2026 disagreement on GW191109 is a flag worth tracking. Useful as a citation for both "hyperbolic templates are now being run on LVK data" and "but the systematic floor is still enormous". Probably influences how one frames LISA/3G hyperbolic-encounter forecasts and which events to target with PM-informed templates.

## Quality Score
6 / 10 — solid execution, honest caveats, but the BF↓100× from Gamba+2023, the QC-ringdown contamination, the missing unbound+prec model, the anecdotal injection study, and the deferred systematic campaign mean the GW190521-as-hyperbolic claim is no stronger than 2023, arguably weaker.

## Relevance Score
8 / 10

## Verdict
Should-Read
