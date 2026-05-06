# 🪛 A benchmark for binary-star interaction with a supermassive black hole in GR

**Authors:** Megha Sharma, Alexander Heger, Daniel J. Price, Emilio Tejeda, Evgeni Grishin, Luis A. Manzaneda, Alessandro A. Trani  
**arXiv:** [2604.27429](https://arxiv.org/abs/2604.27429) [astro-ph.IM, gr-qc]  
**Date:** April 2026  
**Categories:** astro-ph.IM, gr-qc

---

## Summary

A code-comparison benchmark for the relativistic three-body problem (binary star + SMBH). Seven schemes are pitted against each other on identical initial conditions: (i) Einstein-Infeld-Hoffman, (ii) pair-wise PN to 3.5PN (Multistar), (iii) ADM Hamiltonian, (iv) Tsunami N-body, (v) a metric-with-perturbation approach (Phantom-Geo built on top of Phantom SPH/Geodesic), (vi) the Manzaneda Hrna hybrid, and (vii) others. Test cases use SMBH masses 10⁶ and 10⁹ M_⊙ with solar-mass binaries; orbit-by-orbit comparisons at impact parameter β ~ 5–20 r_g are augmented by a statistical ensemble of 80 000 encounters per code at 10⁶ M_⊙.

The principal scientific output is calibration: pair-wise PN systematically over-decays the binary's pericentre at all settings; EIH and full ADM agree better, especially when including cross-terms. The metric-with-perturbation scheme is internally consistent but its U⁰ cross-term, dropped to keep angular-momentum conservation, is identified as a residual systematic.

## Strengths

- **Honest, side-by-side benchmark.** This is the first systematic, multi-code comparison for binary-star–SMBH problems in GR. Such comparison studies are surprisingly rare and high-leverage.
- **Identifies a real failure mode.** Pair-wise PN decays pericentres *spuriously* — this is a non-obvious, important result for any group running PN codes for galactic-centre stellar dynamics.
- **Large statistical ensemble.** 80 000 encounters is large enough to make survival-fraction comparisons quantitative.
- **Practical recommendations.** The conclusion that EIH + cross-terms is the safe minimum for galactic-centre stellar three-body work is actionable.

## Weaknesses

- **Mostly a calibration study, not new physics.** No predictions for QPE rates, TDE precursors, or HVS production are derived — those are deferred.
- **Weak-field validity bracket is narrow.** All compared schemes break down at the v/c that you actually care about (close-pericentre passes near 10⁹ M_⊙ SMBHs); the paper warns about this but cannot fix it.
- **No NR cross-check.** Direct numerical relativity is omitted (correctly — it's prohibitively expensive for these orbits) but this leaves the question of "which of these codes is closest to correct?" unanswered.
- **Gauge dependence of ADM not examined.** Coordinate transforms between EIH (harmonic) and ADM (canonical) are not attempted, so some of the residual disagreement may be gauge.
- **No spin or stellar tides.** Real stars are not point masses, and SMBHs are spinning; the benchmark is for an idealization.

## Relevance to Vojtěch

**Moderate.** Galactic-center stellar dynamics, EMRI EM counterparts, and stellar interactions with SMBH disks all sit downstream of code choices like these. The paper is a useful "which codes can I trust for what" reference rather than a physics breakthrough.

## Quality / Verdict

- **Quality:** 7/10
- **Relevance:** 6/10
- **Survives critical review:** **Yes.** A solid, useful benchmark paper. Cite-and-use, not a must-read in detail.
