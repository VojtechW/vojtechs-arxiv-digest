# Weekly ArXiv Digest — 2026-06-30 to 2026-07-06

**Digest date:** 2026-07-07
**Pool size:** ~656 new + cross-listed papers across gr-qc, astro-ph.HE, hep-th (plus 396 replacements)
**Candidates deep-read:** 10
**Survivors:** 9 (1 failed critical review)

## 📋 Reading Priority

### Must-Read (2)

🎯 **Quadrupole and quadratic-in-spin effects in quasicircular, spinning, asymmetric binaries**
[arXiv:2606.28937](https://arxiv.org/abs/2606.28937) — Rahman, Shahzadi, **Pound** (T2), **Mathews** (T2)
2PA self-force fluxes for a spinning + quadrupolar small body in Kerr, including quadratic-in-secondary-spin, spin-induced quadrupole, and tidally induced quadrupole contributions. Chebyshev grids + 6PN PNSF expansions; data deposited in `PostNewtonianSelfForce` toolkit. Quality **8/10**, Relevance **9/10**. Acknowledgements thank Vojtěch. Circular-only; the eccentric/precessing extension is the natural follow-up.
[Full report](2026-07-07/01_Rahman_Pound_Mathews_quadrupole_quadratic_spin_2606.28937)

🎯 **Efficient Eccentric Effective-One-Body Dynamics via Near-Identity Averaging Transformations**
[arXiv:2606.30594](https://arxiv.org/abs/2606.30594) — Lynch, Buonanno (T3), Gamboa, **van de Meent** (T2)
First port of NIT machinery from EMRI adiabatic inspirals into non-spinning eccentric SEOB. Reduces inspiral cost by up to 2 orders of magnitude (overall 1.5–8× waveform speedup). Argues NNLO NIT order is needed for q~1 mismatches ≤ 8×10⁻⁵. Incremental but well executed. Quality **7/10**, Relevance **9/10**. Focus on NIT-order requirements and the absence of a PA comparison.
[Full report](2026-07-07/02_Lynch_Buonanno_Gamboa_vandeMeent_NIT_EOB_2606.30594)

### Should-Read (3)

🎇 **Extreme Mass Ratio Inspirals in Light of Quasi-periodic Eruptions: Milli-Hertz Gravitational Wave Background**
[arXiv:2606.27661](https://arxiv.org/abs/2606.27661) — Black, Chen, Pan
Disk-collision QPE model → EMRI formation rates → mHz SGWB in LISA band. BH-EMRIs reach 1–10 mHz and can exceed the LISA curve by ~2 dex; stellar EMRIs are tidally destroyed in sub-mHz. Quality **5/10**, Relevance **9/10** — directly on Vojtěch's QPE-EMRI turf. **Read skeptically:** fiducial rates chain three optimistic assumptions (q=0.09, λ=0.06, M_s=100 M☉), no uncertainty propagation, no Ω_GW quoted, and Kejriwal–Witzany–Zajaček–Pasham–Chua 2024 appears un-cited.
[Full report](2026-07-07/03_Black_Chen_Pan_EMRI_QPE_SGWB_2606.27661)

🌟 **Nonlinear stability of subextremal Kerr black holes**
[arXiv:2606.28253](https://arxiv.org/abs/2606.28253) — Peter Hintz
333-page monograph claiming to settle full-subextremal (|a|<M) nonlinear stability of Kerr via a generalized wave-map gauge + Nash-Moser iteration on the tensorial Einstein equation. First proof valid beyond |a|/M ≪ 1 (Klainerman–Szeftel; GKS). Quality **9/10** (contingent), Relevance **3/10** to Vojtěch's physics program but a **landmark** worth being aware of. **Caveat:** relies on a second companion paper (tame estimates) whose stand-alone preprint I could not clearly locate — verify before citing as definitive. Skim §1 and the "companion papers" pointer only.
[Full report](2026-07-07/04_Hintz_Kerr_nonlinear_stability_2606.28253)

🌊 **Radiated Energy Spectrum, Radiated Angular Distribution and Non-linear Memory from the One-loop Gravitational Bremsstrahlung Waveform**
[arXiv:2607.03879](https://arxiv.org/abs/2607.03879) — Bini, Damour (T3), De Angelis, Geralico
Extracts dE/dω, dE/dΩ (G⁴/G⁵) and the multipole decomposition of non-linear memory (up to G⁵) from the one-loop scattering waveform. CoM-frame, 7.5PN fractional expansion. Ancillary Mathematica files (`spectrum_l_m.m`, `memory_l_m.m`) — those are the real deliverable. Quality **7/10**, Relevance **7/10**. Grab the `.m` files; don't read the coefficient tables in-paper.
[Full report](2026-07-07/05_Bini_Damour_DeAngelis_Geralico_1loop_bremsstrahlung_2607.03879)

### Worth-Skimming (4)

🌌 **Dynamics of Relativistic Binaries in Structured and Stochastic Environments: A Lagrange-Fourier-Hansen Framework**
[arXiv:2606.27526](https://arxiv.org/abs/2606.27526) — Zwick, **Dyson** (T2), Seymour, Takátsy, Samsing
Unified framework (secular perturbation theory + Hansen coefficients + rolling averaging) for env-perturbed relativistic binaries. Extends the strictly Newtonian precursor 2506.09140 with Dyson/Seymour adding relativistic content. Novelty likely lies in the rolling window + apsidal/nodal resonances, but the branding overclaims 170-year-old astrodynamics. Quality **6/10** (tentative), Relevance **6/10**. Full-text pass on Sec. II recommended.
[Full report](2026-07-07/06_Zwick_Dyson_LFH_framework_2606.27526)

🪛 **Gravitational wave scattering at O(G⁴): Murua construction and elliptics**
[arXiv:2606.27544](https://arxiv.org/abs/2606.27544) — **Bautista** (T3), Driesse, Haddad, Jakobsen
3-loop WQFT amplitude for GW scattering off a spinless point particle, matched to BHPT partial waves ℓ=2–20 at 10⁻³⁴ precision. Real technical improvement: the Murua construction bypasses cut subtraction at the master-integral level. First momentum-space elliptics in this specific setting (Isabella parallel work). Quality **8/10**, Relevance **6/10**.
[Full report](2026-07-07/07_Bautista_Driesse_Haddad_Jakobsen_WQFT_G4_2606.27544)

🌐 **Environmental effects vs. modified gravity in the LISA massive black hole binary population**
[arXiv:2607.00845](https://arxiv.org/abs/2607.00845) — Copparoni, Barausse
Hierarchical Bayesian analysis of MBHB catalogs: accretion + migration (−4PN) vs Ġ (−4PN) are formally degenerate at single-event level but distinguishable at population level. Quality **6.5/10**, Relevance **7.5/10**. Caveats: Fisher-only single-event posteriors, circular inspirals only, heavy-seed-dominated. **Eccentricity is the natural follow-up.**
[Full report](2026-07-07/08_Copparoni_Barausse_env_vs_MG_2607.00845)

🧭 **Joint inference of line-of-sight acceleration and orbital eccentricity in neutron-star–black-hole binaries**
[arXiv:2606.28156](https://arxiv.org/abs/2606.28156) — Pompili, Gamboa, Buonanno (T3)
Time-domain Doppler remap of LOSA in SEOBNRv6EHM / SEOBNRv5PHM. Reports GW200105 (Γ, e) posterior disfavors both being zero at 90%. Quality **6.5/10**, Relevance **7/10**. The GW200105 headline is a 2D reframing of the pre-existing eccentricity hint, **not** a detection of environmental acceleration; concurrent Roy & Nitz (2606.25304) shares priority.
[Full report](2026-07-07/09_Pompili_Gamboa_Buonanno_LOSA_NSBH_2606.28156)

## ❌ Papers That Failed Critical Review

- **[2606.27429](https://arxiv.org/abs/2606.27429)** — *Zi, Kumar, Zhao, Gu, Shu — "Massive scalar fields in eccentric regime: Detectability and constraints from LISA observations of EMRIs"* — cartesian product of the two known ingredients (eccentric-Kerr massless-scalar EMRI: Barsanti et al. 2210.11121; circular massive-scalar EMRI: Barsanti–Maselli–Sotiriou–Gualtieri 2212.03888), no genuine new physics, no engagement with no-hair-theorem constraints on the secondary's scalar charge, and Fisher-matrix bounds that are neither competitive with existing Solar-System/LIGO bounds nor validated against Bayesian sampling. Quality 4/10, Relevance 3/10.

## 📈 Thematic Trends This Week

**Environmental effects and degeneracies dominated the LISA-forecast literature.** Three separate papers this week (Copparoni–Barausse for MBHBs, Pompili–Gamboa–Buonanno for NSBH LOSA, Zwick–Dyson et al. for a unified secular-perturbation framework) target the same underlying problem: how do we tell astrophysical environments apart from modified gravity in the -4PN sector? The community is converging on population-level hierarchical inference as the differentiator, but none of these papers treats eccentricity self-consistently — an obvious blind spot that Vojtěch is well-positioned to exploit.

**Self-force / EMRI infrastructure continued to mature.** Rahman–Pound–Mathews delivered the χ² + quadrupole flux inputs missing from 2PA aligned quasi-circular EMRI waveforms, and Lynch–Buonanno–Gamboa–van de Meent ported near-identity averaging into non-spinning eccentric SEOB. Both are "ingredient" papers rather than "waveform" papers — the last-mile step of demonstrating LISA-scale phase accuracy remains open.

**Two large mathematical-relativity monographs appeared in one week** (Hintz 333pp on subextremal Kerr nonlinear stability, plus its constraint-damping companion 2606.27658). The full-subextremal claim is a genuine holy-grail result if the tame-estimates companion holds up — the wave-map + Nash-Moser strategy is a serious methodological departure from the Klainerman–Szeftel / DHRT program. Watch this space over the next 6–12 months as the community digests it.

## 📌 Notable Updates

**[2606.09992](https://arxiv.org/abs/2606.09992)** — *O'Connor, Hall, Busmann et al. (incl. **Dheeraj Pasham**, T1) — "EP260321a/SN 2026gzf: The Faintest Shock Breakout Associated with a Broad-Lined Supernova"* — Multi-wavelength characterization of a faint EP shock-breakout / broad-lined SN association. Original submission June 2026; replacement Jul 2026. Astro-ph.HE, adjacent to Pasham's transients program; likely tangential to Vojtěch's EMRI/QPE work.

**[2601.15198](https://arxiv.org/abs/2601.15198)** — *Singh, **Chapman-Bird** (T2), Berry, Veitch — "Revealing massive black hole astrophysics: The potential of hierarchical inference with extreme mass-ratio inspiral observations"* — Hierarchical inference on LISA EMRI catalogs to recover MBH mass function and spin distribution. Directly relevant to Vojtěch's EMRI-population angle; the update is worth a look to see what was added in v2.

**[2507.03380](https://arxiv.org/abs/2507.03380)** — *Kumar, Zi, Bhattacharyya — "Extreme mass-ratio inspirals and extra dimensions: Insights from modified Teukolsky framework"* — Modified-Teukolsky EMRI dephasing in extra-dimensional scenarios. Same author cluster (Kumar, Zi) as the failed 2606.27429 above; check whether the update addresses the no-hair-theorem concerns raised there.
