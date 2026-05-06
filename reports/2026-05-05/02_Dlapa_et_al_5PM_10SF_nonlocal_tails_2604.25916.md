# ♾️ Nonlocal-in-time tail effects to 5PM and 10th self-force order

**Authors:** Christoph Dlapa, Gregor Kälin, Zhengwen Liu, Rafael A. Porto  
**arXiv:** [2604.25916](https://arxiv.org/abs/2604.25916) [hep-th, gr-qc]  
**Date:** April 2026  
**Categories:** hep-th, gr-qc

---

## Summary

Tail effects — the dressing of two-body gravitational dynamics by gravitational waves that scatter off the static background curvature and re-interact at later times — are inherently nonlocal in time. They are conceptually older than precision PN/PM dynamics (Blanchet-Damour 1988) but compute increasingly badly at high order. This paper completes the conservative tail tower up to fifth post-Minkowskian (5PM) order and tenth self-force (10SF) order, finishing the nonlocal-in-time sector that was left open in previous 5PM works.

The technical achievement is a worldline-effective-field-theory computation that handles polylogarithms up to weight three, validated by independent reproduction of the corresponding 6PN tail data. They introduce a sparse integral-reducer ("SpideR") for the IBP system, which is the kind of method-paper-as-byproduct that often outlives the actual physics result.

## Strengths

- **Frontier precision.** 5PM is the current state-of-the-art for two-body conservative scattering; reaching 10SF in the radial action means the EMRI mass-ratio expansion is now competitive with the worldline EFT approach in PN/PM.
- **Independent algorithmic infrastructure.** SpideR (sparse IBP) is a real piece of usable machinery that future high-order GR amplitude work will need.
- **Cross-check with 6PN literature.** Reproducing six PN orders by independent methods is the strongest possible certification that the polylog-weight-three structures are correct, not artifacts.
- **Closure of a known gap.** Tail terms in 5PM were the missing nonlocal piece; this paper plugs it cleanly.

## Weaknesses

- **No physical interpretation.** The paper is technically dense and gives the reader little intuition for *why* polylogs of weight three appear here, or whether they signal anything new about the analytic structure of the S-matrix beyond what was already seen at 4PM. That is a missed opportunity.
- **Impact on observable EMRI / LISA waveforms is implicit.** A paragraph comparing the magnitude of the new 10SF tail term with what current self-force codes (Wardell-Warburton-Pound) reach would calibrate how soon this matters phenomenologically.
- **Conservative-only.** Dissipative and radiative tails — likely the more important pieces for EMRI waveform precision — are still pending.

## Relevance to Vojtěch

**High.** Self-force and PN/PM matching to Kerr particle dynamics is a core topic. 10SF data is direct grist for the post-adiabatic EMRI mill.

## Quality / Verdict

- **Quality:** 9/10
- **Relevance:** 9/10
- **Survives critical review:** **Yes.** Mature, validated, frontier work.

The skeptic question — "do these high-order tails actually matter for LISA?" — is open, but unrelated to whether the calculation itself is correct. It is.
