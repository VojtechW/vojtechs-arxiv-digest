# 🎵 Schrödinger Perturbation Theory for Black Hole Quasinormal Modes

**Citation:** Jacopo Lestingi, Laura Sberna, Stephen R. Green, *Schrödinger perturbation theory for black hole quasinormal modes*, arXiv:[2607.19492](https://arxiv.org/abs/2607.19492) [gr-qc] (cross-list hep-th), 21 Jul 2026 (Nottingham Centre of Gravity).

## Executive Summary
The paper lifts textbook (Schrödinger/Rayleigh) perturbation theory to the *non-self-adjoint* quasinormal-mode problem, using the symplectic-current bilinear form under which Kerr QNMs are orthogonal (Green–Hollands–Sberna–Toomani–Zimmerman 2023). It derives a closed formula for the quasinormal-frequency shift at arbitrary order k in a coupling ζ, reducing at first order to the known eigenvalue-perturbation result, and gives a Green's-function spectral decomposition of the first-order mode shift into a discrete QNM sum plus a continuous (branch-cut + arc) piece. The striking result is a *negative* one: the QNM-sum representation of the mode shift is shown numerically to **diverge**, making the incompleteness of the QNM basis explicit rather than hiding it.

## Key Contributions
- An arbitrary-order QNM perturbation formula for Kerr built on the orthogonal bilinear form — the first systematic framework beyond first-order QNM shifts.
- Spectral (Green's-function) decomposition of the first-order mode shift, exposing a "secular-term" projection that has no analogue in ordinary quantum mechanics.
- Explicit numerical demonstration that the discrete-QNM sum for the mode shift diverges (validated on Pöschl–Teller and slowly-spinning Kerr).
- A high-precision second-order check (≈14 significant digits) confirming the formalism where the analytic answer is known.

## Strengths
- Fills a genuinely stated gap: no prior systematic beyond-first-order QNM-shift framework existed.
- Honest negative result — the divergence is presented as the interesting physics, not swept aside.
- Careful reductions and consistency checks, well embedded in the group's bilinear-form program.

## Weaknesses
- The "systematic framework" is partly formal: the new ingredient (the spectral mode-shift sum) diverges and is bypassed, and the continuum regulariser is "challenging to evaluate" and never actually evaluated — practical advice reverts to numerically solving the modified Teukolsky equation.
- Both validations use the *known analytic* mode shift, not one computed from the new decomposition, so the truly novel piece is exactly the part shown to fail.
- Restricted to the non-degenerate, linear-source case; generic beyond-GR sources with m-mixing / degeneracy are deferred, and no new physical QNM shift is actually computed (toy problems only).

## Relevance to Vojtěch
Squarely in Kerr / Teukolsky perturbation theory and uses shared machinery — symplectic current, GHZ/CCK metric reconstruction, hidden-symmetry-flavoured bilinear forms. Adjacent to, but not core to, his EMRI/self-force work; most useful as a conceptual reference on the (in)completeness of the QNM basis.

## Scores
- **Quality:** 7/10 — genuinely new, honestly executed; the central object diverges.
- **Relevance:** 6/10 — Kerr perturbation theory, one step from self-force.

## Verdict
🌠 **Should-Read.**

## Collaborator flag
🚩 **Laura Sberna (Tier 2)** and **Stephen R. Green (Tier 3)** are genuine authors (2 of 3); this is core output of their Nottingham bilinear-form program.
