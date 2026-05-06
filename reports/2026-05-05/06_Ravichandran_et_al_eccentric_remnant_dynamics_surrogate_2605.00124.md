# 🛞 Merger remnant and eccentricity dynamics surrogates for eccentric nonspinning BBHs

**Authors:** Adhrit Ravichandran, Peter James Nee, Keefe Mitman, Tousif Islam, Scott E. Field, Vijay Varma, Michael Boyle, Andrea Ceja, Nils Deppe, Noora Ghadiri et al.  
**arXiv:** [2605.00124](https://arxiv.org/abs/2605.00124) [gr-qc, astro-ph.HE]  
**Date:** May 2026  
**Categories:** gr-qc, astro-ph.HE

---

## Summary

The paper presents two NR-trained surrogate models, both restricted to nonspinning BBHs with mass ratio q ≤ 4 and reference eccentricity e ≲ 0.23 at t = -1000 M:

1. **NRSur-q4-NoSpin-Remnant** — predicts final mass, spin, and recoil velocity of the merger remnant.
2. **NRSur-q4-NoSpin-Dynamics** — predicts the time-domain evolution of eccentricity and mean anomaly.

Training uses the SXS catalog over a 3D parameter space (q, e, ℓ-mean-anomaly). Systematic errors from the surrogate construction are quantified and provided alongside the model — important for using the surrogate in parameter estimation pipelines.

## Strengths

- **Collaboration quality.** Field, Boyle, Mitman (Tier 3), Nee (Tier 2), Pfeiffer environment — this is the SXS / NRSur ecosystem at its serious end, and they ship error bars.
- **Dynamics surrogates, not just waveforms.** Surrogating *eccentricity and mean anomaly evolution directly* is the right move for current eccentric-search pipelines, which need a fast prediction of mean-anomaly dependence at merger.
- **Mean-anomaly coverage.** Recent NR work (Nee, Liu-Bonga, etc.) has highlighted how mean anomaly imprints on remnants; this paper turns that observation into a usable surrogate.
- **Open-source / reproducible by SXS standards.**

## Weaknesses

- **Mass ratio q ≤ 4 and e ≲ 0.23.** Useful for current-detector populations but not for the high-eccentricity, mass-asymmetric channels (capture, GW-capture in dense clusters, Hills mechanism). LISA EMRIs are entirely out of scope.
- **Nonspinning.** Astrophysical BBHs frequently have spin; with no spin, the surrogate is largely a calibration target, not a production-PE tool.
- **No higher-mode budget.** The accuracy of higher-ℓ modes vs leading (2,2) is not quantified in the abstract, and at q = 4 with eccentricity, higher modes matter.
- **Comparative accuracy** vs. TEOBResumS-Dalí, SEOBNRv5EHM, or recent eccentric phenom models is not shown in the abstract — the reader cannot tell whether this surrogate is the right tool to reach for.

## Relevance to Vojtěch

**Moderate (5–6/10).** Comparable-mass eccentric NR is not Vojtěch's daily territory, but the eccentric/mean-anomaly piece is conceptually adjacent to the EMRI resonance and post-adiabatic problem. Useful as a benchmark for cross-checks of effective-one-body models in the strong-field regime.

## Quality / Verdict

- **Quality:** 8/10
- **Relevance:** 5/10
- **Survives critical review:** **Yes.** Clean, careful surrogate work from a strong NR group, even if narrow in coverage.
