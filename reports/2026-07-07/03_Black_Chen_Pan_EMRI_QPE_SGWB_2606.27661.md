# 🎇 Extreme Mass Ratio Inspirals in Light of Quasi-periodic Eruptions: Milli-Hertz Gravitational Wave Background

**Authors:** Brennen Black, Xian Chen, Zhen Pan
**arXiv:** [2606.27661](https://arxiv.org/abs/2606.27661) · astro-ph.HE, gr-qc · 9 pp, 2 figures
**Submitted:** 26 Jun 2026

## Summary
The authors adopt the disk-collision QPE model, use the observed QPE-to-TDE ratio q≈0.09 (Chakraborty+2025b) plus an isotropic-inclination geometric factor λ≈0.06 to convert observed QPE rates into EMRI formation rates: R_SE = 2.88×10⁻⁶ gal⁻¹ yr⁻¹ (stellar) and R_BHE = 6.07×10⁻⁶ gal⁻¹ yr⁻¹ (BH secondaries). They then run a Bonetti-Sesana Monte Carlo to compute the characteristic strain h_c(f), finding that BH-EMRIs can exceed the LISA sensitivity curve by up to ~2 orders of magnitude between 0.1–10 mHz for the fiducial (M_s = 100 M☉, r_disk = 300 R_g) case, while stellar EMRIs are destroyed before reaching the LISA band.

## Genuinely New?
Partial. Chen+2022 already computed the mHz SGWB from QPEs (eccentric-WD channel); this paper is the disk-collision-model version of the same exercise. Novelty is real but incremental: (i) the circular BH-EMRI channel systematically pushed through, (ii) the SE tidal-destruction cutoff (Linial-Metzger 2023) applied to remove stellar EMRIs from mHz. It is not a new physics insight; it is a rate exercise on well-established territory.

## Strengths
- Clean, transparent master equation linking R_QPE, R_TDE, N_disk.
- Correctly distinguishes SE (destroyed after one disk) vs BHE (survives many).
- Honestly notes that Arcodia+2024b's "R_EMRI ≥ R_QPE" bound fails for BHEs.
- Explores r_disk sensitivity (300 vs 1200 R_g), which spans ~2 orders of magnitude in rate.

## Weaknesses
1. **Chained small-number extrapolations.** q=0.09 rests on ~5–10 optical-TDE QPE detections; λ=0.06 assumes isotropy of orbits (violated in wet-channel EMRIs the paper itself invokes); r_disk fixed at a single value. Each is a large uncertainty; none is propagated. The fiducial rate is the product of three optimistic choices.
2. **Circular corroboration.** They cite agreement with Arcodia+2024b, but both estimates originate from the same eROSITA QPE census — not independent validation.
3. **Fiducial M_s = 100 M☉** is at the aggressive end of Franchini's window. Since h_c² ∝ M_c^(10/3), this alone lifts the SGWB by ~1 order of magnitude vs 10 M☉.
4. **No Ω_GW quoted, no LISA event-rate forecast** — the headline is only "above sensitivity curve", which is thin for a stochastic-background paper.
5. **Load-bearing assumption disk-collision = only QPE channel.** If some fraction of QPEs are repeated partial TDEs or self-lensing binaries, the q→R_EMRI mapping is inflated.
6. **Kejriwal-Witzany-Zajaček-Pasham-Chua 2024** (the direct QPE-EMRI counterparts paper) is apparently not engaged with in the comparison — a striking omission on this exact topic.
7. Peters t_coal is used on the circular orbit only — wet-channel EMRIs likely retain eccentricity, altering t_coal by O(1) and shifting the frequency mapping.

## Relevance to Vojtěch
High — this paper directly addresses whether QPEs can inform LISA rate forecasts, exactly the phenomenology Vojtěch has been building. Should be read especially to check that it does not misrepresent (or ignore) Kejriwal, Witzany et al. 2024. The λ≈0.06 isotropy assumption and the missing eccentricity treatment are natural entry points for a rebuttal or follow-up.

## Scores
- **Quality: 5/10** — technically competent, transparent, but the "fiducial" numbers are stacked-optimistic, uncertainties are not propagated, the key competing QPE-EMRI counterparts paper appears un-cited, and no Ω_GW / event-rate forecast is given.
- **Relevance: 9/10.**
- **Verdict: Should-Read** — on Vojtěch's exact topic and the numerical rates will circulate, but read with a skeptical eye and check the citation list against your own 2024 paper.

## Collaborator flags
None direct — but the missing citation to Kejriwal-**Witzany**-Zajaček-Pasham-Chua 2024 is the salient issue.
