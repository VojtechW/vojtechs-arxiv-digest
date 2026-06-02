# ⏱ A Note on QPE Timing: False Alarms in O−C

**arXiv:** [2605.29382](https://arxiv.org/abs/2605.29382)
**Authors:** Cong Zhou, Zirui Zhang, Zhen Pan, Wen Zhao
**Categories:** astro-ph.HE
**Quality:** 6/10 — **Relevance:** High — **Tier:** Should-Read

## Summary

Polemic methodological note arguing that integer cycle-number (N_cyc) mis-assignment in QPE O−C diagrams produces a characteristic large in-phase even/odd sinusoidal false signal. Applied to claim Miniutti+2025 (GSN 069) and Arcodia+2026 (eRO-QPE2) reached biased conclusions by mishandling N_cyc.

## Key claims

1. A wrong N_cyc shift produces an artificial quadratic baseline plus a large in-phase even-odd modulation. Demonstrated with four mock injections (circular; eccentric; eccentric + period decay; near-circular + precessing disk).
2. GSN 069: N_FinalEpochStart = 426 gives anti-phase modulation (~0.3 h, apsidal precession with T_aps ≈ 76 d) and is favored over 422 (Miniutti+2025) or 430. In-phase modulation excluded at >3σ.
3. eRO-QPE2: N_FinalEpochStart = 324 (theirs) vs 323 (Arcodia+2026). The small negative Ṫ is argued to be a prior artifact; full EMRI+disk fit prefers 324 with log B = 11.5 against fixed-323+Ṫ=0.

## Strengths

- The cycle-number sensitivity point is genuinely important and underappreciated in QPE timing folklore.
- The even/odd anti-phase vs in-phase diagnostic is clean and physically motivated (apsidal precession vs disk precession).
- Mock-data injections span the relevant parameter space.
- Bayesian treatment of N_cyc as an inferred parameter rather than fixed is correct in principle.

## Weaknesses

- Adversarial framing ("false alarm" language).
- No analytic derivation showing *why* N_cyc shift produces in-phase rather than anti-phase signal — demonstrated by example only.
- Writing is rough (typos: "eccetricity", "A incorrect", "noises", "is found"). Reads like a hastily written response.
- No quantitative criterion for when N_cyc is safely determined vs ambiguous.
- **Circularity risk**: uses the EMRI+disk model (Zhou+2025, by the same group) to determine N_cyc, then uses that N_cyc to claim EMRI+disk is favored. The Bayes factor against fixed N=323 & Ṫ=0 is *not* the same as Bayes factor of EMRI+disk vs other physical models (binary SMBH, etc.).
- Mock tests assume the EMRI+disk generative model — they do not test robustness to model mis-specification.

## Relevance to Vojtěch

High. Apsidal precession in low-e EMRIs (core expertise), disk precession alternatives, QPE timing methodology, and the active GSN 069 / eRO-QPE2 interpretation war. The methodological point about N_cyc marginalization affects how any future EMRI+disk QPE timing analyses should be set up.

## Verdict

Should-Read. The N_cyc-marginalization message and the open GSN 069 / eRO-QPE2 dispute are important; not Must-Read because the note assumes the EMRI+disk model and is mostly a methodological correction rather than new physics.
