# 🌀 Enabling gravitational-wave astronomy with spin-precessing black holes on generic orbits

**arXiv:** [2609.01568](https://arxiv.org/abs/2609.01568)
**Authors:** Aldo Gamboa, Lorenzo Pompili, Alessandra Buonanno, Luca Sebastiani, Raffi Enficiaud, Michael Boyle, Lawrence E. Kidder, Harald P. Pfeiffer, Antoni Ramos-Buades, Mark A. Scheel
**Categories:** gr-qc
**Quality:** 9/10 · **Relevance:** 5/10 · **Verdict:** Must-Read (landmark waveform-modeling result)

---

## One-line
The effective-one-body waveform family finally gets a model that treats orbital eccentricity and spin precession *at the same time*, validated against 1524 numerical-relativity simulations with median mismatches below 1%.

## Summary
This paper introduces **SEOBNRv6EPHM**, the first generic-orbit, spin-precessing member of the SEOBNR family, closing the gap between SEOBNRv5PHM (precessing, quasi-circular; arXiv:2303.18046) and SEOBNRv5EHM (eccentric, aligned-spin; arXiv:2412.12823). It reduces to the aligned-spin eccentric SEOBNRv6EHM (companion paper) in the non-precessing limit. Generic orbits are evolved via 13 coupled ODEs — planar EOB equations of motion in a co-precessing frame with a partial-precessing Kerr-deformed Hamiltonian, plus PN-expanded quasi-circular spin/angular-momentum precession equations — and waveforms are built by "twisting up" the co-precessing modes (2,2), (3,3), (2,1), (4,4), (3,2), (4,3). The model handles bound inspiral-merger-ringdown binaries, dynamical captures, and scattering. The centrepiece is validation: SNR-weighted mismatches against 1437 quasi-circular + 87 eccentric SXS precessing NR waveforms (eccentric set: q ≤ 6, χ_p ≤ 0.9, e_gw ≤ 0.6), over total mass [20, 200] M☉ at ι = π/3, give median mismatch < 1% for both classes; q ≤ 4 binaries stay below 4% even at e_gw ~ 0.5, with worst cases ~10%. It matches SEOBNRv5PHM in the quasi-circular limit and beats the only competing generic-orbit model, TEOBResumS-Dalí, by a median factor ~4 in mismatch (>10× for some configs) while being ~2–3× faster than v5PHM in the QC limit and up to ~10× faster than Dalí — so eccentric+precessing parameter estimation costs no more than current quasi-circular analyses. It reproduces non-perturbative NR scattering-angle phenomenology (a turning point in Θ_s that 4PM misses). As a proof of principle it analyses 11 GW events; for GW200129 across six glitch-mitigation schemes, eccentricity is favoured over the QC-precessing NRSur7dq4 hypothesis (log₁₀ B ≈ 0.8–5.4, e_10Hz ≈ 0.13–0.29), backed by the first NR-injection recovery test for an eccentric precessing model.

## Strengths
- **A genuine first.** No prior SEOBNR model combined precession and eccentricity, and this is the first *systematic* accuracy assessment of any generic-orbit model against eccentric spin-precessing NR (1524 simulations) — far beyond the anecdotal validation typical in this area.
- **Quantitative wins, not hand-waving.** Median factor ~4 mismatch improvement over TEOBResumS-Dalí while up to an order of magnitude faster, and it matches the mature QC-precessing model's accuracy.
- **Broad physical coverage in one framework** (IMR + captures + scattering), cross-checked against pioneering generic-spin NR scattering data and reproducing a non-perturbative feature absent from 4PM.
- **Unusually self-critical error budget:** it explicitly names the QC precessing sector (not the eccentric sector) as the dominant error source and introduces an NR-injection recovery test to check the GW200129 eccentricity claim against systematics.

## Weaknesses / caveats
- **The precessing sector is not NR-calibrated.** Calibration parameters (a_6, d_SO) are tuned only to QC aligned-spin NR; precession enters via PN-expanded *quasi-circular* spin equations fed with eccentric dynamics. The eccentric-precessing NR set is used for validation, not calibration — so the hardest regime rests on an untested extrapolation.
- **Thin coverage of the target space:** only 87 eccentric precessing NR waveforms, bounded at q ≤ 6, e_gw ≤ 0.6, χ_p ≤ 0.9. The astrophysically interesting corner (high eccentricity + strong precession + high q simultaneously) is exactly where mismatches degrade to ~10% and NR coverage is sparsest.
- **A known, unquantified dynamical bias:** the scattering test shows both EOB models overpredict polar deflection / final tilt because the QC precession equations omit radial contributions — a real bias that will matter for strongly eccentric periastron passages.
- **Mode asymmetries neglected** (negative-m taken as conjugates), which the authors concede "can affect precession measurements" — directly relevant to the flagship GW200129 eccentricity-vs-precession disentanglement.
- **The GW200129 eccentricity evidence is real but soft and glitch-dependent** (log₁₀ B spans 0.8–5.4; under fair BayesWave draws support is weak ~0.8). "Strengthening evidence" is a fair but generous framing of a proof-of-principle on contaminated data.
- Only six co-precessing multipoles; higher-mode mismodelling propagates through the twisting-up (acknowledged future work).

## Relevance to Vojtěch
**Axis 2** (quality/originality in GW waveform modeling for generic/precessing/eccentric regimes). This is the current state of the art for comparable-mass waveforms in the underexplored eccentric+precessing corner. Honest caveat: it is a comparable-mass EOB/PE model, not EMRI or self-force work — the only bridge to the EMRI-adjacent interests is the Kerr test-body Hamiltonian core and the geodesic/scattering-angle comparisons. Read it as a benchmark of "what production waveform modeling now achieves," not as core reading.

## Where to start
Fig. 2 and the "Agreement with NR waveforms" section for the mismatch distribution (median < 1%, the q ≤ 4 story, the factor-4 win over TEOBResumS-Dalí); then Fig. 3 / the scattering-angle section for the honest limits of the precession dynamics; then the GW200129 section + Fig. 4 and Table 1 for the science payoff and the cost argument.

*In network:* 🚩 Alessandra Buonanno, 🚩 Harald P. Pfeiffer, 🚩 Michael Boyle (Tier-3 notable authors — SXS/AEI EOB collaboration).
