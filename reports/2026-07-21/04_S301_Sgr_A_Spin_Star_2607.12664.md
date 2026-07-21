# ⭐ Discovery of a star sensitive to the spin of Sgr A*

**arXiv:** [2607.12664](https://arxiv.org/abs/2607.12664)
**Authors:** GRAVITY Collaboration — K. Abd El Dayem, R. Abuter, N. Aimar, P. Amaro-Seoane, A. Berdeu, J.-P. Berger, G. Bourdarot, W. Brandner, A. Burkert, D. Calderon, C. Correia, J. Cuadra, R. Davies, D. Defrere, L. Delit, A. Drescher, F. Eisenhauer, L. Esteras Otal, M. Fabricius, H. Feuchtgruber, N. M. Foerster Schreiber, A. Foschi, P. Garcia, R. Garcia Lopez, A. Generozov, R. Genzel, S. Gillessen, F. Gonte, X. Haubois, S. F. Hoenig, M. Houlle, S. Joharle, A. Kaufer, J. Kammerer, P. Kervella, J. Kolb, L. Kreidberg, L. Labadie, S. Lacour, O. Lai, R. Laugier, J.-B. Le Bouquin, J. Leftley, B. Lopez, D. Lutz, F. Mang, A. Merand, F. Millour, M. Montarges, N. Morujao, H. Nowacki, M. Nowak, S. Oberti, J. Osorno, T. Ott, T. Paumard, C. Paladini, H. B. Perets, K. Perraut, G. Perrin, R. Petrov, P. O. Petrucci, T. Piran, N. Pourre, S. Rabien, D. C. Ribeiro, S. Robbe-Dubois, M. Sadun Bordoni, J. Sanchez Bermudez, D. Santos, R. Sari, J. Sauter, S. Scheithauer, J. Scigliuto, J. Shangguan, T. T. Shimizu, F. Soulez, J. Stadler, C. Straubmeier, E. Sturm, M. Subroweit, C. Sykes, L. J. Tacconi, P. Thevenet, I. Urso, F. Vincent, J. Woillez, G. Zins
**Category:** astro-ph.GA (+ gr-qc)
**Submitted:** 2026-07-14

## TL;DR
GRAVITY reports the discovery of **S301**, a faint (m_K = 19.3) main-sequence star on an **8.7-year, e ≈ 0.983** orbit with pericenter r_p ≈ **136–142 R_S** (ten times deeper than S2, peak v ≈ 0.085 c). The star's orbit is fit at PPN β²-order (Schwarzschild), consistent with GR at f_SP = 0.94 ± 0.88. The Kerr β³ signal is not yet measured — the paper argues that with GRAVITY+ astrometry and ELT spectroscopy, S301 can deliver a **>5σ spin measurement within ~10 years**. Origin is attributed to a Hills-mechanism binary capture.

## Summary
Applying a new interferometric imaging pipeline (GRAVITY-RESOLVE) to a decade of GRAVITY data, the team identifies 19 astrometric positions of a new S-star. The orbit sets a new record for the shortest known S-star period (P = 8.68 ± 0.11 yr vs. S55/S0-102 at 12 yr) and the highest peak velocity (25,000 km/s). They fit the orbit including the Schwarzschild-precession multiplier f_SP and derive analytic osculating-element formulas for the Lense-Thirring drift (Δϖ_LT = 0.11° χ cos ξ per orbit). A mock 2026–2035 campaign (100 μas astrometry + 1 km/s RV) is shown to bound χ to <0.2 and separate χ=1 from χ=0 at >5σ. A photometric SED and isochrone fit gives m_* ≈ 1.1–1.5 M⊙; the extreme eccentricity is used to argue Hills-mechanism origin from a ~0.1 AU binary. Two orbit-orientation solutions remain degenerate absent radial velocity — an ERIS spectroscopy attempt did not succeed.

## Strengths
- **Genuine discovery**, not a Monte-Carlo forecast: the star exists in ~10 yr of GRAVITY data and the astrometric fit (χ² = 26/34 dof) is clean.
- Sets a new floor on the S-cluster: shortest period, deepest pericenter, highest v/c yet.
- **Explicit, non-hidden treatment of caveats** — orientation degeneracy, Newtonian-disk confusion (candidly quantifies up-to-order-of-magnitude nodal precession from a disk), need for 2PN modeling, low-SNR 2017 detection.
- Provides analytic per-orbit LT and PPN formulae directly usable by others.
- Ties the discovery to a specific dynamical origin (Hills capture) with a **testable v_rot sin i ≈ 20–70 km/s** prediction from the surviving primary spin-up.

## Weaknesses
- **Spin measurement is a forecast, not a detection.** Marketing framing "sensitive to the spin" is defensible but the actual β³ number carries no signal yet.
- **No radial velocity** ⇒ two-fold orbit-orientation ambiguity persists; ERIS spectroscopy failed.
- **Faint (m_K = 19.3)**, single pericenter passage, one weak 2017 CLEAN detection is load-bearing for a long baseline. A skeptic will point at circular reasoning risk (post-diction of the weak epoch from the preliminary orbit).
- **Newtonian confusion** near apocenter from the extended stellar/BH cluster can be up to ×10 the LT signal in extreme cases; mitigation rests on time-separation and future data.
- The Schwarzschild constraint f_SP = 0.94 ± 0.88 is weaker than S2's — S301's PPN power comes only from projected data.

## Novelty Cross-Check
Self-assessment (quoted from the paper): *"S301 provides the first and currently only practical way to measure the spin of Sgr A* with stellar dynamics."*  Predecessor spin-forecast literature (Waisberg et al. 2018 MNRAS 476; Angélil, Saha, Merritt 2010; Psaltis, Wex, Kramer 2016; Merritt, Alexander, Mikkola, Will 2010; Will 2008) asked *"what stellar orbit is needed to measure the spin?"* — S301 sits inside the parameter box those papers demanded but no one had found. The novelty is genuine and observational: a new object with the required parameters is now on the sky. The GRAVITY-RESOLVE imaging pipeline (Mang et al. companion paper) is a secondary novel technical contribution.

## Relevance to Witzany
**Direct hit.** Galactic-centre S-star at v/c ≈ 0.085, sitting inside the Schwarzschild-barrier map (Extended Data Fig. 7), with an explicit T_orb ≪ T_SP ≪ T_LT ≪ T_Vec-RLX ≪ T_coll timescale hierarchy — exactly the loss-cone / EMRI-precursor regime that Witzany works in. The osculating-element LT formalism is a natural bridge to the EMRI toolset, and the Hills-capture origin ties directly into the loss-cone repopulation channels that seed EMRIs. Amaro Seoane (2025) fractional-dynamics reference is cited. This is an S-cluster paper Witzany needs to know about; it is also a natural setup for a Kerr-geodesic follow-up (2PN and beyond, exact Kerr osculating elements, resonant-relaxation contamination). Not a Kerr-dynamics paper per se, but the physical object the paper reports is precisely a Kerr test particle in the S-cluster.

## Quality Score
- Overall: 9/10
- Direct relevance: 10/10
- Novelty: 9/10
- Technical rigor: 8/10

**Tier:** Must-Read

**Collaborator flags:** Tier 1 (GRAVITY discovery paper on a new spin-sensitive S-star; central to Witzany's programme; likely to be a citation floor for the next decade of S-cluster PPN/Kerr work; potential direct collaboration opening on 2PN / exact Kerr osculating-element modelling and on the Newtonian-confusion mitigation for the forecast spin measurement)
