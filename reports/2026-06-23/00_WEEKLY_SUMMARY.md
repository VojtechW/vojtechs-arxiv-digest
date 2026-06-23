# ArXiv Digest — 2026-06-15 to 2026-06-22

**Range:** Tue 15 Jun 2026 – Mon 22 Jun 2026 (5 arxiv mailings)
**Pool:** 627 unique submissions (376 new + cross-listings, 251 replacements/older)
**Candidates pre-evaluation:** 10
**Survivors:** 7 (after critical review)

---

## 🧭 Reading Priority

### Must-Read

#### 🌀 Relativistic EMRIs in Scalar Clouds: Eccentric and Inclined Orbits

**[arXiv:2606.21439](https://arxiv.org/abs/2606.21439)** — Xu, Brito, Della Monica, Vicente, Yuan

*Quality 7/10 · Relevance 9/10*

First fully relativistic computation of scalar-field fluxes for EMRIs on eccentric and inclined geodesics through a superradiantly-grown scalar cloud — extending Brito-Shah, Duque-Macedo-Vicente-Cardoso, Dyson et al., Li et al. past the circular-orbit limit. The headline physical findings are a dense spectrum of horizon-flux resonances near the LSO driven by relativistic apsidal precession (Ω_φ ≠ Ω_r), and a critical inclination below which a corotating dipolar cloud tidally pumps energy into the orbit through the horizon — both quantitatively presented and benchmarked against Hopper-Evans and the BHP Toolkit to ~5 significant figures. The Schwarzschild-only restriction and fixed O(ε) cloud background are the obvious caveats, but the formalism and cross-checks make this the new reference baseline for any future Kerr generic-orbit treatment.

*Caveats:* Schwarzschild only; test-cloud at O(ε); convergence cost limits infinity-flux to e ≤ 0.4. [Full report](2026-06-23/01_Xu_Brito_EMRI_Scalar_Cloud_Eccentric_Inclined_2606.21439)

---

### Should-Read

#### 💫 Universal Closed Form for Dynamical Love Numbers of Black Holes

**[arXiv:2606.19281](https://arxiv.org/abs/2606.19281)** — M. P. Solon (UCLA, sole author)

*Quality 8/10 · Relevance 7/10*

Solon presents a closed-form, all-orders, all-multipole, all-spin (s = 0, 1, 2) expression for the scheme-independent dynamical tidal response of a Schwarzschild black hole — the leading-log RG solution evaluated on a Newtonian-phase-dressed log τ = log(R_S/R) + 2[ψ(1−η) + γ_E]. The rate is the MST renormalized angular momentum ν^(2), the boundary value is fixed by horizon absorption, and horizon × near-zone × far-zone factorization is verified against shell EFT to O(G^15); the previously mysterious zeta tower in scalar perturbations is reinterpreted as the gravitational Coulomb-phase analog. Schwarzschild-only — Kerr, contact terms, and an SL(2,R)/Love-symmetry origin of ν^(2) are left as open questions.

*Caveats:* Schwarzschild only; contact terms excluded; no hidden-symmetry derivation of ν^(2) yet. [Full report](2026-06-23/02_Solon_Universal_Dynamical_Love_Numbers_2606.19281)

#### 🕳️ Semi-Analytical Loss-Cone Theory for TDE Rates Around Kerr Black Holes

**[arXiv:2606.18050](https://arxiv.org/abs/2606.18050)** — Wenkang Xin (Oxford MMathPhys dissertation, Trinity 2026)

*Quality 7/10 · Relevance 8/10*

Computes inclination-dependent Kerr tidal-disruption and direct-capture boundaries analytically using the ZAMO-frame algebraic transformation of Xin & Mummery 2025, and embeds them in a 2D Fokker-Planck equation in (L², L_z/L) at fixed energy. The clean separation of scales — an O(ε) local bias favouring retrograde disruption but only an O(ε²) global rate correction — is a useful, testable population-level statement: TDE rates are remarkably spin-insensitive. The "first semi-analytical" framing overstates novelty relative to Kesden 2012, and the underlying methodology paper (Xin & Mummery 2025, arXiv:2511.21499) is likely the more important downstream reference.

*Caveats:* dissertation rather than research paper; novelty largely lives in the companion methodology paper; no comparison to observed TDE rates. [Full report](2026-06-23/03_Xin_TDE_Kerr_Loss_Cone_2606.18050)

#### 🌊 Orbital Evolution of Asymmetric Binaries Within Accreting Environments

**[arXiv:2606.18341](https://arxiv.org/abs/2606.18341)** — Radulea, Rubio, Kritos, Maselli

*Quality 5/10 · Relevance 9/10*

A Kerr-geodesic upgrade of the Spieksma-Cannizzaro (2504.08033) Keplerian disk-crossing EMRI model, integrating bound geodesics analytically between impulsive Ostriker-DF and BHL-accretion kicks at each disk crossing. The reported two-stage alignment-then-circularization evolution is presented as a finding although it has been known since Syer-Clarke-Rees 1991, and the claimed Kepler-vs-Kerr divergence visible at a ∼ 10⁶ M is plausibly a phase-decoherence artifact of accumulated periastron precession rather than a genuine relativistic disk-coupling effect. The bibliography is blind to the entire stellar-transit / disk-crossing lineage (Witzany, Šubr-Karas, Suková-Zajaček, Pasham, Speri) — worth reading critically as a benchmark of how isolated different communities working on the same problem are.

*Caveats:* Newtonian disk-crossing physics with hard-coded ln Λ = 3; singular v_z in BHL denominator; the "Kepler-vs-Kerr divergence" is under-diagnosed; weak literature engagement. [Full report](2026-06-23/04_Radulea_EMRI_Accretion_Disk_2606.18341)

---

### Worth-Skimming

#### 🎵 Long-Lived Ringing of Near-Extremal Kerr Black Holes Resonantly Driven by EMRIs

**[arXiv:2606.17883](https://arxiv.org/abs/2606.17883)** — Wen-Biao Han

*Quality 6/10 · Relevance 7/10*

A pole-fitting test on frequency-domain Teukolsky amplitudes of an eccentric-inclined EMRI at a = 0.9999 recovers the independent (2,2,0) ZDM frequency to within ~3% of one pole half-width, with a coherent pole fraction P ≈ 0.6–0.9 across 12 inclination cuts. The result is a genuine step beyond the Thornburg-Wardell-van de Meent QNM "wiggles" because the pole is isolated from smooth source enhancement, but the headline framing of "resonant driving" overstates a sub-dominant effect (P ≤ 1, no Lorentzian peak in |Z|²) and the orbit-on-the-separatrix construction at a single benchmark spin is a long way from a realistic adiabatic EMRI. Worth a skim for the pole-tomography idea and the explicit κ-scaling of the access window; the headline surface-gravity-spectroscopy promise needs the deferred multimode Kerr Green-function calculation.

*Caveats:* single spin, separatrix orbit, no full Green-function construction; "resonant driving" framing overstated. [Full report](2026-06-23/05_Han_Near_Extremal_Kerr_ZDM_EMRI_2606.17883)

#### 🎢 Eccentricity in Disguise? Insights from GW231123 and NR-Simulated BBH Mergers

**[arXiv:2606.15150](https://arxiv.org/abs/2606.15150)** — Chandra, Fernandes, Mittal, Carullo

*Quality 7/10 · Relevance 6/10*

~1000 eccentric NR injections recovered with the quasi-spherical NRSur7dq4 surrogate show that high-spin recovery can mimic eccentricity; applied to GW231123, eccentric NR fits are statistically acceptable and favour higher M_f and e_0 ≳ 0.5, but the quasi-spherical model still wins on maximum likelihood (ln L > 208). The real contribution is a quantitative map of where eccentricity-vs-spin confusion bites — only at SNR 21–67 for M_T > 300 M_⊙ is the degeneracy resolvable. Useful awareness paper for anyone interpreting extreme-spin BBH inferences from current waveform models.

*Caveats:* setup is adversarial by construction; no new eccentric IMR model offered. [Full report](2026-06-23/06_Chandra_Eccentricity_GW231123_2606.15150)

#### 〰️ Dynamical Tidal Response of Neutron Stars: from EFT to Waveforms

**[arXiv:2606.19446](https://arxiv.org/abs/2606.19446)** — Apostolidis, De Luca, Gualtieri, Katagiri, Pani, Santoni

*Quality 7/10 · Relevance 6/10*

Extends the Schwarzschild Born-series + dim-reg/MS worldline-EFT framework to NS interiors, fixing the scheme-dependent finite parts of the O(ω²) electric quadrupole coupling and adding a b₀-dependent NS-specific term β₂ = −(64/45)(1 + (321/224)Λ₀) to the otherwise universal Schwarzschild RG running. The calculation is explicit and reproducible with two independent interior cross-checks; the "first complete" claim is narrower than advertised (Saketh et al. 2026 did the same in parallel, Mandal-Steinhoff et al. 2023 already had the counterterms), and the structural "modes alone don't suffice" point is a ~5% effect for realistic NS parameters. Not directly an EMRI/Kerr paper but useful for the EFT/RG structural lesson.

*Caveats:* no benchmark against Hinderer-Lackey TIDV or Pratten-Schmidt; structural deviations small in practice. [Full report](2026-06-23/07_Apostolidis_NS_Dynamical_Tidal_EFT_2606.19446)

---

## ❌ Papers That Failed Critical Review

- **[arXiv:2606.14894](https://arxiv.org/abs/2606.14894)** — Nair, Datta, "Tidal Stripping of Matter Bound to the Secondary in EMRIs." A Hernquist cloud truncated at the Roche radius plugged into a Schwarzschild-circular quadrupole chirp with no backreaction, no self-force, no debris dynamics, and an ad hoc relativistic cutoff. The advertised O(10³) rad dephasing in subsolar cases is essentially "fractional secondary mass change × inspiral cycles" — an upper-bound estimate rather than a quantitative prediction. The conceptual point (matter bound to the secondary matters, not just the primary) is fine, but the modeling is a toy. *Quality 4/10.*

- **[arXiv:2606.23450](https://arxiv.org/abs/2606.23450)** — Haiashi, Menezes, "NLO Angular Impulse and Leading Singularities to all orders in spin for Kerr Black Holes." A clean rederivation of the 2PM all-orders-in-spin angular impulse via KMOC + leading singularities, with checks against SSC preservation, |S| conservation, and the S² radial-action result. The territory was already mapped by Vines 2017, Aoude-Haddad-Helset 2022, Chen-Chung-Huang-Kim 2021, and the Bern et al. program — the contribution is a clean independent rederivation in a different observable channel rather than new physics. The most useful piece is the honest accounting of the spin-kick-vs-radial-action observable distinction. *Quality 5/10.*

- **2606.16280** (Gauss-Bonnet zoom-whirl), **2606.23021** (magnetically charged BH + quintessence zoom-whirl), **2606.23635** (Freund-Nambu zoom-whirl), **2606.23056** (f(R) GW polarization), **2606.15295** (f(Q) gravity), **2606.21029** (open-source rational-orbits tool) — all template-style "compute EMRI/waveform/polarization on [exotic gravity X]" papers. Excluded per the hard-exclusion rule on routine exercises and template QNM/orbit computations on weakly-motivated backgrounds.

---

## 🌌 Thematic Trends This Week

**Environmental EMRI physics is converging from multiple angles.** Three of this week's strong candidates (Xu et al. on scalar-cloud EMRIs, Lui-Drummond-Torres-Orjuela on spinning-secondary aerodynamics — already covered in last week's digest as 2606.01569, and Radulea et al. on disk-crossing) attack different facets of the same problem: how non-vacuum dynamics shapes the LISA-band signal of an EMRI. The collective message is that the EMRI community now treats environment as a first-class modelling problem rather than a perturbative afterthought — the calculations are increasingly relativistic, the resonance structure increasingly fine-grained, and the modeling stacks (pybhpt, FastEMRIWaveforms, KerrSpinningFluxes) are converging on shared infrastructure. Vojtěch's action-angle / canonical framework is at the substrate level of this convergence.

**Tidal responses, dynamical Love numbers, and the Kerr structural story.** The Solon paper on universal dynamical Love numbers (closed-form via MST ν^(2)) and the Apostolidis et al. NS-tidal-EFT paper both push on the same question — what is the universal vs object-specific content of the dynamical tidal response — from opposite directions (BH structural / extended-body matter). The natural next step is the Kerr generalization, which several groups are now poised to attempt; the closed-form ν^(2) result will be the benchmark.

**Eccentricity-vs-spin confusion remains the systematic gap of current BBH science.** Chandra-Carullo's GW231123 analysis is the latest in an ongoing series quantifying how the absence of eccentric merger-ringdown waveforms biases inferred spin. The takeaway is calibration-level: high-spin BBH inferences with current pipelines should be flagged with this systematic as a caveat, and the field continues to need a true eccentric IMR model rather than another diagnostic of how the gap manifests.

---

## 🔮 Notable Updates

- **[arXiv:2601.05223](https://arxiv.org/abs/2601.05223)** — Pound, Trestini, Nasipak, "Constants of motion in gravitational self-force theory" (replacement). Three Tier-2 collaborators on a paper directly relevant to Vojtěch's action-angle / Hamilton-Jacobi work on self-forced Kerr orbits. The original was submitted in January 2026; the v2 is worth checking for any structural changes to the gauge-invariant constants-of-motion construction.

- **[arXiv:2603.11167](https://arxiv.org/abs/2603.11167)** — Burke et al. (T2), "GW Measurement of the M_BH–M_⋆ relation" (replacement). Relevant to EMRI population inference with LISA.

- **[arXiv:2604.15129](https://arxiv.org/abs/2604.15129)** — Burke et al. (T2), Las Cumbres Observatory GW follow-up (replacement). Multi-messenger / EM-counterpart context.

- **[arXiv:2602.00691](https://arxiv.org/abs/2602.00691)** — Karas et al. (T2), Cherenkov / gamma-ray prospects (replacement).

- **[arXiv:2606.01569](https://arxiv.org/abs/2606.01569)** — Lui, Drummond, Torres-Orjuela. Cross-listed this week into gr-qc but originally posted ~2 Jun and already covered in the previous digest (2026-06-09). No content changes.

---

*Generated by automated weekly arxiv digest on 2026-06-23.*
