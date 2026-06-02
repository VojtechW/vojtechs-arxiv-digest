# 🌌 Recoil-Regulated EMRIs in AGN Disks

**arXiv:** [2605.29305](https://arxiv.org/abs/2605.29305)
**Authors:** LingQin Xue, Zoltán Haiman, Hiromichi Tagawa, Imre Bartos
**Categories:** astro-ph.HE
**Quality:** 6.5/10 — **Relevance:** High — **Tier:** Should-Read

## Summary

Semi-analytic + Monte Carlo population study showing that recoil kicks from hierarchical mergers and binary-single interactions in AGN disks suppress wet EMRI formation by O(10), with LISA rates 0.6–29 yr⁻¹.

## Key claims

- Stellar interactions (mergers, binary-single) reduce EMRI formation rate by O(10)–O(100) across most of the (M_SMBH, λ_E) plane (Table 2 — e.g. 9621 → 6.5 Gyr⁻¹ at M = 10⁶, λ_E = 10⁻²).
- Detectable EMRIs preferentially come from young AGNs (≲ 10–20 Myr) and often involve merger-grown secondaries.
- LISA rates 0.6–29.3 yr⁻¹ depending on ERDF and SMBH mass function.
- ~1% of EMRIs in normal AGNs have binary-sBH secondaries; ~10% in low-mass/low-λ_E AGNs.
- QPE channel via recoil-displaced sBHs predicted at ~10⁻¹¹ Mpc⁻³ yr⁻¹ — three orders below observed QPE rate; authors acknowledge insufficiency.

## Strengths

- Prior wet-EMRI literature largely ignored hierarchical mergers and binary-single recoils — adding this is a real gap-filler.
- Updates inclination damping with recent hydrodynamic fits.
- Sweeps 5×4 grid in (M_SMBH, λ_E) plus four mass functions and two ERDFs.
- Uses FastEMRIWaveforms for SNR — proper detector modeling.
- Limitations section honest about migration traps, type-I/II transition, AGN intermittency.

## Weaknesses

- Built atop the Tagawa-family semi-analytic machinery which overestimates binary formation rates vs N-body (authors admit).
- "Effective migration rate Γ_mig · p_disk" for off-disk sBHs is a hand-wavy interpolation between type-I and type-II regimes — and is the key driver of the new enhancement in region I.
- f_mig = 2 is a fudge factor with no derivation.
- QPE comparison is weak (three OoM short) and acknowledged as plausibility argument, not prediction.
- Identical framework as previous papers — incremental.
- Eccentricity set to zero throughout for SNR computation — fine for rate, but circular EMRI from AGN disks is the expected limit so doesn't probe new dynamics.

## Relevance to Vojtěch

Directly on-axis: EMRIs, AGN-channel inspirals, wet-channel rates, demographic predictions for LISA. The recoil/binary-single suppression argument matters for any AGN-channel rate calculation. Worth knowing the number 0.6–29 yr⁻¹ and that detectable wet EMRIs are biased toward young AGNs.

## Verdict

Should-Read. Solid execution of a well-motivated incremental extension; not groundbreaking but a useful population-synthesis update with explicit demographic sweeps.
