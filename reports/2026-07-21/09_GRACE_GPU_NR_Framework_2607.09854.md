# 🖥️ GRACE: An Open-Source Framework for GPU-Accelerated Numerical Relativity

**arXiv:** [2607.09854](https://arxiv.org/abs/2607.09854)
**Authors:** Carlo Musolino, Christian Ecker, Konrad Topolski, Marie Cassing, Keneth Miler, Harry Ho-Yin Ng, Khalil Pierre, Elias R. Most, Luciano Rezzolla
**Category:** gr-qc (+astro-ph.HE)
**Submitted:** 2026-07-10

## TL;DR
Frankfurt/Princeton (Rezzolla/Most) group releases GRACE: a from-scratch, Kokkos+p4est, Z4c-based GRMHD+dynamical-spacetime code. Full validation suite from MHD shock tubes to a magnetized unequal-mass BNS merger, publicly released with post-processing companion GRACEpy. Legitimate infrastructure paper — but arrives into an unusually crowded Kokkos-NR field, and its differentiation from KHARMA / GRaM-X / SACRA-K deserves scrutiny.

## Summary
GRACE couples ideal GRMHD (constrained-transport divergence cleaning) to Einstein evolution in the Z4c formulation. Performance portability via Kokkos, block-structured AMR via p4est. Validation ladder: magnetized shock tubes, magnetic rotor, (magnetized) Bondi accretion onto Schwarzschild, ringdown of a perturbed spinning puncture, TOV oscillation spectra (fixed and dynamical), a BBH merger, an equal-mass unmagnetized BNS with ideal-gas EOS, and an unequal-mass magnetized BNS with a finite-temperature tabulated EOS — inspiral compared against the Rezzolla-group FIL code. Single-device throughput plus strong/weak scaling on multiple GPU and CPU architectures. Public release including analysis/post-processing suite GRACEpy.

## Strengths
- Very broad validation suite ("shock tube to magnetized BNS merger") is exactly what a new NR-GRMHD framework must deliver — not a preliminary announcement.
- The unequal-mass magnetized BNS with finite-T tabulated EOS + cross-check against FIL is a serious application-scale test, not a toy.
- p4est (tree-based AMR) is a legitimate architectural alternative to AMReX/CarpetX (GRaM-X) and box-in-box (SACRA-K, prague); worth having independent implementations.
- Public release with companion analysis package raises the bar for reusability.
- Rezzolla/Most group has strong track record on GRMHD codes (WhiskyMHD, FIL, BHAC lineage).

## Weaknesses
- Field is crowded: KHARMA (2024, Kokkos, stationary GRMHD), GRaM-X (2022, AMReX+CarpetX, dynamical GRMHD), SACRA-K (arXiv:2607.08743, appeared *one day earlier*, Kokkos, BSSN+Z4c, box-in-box AMR). GRACE needs to justify its niche; the abstract does not clearly benchmark against these codes on identical problems.
- No head-to-head throughput comparison against GRaM-X/KHARMA/SACRA-K is advertised in the abstract, only against FIL for physics.
- Only inspiral is compared with FIL — nothing said about post-merger comparisons (typically where GRMHD codes disagree most).
- "Developed from scratch" is oversold as a virtue: it also means every wheel is reinvented and validated independently.
- Full text not accessible via MCP (HTML unavailable, PDF extra not installed), so convergence orders, constraint-violation levels, and p4est-reconstruction interactions cannot be verified here from the abstract alone.

## Novelty Cross-Check
Self-assessment (from abstract): "a new GPU-accelerated numerical-relativity framework designed to run efficiently on heterogeneous high-performance computing platforms. Developed from scratch and built exclusively on open-source libraries…"

Predecessors:
- **GRaM-X** (2210.17509, Shankar+ 2022): first GPU-accelerated *dynamical-spacetime* GRMHD code with AMR, built on Einstein Toolkit + CarpetX + AMReX. Same physics scope (Z4c + Valencia GRMHD, tabulated EOS). GRACE's differentiators: (i) no Einstein Toolkit dependency, (ii) p4est instead of AMReX, (iii) integrated code base rather than plug-in.
- **KHARMA** (2408.01361, Prather 2024): Kokkos-based, but stationary spacetimes only — not a direct competitor for BNS.
- **SACRA-K** (2607.08743, Han/Kiuchi/Shibata, one day before GRACE): Kokkos port of SACRA, BSSN+Z4c, box-in-box AMR, BBH/BHNS/BNS validated. Very close scope.

Genuinely new: the *specific combination* of p4est + Kokkos + Z4c + full GRMHD + BNS-scale validation in a public code, and Frankfurt group's own infrastructure independent of ET. Not paradigm-changing; incremental but useful.

## Relevance to Witzany
Witzany is EMRI / GR-analytics-adjacent, not primarily NR-GRMHD. However:
- A validated, open, GPU-portable NR-GRMHD infrastructure is community infrastructure worth being aware of.
- **Khalil Pierre** (Tier 2 collaborator flag) is on the author list — worth noting personally.
- Not directly usable for EMRI work (no self-force, no perturbation-theory backend), but useful to bookmark for BNS-remnant physics / environmental-effect discussions.

## Quality Score
- Overall: 7/10
- Direct relevance: 3/10
- Novelty: 5/10
- Technical rigor: 7/10 (from abstract; cannot fully verify)

**Tier:** Worth-Skimming

**Collaborator flags:** Khalil Pierre (Tier 2)
