# 🫧 Tidal Stripping of Matter Bound to the Secondary

**arXiv:** [2606.14894](https://arxiv.org/abs/2606.14894)
**Title:** *Tidal Stripping of Matter Bound to the Secondary in Extreme Mass-Ratio Inspirals*
**Authors:** Sreejith Nair, Sayak Datta
**Categories:** gr-qc, astro-ph.HE, hep-ex, hep-ph
**Verdict:** Should-Read — Quality 5/10, Relevance 8/10

---

## One-line summary

Short Letter: matter bound to the EMRI *secondary* (gas envelope, DM mini-spike, supernova fallback) is tidally stripped during inspiral; modeling the bound mass via an instantaneous Hill radius on a Hernquist profile gives a time-varying μ(Ω) that imprints O(1)–O(10³) radians of dephasing in the LISA band, even for planetary-mass envelopes.

## Strengths

- **Genuinely new framing.** Almost all of the existing environmental-EMRI literature (Eda+13/15, Cardoso/Destounis/Maselli, Coogan/Kavanagh/Bertone 22, Cole+23, Duque+24, Dyson+25) dresses the *primary*. Dressing the secondary is conceptually clean and underexplored; the closest neighbors are Brito–Shah scalar clouds and Barsanti+ / Maselli–Franchini–Gualtieri–Sotiriou scalar-charge work.
- **Leading-order argument is correct.** The secondary mass enters the chirp rate at leading order in q, so even δμ/μ₀ ~ 10⁻⁴ has phase reach — the right yardstick (matching LISA's fractional-mass precision) is identified.
- **Qualitative discriminator.** An inflection in δϕ̈(t) where μ(Ω*) = m_ref cannot be reproduced by constant-mass vacuum templates at Newtonian order — a possible degeneracy-breaker against spin/eccentricity.
- **(m_e, a₀) sensitivity map** identifies a non-monotonic optimum at a₀ ~ r_H(t₀).

## Weaknesses

- **Crudest possible modeling.** Static Hill radius applied adiabatically to a Hernquist profile. No N-body/hydro, no orbital averaging of the tidal tensor, no eccentricity, no Kerr spin, no PN corrections — Newtonian quadrupole flux with Schwarzschild ε_orb.
- **Hill radius is a Newtonian three-body concept.** The instantaneous-stripping prescription assumes infinitely fast removal once r > r_H; subhalo N-body experience (Peñarrubia tidal-track) suggests this *underestimates* retained mass by factors of several.
- **Debris dynamics neglected.** No accretion drag, no dynamical friction from the stream, no self-gravity of the cloud. These are precisely where the physics could quantitatively flip — e.g., recaptured gas, or wake-induced torques (the Kavanagh–Nichols / Coogan dynamical-friction channel that dominates DM-spike dephasing for the primary).
- **Hernquist for a bound gas envelope or fallback shell is ad hoc.** For adiabatic DM spikes around PBH secondaries the proper profile is ρ ∝ r^{−9/4} (Eroshenko / Bertone–Merritt); using Hernquist discards the very feature that makes DM-spike phasing predictive.
- **No Fisher/Bayesian study.** Bias and detectability are claimed "at the fractional-mass-variation level" — handwave, deferred.
- **Inflection-vs-vacuum claim only at Newtonian order.** Untested against PN, where degeneracies with spin/eccentricity live (authors flag).
- **Initial conditions ambiguous.** m_e is the cloud mass at infinity; the binary formed with a particular Hill history, so the inferred a₀ depends on where and how the secondary acquired the cloud. Treated as free parameters with no formation-channel prior.

## Comparison to prior literature

Eda–Itoh–Kuroyanagi–Silk; Coogan–Kavanagh–Bertone 22; Kavanagh–Nichols; Cole–Cardoso et al. all dress the *primary*, with dephasing driven by dynamical friction of the secondary through that spike — fundamentally different physics. Becker–Sagunski–Annulli and Cardoso–Destounis–Duque–Macedo–Maselli develop the relativistic framework of BH-in-matter for the primary. This paper's twist is most analogous to scalar-hair-on-secondary work (Barsanti+; Maselli–Franchini–Gualtieri–Sotiriou) where the secondary's *charge* drives leading-order effects. Nair–Datta's mass-loss is the *matter* analog — but the dynamical-friction effect from a primary-dressed environment is also leading-order, and the paper does not compare to it.

## Relevance to Vojtěch's research

Intersects EMRI environmental effects with secondary dressing. The open-subsystem energy-balance treatment (adiabatic μ̇ entering the flux balance) is exactly the kind of two-timescale problem Vojtěch's action-angle / self-force framework is suited for. The authors bypass the conservative-self-force coupling and just feed μ(Ω) into the energy-balance law; a proper treatment would need an open-system formulation in which both flux and the secondary's binding energy evolve together.

## Bottom line

Short Letter, ~4–5 pages of physics, worth ~20 minutes. Read for the conceptual framing and the falsifiable inflection signature; do not trust the quantitative dephasing numbers as predictions — only as scoping estimates. A natural collaboration prompt: redo it with a proper open-subsystem formulation.
