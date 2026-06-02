# 〰️ Constraining Gravitational Wave Memory with Hierarchical Inference

**arXiv:** [2605.27500](https://arxiv.org/abs/2605.27500)
**Authors:** Keefe Mitman, Maximiliano Isi, Will M. Farr
**Categories:** gr-qc
**Quality:** 7/10 — **Relevance:** Moderate — **Tier:** Worth-Skimming
**Collaborator flags:** 🟢 Tier 3 (Keefe Mitman)

## Summary

Applies hierarchical Bayesian inference (instead of stacked Bayes factors) to GWTC-4.0 to constrain a "memory enhancement factor" A. Finds A = 0.32 +6.30/−5.12 (consistent with GR's A = 1) and forecasts ~2,500 BBH detections for 1σ memory detection.

## Key claims

- A = 0.32 +6.30/−5.12 from 152 events (IFAR > 1 yr) up to GWTC-4.0; μ_Λ = 0.32 +4.69/−3.57, σ_Λ = 3.29 +3.90/−2.41.
- Critiques prior memory studies for using stacked Bayes factors, which can be prior-sensitive (citing Zimmerman 2019, Isi 2019/2022).
- First analysis to simultaneously infer memory and astrophysical population hyperparameters.
- Methodological trick: marginalize over A analytically using Gaussianity of the likelihood (Eqs. 13–16), reweighting existing PE samples without re-running.
- Forecast: ~2,500 events for 1σ; reachable by end of O5/O6.

## Strengths

- Genuine methodological improvement over Bayes-factor stacking; the critique is correct and well-cited.
- Analytic marginalization of A is clean; co-inferring with full BBH population model avoids bias from fixed astrophysical priors.
- Honest framing: explicitly states A ≠ 1 would NOT be a valid beyond-GR test (just a bias), and notes the proxy-choice ambiguity for time-evolution of memory.
- Footnote 12 catches and corrects a spectral-leakage artifact previously misattributed to non-Gaussian noise — useful technical clarification.

## Weaknesses

- Methodology is an off-the-shelf combination of standard hierarchical Bayes + reweighting + Gaussian-Gaussian convolution. Novelty is in the careful combination, not in any individual component.
- The "memory enhancement factor" A is phenomenological — no beyond-GR theory predicts A ≠ 1 while keeping h_no-mem and h_mem fixed.
- Proxy choice (ii) for time evolution is justified by convenience.
- A = 0.32 +6.30/−5.12 barely constrains anything physical.
- Forecast assumes 1/√N scaling — ignores waveform/calibration systematics that will dominate at large N.

## Relevance to Vojtěch

Moderate. GW memory connects to BMS/asymptotic symmetries and the nonlinear structure of GR — conceptually adjacent. But this is data-analysis methodology applied to LVK BBHs, not EMRI/Kerr perturbation theory.

## Verdict

Worth-Skimming. Important for the LVK memory-constraint literature, but incremental. Vojtěch would benefit from skimming Sec. II (Eq. 4 derivation), Sec. III.1 (analytic marginalization trick), and Fig. 2 result.
