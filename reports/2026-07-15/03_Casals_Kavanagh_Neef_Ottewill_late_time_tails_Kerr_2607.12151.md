# 〰️ High-order gravitational late-time tails in Kerr spacetime

**Citation:** Marc Casals, Chris Kavanagh, Jakob Neef, Adrian Ottewill, *High-order gravitational late-time tails in Kerr spacetime*, arXiv:[2607.12151](https://arxiv.org/abs/2607.12151) [gr-qc, hep-th], 13 Jul 2026.

## Executive Summary
Analytical extension of the authors' 2016 scalar-field programme (arXiv:1608.05392) to gravitational (s=−2) perturbations of subextremal Kerr, delivering the first three orders in the late-time expansion of the Teukolsky retarded Green function — at finite radius, on H⁺, and on ℐ⁺. The tail powers are given for generic integer spin; the coefficients are new for s=−2. Technically demanding, systematic small-frequency computation with Mathematica notebooks attached — the natural culmination of the Casals–Ottewill programme applied to physical gravitational perturbations.

## Key Contributions
- **First analytic gravitational (s=−2) tail coefficients** for Teukolsky retarded Green function in Kerr, to three orders, for arbitrary ℓ,m.
- Explicit **logarithmic corrections** at second/third order: t^(−2ℓ−5) ln t (interior), v^(−2ℓ−5−b) ln v with m-dependent b-shift on H⁺, and u^(−ℓ+s−3) ln u plus u^(−ℓ+s−4) ln²u on ℐ⁺.
- Tail power laws given for generic integer spin s — clean uniform statement across scalar, EM and gravitational sectors including the m=0 anomaly on the horizon.
- Full-Green-function decay laws for s=−2 (not just fixed-mode), obtained by summing over ℓ,m.
- **Small-frequency expansions** of MST-type scattering data (Wronskians, transmission/reflection coefficients) that are of independent interest for self-force and GSF work.
- Two supplementary notebooks: generic-ℓ expansions to three orders and arbitrary-order expansions at fixed ℓ.

## Strengths
- Clean, systematic MST small-frequency machinery — a mature technique whose 2016 scalar predecessor has held up against later numerical work (Csukás–Rácz 2404.13447; Burko–Khanna 1905.09082).
- Delivers **explicit coefficients**, not just decay powers — enables cross-checks with time-domain solvers and self-force Green-function reconstructions.
- Covers all three physical asymptotic regions (finite r, H⁺, ℐ⁺), whereas most prior analytic work stuck to a single region.
- Handles Kerr's spheroidal structure at generic (ℓ,m) rather than only axisymmetric.

## Weaknesses
- Only **three orders** for s=−2 (versus five orders for the 2016 scalar case) — the group presumably hit the same combinatorial wall; the paper's marginal analytic reach is thus incremental.
- No comparison to (or absorption of) the **nonlinear/sourced tails** now dominating the ringdown literature (Ma–Zhang 2603.20379, Cardoso et al. 2407.04682, 2511.21898). Linear tails are quickly becoming a niche next to nonlinear ones; the paper does not engage this shift.
- s=−1 (EM) coefficients are conspicuously absent despite the "generic s" framing — reads as a completeness gap rather than a principled choice.
- Practical observational impact stays limited: the higher-order log corrections live many decades below leading QNM+tail signals detectable by LIGO/LISA.

## Relevance to Vojtěch
Squarely in-scope: Teukolsky equation, Kerr perturbation theory, and MST-type small-ω expansions are core self-force machinery. The small-frequency expansions of scattering data and the explicit s=−2 Green function are directly reusable in self-force Green-function methods, quasilocal-plus-tail decompositions, and the near-static piece of ω-mode computations that arise in spinning-particle and eccentric-orbit self-force. Not an EMRI paper per se, but foundational Teukolsky infrastructure Vojtěch's collaborators actually use.

## Scores
- **Quality:** 8/10 — rigorous, extensive, coefficient-level results; but limited to 3 orders and side-stepping nonlinear tails.
- **Relevance:** 8/10 — Teukolsky Green function + small-ω Kerr scattering data.

## Verdict
🌠 **Should-Read** — mine the small-frequency scattering-data section and the notebooks; the tail asymptotics themselves can be skimmed unless a specific application needs the coefficients.

## Collaborator flag
**Chris Kavanagh** — Tier-2.
