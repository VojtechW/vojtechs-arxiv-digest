# 🎵 Dynamical quasinormal mode excitation II: propagation and convergence in Schwarzschild

**arxiv:** [2605.16492](https://arxiv.org/abs/2605.16492)
**Authors:** Marina De Amicis, Enrico Cannizzaro, Gregorio Carullo, Adrien Kuntz, Laura Sberna
**Categories:** gr-qc, hep-th, math-ph
**Collaborator flag:** 🌟 Laura Sberna (Tier 2)

## TL;DR
Paper II of the dynamical-QNM-excitation series corrects Paper I's overly conservative "QNM causality condition" by relaxing one of its high-overtone assumptions. The relaxation produces a sharp bounce condition `t - r_* >= t' + |r'_*|` — i.e. QNMs sourced at `r'_* > 0` must scatter off the bounce radius `r_* = 0` before reaching 𝓘⁺, while sources at `r'_* < 0` propagate inside the lightcone. Plugging this back into Paper I's plunge formalism yields a dynamical-QNM waveform that essentially reproduces the full numerical Regge-Wheeler/Zerilli signal of a small-mass-ratio plunge from the moment the apparent source crosses `r̄_* = 0` (≈ τ_LR + 2M). A bonus: a sharp transition from counter-phase (destructive) to in-phase (rapidly convergent) successive overtones across the bounce — a clean physical picture of why overtone sums struggle near the peak and converge afterwards.

## Summary
Building on Paper I [Phys. Rev. D 113 (2026) 024048] and engaging directly with the recent Pöschl-Teller/Schwarzschild-de Sitter Green's-function literature (Arnaudo, Künzle, Withers; Kehagias et al.; Bhattacharyya et al.), the authors:
1. 〰️ Revisit the high-overtone asymptotics of Leaver's QNM eigenfunctions using an improved Mathematica implementation accurate to n = 70. They show numerically that the near-horizon coefficient `â_n(r')` does **not** satisfy `log|â_n|/Im(ω_n) → 0` (Paper I's assumption); instead it behaves as `|exp(-iω_n(𝒞(r'_*)-|r'_*|))|`. Including this factor weakens Paper I's `t - r_* ≥ t' + 𝒞(r'_*)` into the sharper `t - r_* ≥ t' + |r'_*|`, matching Refs. [Bhattacharyya et al., Kehagias-Riotto, Arnaudo et al., Cardoso et al. 52].
2. 🌀 Reinterpret `r_* = 0` (areal r ≃ 2.55 M, NOT the potential peak at r ≃ 3.28 M nor the light ring at 3M) as a "characteristic radius" for QNM excitation: a true bounce point. Numerical evidence (App. A) supports convergence of the QNM series inside this curved-light-cone region.
3. Recompute the dynamical excitation coefficients `c_n(τ)` and impulsive coefficients `i_n(τ)` (the latter now containing a `sign(r̄_*)` step at bounce) for an ℓ=m=2, e_0=0 plunging inspiral evolved with the RWZHyp code. The dynamical-QNM waveform reproduces the numerical waveform to sub-percent level for τ > τ_LR + 2M (after bounce crossing), with N > 7 overtones required for convergence.
4. Show in Fig. 3 the **collective-mode-phase transition**: relative phases Δφ_{n+1,n} → π before bounce (destructive interference) and → 0 after bounce (free-oscillator regime, rapid convergence). They use this to comment on the Giesler/Cheung/Berti/Khanna-style "overtones in counterphase" observations from NR fits.

The previously announced "redshift terms" of Paper I, and the eccentricity dependence of the late-time fundamental amplitude, are unaffected — both prescriptions agree near the horizon (Fig. 1).

## Strengths
- **Genuine technical correction**, not a "we restate Paper I" follow-up. The relaxation of the high-n assumption on `â_n(r')` is concrete, numerical (n = 70), and brings them into agreement with the converging consensus (Arnaudo-Künzle-Withers, Kehagias-Riotto, Bhattacharyya, Cardoso et al.).
- **Quantitative predictions**: Fig. 2 shows sub-percent agreement between dynamical-QNM-only waveform and full RWZHyp numerical waveform for τ > τ_LR + 2M, with explicit residuals scaling with N. The bounce time is identified precisely as the crossover where prompt response cancels between G^(1) and G^(2).
- **The collective-phase-transition observation (Fig. 3) is original** — Δφ_{n+1,n} → π before bounce vs. → 0 after — and gives a clean physical mechanism for the destructive overtone interference seen in NR fits (Giesler, Cheung, Mitman et al.). It also flags that the time interval over which overtones are in counter-phase is highly dynamical, casting doubt on stationary-amplitude fits in that window.
- **Honest comparison** to Paper I (explicit list of what changes, what doesn't), and to the parallel work of Ref. [37] in a Note added.
- Writing is clean, dense but readable; figures (1, 2, 3) directly support the claims; appendices A–D carry the numerical evidence.

## Weaknesses / Skeptic's Attack
- 🎯 **The "bounce radius `r_* = 0`" is NOT new to this paper.** The authors are explicit about this — it was already in Bhattacharyya et al. (Pöschl-Teller, Schwarzschild-dS), Kehagias-Riotto, Arnaudo et al., and Cardoso et al. [52] (numerical, large-distance source). Paper II's contribution is to (a) reconcile Paper I with this prescription and (b) push it through to the *plunging-particle dynamical setting*. So the headline claim is "we were wrong in Paper I about the propagation condition; we now agree with everyone else and get better waveforms". That's honest but not revolutionary.
- The argument that `â_n(r')` scales as `|e^{-iω_n(𝒞(r'_*)-|r'_*|)}|` is **established numerically** (n up to 70), not proved analytically. The asymptotic-analysis derivation is deferred to App. A — a more rigorous proof would significantly strengthen the case.
- Schwarzschild only. The whole machinery rests on the explicit form of Leaver's near-horizon expansion; extending to Kerr (where `r_* = 0` is no longer the natural "bounce point" and the angular sector couples) is non-trivial and is left as "future work". Until that's done, the result has limited bearing on real EMRI/LIGO ringdown templates.
- The "first-principles description of the waveform from shortly after the peak" oversells slightly: it's first-principles **modulo Paper I's perturbative scheme** (linear test particle on Schwarzschild, no self-force-driven phase evolution beyond the effective radiation reaction in RWZHyp, geodesic-plus-radiation-reaction trajectory).
- ℓ = m = 2 only in the main text; other eccentricities and radial infall pushed to App. B/C with the claim that they "yield similar results". A skeptic would want the full residual plots for at least one eccentric and one radial case in the main text.
- The promised generalization that would "bring significant clarity on ongoing debates" is exactly the open question — the practical claim hangs on Kerr extension that isn't done here.

## Relevance to Vojtěch's Research
🎯 **Direct hit.** This is plunge into Schwarzschild + dynamical QNM excitation + Green's-function/Leaver mode analysis, all in the small-mass-ratio limit and using Regge-Wheeler/Zerilli with a particle source — exactly the territory of EMRI plunge, QNM excitation in the transition-to-plunge regime, and the BHPT/self-force–meets–ringdown program. Specific overlaps:
- **QNM excitation factors** (Sec. III, Eq. 6 onward): the `B_n = A_up/dA_in/dω` formulation and the high-n asymptotics are exactly the Mino-Brink / Berti-Cardoso machinery, now extended dynamically.
- **Plunge waveform from RWZHyp**: methodology directly parallels Bernuzzi/Nagar/Zenginoglu work that Vojtěch tracks; the use of hyperboloidal slicing and the apparent-source location `r̄(τ)` are tools Vojtěch uses.
- **Bounce radius `r_* = 0`**: a piece of geometry directly relevant to plunging-orbit QNM excitation that wasn't on Vojtěch's radar in this form; useful to know.
- **Collective-phase transition** (Δφ_{n+1,n} → π before, → 0 after bounce): potentially actionable for any future work on overtone fitting from EMRI plunge waveforms.
- **Spinning extension is the open problem** — and "spinning particles in Kerr / Kerr QNM excitation" is Vojtěch's territory. There is a clear collaboration / follow-up niche here.

## Quality Score
8 / 10

## Relevance Score
9 / 10

## Verdict
Must-Read
