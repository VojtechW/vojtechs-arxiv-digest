# 💥 Star-Disk Collisions II: Debris Stream Dynamics and Implications for QPEs and Other Transients Near SMBHs

**arXiv:** [2607.08823](https://arxiv.org/abs/2607.08823)
**Authors:** Philippe Z. Yao, Eliot Quataert, Yan-Fei Jiang, Itai Linial
**Category:** astro-ph.HE
**Submitted:** 2026-07-09

## TL;DR
Three-dimensional Athena++ simulations of a stellar-mass orbiter grazing a Keplerian disk around a 10^6 M_sun SMBH, now including the black hole's tidal potential and Coriolis/centrifugal forces so that stripped debris exits the Hill sphere and forms an extended, asymmetric, triaxial stream. Follow-up impacts of that stream on the disk shock both stellar and disk gas to high specific energies, drive a wind-like outflow, and — under a standard 10% radiative efficiency — reproduce the observed ~10-20% QPE duty cycle, 10^42-10^43 erg/s luminosities, and ~3x10^6 K temperatures, independent of orbital period. The paper is the numerical-simulation counterpart to the Linial, Metzger and Quataert (2025) analytic model.

## Summary
This is "Paper II" of the Yao/Quataert/Jiang program that argues QPEs are not powered by direct star-disk crossings but by follow-up collisions between tidally sheared stellar debris and the disk. Paper I (Yao et al. 2025, 2D, no BH gravity) established the mass-stripping rate per collision and argued qualitatively that a tidal stream would form and dominate the emission; Linial, Metzger and Quataert (2025) built that qualitative picture into an analytic light-curve model. Paper II now supplies the 3D hydrodynamic simulations: three orbital separations (a/rt = 3.5, 5, 8; P_orb = 18, 31, 63 hr), a custom potential module for tidal + Coriolis + centrifugal forces in the star's rotating frame, and a thickened Gaussian disk repeatedly reintroduced every half-orbit to fight numerical diffusion. Passive scalars track shocked stellar vs disk mass. Key quantitative outputs: ~10^-4 M_sun stripped per collision (unchanged from Paper I); a few percent of the shocked debris exceeds 2v*^2 and becomes unbound; stream-axis scaling in Hill-sphere units is nearly self-similar in a/rt; the ratio of shocked disk to shocked star energy climbs steeply toward short periods and becomes comparable at a/rt = 3.5. From those, they infer flare durations 2.5-5.2 hr giving 8-14% (1 flare/orbit) or 16-27% (2/orbit) duty cycles — matching the observationally constant ~10-20% across a decade in period.

## Strengths
- Genuine 3D hydro with the BH tidal potential and Coriolis force — the essential physics the Paper I 2D setup deliberately omitted.
- Fills the gap between Paper I's mass-stripping calibration and Linial+2025's analytic radiation model with a numerical prediction of stream geometry, mass and shocked energetics.
- Duty-cycle prediction is well-posed and quantitatively agrees with observation across two decades in P_orb without period-dependent tuning.
- Honest with limitations: numerical diffusion in the disk is estimated at ~50% and they refuse to plot the shocked-disk mass evolution because of it.
- Directly engages the recent critiques of star-disk models (Guo & Shen 2026 arXiv:2504.12762; Mummery 2025 arXiv:2504.21456) and shows how the debris-stream variant addresses the mass budget objection.

## Weaknesses
- No radiation transport. Flare luminosities are inferred from shocked mass times an assumed efficiency of 0.1 — the actual light curve shape, spectrum and hard/soft asymmetry are not predicted. The Vurm-Linial-Metzger 2025 (arXiv:2410.05166) and Huang-Linial-Jiang 2025 (arXiv:2506.11231) 2D rad-hydro branches are not merged in here.
- Only circular orbits and one stellar model at one SMBH mass. The eccentric-orbit long-short pattern, which is the primary observational discriminator invoked against pure star-disk collision models (Franchini+ 2023, Chakraborty+ 2025), is deferred.
- Disk is artificially thickened by ~4x to combat diffusion. Since disk scale-height controls the collision cross-section and the shock geometry, the extrapolation to real thin disks is not trivial.
- Star sits fixed at the origin; the frame co-rotates. So global disk depletion, refilling, warp and precession — the timescales that produce super-periods (Chakraborty+ 2024/2025) — cannot be captured.
- The one-vs-two-flares-per-orbit conclusion contradicts the O-C timing of eRO-QPE2 (Arcodia+ 2026), which the authors acknowledge but do not resolve.

## Novelty Cross-Check
Self-assessment (verbatim from the introduction):

> "Our initial calculations in Yao et al. (2025) did not include the black hole's tidal gravity, but we argued that its influence would lead to a tidally stretched debris stream that would dominate the radiation in star-disk QPE models. Linial et al. (2025) then developed this into an analytic model of QPE flares. The goal of this paper is to build on the debris-disk collision model proposed in Yao et al. (2025) and explored analytically in detail in Linial et al. (2025). ... Compared to our previous set of 2D simulations presented in Yao et al. (2025), in addition to the extra dimension, we include the following additional physics: The tidal potential of a 10^6 M_sun SMBH, including the centrifugal and Coriolis forces in the co-rotating frame of the star and the BH; The Keplerian rotation of the accretion disk, and its tilt relative to the stellar orbital plane; A realistic orbital period as a function of the orbital distance to the SMBH."

And from the summary: *"To the best of our knowledge, this is one of the few QPE models that are able to explain this remarkable regularity of the observed duty cycle in QPEs."*

Predecessor cross-check:
- **Yao et al. 2025 (Paper I, arXiv:2407.14578)**: 2D Athena++, no BH gravity, star fixed with a symmetric disk. Established that mass stripping saturates after several collisions at ~10^-4 M_sun, argued that circularization shocks — not direct impacts — dominate emission. Paper II delivers the follow-up simulations Paper I explicitly promised.
- **Linial, Metzger & Quataert 2025 (arXiv:2506.10096)**: Purely analytic; treated stream tidal stretching, half-orbit later stream-disk impact, thermal/radiation-mediated shock. Predicts 10^42-10^43 erg/s, ~100 eV; Paper II now supplies the numerically-measured stream mass/geometry inputs those analytics needed.

Novelty claim is honest. Paper II is not a repackaging — it introduces the essential SMBH tidal + Coriolis physics missing from Paper I and quantifies stream properties that Linial+2025 had to parametrise.

## Relevance to Witzany
Directly on-target for Witzany's active QPE work. QPEs as stellar EMRI EM counterparts is the central framing; the paper explicitly invokes "The star plausibly originates from an extreme mass-ratio inspiral (EMRI) produced by Hills breakup of a tight binary on an initially highly eccentric orbit, later circularized by gravitational waves (GWs) and disk drag". It confronts the same population of sources any competing star-through-disk model must address (GSN 069, RX J1301.9, eRO-QPE1/2, AT2019qiz, Ansky, AT2022upj). The Linial-Metzger-Quataert-Yao axis is the natural comparison line to any independent EMRI+disk QPE model. Read fully.

**Collaborator flags:** Tier 1: Itai Linial (co-author, direct competitor/collaborator in the EMRI+disk QPE model space), Eliot Quataert. Tier 2: Yan-Fei Jiang, Philippe Yao.

## Quality Score
- Overall: 8.5/10
- Direct relevance: 10/10
- Novelty: 8/10
- Technical rigor: 8/10

**Tier:** Must-Read

**Collaborator flags:** Linial (Tier 1), Quataert (Tier 1), Jiang, Yao (Tier 2).
