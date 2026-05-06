# 🪄 Regularized Teukolsky Green Function in Schwarzschild

**arXiv:** [2604.21219](https://arxiv.org/abs/2604.21219)
**Authors:** David Q. Aruquipa, Marc Casals, Brien C. Nolan
**Categories:** gr-qc, hep-th
**Quality:** 7/10 | **Relevance:** 8/10

---

## Summary

The authors construct the Hadamard form of the retarded Green function for the spin-weight s=−2 Bardeen–Press / Teukolsky equation on Schwarzschild, working on the conformally related product spacetime ℳ₂ × 𝕊². In this conformal frame the singular (direct) part of the Hadamard parametrix factorizes cleanly: the angular factor reduces to an explicit combination of spin-weighted spherical harmonics and Euler angles, and the radial / temporal piece is a spin-dependent transport-equation factor times the square root of the van Vleck determinant. Multipole-mode decompositions are given for spin-1 (electromagnetic) and spin-2 (gravitational) perturbations, and the retarded-minus-direct ("tail") expression is shown to give a better practical representation near coincidence than previously available.

## Strengths

- **Closed-form direct part.** The factorization on ℳ₂ × 𝕊² turns a notoriously messy parametrix into something whose angular and radial structure is genuinely under analytic control. This is exactly the kind of structural result that the self-force community has been asking for.
- **Established team.** Casals is a leading figure in Hadamard regularization for self-force; Nolan is a long-time collaborator on quasilocal expansions. The technical machinery is mature.
- **Explicit ℓ-mode decomposition** at both spin-1 and spin-2 — directly usable as input to mode-sum regularization or as a benchmark for puncture / effective-source methods.
- **Tail-only Green function.** Subtracting the direct part yields an object that should be much better behaved near coincidence than the full retarded Green function — a real numerical benefit for time-domain self-force codes.

## Weaknesses

- **Schwarzschild only.** The whole point of the EMRI program is Kerr. The conformal trick that gives ℳ₂ × 𝕊² product structure on Schwarzschild does not survive on Kerr, and the paper does not (from the abstract) sketch how the construction would generalize. This is the elephant in the room.
- **Constant-radius worldlines.** Results are stated for circular timelike orbits and static worldlines. Eccentric orbits — which is where the puncture/mode-sum infrastructure is being most actively pushed in 2024–2026 — are out of scope.
- **Computational tractability not demonstrated.** The Hadamard parametrix is formal; the practical question is whether the new closed-form expressions outperform existing puncture / effective-source schemes (Bourg, Wardell, Pound) in actual self-force runs. No timings, no convergence diagnostics, no comparison.
- **Unclear positioning vs. recent Casals work.** Casals has produced several Hadamard / global-Hadamard papers in the last 5 years. The relationship to those (especially Casals 2023, *Phys. Rev. D* 108:044033) is not made fully explicit in the abstract.

## Relevance to Vojtěch

Direct: Teukolsky equation, BHPT, self-force regularization. Casals is a familiar name in the self-force community. The result, while restricted to Schwarzschild, gives a structural factorization that may serve as a template for Kerr work and is exactly the sort of analytic backbone Vojtěch likes for self-force infrastructure.

**Score: Relevance 8/10, Quality 7/10.**

## Verdict

**Should-Read.** This is a rigorous, well-executed analytic result by a credible team that fills a real gap in Hadamard regularization for the Teukolsky equation. Read for the factorization structure (which may suggest how to attack the Kerr case via Killing tensor / hidden-symmetry decomposition) and for the explicit angular factor, which is the most concrete deliverable. Pair with [Bourg et al. 2024](https://arxiv.org/abs/2402.06622) for context on the puncture-scheme alternative.

## Caveats / Collaborator Flags

- No direct Tier-1/Tier-2 author hits, but Casals is a long-standing self-force community figure adjacent to the Tier-2 set (Wardell, Pound, Warburton).
