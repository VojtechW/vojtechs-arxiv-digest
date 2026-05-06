# 🧩 Beyond the separatrix: analytic continuation of Darwin variables for plunging geodesics in Schwarzschild

**Authors:** Francisco M. Blanco  
**arXiv:** [2604.28140](https://arxiv.org/abs/2604.28140) [gr-qc, astro-ph.HE, astro-ph.SR]  
**Date:** April 2026  
**Categories:** gr-qc, astro-ph.HE

---

## Summary

Darwin variables (semi-latus rectum p, eccentricity e) parametrize bound Schwarzschild geodesics elegantly but become singular at the separatrix (where the orbit transitions from bound to plunge). Below the separatrix, real Darwin parameters are not defined: the radial motion has no two distinct turning points. Blanco constructs an *analytic continuation of the Darwin variables into the complex plane* that yields, when restricted back, a real and *smooth* parametrization that crosses the separatrix into the plunge regime. The key technical content is to identify the right complex-plane Riemann sheet and the resulting unified, single-phase description of bound, marginal, and plunging orbits in Schwarzschild.

A simple toy application demonstrates that the parametrization remains usable when external (model) forces drive an orbit across the separatrix.

## Strengths

- **Genuinely original idea.** The Cutler-Kennefick-Poisson plunge paper (1994) treats the plunge in (E, L) space; Hopper et al. studied near-separatrix dynamics; van de Meent constructed inhomogeneous solutions. None of these introduce the analytic-continuation-of-(p, e) trick. The conceptual move is small but new.
- **Elegant unification.** A single phase variable describing all orbital regimes is structurally clean and likely useful for action-angle / Hamilton-Jacobi-style work.
- **Tier 2 collaborator.** Blanco is on the close-community list; we should track his trajectory.
- **Toy radiation-driven model included.** The paper does take the small step of letting the orbit evolve through the separatrix under an external force, which is the practical use case.

## Weaknesses

- **Schwarzschild-only.** Kerr is where the analytical structure is interesting (resonances, prograde/retrograde, inclined orbits, near-extremal limit). The Schwarzschild restriction limits direct EMRI applicability. Authors flag Kerr as future work; until that's done, the paper is a proof-of-concept.
- **No back-reaction.** The toy force is generic, not the gravitational self-force. So the practical utility for waveform-modelling self-force pipelines is presently aspirational.
- **No comparison with existing parametrizations.** A direct numerical comparison against (E, L_z) integrators or geodesic-action expansions in the regions where both apply would calibrate efficiency vs. accuracy claims.
- **Computational advantage not demonstrated.** The reader is left wondering whether this is *just* mathematically nicer, or actually computationally cheaper / more stable.

## Relevance to Vojtěch

**Moderate-to-high.** The analytical-structure aspect aligns with Vojtěch's interests in action-angle methods, integrability, and clever closed-form parametrizations. Blanco being on the close-collaborator list also makes this worth following. Direct use is bounded by the Schwarzschild restriction, but the conceptual advance points the way to a Kerr generalization.

## Quality / Verdict

- **Quality:** 7/10
- **Relevance:** 7/10 (would jump to 9 with a Kerr generalization)
- **Survives critical review:** **Yes.** Mathematically clean, conceptually new, and a natural seed for Kerr extensions and self-force–driven evolution through the separatrix.
