# 💥 Star–Disk Collisions II: debris streams and QPEs

**Citation:** Philippe Z. Yao, Eliot Quataert, Yan-Fei Jiang, Itai Linial, *Star-Disk Collisions II: Debris Stream Dynamics and Implications for QPEs and Other Transients Near SMBHs*, arXiv:[2607.08823](https://arxiv.org/abs/2607.08823) [astro-ph.HE], 12 Jul 2026.

## Executive Summary
First 3D `Athena++` hydrodynamic simulations of star–disk collisions around a 10⁶ M☉ SMBH that self-consistently include the BH tidal potential (Hill + Coriolis), Keplerian disk rotation with tilt, and realistic orbital periods (18/31/63 hr; a/r_t = 3.5, 5, 8). Freshly stripped debris exits the Hill sphere, is tidally sheared into an asymmetric triaxial stream (R₁,R₂,R₃), and collides with the disk half an orbit later. The paper quantifies shocked stellar vs. shocked disk energetics, stream geometry, unbound outflows, and — most importantly — predicts flare durations t_dur ~ 2R₁/v_★, giving a duty cycle of ~10–20% independent of orbital period, matching observed QPE regularity.

## Key Contributions
1. First 3D sims with tides + disk rotation, bridging Paper I (Yao+2025, 2D, no tides) and Linial+2025 (analytic Hill's-equations model).
2. Numerical confirmation of the triaxial stream self-similarity predicted analytically by Linial+2025 (R₁,₂,₃ scale with r_H across all three separations).
3. Mass loss per collision (~10⁻⁴ M☉) essentially unchanged by tidal gravity vs. Paper I — validates Paper I's mass-loss formula.
4. Ratio of shocked disk / shocked debris energy scales inversely with orbital period; at ART3.5 they become comparable, providing a natural handle on the "one vs. two flares per orbit" question.
5. Predicts unbound outflows (~5×10⁻⁵–10⁻⁴ M☉/collision) that could feed TDE-like slow outflows and set disk depletion timescales.
6. Debris shock temperatures reach ~3×10⁶ K, marginally consistent with observed kT ~ 50–200 eV.

## Strengths
- Bridges numerics–analytics gap in the leading QPE model with a well-executed 3D setup.
- Directly reproduces the observed duty-cycle universality — a key phenomenological puzzle.
- Careful, honest treatment of caveats (numerical diffusion in disk, artificial R₁⁺ truncation).
- Engages with recent observational tests: cites Arcodia+2026 O–C timing of eRO-QPE2 (favoring 1 flare/orbit) and Guo & Shen 2026 / Mummery 2025 challenges.
- Predictive: inter-flare faint emission from shocked disk debris is a testable stacking signature.

## Weaknesses
- Pure hydro — no radiative transfer, so light-curve morphology, spectral evolution, and photon-starved-shock thermalization all deferred (implicitly to Vurm+2025, Huang+2025).
- Circular orbits only. Long/short flare alternation cannot be modeled; eccentricity effects on stream asymmetry only qualitatively discussed.
- Single M_BH = 10⁶ M☉, single solar-mass star, only 3 separations, only 3 collisions.
- Star-centered domain cannot track disk replenishment or global disk evolution.
- Radiative efficiency ε_rad = 0.1 imposed by hand.
- Shocked-disk mass has ≲50% numerical-diffusion error, so the shocked-disk-vs-debris crossover point is soft.

## Relevance to Vojtěch
Very high. State-of-the-art numerical backing for the Linial+Metzger EMRI+TDE→QPE picture; directly informs which orbital-parameter regimes give observable single/double flares — critical for EMRI–EM matching. Suková, Zajaček, **Witzany**, Karas 2021 is cited in §I as a foundational star-disk collision reference, indicating the authors treat Vojtěch's group as part of the immediate intellectual lineage.

## Scores
- **Quality:** 8/10 — solid, well-scoped numerical study with appropriate humility.
- **Relevance:** 9/10 — directly on Vojtěch's central research topic.

## Verdict
🌟 **Must-Read.**

## Collaborator flag
No Tier 1/2 authors. Vojtěch's 2021 paper is cited in the introduction — worth noting for future correspondence, especially on eccentric-orbit follow-ups where GR/EMRI expertise is complementary.
