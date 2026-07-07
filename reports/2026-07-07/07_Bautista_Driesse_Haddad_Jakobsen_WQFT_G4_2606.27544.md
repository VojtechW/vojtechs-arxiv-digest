# 🪛 Gravitational wave scattering at O(G⁴): Murua construction and elliptics

**Authors:** Yilber Fabian Bautista (T3), Mathias Driesse, Kays Haddad, Gustav Uhre Jakobsen
**arXiv:** [2606.27544](https://arxiv.org/abs/2606.27544) · hep-th · 7 pp, 2 figures
**Submitted:** 25 Jun 2026

## Summary
The authors compute the amplitude for a gravitational wave scattering off a spinless point-particle at O(G⁴) (three-loop) in worldline QFT (WQFT), and match the resulting Magnusian phase shift to Schwarzschild BHPT for partial waves ℓ = 2–20 to relative precision 10⁻³⁴. Two technical innovations are advertised: (i) a **Murua construction** that replaces cut-subtraction with weighted causal-prescription combinations at the master-integral level, and (ii) the first appearance of elliptic integrals (complete K, E of a kinematic modulus obtained from a Picard–Fuchs equation) in momentum-space graviton-off-BH scattering.

## Genuinely New?
Partially. The Murua-weighted decomposition is a real technical improvement over their own earlier cut-subtraction procedure (ref. [38]): it commutes with IBP, so one no longer has to subtract cuts diagram-by-diagram. The elliptic-in-momentum claim is qualified in a footnote: Isabella (Correia–Isabella group) has parallel results for scalar-wave scattering, and elliptics at G⁴ in the two-body problem are well established (Klemm–Nega–Sauer–Plefka). So this is the first WQFT graviton-scattering appearance, not a truly first-of-its-kind discovery. The BHPT match at G⁴ extends prior WQFT–BHPT agreement by one PM order for the wave-scattering (not two-body) observable.

## Strengths
- Clean separation of causality-prescription combinatorics from IBP is genuinely useful and will likely be adopted by the WQFT community.
- 10⁻³⁴ numerical agreement (analytic-vs-analytic, in a polynomial in ℓ(ℓ+1)) constitutes essentially a proof of equivalence at fixed ℓ.
- Picard–Fuchs derivation of the elliptic sector is transparent; canonical DE form allows high-precision AMFlow boundary evaluation.
- Clear roadmap to spin (G⁵, Kerr, Wilson coefficients).

## Weaknesses
- The BHPT match is a consistency check, not a validation: WQFT is the calculator, BHPT is the known target. Dissipation only enters at O(G⁵), so this G⁴ test is purely conservative and cannot distinguish subtle worldline actions.
- Only the Magnusian phase shift is compared; the amplitude-level match is deferred (one M^(2,1) coefficient not reconstructed).
- "First appearance" of momentum-space elliptics is footnoted as parallel to Isabella's scalar-wave result — the framing in the abstract is stronger than the qualified claim in the body.
- Spinless, extreme mass-ratio only. No self-force expansion beyond leading test-particle limit.
- Numerical ℓ-check up to 20 only, no analytic all-ℓ proof (though for a polynomial in L this is effectively airtight).

## Relevance to Vojtěch
Directly relevant. The G⁴ spinless test-particle wave-scattering phase shift is exactly the regime BHPT/self-force practitioners compute rigorously; this paper is a WQFT-side handshake with that community. The Murua construction is likely to spread into WQFT calculations. However, the paper does not feed information back into BHPT — no new BHPT prediction, no new self-force result. For the EMRI/BHPT program specifically, this is a validation from the amplitudes side rather than a new input.

## Scores
- **Quality: 8/10** — technically sharp, honestly qualified in the body; the elliptics-novelty framing in the abstract slightly overreaches.
- **Relevance: 6/10** — of interest for the WQFT–BHPT crosswalk, but no new BHPT-side content.
- **Verdict: Worth-Skimming.** Legitimate, incremental technical letter. The Murua construction is the durable contribution; the elliptics claim is real but hedged.

## Collaborator flags
Yilber Fabian Bautista (T3).
