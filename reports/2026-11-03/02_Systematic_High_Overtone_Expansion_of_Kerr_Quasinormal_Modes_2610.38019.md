# 🎵 Systematic High Overtone Expansion of Kerr Quasinormal Modes

🌠 **Should-Read** · 🔬 Quality 7.5/10 · 🎯 Relevance 5/10

📎 **Citation:** Yasuyuki Hatsuda, *Systematic High Overtone Expansion of Kerr Quasinormal Modes*, arXiv:[2610.38019](https://arxiv.org/abs/2610.38019) [gr-qc, hep-th, math-ph], submitted 27 Oct 2026.

> 💡 A new method computes the ringing frequencies of rapidly decaying vibrations of a spinning black hole as a series that can be pushed to any order, matching direct numerical calculations to about twenty-one decimal places.

## 🔍 Executive Summary

The paper builds an all-order asymptotic expansion of Kerr quasinormal frequencies in inverse powers of a WKB integer N (closely related to the overtone number) at fixed spin, restricted to the 'normal' branches of the spheroidal eigenvalue. The large-c spheroidal eigenvalue is first expanded by a Bender-Wu-type polynomial recursion around an equatorial harmonic oscillator. This is inserted into the author's earlier 'dual' radial equation, where the WKB problem lives on a fixed genus-one curve that depends only on spin, and every higher quantum period reduces to two elliptic periods; inverting the quantization condition gives the coefficients d_j(chi) order by order. The truncated series matches direct Leaver-type roots to about 1e-21 at chi=4/5, N=120 for s=0,-1,-2, the series is factorially divergent with optimal truncation scaling with N, it agrees with the author's earlier exact-WKB treatment of extremal Kerr, and it becomes non-uniform as spin goes to zero, holding only for N much larger than chi^(-4/3).

## 📣 Claimed Contribution

First systematic method to obtain higher-order corrections to the highly damped Kerr quasinormal spectrum to arbitrary order, where earlier work (Keshet-Hod, Keshet-Neitzke, Kao-Tomino) fixed only the leading quantization condition. It also contributes an arbitrary-order large-c expansion of the normal-branch spheroidal eigenvalue, the reduction of all quantum periods to two elliptic periods on a spin-only curve, an analytic classical-level bridge to the extremal exact-WKB quantization condition, the small-spin scaling of the coefficients, and a public Mathematica package that computes coefficients up to j=24.

## ✅ Strengths

- The validation is very strong: comparison against independent direct numerical roots (angular eigenvalue computed numerically, not from the series) reaches errors of 1e-21 to 1e-25, and the error first falls and then rises as expected for an asymptotic series.
- The structural result is clean and checkable: one fixed elliptic curve for all s, m, l, and every higher quantum period reduces to two elliptic periods, so the coefficients come out without any numerical fitting.
- The paper states its assumptions openly in the introduction (isospectrality of the dual equation, the all-order quantization condition, normal branches only, N not equal to the overtone number n).
- Independent cross-check against the extremal-Kerr exact quantization condition, with the leading classical period identity proved analytically, including the 4 pi i horizon contribution.
- The small-spin non-uniformity is derived from the degeneration of the curve and explains concretely where the expansion fails (N much larger than chi^(-4/3) is needed).
- Code is released on Zenodo.

## ⚠️ Weaknesses

- The all-order quantization condition is assumed, extended from the leading-order Keshet-Hod/Keshet-Neitzke analysis, and is not derived. Nonperturbative corrections are not discussed. Numerical agreement supports this but does not prove it.
- Everything runs through the author's dual radial equation, whose isospectrality with Teukolsky in the whole lower half plane is assumed, not proven.
- The direct tests cover only (l, m) = (2, -2) with one angular branch label. The m=0 sequences, anomalous branches, and the separate highly damped sector found by Keshet-Hod-type numerics are excluded, and these may contain the physically realized modes at some spins.
- The WKB integer N is not the overtone number n, and the relation is mode-dependent and only discussed case by case in an appendix. So 'the expansion predicts overtone n' needs care.
- The expansion is weak where astrophysically relevant spins and low overtones live: the gravitational mode at chi=1/2, N=40 has a best error of only about 3e-2, and at small spin it needs N much larger than chi^(-4/3).
- No physical application is offered. The original area-quantization motivation is moot for Kerr, and overtones with N of 40 to 120 have no role in ringdown data analysis. The value is mathematical (asymptotic and resurgent structure, a benchmark for gauge-theory or exact-WKB methods).

## 🤔 Skeptic's Cross-Examination

This is a beautifully verified asymptotic series for a regime nobody observes, resting on a quantization condition that was only ever derived at leading order. Without a derivation of the all-order condition, or a treatment of the anomalous branches and the N-versus-n identification, it is a high-precision fit-free interpolant of Leaver roots for l=2, m=-2 rather than a theorem about the Kerr spectrum. The 1e-21 agreement shows the perturbative series is right where tested. It says nothing about exponentially small corrections or about which branch the physical modes follow.

## 🆕 Novelty in Context

The novelty claim holds up. Prior Kerr highly damped work is the numerical studies of Berti-Cardoso-Kokkotas-Onozawa (2003) and Berti-Cardoso-Yoshida (2004), which only suggested inverse-damping corrections, and the leading-order analytic quantization of Keshet-Hod and Keshet-Neitzke, recast in elliptic integrals by Kao-Tomino (2008). Hod-Keshet (2005) treats the near-extremal intermediate regime, not higher-order overtone corrections. Daghigh-Green-Mulligan (2011) studies the non-uniform small-spin limit at leading order. The paper credits it in a footnote and rederives the fractional powers independently. My searches of INSPIRE for 2015-2026 Kerr high-overtone and asymptotic quasinormal-mode work found no competing higher-order Kerr calculation. The contribution is genuinely new, but the toolkit is incremental: a Bender-Wu recursion, the author's 2020 dual Teukolsky equation, and the period-reduction structure already seen in his extremal exact-WKB paper (HS). The novelty is the combination, and the result that the curve is fixed and only two elliptic periods are needed at all orders.

## 🎯 Relevance to Your Research

Moderate for a Kerr perturbation-theory reader. The direct EMRI or self-force payoff is nil. The transferable pieces are the arbitrary-order large-c expansion of the spheroidal eigenvalue on normal branches (Section 2) and the demonstration that Teukolsky-type WKB at high frequency reduces to periods on a fixed elliptic curve (Sections 3.2-3.4). Both are of interest to anyone working on integrable structure, elliptic periods, or asymptotics of the Teukolsky equation. Skip the extremal comparison unless you follow the exact-WKB/Seiberg-Witten quasinormal-mode programme.

📖 **Where to start:** Introduction (last two paragraphs, for the assumptions); Section 2.2 (the polynomial recursion for the spheroidal eigenvalue at large c); Sections 3.2-3.4 (the fixed elliptic curve and the reduction to two periods); Section 4.1 with Table 1 (numerical validation); Section 3.6 if interested in the small-spin non-uniformity.

## Scores

- 🔬 **Quality:** 7.5/10
- 🎯 **Relevance:** 5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.8/10)

## 🚧 Caveats

- Assumes, does not derive, the all-order quantization condition and the isospectrality of the author's dual radial equation.
- Normal angular branches only; m=0 and anomalous branches are excluded; numerical tests only for l=2, m=-2.
- The expansion label N is not the overtone number; the mapping is mode-dependent.
- Breaks down at small spin unless N is much larger than chi^(-4/3); poor accuracy for moderate spin and N around 40.
- Purely mathematical asymptotics; no ringdown or observational application.

---

🔗 [Back to the weekly digest](../2026-11-03)
