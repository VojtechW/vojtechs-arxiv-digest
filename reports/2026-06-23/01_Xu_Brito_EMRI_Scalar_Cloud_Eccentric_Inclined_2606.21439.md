# 🌀 Relativistic EMRIs in Scalar Clouds: Eccentric and Inclined Orbits

**arXiv:** [2606.21439](https://arxiv.org/abs/2606.21439)
**Authors:** Qi-Xuan Xu, Richard Brito, Riccardo Della Monica, Rodrigo Vicente, Chen Yuan
**Categories:** gr-qc, astro-ph.HE, hep-ph
**Comments:** 30 pages, 11 figures (companion Letter: arXiv:2605.03756)

---

## Summary

First fully relativistic computation of scalar-field energy and angular-momentum fluxes for an EMRI moving on eccentric and inclined geodesics through a superradiantly-grown scalar cloud, on a Schwarzschild background. The work extends the prior circular-orbit-only literature (Brito-Shah 2023; Duque-Macedo-Vicente-Cardoso 2024; Dyson et al. 2025; Li et al. 2025; Keijzer et al. 2026) to generic bound geodesic motion using the Hopper-Evans method of extended homogeneous solutions, with inclination handled cleanly via Wigner D-matrix rotations of the cloud (exploiting Schwarzschild spherical symmetry).

## What's genuinely new

- **Eccentric + inclined orbital coverage** for relativistic EMRI-in-scalar-cloud fluxes; previous works were limited to circular equatorial motion.
- A **dense spectrum of horizon-flux resonances near LSO**, driven by relativistic apsidal precession (Ω_φ ≠ Ω_r) — orbital harmonics σ_{mn} = mΩ_φ + nΩ_r match cloud level splittings even in axisymmetric clouds. This is absent in the Newtonian limit.
- A **critical inclination angle below which a corotating dipolar cloud pumps energy into the orbit** through the horizon (tidal acceleration analog of the Earth-Moon system, NOT superradiance) — boundary mapped quantitatively in (p, β) space.

## Strengths

- **Rigorous numerics.** Fluxes validated against the BHP Toolkit (circular) and Hopper-Evans (eccentric to e=0.9) to ~5 significant digits; ℓ_f and n convergence in Appendix C.
- **Honest about limitations.** Authors openly defer: O(ε²) cloud backreaction, conservative self-force from the cloud, geometric torques of Dyson & D'Orazio (2026), eigenfrequency shifts of Cannizzaro et al. (2024). They flag the absence of a first-principles balance-law derivation.
- **Newtonian benchmark.** Reproduces Tomaselli-Spieksma-Bertone (2023) ionization power/torque in the appropriate limit; residual ~20% deviations near sharp transitions are flagged for further study.
- **Correct physical interpretation.** The "cloud → orbit" energy channel is framed as tidal acceleration, not naive superradiance.

## Weaknesses

- **Schwarzschild restriction.** The justification (Mμ ≪ 1 implies superradiance saturates spin to low values; Dyson+25 shows Schwarzschild approximates low-spin Kerr) is reasonable but the EMRI regime is precisely where central BH spin matters most for observables. This is a tractable starting point, not the endpoint.
- **Test-cloud / fixed-background scheme.** Self-consistent treatment requires conservative metric corrections and backreaction on quasi-bound-state frequencies — all deferred.
- **Convergence cost limits the eccentric infinity-flux results to e ≤ 0.4**; the most striking high-eccentricity claims live in the horizon-flux channel.
- **Title overpromises.** Orbital inclination on Schwarzschild is geometrically trivial (spherical-tilt of the cloud); the technically harder inclined-on-Kerr-with-non-axisymmetric-cloud problem is explicitly punted.

## Relevance to Vojtěch

**High.** This sits squarely on the EMRI/Teukolsky/environments/resonance line: (a) flux computations for generic Kerr-like orbits; (b) environmental EMRI physics (ultralight bosons / scalar DM); (c) orbital resonances — the apsidal-precession-driven dense spectrum near LSO is precisely the kind of fine-grained resonance structure that environment-vs-vacuum discrimination relies on. Brito and Vicente are direct competitors in this space; the work is a useful reference baseline for any future Kerr generic-orbit extension that Vojtěch's group might pursue.

## Scores

- **Quality: 7/10**
- **Relevance: 9/10**
- **Verdict: Should-Read** — especially Sec. III–V (results) and the convergence-check appendices.
