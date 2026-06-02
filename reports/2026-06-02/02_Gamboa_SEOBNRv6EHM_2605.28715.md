# 🌊 Accurate Waveforms for Generic Planar-Orbit BBHs: SEOBNRv6EHM

**arXiv:** [2605.28715](https://arxiv.org/abs/2605.28715)
**Authors:** Aldo Gamboa, Alessandra Buonanno, Lorenzo Pompili, Raffi Enficiaud, Michael Boyle, Lawrence E. Kidder, Oliver Long, Peter James Nee, Harald P. Pfeiffer, Mark A. Scheel
**Categories:** gr-qc astro-ph.HE
**Quality:** 8.5/10 — **Relevance:** High (Axis 2) — **Tier:** Should-Read (borderline Must-Read)
**Collaborator flags:** 🟢 Tier 2 (Oliver Long, Peter James Nee), Tier 3 (Buonanno, Boyle, Pfeiffer)

## Summary

SEOBNRv6EHM is a multipolar, time-domain SEOBNR upgrade for generic planar-orbit BBHs (bound eccentric, dynamical capture, scattering). It introduces a sigmoid-resummed radiation-reaction (RR) force in EOB phase-space variables and achieves mismatches ≲2% even at eccentricities up to e ~ 0.9 against NR.

## Key claims

- New resummation of F_φ, F_r with quasi-circular factorized modes multiplied by sigmoid-bounded eccentric corrections (Eqs. 11a–11f).
- A new RR gauge (α=−2, β=−1) chosen so denominators stay regular at high eccentricity (Fig. 2). v5EHM's gauge fails for this resummation — useful transparency.
- Calibrated to 425 QC SXS NR; **validated** against 592 QC + 319 eccentric + 1 dynamical capture + 2 scattering SXS waveforms plus 61 scattering-angle comparisons.
- Median max mismatch ~0.02% over 20–200 M☉; ≲2% even for highest-eccentricity configurations (e up to ~0.9, 14 periastra). Order-of-magnitude improvement over v5EHM and TEOBResumS-Dalí.
- Walltime: 2–6× faster than v5EHM and Dalí; ~3× speedup in Bayesian PE.
- Multipoles (2,2),(2,1),(3,3),(3,2),(4,4),(4,3); no inherent parameter-space restrictions besides high-e near merger.

## Strengths

- Genuine technical novelty: the sigmoid resummation bounding eccentric RR corrections is more than parameter retuning. Explicit RR-gauge study is informative.
- One of the largest eccentric NR comparison suites in the literature.
- Honest acknowledgment of tensions: the 1PN truncation of eccentric corrections is chosen empirically because higher-PN orders improve scattering angles but degrade waveform mismatches — a structural tension flagged rather than hidden.
- Concedes higher-mode SNR-weighted mismatch degrades more than v5EHM (factor 3.6 vs 2.7).

## Weaknesses

- Calibration uses only QC NR. All eccentric performance relies on analytical construction + sigmoid choices — no eccentric-NR calibration loop. Sec VII admits "different analytical choices were made based on comparisons against eccentric NR".
- Merger-ringdown is still attached via QC prescription; no first-principles eccentric MR.
- Only 1 dynamical capture + 2 scattering NR waveforms for the most novel piece of parameter space.
- 1PN-vs-higher-PN tension in eccentric corrections is unresolved and may indicate the QC factorization paradigm is hitting its limit.
- No spin precession.

## Relevance to Vojtěch

Centerpiece waveform-modeling reference for current LVK and future LISA/ET in the eccentric/generic-planar regime. Specific items of interest:
- Sigmoid resummation as an alternative to standard Padé/EOB factorization — potentially relevant for small-mass-ratio adaptations.
- Explicit RR-gauge dependence at high eccentricity intersects with PN-to-Kerr matching and self-force consistency.
- SF-informed extended Hamiltonian from Khalil et al. is the EOB Hamiltonian.

## Verdict

Should-Read; borderline Must-Read for waveform-modeling tracking. Key reference release for the SEOBNR eccentric family.
