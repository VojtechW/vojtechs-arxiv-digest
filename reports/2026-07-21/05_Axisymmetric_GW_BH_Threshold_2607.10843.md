# 🌊 Comparing Twist-Free Axisymmetric Gravitational Waves Near the Black Hole Threshold

**arXiv:** [2607.10843](https://arxiv.org/abs/2607.10843)
**Authors:** Ananya Adhikari, Tomáš Ledvinka, Daniela Cors, Thomas W. Baumgarte, Anton Khirnov, Bernd Brügmann, David Hilditch
**Category:** gr-qc
**Submitted:** 2026-07-12

## TL;DR
Extended follow-up to the 2023 PRL (Baumgarte et al., 2305.17171) three-code comparison of vacuum axisymmetric collapse. New material: off-center Brill waves in the `prague` code, time-asymmetric Teukolsky-based initial data in `bamps`, apparent-horizon comparisons (two AH finders on the same data), and a construction of null "reference coordinates" adapted along the symmetry axis for cross-code comparison of deeply strong-field data. Physics conclusion is honest rather than dramatic: no universal critical solution at current tuning, but excellent agreement in gauge-invariant quantities across three independent codes.

## Summary
Three independent NR codes — `bamps` (adaptive-multidomain pseudospectral, first-order generalized-harmonic, cartoon 2+1), `prague` (Cactus/ET-derived, BSSN with quasi-maximal slicing, FMR, cartoon), and `sphGR` (spherical polar, 8th-order finite-differencing, BSSN with shock-avoiding Bona-Massó) — are compared on near-threshold vacuum axisymmetric collapse across four families of initial data: centered Brill (A>0, A<0), off-center Brill, and time-asymmetric Teukolsky-based (Ledvinka-Khirnov 2021). Best tuning: ~7 decimal places (well short of the 12+ decimals routine in spherical work). Key results: (i) Kretschmann-scalar scaling with family-dependent exponents and periods — no universality; γ_TA ≈ 0.51 in the near-tuned regime, γ_B ≈ 0.23 in near-tuned Brill; (ii) time-asymmetric data show *no* accumulation of curvature peaks at the origin, unlike A<0 Brill — undermining the DSS-at-origin picture; (iii) two independent apparent-horizon finders (shooting and flow) agree on identical data; (iv) a family-dependent gauge failure in `bamps` (a "gauge G1" fails in a subcritical window; alternative G2 heals it but fails closer to threshold) — flagged honestly as a lesson for future improvement; (v) `prague` shows late-time noise from mesh-refinement boundaries, another honest self-critique.

## Strengths
- Rare *multi-code* comparison in a subfield where individual codes have historically produced *contradictory* critical exponents. Consensus among independent codes is the main deliverable, and the paper achieves it.
- Time-asymmetric waves are evolved in `bamps` for the first time — a genuine extension, not a redo.
- Table 1 (historical overview of axisymmetric-wave collapse simulations, 1978–2026) is a valuable community resource on its own.
- Honest self-critique: authors admit each code's shortcomings (bamps gauge failure window, prague mesh-refinement noise, sphGR origin errors).
- Physics conclusion is nuanced and correct: at current tuning, non-universal power laws and periods persist across families; DSS may exist within a family but not universally.
- Best-tuned bracket ΔA ~ 1.5 × 10⁻⁷ around the time-asymmetric threshold with matching AHs found by two independent AH finders — hard to fake.
- The reference-coordinate construction (single-null / double-null adapted to the central geodesic) for comparing strong-field data across radically different foliations is methodologically well thought-through.

## Weaknesses
- Still limited to ~7 decimals of tuning, whereas spherical Choptuik reaches ~15 — so "no universality" conclusions come with the disclaimer "at current level of fine-tuning." Paper does not fully close this door.
- Off-center Brill in `prague` is a modest extension of the 2023 PRL scope.
- Not a paradigm shift — this is a consolidation/extension paper, and it is honest about that.
- The gauge G1/G2 story shows the field-dependent fragility of these results — any of the individual numbers should be read as provisional.
- Quantitative disagreement in supercritical AH masses (up to a factor of a few between `bamps` and `prague`) is attributed to foliation dependence, but the reader is left without a foliation-invariant proxy for the initial horizon mass.

## Novelty Cross-Check
Self-assessment (from abstract): "Building on earlier work we provide further details of a comparison between three independent numerical codes… paying special attention to the relative strengths and weaknesses of each and examining various features of near-threshold collapse of vacuum gravitational waves for the first time. In particular, we observe quasi-universal strong-field features appearing in curvature scalars… We evolve, for the first time, time-asymmetric wave initial data within the `bamps` code."

Predecessors:
- **Baumgarte, Brügmann, Cors, Gundlach, Hilditch, Khirnov, Ledvinka, Renkhoff, Suárez Fernández** (2305.17171, PRL 2023): the parent three-code comparison paper. Established the "different families → different exponents" claim in a PRL-length letter. The current paper is the detailed follow-up.
- **Ledvinka & Khirnov** (2102.09579, PRL 2021): non-universal echoes, time-asymmetric initial data introduced. Extended here into `bamps`.
- **Suárez Fernández et al.** (2205.04379): off-center Brill wave evolutions in `bamps` — now cross-checked in `prague` and `sphGR`.

Genuinely new: (a) first time-asymmetric evolution in `bamps`; (b) three-code cross-check on off-center Brill; (c) AH finder cross-checks in supercritical near-threshold spacetimes; (d) construction of null reference coordinates for the time-asymmetric family (in which the assumed-DSS origin-centered coordinates *fail*). Modest but real.

## Relevance to Witzany
Moderate direct relevance:
- **Tomáš Ledvinka is a Prague / Charles University colleague** — direct community relevance for Witzany.
- **Anton Khirnov also at Charles University** — same institute.
- Strong-field / critical-collapse territory is a step removed from Witzany's EMRI/self-force core, but overlaps with his broader GR interests (curvature invariants, gauge-invariant characterization, coordinate-independent comparisons).
- The null reference-coordinate construction (using a central geodesic + affine parameter) is a technique with echoes in gauge-invariant analytics — worth a skim for the methodology alone.
- No immediate EMRI relevance, but a good "know what the Prague axisymmetric group is doing" data point.

## Quality Score
- Overall: 7.5/10
- Direct relevance: 5/10
- Novelty: 5.5/10
- Technical rigor: 8/10

**Tier:** Should-Read

**Collaborator flags:** Tomáš Ledvinka (Tier 2), Anton Khirnov (Tier 2/3, Charles Univ. Prague)
