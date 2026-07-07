# 🎯 Efficient Eccentric Effective-One-Body Dynamics via Near-Identity Averaging Transformations

**Authors:** Philip Lynch, Alessandra Buonanno (T3), Aldo Gamboa, **Maarten van de Meent** (T2)
**arXiv:** [2606.30594](https://arxiv.org/abs/2606.30594) · gr-qc, astro-ph.IM · 29 pp, 13 figures
**Submitted:** 29 Jun 2026

## Summary
The authors recast the non-spinning eccentric SEOB equations of motion in osculating orbital elements and apply near-identity averaging transformations (NITs) to remove the fast orbital-timescale oscillations from the inspiral. The averaged system is evolved on the radiation-reaction timescale, then remapped to full EOB dynamics for the transition to plunge. They report inspiral-cost reductions up to two orders of magnitude, overall waveform speed-ups of 1.5–8×, and demonstrate that NNLO order is required to match comparable-mass mismatches below 8.05×10⁻⁵.

## Genuinely New?
Moderately. NIT in the self-force / EMRI adiabatic-inspiral context is well established (Van de Meent–Warburton; Lynch's thesis; Drummond–Lynch et al. 2023 for spinning-body Kerr). Applying it to non-spinning SEOB is the logical next step; InspireHEP shows no prior Lynch/van de Meent EOB collaboration — so this is the first port. That said: (i) the underlying machinery is imported wholesale from EMRI work, (ii) the "osculating elements + NIT + remap at plunge" mapping is the Lynch-thesis recipe reused in a new Hamiltonian, and (iii) NNLO in EOB is the counterpart of what Van de Meent/Warburton showed is needed for comparable-mass EMRIs. Real, incremental, publishable — but not a conceptual breakthrough.

## Strengths
- Clean problem framing; the bottleneck is real (SEOBNRv5EHM inspiral cost, cf. Gamboa 2024, Pompili 2026).
- Mismatch validation across parameter space is the right test.
- NNLO is well-motivated post hoc: for q~1 the fast-timescale small parameter is not truly small, so higher-order NIT is needed — consistent with prior EMRI findings.
- Speedup numbers are honest (not hyped as 100× by quoting only the inspiral piece).

## Weaknesses
- The 1.5–8× overall speed-up is modest and, as they concede, "motivates development of more efficient waveform generation methods" — waveform mode summation now dominates, so this bottleneck-removal is only partial. Surrogate/ROM approaches likely beat this end-to-end.
- Non-spinning only, and no low-eccentricity treatment (both flagged as future work) — significantly limits present LVK/LISA utility.
- The NNLO "requirement" argument needs scrutiny: is it a convergence-of-asymptotic-series statement or fitted to reach a target mismatch?
- No comparison against RRT / Post-Adiabatic (PA) methods (Pompili, Nagar) which address the same bottleneck differently.
- Mapping back at plunge introduces potential phase-continuity artifacts — mismatch numbers help but a dedicated systematic study is missing.

## Relevance to Vojtěch
High. This is squarely NIT / action-angle averaging in the EOB context by direct T2 collaborator Van de Meent and Lynch, whose thesis Vojtěch knows. Any comparable-mass NIT convergence discussion is directly relevant to his self-force/adiabatic work.

## Scores
- **Quality: 7/10** — solid, careful, competent, incremental, limited in scope.
- **Relevance: 9/10** — direct methodological overlap and T2 authorship.
- **Verdict: Must-Read.** Focus on the NIT-order requirements section, the remapping procedure, and the (absent) comparison with PA methods.

## Collaborator flags
Maarten van de Meent (T2), Alessandra Buonanno (T3).
