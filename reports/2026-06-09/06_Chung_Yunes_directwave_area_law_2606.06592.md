# 🕳️ Chung, Lam, Liu, Yunes — Measuring a Black Hole's Area Immediately after Merger: A Direct-Wave Test of Hawking's Area Law

**arXiv:** [2606.06592](https://arxiv.org/abs/2606.06592)
**Categories:** gr-qc astro-ph.HE
**Length:** 5 pages main + 2 pages End Matter (LIGO P2600278) — Letter
**Recommendation:** Worth-Skimming · **Quality:** 5/10

## Summary

Chung et al. interpret the frequency and damping rate of the recently identified "direct-wave" near-merger waveform component (Lu+ 2025; Kankani–McWilliams 2026; Oshita+ 2025) in GW250114 as `ω_DW ≃ m Ω_H` and `γ_DW ≃ κ`, and define a Kerr-equivalent horizon area `𝒜_DW = 2π/[√(Ω_H² + κ²)(√(Ω_H² + κ²) + κ)]`. They check consistency with the IMR-inferred remnant area, finding `Δ𝒜 ≈ 0` (odds ratio ~ 1) — a zeroth-order consistency check with no strong evidence for area-law violation.

## Key Results

- New diagnostic: Kerr-equivalent area from direct-wave fit parameters in pyRing on H1+L1 strain.
- For start times t₀ ∈ [−4.5, −3] M_f^det (i.e., before peak amplitude), 𝒜_DW is consistent with 𝒜_RD and with the IMR-inferred remnant area.
- The first-law area increment δ𝒜 (the inequality that actually tests Hawking's law) requires direct-wave SNR ~ 10³ — far beyond GW250114.
- Cross-checked against Lu et al. 2025 (rational-filter direct-wave search).

## Strengths

- Conceptually clean: states assumptions A.1–A.3 explicitly and acknowledges that what is measured is a "Kerr-equivalent effective area," not the true dynamical-horizon area.
- Honest scope: notes that the test resolves Δ𝒜 = 0 only to O(δ𝒜), and that the first-law increment is unresolvable at current SNR.
- Real LIGO data (GW250114), not just injections.
- Quantitative start-time robustness diagnostic (Eq. 9) with fractional deviations of 40–50%.

## Weaknesses

- Incremental novelty: direct-wave identification is from Lu et al. 2025 and follow-ups; the GW250114 remnant area was already measured by Abac et al. 2025c/2026a. This paper combines those with the phenomenological identification (Ω_H, κ) ↔ direct-wave fit parameters.
- The "test" is Δ𝒜 = 0 consistency at zeroth order — the actual area-law inequality δ𝒜 ≥ 0 is beyond reach. Significantly weaker than the title suggests.
- Result only "works" in a narrow window t₀ ∈ [−4.5, −3] M_f^det; an unexplained outlier at −4 M_f^det is dismissed as "fluctuation." Fractional deviations of 40–50% in Ω_H, κ are large.
- Method M.1 fixes (M, a) to maximum-posterior IMR values to break degeneracy — somewhat circularises the comparison with 𝒜_RD.
- The identification ω_DW ≃ m Ω_H, γ_DW ≃ κ as a near-horizon limit of a "frame-dragged, redshifted perturber" is asserted, not derived; relies on external Lu/Kankani/Oshita work.

## Relevance to Vojtěch

Moderate. Touches BH thermodynamics (area law, first law) and ringdown-adjacent observables. The conceptual question "what is an effective horizon area for a non-stationary spacetime?" is the kind Vojtěch values. However, the concrete calculation is parameter estimation on LIGO data plus a phenomenological identification; the BH-physics content is fairly thin (Eq. 6 algebra + SNR estimate).

## Honest Assessment

A careful, well-hedged paper that does exactly what the skeptic predicted — re-does the area-law comparison on GW250114 with a new waveform parameterisation (direct waves rather than QNM-only ringdown) and claims novelty. The authors themselves admit they are not resolving δ𝒜 and that this is a Δ𝒜 = 0 consistency check. The genuinely interesting question — whether ω_DW/m and γ_DW really *are* the near-horizon Ω_H, κ during the merger–ringdown transition — is asserted, not proven. Useful as a data point in the GW250114 spectroscopy literature, not a conceptual breakthrough.
