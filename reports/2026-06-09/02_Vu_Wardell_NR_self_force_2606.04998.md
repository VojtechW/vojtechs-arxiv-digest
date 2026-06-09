# 🪛 Vu, Nishimura, Osburn, Thompson, Kidder, Upton, Wardell — Self-Force Calculations with Numerical Relativity Methods

**arXiv:** [2606.04998](https://arxiv.org/abs/2606.04998)
**Categories:** gr-qc
**Length:** 19 pages, 7 figures (reproducible ancillary input files)
**Recommendation:** Should-Read · **Quality:** 7/10

## Summary

The SpECTRE collaboration adapts its elliptic NR initial-data infrastructure (discontinuous-Galerkin + hp-adaptive mesh refinement + multigrid–Schwarz preconditioned GMRES) to the *m*-mode scalar self-force problem on circular equatorial Kerr orbits, achieving exponential convergence and reaching the Thorne limit a/M = 0.998. The open-source release inside SpECTRE positions this as the infrastructure layer for upcoming gravitational + second-order SF on the same backbone.

## Key Results

- Scalar charge on circular equatorial Kerr orbits, prograde and retrograde, down to ISCO, |a|/M up to 0.998.
- Exponential convergence in number of grid points despite the non-smooth puncture solution.
- ~ few seconds per *m*-mode on an Apple M2 Pro laptop; 20 *m*-modes computed in parallel.
- Numerical resolution error driven well below *m*-truncation error; validation against Warburton & Barack reference values.
- Technical engineering: complex-valued GMRES with complex-shift preconditioning for Helmholtz-type problems; "vtu" piecewise-constant null slicing in horizon-penetrating coordinates.

## Strengths

- Honest, explicit comparison with Macedo et al. (hyperboloidal *m*-mode); credits inspiration and identifies what is new vs. inherited, even conceding the rival's "arguably more elegant" coordinate map.
- Reference benchmarking against established solutions; quantitative error budget separated into resolution and truncation contributions.
- Real engineering content (complex-shift preconditioner, additive Schwarz multigrid, LU factorisation caching across AMR iterations) — reusable downstream.
- Open-source release in SpECTRE.
- Realistic scope statement: scalar, circular, Kerr → gravitational + eccentric + 2nd-order is the explicit roadmap.

## Weaknesses

- Scalar field, circular equatorial Kerr in 2026 — the genuinely hard problems (Lorenz-gauge metric perturbation, eccentric/inclined orbits, 2nd-order source construction) are explicitly deferred. The headline promises more than this paper delivers.
- No quantitative head-to-head on identical configurations against Macedo et al. — qualitative comparison only.
- Reaching a/M = 0.998 is impressive in spin coverage but trivial for a scalar field (no qualitatively new regularity behaviour at near-extremality).
- "Few seconds per *m*-mode on a laptop" without FLOP/CPU-time comparison to FD *m*-mode codes; comparable codes might be similarly fast.
- No quoted phase agreement over LISA-relevant inspiral durations.

## Relevance to Vojtěch

Wardell is a Tier-2 collaborator. The current scalar/circular content is not directly usable for Vojtěch's spinning-particle or PN-Kerr work, but this is the *infrastructure paper* signalling where the Wardell–Pound–Upton program is going. The forthcoming gravitational and second-order results from this SpECTRE pipeline will likely be must-reads. The DG + hp-AMR architecture is also relevant context for anyone planning numerical SF computations against EOB/PN benchmarks.

## Honest Assessment

A solid, careful infrastructure paper from a strong collaboration. Properly benchmarked, honest about scope. Not field-changing on physics content, but the methodology and open-source release set the stage for the next wave of Kerr SF results. Read the introduction, §VI (comparison with Macedo et al.), and skim the solver section.
