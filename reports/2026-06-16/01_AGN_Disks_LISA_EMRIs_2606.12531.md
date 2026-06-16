# 🌟 Illuminating AGN Disks with LISA EMRIs

**arXiv:** [2606.12531](https://arxiv.org/abs/2606.12531)
**Title:** *Gotta light? Illuminating AGN disks with LISA EMRIs*
**Authors:** Federico Fantocolli, Francisco Duque, Jonathan Gair
**Categories:** gr-qc, astro-ph.HE
**Verdict:** Must-Read — Quality 8/10, Relevance 9/10

---

## One-line summary

First fully Bayesian LISA forecast using *relativistic* (Teukolsky-based) gas torques on circular equatorial EMRIs in Novikov–Thorne disks, finding that the surface density Σ₀ and disk scale-height h₀ — and hence the α-viscosity and Eddington fraction f_Edd — can be measured separately from the EMRI waveform alone, *without* requiring an EM counterpart, by breaking the Newtonian Σ/h² degeneracy.

## Strengths

- **Genuine methodological advance.** The Duque (2025a) / Hegade-K.R. (2025) relativistic Lindblad-resonance torques (Teukolsky + Hirata, ~O(1–10) enhancement over Newtonian power-law) are plugged into FastEMRIWaveforms and an *eryn* MCMC inference is run end-to-end. Previous Pan/Lyu/Tagawa-style AGN-EMRI work was Newtonian power-law and largely Fisher-only.
- **Calls out where Fisher fails.** They show explicitly that the Fisher matrix breaks down even at SNR ≈ 50 in the (Σ,h) sub-block when the system is in the strong-environmental-dephasing regime — a methodological warning relevant beyond this paper. The (u,v) = (ln Σ/h², ln hΣ²) reparametrization isolates the truly degenerate direction.
- **Predictive empirical scaling.** An empirical U ∝ (ΔΦ)^(−1/2) fit calibrated across five fiducial systems (Appendix B) gives a back-of-envelope tool for assessing constrainability of α and f_Edd from a measured dephasing.
- **Honest scope statement.** Caveats are listed up front: no stochastic torques, no pressure outside regularization, no co-orbital torques, noiseless data, narrow 1.5% prior windows.

## Weaknesses

- **EM "illumination" is asserted, not computed.** No photoionization spectrum, no accretion luminosity curve, no AGN catalogue cross-match is actually produced. The proposed multi-messenger pipeline relies on existing literature (Lyu 2026; Liu 2026b) for the EM side.
- **Narrow orbital configuration.** Circular, equatorial, prograde, near-plunge. The QPE-EMRI population (Linial–Metzger; Franchini; Kejriwal–Witzany–Zajaček–Pasham–Chua) lives at inclined/eccentric large-r orbits with disk crossings — precisely complementary, but the present paper does not cover it.
- **Only five fiducial systems, all at SNR=50.** The γ ≈ −0.5 power-law from the U∝(ΔΦ)^γ fit may be polluted by mixed prefactors across the five systems; authors note this themselves.
- **Comparison literature is thin.** No quantitative comparison to Pan/Lyu/Yang/Tagawa-Haiman AGN-EMRI lineage. Suková/Karas star-AGN-torus transit work is not cited at all.
- **α constraint is modest.** ~60% uncertainty on viscosity even in the best intermediate-mass case.

## Relevance to Vojtěch's research

Directly central. The paper

1. **cites Kejriwal, Witzany, Zajaček, Pasham, Chua 2024** explicitly when discussing QPE-EMRI models as a population distinct from the in-band wet-EMRIs they study;
2. lives squarely in Vojtěch's environmental-EMRI / accretion-effects niche;
3. delivers a *methodological warning* — Fisher fails for environmental parameters even at SNR=50 — that affects any forthcoming PE forecast in this area;
4. uses the Duque–Hegade-K.R. relativistic-torque framework, which is complementary to BHPT-based work;
5. leaves wide open the natural follow-up: extend to *inclined and/or eccentric* orbits, which is the regime where Vojtěch's QPE-EMRI line of work would extract the most discriminating power.

## Citation context

Properly cites: Vojtěch's group (Kejriwal–Witzany 2024); Pan/Lyu/Yang for the dark-siren angle; Duque 2025a, Hegade-K.R. 2025 for relativistic torques. Notably absent: Suková/Karas torus-transit line; full numerical comparison to Pan, Lyu, Yang, Tagawa, Haiman AGN-EMRI literature.

## Bottom line

A solid, careful paper from the Gair group that pushes the EMRI-in-AGN-disk problem out of the Fisher/Newtonian comfort zone and into a proper Bayesian + relativistic setup. The Σ/h² degeneracy-breaking result is the one durable physics takeaway, and the methodological warning about Fisher failure is the durable forecasting takeaway. **Must-read** — start at Sections 2 (torque setup) and 3.1 (the Bayesian results), and engage critically with the QPE-EMRI discussion in 3.2.
