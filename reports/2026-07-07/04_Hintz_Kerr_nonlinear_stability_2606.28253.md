# 🌟 Nonlinear stability of subextremal Kerr black holes

**Authors:** Peter Hintz
**arXiv:** [2606.28253](https://arxiv.org/abs/2606.28253) · gr-qc, math.AP · 333 pp, 18 figures
**Submitted:** 26 Jun 2026

## Summary
A 333-page monograph claiming to settle the global nonlinear stability of the Kerr family in the **full subextremal range** |a|<M, showing that vacuum spacetimes evolving from data close to Kerr settle to a nearby Kerr member at rate O(t*⁻²⁻ᵋ) in compact regions. The proof uses a generalized wave-map gauge with finite-dimensional gauge source terms (extending Hintz–Vasy's Kerr-de Sitter strategy), treats final-state parameters, gravitational wave tails, and gauge sources as unknowns in a **Nash-Moser iteration**, and works **directly with the tensorial Einstein equation** rather than reducing to scalar equations (except invoking Teukolsky for linear mode stability).

## Genuinely New?
Yes — this is the first proof valid for **arbitrary** subextremal a/M. Prior full-vacuum Kerr nonlinear stability results (Klainerman–Szeftel 2104.11857 + 2205.14808; Giorgi–Klainerman–Szeftel series) were restricted to **|a|/M ≪ 1** and used a Newman–Penrose/Teukolsky-based approach with GCM spheres. Dafermos–Holzegel–Rodnianski–Taylor (arXiv:2104.08222) handled **Schwarzschild only** (a=0). Extending past |a|/M ≪ 1 was the outstanding barrier due to loss of ergoregion smallness and mode-coupling; Hintz's route is fundamentally different in gauge philosophy and analytic machinery.

## Strengths
- **Full subextremal range** — the target that has been the community's holy grail since ~2000.
- Gauge-fixed tensorial formulation avoids fragile scalar decoupling, arguably more robust.
- Modular architecture: builds on Häfner–Hintz–Vasy linear stability (arXiv:2506.21183), Andersson–Whiting–Häfner mode stability, and Hintz's own quasilinear wave analysis (arXiv:2410.03639).
- Nash-Moser handles the derivative-loss problem elegantly (as in Hintz-Vasy Kerr-de Sitter).

## Weaknesses / caveats
- **The proof relies on two explicit companion papers.** One (arXiv:2606.27658, constraint damping) posted the same day and appears self-contained. The **second companion**, providing tame estimates for a class of wave-type equations, is referenced as "by the author" — a stand-alone preprint number was not clearly locatable at the time of writing. This gates completeness; the result is only as sound as that companion.
- Single-author, 333 pages, released only ~11 days ago. No independent verification, no seminar circulation trail. Klainerman–Szeftel and DHRT proofs took years of scrutiny; expect the same.
- Priority/independence dispute with Klainerman–Szeftel remains a sensitive backdrop (cf. Dafermos' 2023 note).

## Relevance to Vojtěch
**Limited direct utility for self-force/EMRI work.** This is a global nonlinear PDE result about the vacuum Einstein equation; it does not produce new tools for waveform generation, geodesic dynamics, or Teukolsky mode computation. However, it **rigorously justifies** the physicist assumption that Kerr is an attractor and quantifies the tail decay (t*⁻²⁻ᵋ) — physically meaningful for late-time ringdown asymptotics and for the well-posedness of "small perturbation of Kerr" underlying all EMRI/self-force computations. Landmark status warrants awareness even without technical uptake.

## Scores
- **Quality: 9/10** (contingent on the second companion appearing and holding up). Architecturally coherent, extends a proven Hintz–Vasy program, methodologically the cleanest route to full subextremality on the table.
- **Relevance: 3/10** — foundational not operational for Vojtěch's physics program.
- **Verdict: Should-Read (landmark).** Genuinely landmark **if the tame-estimates companion delivers.** Not yet fully self-contained on arXiv — verify the second companion before citing as definitive. Skim intro (§1) and the "companion papers" section only.

## Collaborator flags
None. Landmark mathematical-GR result.
