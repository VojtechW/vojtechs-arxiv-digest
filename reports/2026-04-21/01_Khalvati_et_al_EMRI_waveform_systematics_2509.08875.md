# 🌀 Systematic errors in fast relativistic waveforms for Extreme Mass Ratio Inspirals

**arXiv:** [2509.08875](https://arxiv.org/abs/2509.08875)
**Authors:** Hassan Khalvati, Philip Lynch, Ollie Burke, Lorenzo Speri, Maarten van de Meent, Zachary Nasipak
**Categories:** gr-qc
**Submitted:** 2025-09-10 (v2 appeared this week)
**Collaborator note:** Lynch and van de Meent are extended-network collaborators.

---

## Quality Assessment

**Quality Score:** 8/10
**Relevance Score:** 9/10
**Verdict:** PASS — Must-Read

---

## Summary

This paper systematically quantifies two critical sources of systematic error in fast EMRI waveform frameworks: (1) truncation of multipolar mode sums in radiation-reaction flux calculations, and (2) interpolation errors in the offline/online architecture used by FastEMRIWaveforms. The authors demonstrate that mode truncation at low ℓ_max introduces multi-radian phase errors and parameter estimation biases for high-spin systems, recommend ℓ_max ≥ 30 for spins a ≥ 0.9, and develop an efficient Chebyshev interpolation scheme that achieves relative accuracy δ = 10⁻⁶ with significantly fewer grid points than spline methods. The practical guideline δ ≲ q (mass ratio) is validated via Bayesian MCMC parameter estimation studies.

---

## Strengths

- **Well-motivated and timely**: Directly addresses the gap between theoretically accurate self-force computations and practical fast waveform models used in LISA pipelines. The offline/online architecture is ubiquitous yet understudied for systematics.
- **Comprehensive dual-source analysis**: Cleanly separates mode truncation from interpolation errors with clear scaling laws. The phase error formula ΔΦ ∝ ⟨ε⟩/q elegantly quantifies cumulative effects.
- **Rigorous methodology**: Full Bayesian MCMC parameter estimation (not just mismatch) using state-of-the-art LISA response functions. Goes beyond the usual "mismatch < 10⁻³" claims.
- **Novel Chebyshev interpolation method**: Tunable relative-error scheme with coefficient pruning and Clenshaw acceleration. Genuine algorithmic contribution with better scaling to higher-dimensional parameter spaces (eccentric/inclined orbits).
- **Actionable guidelines**: The δ ≲ q criterion is concrete and implementable. The recommendation ℓ_max ≥ 30 for high-spin is directly useful.

---

## Weaknesses

- **Scope limited to circular equatorial orbits**: All numerical work assumes circular, equatorial inspirals. The harder eccentric/inclined case (the realistic EMRI scenario) is deferred entirely. For Vojtěch's work on eccentric/resonant orbits, the direct applicability is limited.
- **No comparison with existing production codes**: The paper develops Chebyshev methods but does not benchmark against FastEMRIWaveforms or other deployed models head-to-head.
- **Mode truncation finding is somewhat expected**: Practitioners already knew low ℓ_max is problematic. The quantification is useful but not deeply surprising.
- **Bayesian study narrow**: Only a = 0.9, M = 10⁶ M☉ tested. Broader spin/mass coverage would strengthen claims.

---

## Critical Cross-Examination

**A skeptic would say:** "This is essentially a careful error-budget analysis — important but not physics." That's partly fair. The core contribution is quantifying known issues rather than discovering new ones. However, the Chebyshev scheme is a genuine methodological advance, and the δ ≲ q guideline provides a principled accuracy target that was previously missing.

**Weakest point:** The restriction to circular equatorial orbits limits the paper's applicability to exactly the regime where EMRI waveforms are already best understood. The truly challenging case — generic orbits with eccentricity and inclination — remains open. The paper's conclusions about ℓ_max requirements likely underestimate the demands of eccentric orbits.

---

## Key Conclusions

1. Mode truncation at ℓ_max = 10 causes multi-radian phase errors; ℓ_max ≥ 30 needed for a ≥ 0.9.
2. Chebyshev interpolation achieves δ = 10⁻⁶ with 31 × 78 grid points (more efficient than splines).
3. For 4-year LISA observations with SNR ~ O(100), flux accuracy δ ≲ q ensures negligible parameter estimation bias.
4. High-spin regimes (a ≥ 0.9) are the bottleneck for both mode truncation and interpolation accuracy.

---

## Relevance to Your Research

This paper is directly relevant to your work on EMRI modeling and connects to your extended-network collaborators (Lynch, van de Meent). The ℓ_max requirements are important for anyone computing Teukolsky fluxes, and the Chebyshev interpolation scheme could be valuable for your flux computations via pybhpt. The restriction to circular orbits means the eccentric/resonant aspects of your work are not directly addressed, but the methodology is extensible.

**Recommended sections:** Focus on Sec. III.1 (mode truncation results, Figs. 1-2), Sec. II.3.2 (Chebyshev method), and Sec. III.2.3 (PE bias studies).
