# 🎯 Not All Resonances Are Created Equal: Prioritizing Tidal Resonances in EMRIs

**arXiv:** [2609.03732](https://arxiv.org/abs/2609.03732)
**Authors:** Béatrice Bonga, Patrick Bourg, Bram ten Brink, H. A. (Bart) Peters
**Categories:** gr-qc
**Quality:** 7/10 · **Relevance:** 9/10 · **Verdict:** Must-Read

---

## One-line
When a distant star or black hole tugs on a small body inspiralling into a supermassive black hole, it occasionally kicks the orbit at "resonances"; this paper maps out where all such kicks occur across orbit space and ranks the few that actually matter for LISA waveforms.

## Summary
Working in the weak-tide, three-body hierarchy with the perturber held **stationary** over the resonance crossing, the authors systematically survey tidal resonances for generic Kerr orbits. For a family of (n, k, m) triplets (mainly n = 3, 4) they compute (i) resonance contours in (p, e, x), (ii) resonance durations T^res_nkm = √(4π/((μ/M)|Γ_nkm|)), and (iii) jump amplitudes in L_z and Q (with ΔE = 0 enforced by time-translation symmetry, verified consistent with numerical noise). Durations are obtained from FEW using both exact-Kerr (equatorial only) and PN5 flux modules; low-spin resonances last ~10× longer than high-spin, n = 3 ~10× longer than n = 4, retrograde ~10× longer than prograde. A computational shortcut computes h_μν from **Schwarzschild** tidal perturbation theory (lightcone gauge) while keeping **Kerr** geodesics, giving a 20–50× speedup with jump-amplitude agreement ≲ 0.1% (up to ~1% at high e) for the tested (3, 0, −2) mode. Ranking by the phase-independent product (jump × duration), the dominant prograde modes are (3, −1, −1) and (3, 0, −2), with (3, −3, 1), (4, −1, −1), (4, 0, −2) a secondary tier; retrograde shifts to (3, −1, 1), (3, 0, 2). Jumps grow steeply as e → 1 and vanish as e → 0. All contour/jump data are released publicly, aimed at integration into FEW/LISA pipelines.

## Strengths
- **Genuinely comprehensive parameter-space survey** (generic Kerr, spins 0.1/0.5/0.9, full (p, e, x), many (n, k, m)) where prior work gave single examples or population statistics — plus a public data release with a concrete engineering path into FEW.
- **Honest, well-quantified approximation control:** the Schwarzschild-tide-on-Kerr-geodesic hybrid is validated at ≲ 0.1–1% against Kerr tidal theory at the gauge-invariant jump level; the dual Kerr/PN5 duration computation cross-checks itself; a "two-for-one" relation is used as an independent check.
- **Physically sensible ranking** with a clear caveat that it is an efficiency guide, not a hard truncation, because the phase e^{iχ} can make "modest" resonances matter indirectly.
- Clear, well-organized writing with explicit statements of what is deferred.

## Weaknesses / caveats
- **The stationary-perturber approximation is load-bearing**, and the authors themselves flag that relaxing it "introduces a qualitatively new structure" (up to two resonances per (n, k, m, s) and a more complex forcing) — so the entire ranking could reshuffle in the realistic dynamic case (deferred to a paper "in preparation"). The ranking's shelf life is uncertain.
- **No observable is actually computed:** the jumps in L_z and Q are never translated into waveform dephasing (radians), a mismatch, or a LISA SNR/detectability threshold. "Potentially detectable" and the whole prioritization rest on the phase-independent proxy.
- **Several acknowledged unexplained features:** jumps vanish for circular orbits ("we do not have a rigorous explanation"); a PN5 duration spike near e ≈ 0.35 at a = 0.9 ("could not pin down its precise cause"); the spin/inclination dependence pattern of jumps "is not yet understood."
- **Approximation stacking** (stationary tide + leading electric-quadrupole tidal field + Schwarzschild h_μν on Kerr geodesics + phase-independent ranking); each is individually defended, but combined error is not propagated.
- Numerical accuracy degrades at high e and high a — precisely where jumps are largest and most consequential.
- Incremental in method: it operationalizes effects established by Bonga–Yang–Hughes and Gupta et al. rather than introducing new dynamics.

## Novelty context
Tidal resonances were introduced by Bonga, Yang & Hughes 2019 ([arXiv:1905.00030](https://arxiv.org/abs/1905.00030)); Gupta, Bonga, Chua & Tanaka 2021 ([arXiv:2104.03422](https://arxiv.org/abs/2104.03422)) and Gupta, Speri, Bonga, Chua & Tanaka 2022 ([arXiv:2205.04808](https://arxiv.org/abs/2205.04808)) argued for their importance and began modeling them; the "two-for-one" ΔQ–ΔL_z relation is from the latter. What is new here is (a) a systematic contour+duration+jump survey across the full generic-Kerr (p, e, x) space for a whole (n, k, m) family, (b) an explicit tiered ranking for pro/retrograde orbits, (c) the Schwarzschild-tide-on-Kerr-geodesic speed hack that also captures m = 0 modes, and (d) a public dataset built for FEW ingestion. A consolidation/engineering advance, not a conceptual one.

## Relevance to Vojtěch
**Axis 1** (core), directly. Orbital resonances in EMRIs, generic Kerr geodesics, Carter-constant Q jumps, radiation-reaction-driven transient resonances, and FEW integration are squarely his territory. The paper also explicitly motivates via QPEs and Sgr A* faint stars.

## Where to start
Sec. 2.3–2.5 (resonance condition, the stationary and Schwarzschild-tide approximations — the key modeling assumptions and their justifications), then Sec. 6 (Discussion — the ranking and the crucial dynamic-perturber caveat), then skim Sec. 4–5 for the duration/jump trends and tier tables.

*In network:* 🚩 Béatrice Bonga, 🚩 Patrick Bourg (extended-network collaborators).
