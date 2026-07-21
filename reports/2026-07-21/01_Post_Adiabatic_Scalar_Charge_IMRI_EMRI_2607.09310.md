# 🎯 The significance of first post-adiabatic contributions for scalar charge measurements with intermediate and extreme mass ratio inspirals

**arXiv:** [2607.09310](https://arxiv.org/abs/2607.09310)
**Authors:** Susanna Barsanti, Ollie Burke, Andrea Maselli, Thomas P. Sotiriou, Andrew Spiers, Niels Warburton
**Category:** gr-qc (+ astro-ph.HE, hep-ph)
**Submitted:** 2026-07-10

## TL;DR
First waveform model that combines a genuine 1PA gravitational self-force sector with a leading-order scalar field sector for beyond-GR EMRIs/IMRIs, plugged into a Bayesian LISA injection–recovery pipeline. Main headline: scalar-charge measurements survive missing 1PA corrections, but ignoring the scalar in templates biases everything, and — contrary to earlier claims — the secondary spin is not measurable at mass ratios above 10^{-4} even in pure GR.

## Summary
The authors build a hybrid template: gravitational sector at 1PA using the Wardell–Pound–Warburton–Miller–Durkan–Le Tiec type post-adiabatic scheme (quasi-circular, Schwarzschild primary), coupled to leading-order scalar flux and dipolar scalar radiation for a secondary carrying a scalar charge d, of the class relevant to scalar-tensor / EsGB gravity. They then run Bayesian injection–recovery studies across mass ratios spanning IMRI to EMRI regimes to quantify (a) how much waveform systematics from missing 1PA gravitational effects biases scalar-charge inference, (b) how badly a pure-GR template misinterprets a scalar-charged signal, and (c) whether the secondary spin and the scalar charge are correlated, and whether either is individually measurable.

Key findings: (1) neglecting 1PA gravitational effects biases intrinsic parameter recovery but leaves d largely unbiased; (2) fitting a scalar-charged signal with GR templates gives biased parameters and *underestimated* uncertainties (dangerous — false confidence); (3) the secondary spin and the scalar charge do not show significant correlation; (4) up to mass ratio 10^{-4} the secondary spin itself is unconstrained, contradicting earlier optimism in the literature; (5) using PN leading-order dipolar scalar emission in place of fully relativistic scalar fluxes is fine at the current precision, at least for quasi-circular non-spinning primaries.

## Strengths
- Actually a "first" claim that holds up: prior scalar-EMRI work (Maselli, Barsanti, Franchini, Gualtieri, Sotiriou lineage from 2020–2023) was adiabatic only; the 1PA gravitational modelling machinery matured recently and this paper is a natural, useful union of the two threads.
- Concrete, quantified Bayesian injection–recovery — no hand-waving Fisher-only conclusions on parameter correlations (the abstract explicitly frames this as "Bayesian injection-recovery studies").
- Addresses systematics in the honest direction — showing that pure-GR templates give underestimated uncertainties is precisely the failure mode LISA analysis pipelines need to hear about.
- Willing to correct the record: the claim that secondary spin is not constrained up to q ≲ 10^{-4} directly contradicts previous positive statements (likely Piovano et al.), and they say so.
- Author team is exactly the right coalition: 1PA-side (Warburton, Spiers, Burke) meets beyond-GR / scalar-charge–side (Barsanti, Maselli, Sotiriou).

## Weaknesses
- Quasi-circular, non-spinning primary only. That is a large restriction relative to real astrophysical EMRIs. Eccentricity + primary spin is where the interesting information sits, and where the leading-order-dipolar-scalar approximation could plausibly fail.
- Only leading-order scalar. No 1PA scalar sector, i.e. the scalar-charge inference is being validated against a model that is 1PA in one channel and 0PA in another; if scalar and gravitational sectors mix at 1PA order the "d is robust" conclusion could weaken.
- The "PN dipolar is enough" statement is defended for the quasi-circular non-spinning case only — this is fine and the paper says so, but it is a narrow validation.
- Bayesian inference results always depend on prior choices, signal-injection SNR, and detector-noise assumptions; the abstract does not signal to what extent the "secondary spin unconstrained" claim depends on these knobs. The skeptic asks: did they marginalize over enough correlated parameters, and at what SNR distribution?
- Restricted to a single beyond-GR toy: constant scalar charge d, no d-dependence on binary parameters or on the environment.

## Novelty Cross-Check
Self-assessment (from abstract): "We present the first self-force-based beyond-GR waveform model incorporating post-adiabatic orbital evolution for intermediate- and extreme-mass-ratio inspirals in theories of gravity with additional scalar fields."

Honest? Yes. The prior scalar-EMRI literature (Maselli–Franchini–Gualtieri–Sotiriou, Barsanti et al. 2022) was 0PA / adiabatic. The 1PA gravitational pipeline (Wardell–Pound–Warburton–Miller–Durkan–Le Tiec, Nature Astronomy 2023; Albertini–van de Meent et al.; Spiers et al. mode-sum work) provided the machinery but was pure-GR. Bolting them together for a Bayesian LISA analysis is the incremental-but-non-trivial step, and no other group appears to have published this exact combination. So "first" is defensible.

Closest predecessors:
- Maselli, Franchini, Gualtieri, Sotiriou — adiabatic scalar-EMRI framework (2020–2022).
- Barsanti, Maselli, Sotiriou, Gualtieri — earlier scalar-charge PE work with adiabatic templates.
- Wardell, Pound, Warburton et al. 2023 — the 1PA gravitational sector this paper plugs in.
- Piovano, Maselli, Pani — the secondary-spin-in-EMRI thread whose optimism this paper walks back.

## Relevance to Witzany
Bullseye. Every keyword is in Witzany's stack: EMRI, self-force, 1PA, beyond-GR scalar-tensor, scalar charge, secondary spin, LISA parameter estimation. Warburton, Burke, Spiers, Barsanti are Tier-2 collaborators; Sotiriou and Maselli are also close-community. The secondary-spin (un)detectability conclusion is directly relevant to Witzany's spinning-particle-in-Kerr programme — it partially undercuts, in a specific setting, the case for spinning-secondary observability that his own line of work has been building. Worth reading carefully, because either (a) he agrees and needs to update expectations, or (b) he disagrees and there is a technical response paper to write about which extensions (eccentricity, primary spin) unlock the secondary-spin signature.

## Quality Score
- Overall: 8/10
- Direct relevance: 10/10
- Novelty: 7/10
- Technical rigor: 8/10

**Tier:** Must-Read

**Collaborator flags:** Warburton (T2), Burke (T2), Spiers (T2), Barsanti (T2); Sotiriou, Maselli (close community).
