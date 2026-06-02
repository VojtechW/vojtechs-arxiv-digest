# 🎯 Eccentric and Unbound Compact Binaries in the LVK Catalog with SEOBNRv6EHM

**arXiv:** [2605.28716](https://arxiv.org/abs/2605.28716)
**Authors:** Lorenzo Pompili, Aldo Gamboa, Alessandra Buonanno
**Categories:** gr-qc
**Quality:** 8.5/10 — **Relevance:** High (Axis 2) — **Tier:** Should-Read (borderline Must-Read)
**Collaborator flags:** 🟢 Tier 3 (Buonanno)

> Note: title says v5EHM but the paper actually uses v6EHM, introduced in companion paper 2605.28715.

## Summary

First large-scale parameter-estimation study using SEOBNRv6EHM on 26 LVK O1–O4 events, demonstrating reduced waveform biases vs v5EHM and TEOBResumS-Dalí, and exploring an "unbound-orbit" reanalysis of five high-mass events (including GW190521).

## Key claims

- v6EHM validated against 592 QC + 319 eccentric + scattering SXS NR runs; mismatch ~2% (v6) vs ~20% (v5EHM) vs ~30% (TEOB-Dalí) for SXS:BBH:2527.
- 2.5–3.5× speedup over v5EHM in real PE; BNS-length runs (GW170817) feasible in ~5 days.
- NR injection-recovery (six configs, e up to 0.34): v5EHM and TEOB-Dalí show parameter biases outside 90% CR at high e; v6EHM unbiased.
- Six events with log₁₀ B_QCAS^EAS > 0.5 (GW200129, GW200208_222617, GW200105, GW231223, GW190701, GW230712); five retain support against QCP.
- Unbound reanalysis: GW190521, GW191109, GW231221 show log₁₀ B_QCP^unbound ≈ 0.2–1.6 favoring direct-capture. **Honestly flagged as astrophysically unrealistic** (v∞ > 0.04c, prior odds 10⁻³–10⁻⁴ against).

## Strengths

- Genuinely first NR-injection waveform-systematics comparison across the three leading eccentric IMR models.
- Careful uncertainty discussion: prior choice, glitch sensitivity, astrophysical prior re-weighting (with realistic R_EAS/R_QCAS ≈ 0.023, only GW200129 survives).
- Honest framing of the unbound result — explicitly does NOT claim astrophysical unbound origin.
- Rigorous treatment of waveform-starting-frequency vs orbit-averaged-vs-instantaneous mismatch (Appendix A).
- Multiple sampling parametrizations including Cartesian (e_x, e_y).

## Weaknesses

- Heavy reliance on companion paper 2605.28715 for model details — readers must consult it for the algorithmic innovations.
- Merger-ringdown still uses QC attachment even in "unbound" runs; the "unbound" waveform is therefore a hybrid that cannot truly distinguish marginally-bound from marginally-unbound orbits (admitted in the paper).
- Five-event unbound headline is partially manufactured by waveform limitations (railing at E₀ = 1.0002 prior boundary).
- Equal-mass, nonspinning NR injections only — systematic claim does not probe q ≠ 1 or precessing eccentric cases.

## Relevance to Vojtěch

Squarely waveform-modeling + eccentric/generic-orbit PE; directly intersects EOB calibration choices, eccentricity-precession degeneracies, and dynamical-capture interpretation of GW190521. The honest discussion of the e-precession degeneracy and the "marginally bound vs marginally unbound" indistinguishability is the kind of conceptual clarity worth absorbing.

## Verdict

Should-Read; borderline Must-Read for the NR-injection systematics comparison (genuinely a first) and for the unbound-event discussion.
