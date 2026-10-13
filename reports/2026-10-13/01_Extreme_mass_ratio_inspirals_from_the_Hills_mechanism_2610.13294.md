# 💫 Extreme mass ratio inspirals from the Hills mechanism, The eccentricity distribution of Hills EMRIs in LISA

🌠 **Should-Read** · 🔬 Quality 5.5/10 · 🎯 Relevance 6/10

📎 **Citation:** Biancamaria Sersante, Davide Mancieri, Kevin Leopoldo Muñoz Zavala, Luca Broggi, Zephyr Penoyre, Elena Maria Rossi, Alberto Sesana, *Extreme mass ratio inspirals from the Hills mechanism, The eccentricity distribution of Hills EMRIs in LISA*, arXiv:[2610.13294](https://arxiv.org/abs/2610.13294) [astro-ph.HE], submitted 09 Oct 2026.

> 💡 Following stellar black-hole binaries from the star cluster around a Milky-Way-like massive black hole until one member spirals in, the authors find that black holes captured when a binary is torn apart reach the LISA band on much more circular orbits than those delivered by ordinary star-by-star scattering (average eccentricity about 0.1 versus 0.48), but they are about eight times rarer when both channels start with the same total black-hole mass.

## 🔍 Executive Summary

The paper links four existing tools into a single pipeline for extreme mass ratio inspirals made by the Hills mechanism, in which the massive black hole tears apart a stellar-mass black-hole binary and keeps one member. The steps are an orbit-averaged two-dimensional Fokker-Planck model of the nuclear cluster that supplies binaries to the tidal radius, restricted three-body calculations of the break-up, an orbit-averaged Monte Carlo of relaxation plus semi-relativistic gravitational-wave losses for the captured black hole, and FastEMRIWaveforms Teukolsky-flux inspirals (on a non-spinning black hole) down to plunge. For one fiducial setup (a 4 million solar mass black hole and circular, equal-mass 20 solar mass binaries with 0.1 AU separation), Hills inspirals have mean eccentricity 0.097 at a nominal LISA-band entry and 0.035 at plunge. A same-group classical relaxation sample gives 0.48 and 0.23. Hills inspirals form at about 1.6e-8 per year per galaxy, about 12 per cent of the classical rate for equal initial black-hole mass, so how much they change the overall eccentricity distribution depends mainly on the unknown binary fraction.

## 📣 Claimed Contribution

The first self-consistent end-to-end model of the Hills EMRI channel, from binary supply through tidal separation, post-capture relaxation and relativistic inspiral to plunge. With it the authors give (I) the orbital properties of Hills EMRIs, (II) eccentricity distributions at LISA-band entry and at plunge compared with classical relaxation EMRIs, and (III) per-galaxy rates relative to the classical channel, plus the conditional probability of a Hills origin as a function of measured eccentricity and binary mass fraction, and a period-eccentricity diagnostic for EMRI-driven quasi-periodic eruption models.

## ✅ Strengths

- A truly end-to-end chain with each step handing over to the next. The Fokker-Planck flux into the binary tidal sphere sets the encounter-depth distribution, three-body break-ups set the capture orbits, and Monte Carlo relaxation sets where the gravitational-wave inspiral begins. The capture semi-major axis and eccentricity agree with the analytic scalings of Sari, Kobayashi and Rossi.
- The physical explanation is clear and checkable. Hills captures leave relaxation at a mean semi-latus rectum of about 84 gravitational radii, against about 26 for classical EMRIs, so they have longer to circularize. This is shown directly in the semi-latus rectum distributions.
- The final inspiral uses Teukolsky fluxes from FastEMRIWaveforms, with fifth-order post-Newtonian fluxes for eccentricities above about 0.9, instead of Peters-type formulae.
- The authors are candid about the rate dilution. With 10 per cent of black-hole mass in binaries, the probability of a Hills origin stays below 20 per cent even for the most circular plunging systems, so low eccentricity alone does not identify the channel.
- The quasi-periodic eruption section is restrained. It offers a period-eccentricity diagnostic and explicitly declines to claim a Hills origin for any source.

## ⚠️ Weaknesses

- There is a single fiducial model: one black-hole mass (4e6 solar masses, at the high end of LISA's EMRI sensitivity), one binary mass, one inner separation (0.1 AU) and circular inner orbits. The capture semi-major axis scales linearly with binary separation, so both the eccentricity distribution and the 12 per cent rate ratio depend directly on a choice that is not varied.
- Binaries are treated as point masses of twice a single black hole's mass in the Fokker-Planck step. There is no hardening, softening or ionization by cluster encounters and no in-cluster gravitational-wave mergers, even though the chosen separation is the one whose merger time equals 10 Gyr. The binary supply rate, the bottleneck the authors identify, is therefore not modelled self-consistently despite the 'self-consistent' framing.
- The classical comparison sample is taken from a separate earlier calculation (Mancieri 2026 / Mancieri et al. 2025) with a different, stricter slowly-evolving cutoff. The authors themselves attribute a sharp artificial cutoff at plunge eccentricity 0.026 in the classical distribution to this mismatch, which matters exactly in the low-eccentricity region where the channels are being told apart.
- LISA-band entry is a fixed semi-major axis taken from a circular-orbit 10^4 s period (about 19 gravitational radii). This ignores harmonic content and signal-to-noise selection, so 'eccentricity at LISA entry' is a nominal value, not an observable distribution. The authors acknowledge that no LISA selection effects are included.
- The black hole is non-spinning. FastEMRIWaveforms' Kerr flux module is run with a Schwarzschild separatrix, and inclined orbits are not considered.
- The Monte Carlo relaxation code and the improved Fokker-Planck loss-cone sink are deferred to 'a future publication', so key machinery cannot be fully checked from this paper.
- The text is long and repetitive (headline numbers are restated three or four times), with some sloppiness, such as '3.6.e-6 pc', a dangling '=' and the mean classical eccentricity quoted as 0.477944.

## 🤔 Skeptic's Cross-Examination

The headline result, that Hills EMRIs are more circular than relaxation EMRIs with some residual eccentricity from relaxation, was already published by Miller et al. (2005) and Raveh and Perets (2021). This paper adds more machinery but evaluates it at one hand-picked binary configuration and one black-hole mass, and the step that controls the rate (binary survival and supply in the cluster) is the crudest part of the pipeline. The 12 per cent rate ratio and the conditional probability curves are therefore illustrative rather than predictive. The eccentricity contrast is also partly shaped by a classical comparison sample built with different cuts.

## 🆕 Novelty in Context

The qualitative result is old. Miller et al. (2005) already predicted that Hills-captured compact objects give nearly circular LISA EMRIs. Raveh and Perets (2021, arXiv:2011.13952) already ran Monte Carlo relaxation on binary-disruption captures and found that relaxation leaves a residual eccentricity well above the Miller estimate. That is the same qualitative correction this paper reports, and the paper says so. Sari and Fragione (2019, arXiv:1907.03312) treated Hills-injected main-sequence EMRI rates analytically, and Chen and Han (2018) covered the complementary channel where the binary survives capture. I could not confirm whether Sari and Fragione is cited, because full-text search failed. What is new is narrower than 'first self-consistent modelling'. This is the first pipeline that couples a time-dependent Fokker-Planck binary supply, explicit three-body break-up and Teukolsky-flux inspirals, and so gives a rate relative to classical EMRIs worked out in the same group's framework (Broggi 2022, Mancieri 2026). That is a real but incremental improvement on Raveh and Perets. The headline numbers come from a single fiducial model in which the key parameters (binary separation, mass and binary fraction) are fixed by hand.

## 🎯 Relevance to Your Research

This is moderately relevant for EMRI work. It gives a physically motivated low-eccentricity EMRI subpopulation (mean eccentricity about 0.1 at nominal band entry, a few per cent at plunge) and is useful as a population prior when deciding which eccentricity range waveform models and searches must cover. It is also relevant to quasi-periodic eruptions modelled as EMRIs crossing a disc, through the period-eccentricity diagnostic figure. It does not touch waveform or self-force methodology: the inspiral is off-the-shelf FastEMRIWaveforms adiabatic evolution in Schwarzschild.

📖 **Where to start:** Section 3.1 (eccentricity distributions at plunge and LISA entry, and the semi-latus rectum explanation) and Section 3.2 (rate ratio and the probability of a Hills origin as a function of binary fraction). Section 4.1 and its period-eccentricity figure if you care about quasi-periodic eruptions. Skim Section 2.3 for the relaxation-to-inspiral handoff criterion (gravitational-wave time below 1e-3 of the relaxation time).

## Scores

- 🔬 **Quality:** 5.5/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- Only one fiducial model: a 4 million solar mass black hole, 20 solar mass equal-mass circular binaries, 0.1 AU separation. Nothing is varied.
- The main qualitative result (more circular orbits, with residual eccentricity from relaxation) was already found by Miller et al. 2005 and Raveh and Perets 2021.
- Binaries are point masses in the cluster model: no hardening, ionization or in-cluster mergers.
- The classical comparison sample comes from a separate calculation with different cuts, which produces an artificial low-eccentricity cutoff.
- 'LISA-band entry' is a fixed circular-orbit separation. There are no detector selection effects and the black hole is non-spinning.

## In Network

- 🚩 Alberto Sesana — notable author

---

🔗 [Back to the weekly digest](../2026-10-13)
