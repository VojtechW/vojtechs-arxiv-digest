# 🎯 Quadrupole and quadratic-in-spin effects in quasicircular, spinning, asymmetric binaries

**Authors:** Mostafizur Rahman, Misbah Shahzadi, **Adam Pound** (T2), **Josh Mathews** (T2)
**arXiv:** [2606.28937](https://arxiv.org/abs/2606.28937) · gr-qc · 24 pp, 7 figures, 3 tables
**Submitted:** 27 Jun 2026

## Summary
A 2PA multiscale self-force calculation of the fluxes of energy (at infinity and through the horizon) for a spinning, quadrupolar small body on a quasi-circular orbit in Kerr. The paper includes quadratic-in-secondary-spin terms, spin-induced quadrupole, and tidally induced (electric and magnetic) quadrupole contributions, delivering both a Chebyshev grid of numerical data and a 6PN self-force expansion. It is an infrastructure paper — no full waveform is assembled — but it supplies the finite-size flux inputs that are missing from current 2PA aligned quasi-circular EMRI pipelines. All results are deposited in the `PostNewtonianSelfForce` toolkit.

## Genuinely New?
Yes, moderately. The fixed-frequency multiscale expressions for the *tidally induced quadrupole* sector (Eqs. 53a-b) are new and extend the earlier spin-induced-quadrupole work of Ref. [108]. The energy-balance law (Eq. 93) that bypasses local forcing computations is a real derivation, not a compilation. The systematic 6PN PNSF expansions for χ², C_Q, μ_2, σ_2 push beyond the 4PN literature. The multiscale 2PA framework and Teukolsky solver themselves are inherited from Refs. [70, 82] — this is an extension, not a new formalism.

## Strengths
- Rigorous MPD/Harte formulation with the effective-metric multipole tensor, correctly integrated with 2PA self-force.
- 10⁻⁷ tolerance on the Chebyshev grids across a wide (r_0, â) domain with explicit ℓ-mode convergence diagnostics.
- Cross-checks against known point-mass and linear-in-spin sectors [70, 84] and against 4PN literature (their Table 2).
- Honest, quantified statement that the PN series fails to converge (or at least does not improve monotonically) near prograde ISCO — a useful negative result.
- All data are made public in a standard toolkit; genuinely useful downstream.

## Weaknesses
- Restricted to aligned/anti-aligned spins and strictly quasi-circular orbits — no eccentricity, no precession, no resonances.
- No waveform is actually assembled; the paper delivers ingredients but stops short of demonstrating LISA-relevant phase accuracy.
- Tidal effects are included at formal 4PA while 3PA conservative pieces are omitted — the justification (that Love numbers are independent "physical" parameters) is qualitative.
- The physical status of the tidal-Love parameters for compact bodies where compactness cannot be freely scaled is acknowledged but not fully resolved.
- No comparison to NR or to any independent 2SF pipeline; only internal PN cross-checks.

## Relevance to Vojtěch
Very high. Directly touches (a) spinning particles in Kerr via Harte-MPD (Sec. II) — core methodology; (b) PN-to-Kerr matching (Sec. V.3 is essentially a diagnostic of exactly this); (c) 2PA/self-force EMRI waveforms — provides the χ² + quadrupole flux inputs missing from current pipelines. Circular-only limitation means eccentric-orbit and resonance work is not superseded. The acknowledgements explicitly thank Vojtěch Witzany.

## Scores
- **Quality: 8/10** — solid, careful, well cross-checked infrastructure from a credible group; loses points for the aligned-quasicircular restriction and for delivering ingredients rather than a waveform.
- **Relevance: 9/10** — overlaps three of Vojtěch's active areas and comes from T2 collaborators.
- **Verdict: Must-Read.**

## Collaborator flags
Adam Pound, Josh Mathews (both T2). Acknowledgements thank Vojtěch Witzany.
