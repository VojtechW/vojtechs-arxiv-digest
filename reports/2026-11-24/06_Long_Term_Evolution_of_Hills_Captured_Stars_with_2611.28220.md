# 💡 Long-Term Evolution of Hills-Captured Stars with TDE Disk Collisions: Links to Repeating Nuclear Transients

🌠 **Should-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 7/10

📎 **Citation:** Howard Hao-Tse Huang, Philippe Z. Yao, Wenbin Lu, Eliot Quataert, *Long-Term Evolution of Hills-Captured Stars with TDE Disk Collisions: Links to Repeating Nuclear Transients*, arXiv:[2611.28220](https://arxiv.org/abs/2611.28220) [astro-ph.HE], submitted 20 Nov 2026.

> 💡 Stars captured by a massive black hole after their binary is torn apart can be dragged onto the hours-to-days orbits needed to explain repeating X-ray flares, but mostly because they keep crashing through the gas discs left by earlier star disruptions; gravitational waves and random stellar encounters alone would let most of them be destroyed first, and the stripping of stars in the gas sets a shortest reachable orbital period that grows with black hole mass.

## 🔍 Executive Summary

The paper follows stars captured via the Hills mechanism (a binary broken up near the black hole) onto very eccentric orbits a few tidal radii from a 1e5 to 1e7 solar-mass black hole. It evolves the orbit and stellar mass under drag and ablation from recurrent, viscously spreading tidal-disruption-event discs, Peters gravitational-wave decay and Gaussian angular-momentum diffusion, using a Monte Carlo scheme. Drag plus mass loss together set a period floor that scales roughly linearly with black hole mass, does not depend on disc surface density or TDE rate, and rules out sub-day orbits above about 1e6 solar masses unless gravitational waves dominate. With relaxation switched on, the standard EMRI criterion (gravitational-wave time equals angular-momentum relaxation time) overestimates how many stars survive. TDE-disc drag raises the fraction of stars reaching orbits of 10 days or less from at most about 0.1 to about 0.3 in the fiducial model (t_rel = 10 Gyr, TDE rate 1e-4 per year, H/r = 0.1), and towards unity at higher TDE rates.

## 📣 Claimed Contribution

First end-to-end model of the coupled orbital and stellar evolution of Hills-captured stars that combines recurrent TDE-disc drag, simulation-calibrated collisional mass loss with a MESA mass-radius response, gravitational-wave decay and stochastic two-body relaxation. Claimed results: (i) a collisional-ablation period floor P_min roughly proportional to M_BH, which explains why short-period QPEs prefer low-mass black holes; (ii) the conventional t_GW = t_L,rel EMRI criterion severely overestimates survival, and a replacement boundary t_GW (or t_EMRI) = 3 t_TDE, built on the time to diffuse across the tidal-disruption boundary, fits the Monte Carlo; (iii) TDE-disc drag boosts the fraction reaching QPE orbits by an order of magnitude or more if H/r is about 0.1; (iv) most repeating partial TDEs lie below the Hills-capture period minimum and need additional decay, plausibly from disc drag.

## ✅ Strengths

- Tackles a real gap: every orbiter model of quasi-periodic eruptions assumes a star sitting intact on an orbit of tens to hundreds of gravitational radii, and this paper actually tests whether a delivery channel can put it there.
- The period-floor argument is clean and analytic: drag and ablation both scale linearly with disc surface density, so d ln M / d ln a is independent of the TDE rate and disc mass. That gives P_min proportional to M_BH, a falsifiable prediction for the period versus black hole mass distribution.
- Builds on hydrodynamic mass-loss fits (Yao et al. 2025) and a MESA stellar response rather than an ad hoc stripping law.
- Makes explicit, intuitive why t_GW = t_L,rel fails for orbits whose pericentre sits just outside the disruption radius: a fractionally tiny change in pericentre is fatal, so the relevant clock is t_TDE = (L - L_min)^2 / L_c^2 t_rel. An empirical boundary t_GW = 3 t_TDE is validated against the Monte Carlo.
- The discussion is candid about tensions: the fiducial combination of high TDE rate and long relaxation time may not be self-consistent, eRO-QPE2 and RX J1301.9+2747 cannot be reproduced with solar-type stars, eRO-QPE4 is a tension, and the relaxation time is named as the dominant systematic.

## ⚠️ Weaknesses

- The relaxation treatment is a toy: one radius-independent t_2B,rel, angular-momentum diffusion only, no energy diffusion, no resonant relaxation and no mass segregation. Yet the paper's own conclusion is that the survival fraction changes by more than an order of magnitude between t_rel = 1 and 10 Gyr. The headline fractions therefore rest on a free parameter, not on a model of the nucleus.
- The disc is time-averaged (an orbit-averaged surface density) rather than truly episodic. Drag is applied as an impulse opposite to the stellar velocity, only at pericentre and apocentre; disc rotation, the actual node locations and orbit-disc inclination are all ignored. That is crude for collision speeds and drag on prograde or low-inclination orbits.
- The favourable results depend on an assumed geometrically thick (H/r ~ 0.1), low-density disc lasting well below Eddington. The paper itself admits thermal pressure cannot hold that up, so it appeals to magnetic support; for H/r = 0.03, sub-day orbits are essentially suppressed.
- The mass-loss prescription is extrapolated from 2D polytrope simulations over a limited range of ram pressures far beyond their calibration. Mass-loss uncertainty propagates as P_final proportional to f_ml^(3/2), and tidal heating, which can inflate the star and move the disruption radius, is omitted.
- The new EMRI-boundary result is partly anticipated: the paper itself cites Kaur 2025 for the same overestimate, and the use of the distance to the loss-cone boundary (L - L_min) rather than L is standard Fokker-Planck reasoning. The factor of 3 in t_GW = 3 t_TDE is a fit, not a derivation.
- No QPE rate is predicted. The output is a survival fraction per Hills capture, and turning it into a rate needs the binary fraction and separation distribution, which the paper does not supply. The comparison with observations is therefore qualitative.

## 🤔 Skeptic's Cross-Examination

Every quantitative result that matters (survival fractions of 0.01 to 1, the favoured TDE-rate window, the need for t_rel of 10 Gyr or more) is driven by two free knobs: a uniform relaxation time and a constant disc aspect ratio of 0.1. The paper admits the fiducial combination may be dynamically inconsistent, and that thin discs kill sub-day orbits. Strip those away and what is robust is a scaling argument for the period floor, which itself rests on mass-loss fits extrapolated far outside their simulation range, with drag applied at pericentre and apocentre instead of at the true disc crossings.

## 🆕 Novelty in Context

The ingredients are all from earlier work, much of it by the same group. Linial and Metzger (2023) proposed recurrent TDE discs engulfing tightly bound stars as the gas supply for quasi-periodic eruptions. Linial and Quataert (2023, arXiv:2309.15849) studied drag-induced period decay and stripping for repeating transients such as ASASSN-14ko. Yao et al. (2025) calibrated the per-collision mass loss. Lu and Quataert (2023) used Hills capture plus gravitational-wave decay for QPE progenitors. Cao et al. (2025, arXiv:2412.01159) already computed QPE formation rates from Hills capture with loss-cone theory, and found negligible rates around single black holes from inefficient relaxation. Pan and Yang (2021) showed discs can boost EMRI rates by orders of magnitude. The genuinely new piece is putting these together in one time-dependent Monte Carlo with recurrent TDE discs as the dissipation source, plus the resulting ablation period floor and its P_min proportional to M_BH scaling. The claim that the conventional EMRI criterion 'severely overestimates' survival is honestly attributed in part to Kaur 2025. It is a refinement specific to stars starting next to the loss cone, as Hills-captured stars do, not a general overturning of EMRI rate calculations, and readers from the compact-object EMRI side should not read it as one. A literature check with InspireHEP and the arXiv abstracts found no prior paper doing the full coupled calculation, so the integration claim stands. NASA ADS queries failed during this review.

## 🎯 Relevance to Your Research

Directly relevant to the astrophysics of stellar EMRIs and quasi-periodic eruptions: how stars reach orbits of tens to hundreds of gravitational radii, how loss-cone proximity changes the usual EMRI-formation criterion, and how gas drag competes with gravitational-wave decay. It contains no relativistic orbital dynamics beyond Peters decay, so it matters for the environment and formation side of EMRI work, not for waveforms or self-force.

📖 **Where to start:** Section 3 for the ablation period-floor argument and the P_min proportional to M_BH scaling. Section 5.2.2 for why t_GW = t_L,rel fails near the loss cone and the t_GW = 3 t_TDE replacement. Section 5.3.3 and the first part of Section 6 for the comparison with observed QPEs and repeating partial TDEs, and the admitted tensions. Sections 2.2 and 5.1 only to see how crude the drag and relaxation prescriptions are.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 7/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.5/10)

## 🚧 Caveats

- The headline survival fractions are set by an assumed uniform two-body relaxation time; going from 1 to 10 Gyr changes them by more than an order of magnitude.
- Sub-day orbits need a thick (H/r ~ 0.1), magnetically supported TDE disc that lasts long after the disruption; for H/r = 0.03 they essentially vanish.
- Disc drag is an orbit-averaged impulse at pericentre and apocentre only, ignoring disc rotation and orbit inclination; mass loss is extrapolated from 2D simulations and tidal heating is omitted.
- The 'EMRI criterion overestimates' result applies to stars starting right next to the loss cone (Hills captures), was partly noted by Kaur 2025, and uses an empirically fitted factor of 3.
- No QPE rate is predicted, only fractions per Hills capture; the comparison with observations is qualitative.

---

🔗 [Back to the weekly digest](../2026-11-24)
