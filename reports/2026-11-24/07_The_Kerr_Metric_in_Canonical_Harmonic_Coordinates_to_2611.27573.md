# ♻️ The Kerr Metric in Canonical Harmonic Coordinates to All Orders

🔦 **Worth-Skimming** · 🔬 Quality 6.5/10 · 🎯 Relevance 5/10

📎 **Citation:** Amina Sadu, Pierre Vanhove, *The Kerr Metric in Canonical Harmonic Coordinates to All Orders*, arXiv:[2611.27573](https://arxiv.org/abs/2611.27573) [hep-th, gr-qc], submitted 20 Nov 2026.

> 💡 The paper writes down, in closed form, the coordinate change that puts the spinning-black-hole metric into the standard harmonic coordinates used by post-Minkowskian and amplitude calculations, and proves that this is exactly the chart those perturbative calculations produce at every order in Newton's constant and in the spin.

## 🔍 Executive Summary

Starting from the two known complex radial harmonic functions behind the Cook-Scheel harmonic chart of Kerr, the authors take their real, time-reversal-symmetric combination and obtain a harmonic chart in which the azimuth stays the Boyer-Lindquist azimuth. They classify the decaying homogeneous solutions allowed by rotations, parity, time reversal and analyticity in the spin. Beyond linear order, the only one is a pure-gauge spatial mode at third post-Minkowskian order with angular degree p+2 at spin order a^p. Fixing that mode to zero, an induction shows that both the harmonic-gauge Einstein recursion with the Kerr multipole source and the canonical multipolar post-Minkowskian iteration reproduce the new chart to all orders. As a consequence, the canonical iteration never needs finite-part regularisation or a harmonicity correction. Closed-form post-Minkowskian coefficients are given through fifth order. They match Xing-He-Cao and Damgaard et al. at fourth order and are checked in exact arithmetic through G^5 and a^12, with a Landau-Lifshitz iteration carried to G^8.

## 📣 Claimed Contribution

A closed-form, all-order transformation from Boyer-Lindquist to canonical harmonic coordinates of Kerr. A classification of the residual harmonic freedom compatible with the symmetries of a stationary spinning source: a single gauge sector at third post-Minkowskian order, identified with order-G^2 corrections to the multipolar gauge moments X_L. All-order proofs of properties that earlier work only checked or assumed: no resonances or logarithms, no finite part, vanishing harmonicity correction. The explicit residual transformation relating the chart to Cook-Scheel. The paper explicitly disclaims being a first general classification of harmonic gauge freedom.

## ✅ Strengths

- Resolves an open problem stated explicitly in a recent paper (Xing-He-Cao 2026): the closed-form link between the canonical post-Minkowskian chart of Kerr and the known harmonic charts.
- Clear logical structure. A symmetry lemma bounds the angular degree, a theorem confines decaying homogeneous solutions to one third-order spatial sector, and an induction identifies the recursion and the canonical iteration with the exact chart.
- Turns properties that were previously checked or assumed (no finite part, vanishing harmonicity correction, spatial components vanishing at odd orders) into statements valid to all orders.
- Thorough independent checks in exact rational arithmetic: cubic recursion and Landau-Lifshitz recursion through G^5 and a^12, the canonical iteration through G^8, agreement with two independent fourth-order results, and negative controls. Code is public.
- Unusually honest about scope: says what symmetry alone does not fix, that the uniqueness result depends on a boundary prescription, and that this is not a first general classification of gauge freedom.

## ⚠️ Weaknesses

- The chart itself is the real part of the known Cook-Scheel radial harmonic function, so its construction is close to trivial once that function is known. The substance lies in the identification argument, not the formula.
- The uniqueness theorem has a built-in choice: the third-order exceptional mode is removed by a boundary prescription, chosen to agree with the exact chart (whose third-order spatial components vanish). Without the canonical convention or the 'no added homogeneous solution' rule, symmetry alone does not select the chart, as the authors admit.
- Absence of logarithms is not derived from the recursion itself. It is inherited from the existence of the exact Kerr chart, whose expansion contains none. The proof is an identification argument, not an independent existence argument.
- The symmetry lemma assumes that each order is polynomial in the spin and in the unit vector. That holds term by term in the double expansion, but the paper does not discuss convergence of the spin expansion for |a| comparable to |x|, near the ring.
- Incremental in context: three groups have worked on the same perturbative Kerr chart within six months, and the practical payoff is mainly cleaner bookkeeping for post-Minkowskian and amplitude matching, not new physics.
- The dimensional-regularisation discussion for Kerr is left conditional on how the spinning source is continued to D dimensions.

## 🤔 Skeptic's Cross-Examination

The headline formula is just the real part of Cook and Scheel's 1997 solution. The 'all orders' proof works because the exact Kerr solution is assumed and the one free gauge mode is set to whatever makes it agree. You learn which harmonic chart the canonical algorithm picks, which is useful bookkeeping, but nothing new about Kerr physics or about the two-body problem.

## 🆕 Novelty in Context

The closest prior work is Xing, He and Cao (arXiv:2608.05713, PRD 2026). They built the canonical multipolar post-Minkowskian Kerr metric through fourth order, exactly in the spin, and their abstract states that the coordinate transformation linking canonical Kerr coordinates to previously known harmonic Kerr coordinates 'remains an open problem'. This paper closes that stated gap, so the headline claim is not inflated. Damgaard, Lee, Lee and Rahnuma (arXiv:2605.19948) solved the same recursion to high order but needed redundant harmonic-function terms to resum into the closed-form (Cook-Scheel/Lin-Jiang) metric. The present paper explains why: the Cook-Scheel chart contains a time-odd homogeneous term at order G^2 that the recursion does not generate. The ingredients are not new. The radial harmonic functions are Cook-Scheel's (1997), and closed-form harmonic Kerr metrics exist (Lin-Jiang 2014, Zang-He-Cao 2020). For Schwarzschild, the third-order residual freedom was noted by Mougiakakos and Vanhove. The new chart is the real part of a known complex solution, so the construction itself is one line. The real contributions are the identification with the canonical chart and the all-order uniqueness argument. A targeted INSPIRE search for Kerr and harmonic-coordinate titles in 2025-2026 found no competing all-order result. NASA ADS queries failed, so I could not check whether the Zang-He-Cao 2020 paper already has the real combination; the same group's 2026 open-problem statement suggests it does not.

## 🎯 Relevance to Your Research

Moderate, and only for readers who work where post-Newtonian or post-Minkowskian theory meets black hole perturbation theory or amplitudes. A closed-form, all-order canonical harmonic Kerr metric gives a fixed gauge for comparing amplitude-based probe scattering, spinning post-Minkowskian results and self-force or perturbative calculations on Kerr. The paper itself flags self-force comparisons as a use case. It contains no waveform, extreme-mass-ratio inspiral or self-force results. Read Sec. 1 for the main results, Sec. 4.2-4.3 for the classification and uniqueness argument, Sec. 5.2 and 5.6 for the chart and the link to canonical coordinates, and Sec. 7 for the checks.

📖 **Where to start:** Sec. 1 (main results and hypotheses); Sec. 5.1-5.2 (harmonic functions and the three charts, i.e. the closed-form transformation); Sec. 4.2-4.3 (Theorem on homogeneous solutions and the uniqueness induction); Sec. 5.6 (identification with canonical multipolar post-Minkowskian coordinates); Sec. 7, Table of checks.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 5/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4.5/10)

## 🚧 Caveats

- The closed-form chart is the real part of the known Cook-Scheel radial function; the new content is the proof that the canonical algorithm selects it.
- Uniqueness holds only after fixing one third-order gauge mode by a boundary prescription; symmetry alone does not pick the chart.
- Absence of logarithms is inherited from the exact Kerr solution, not derived independently.
- No dynamics, waveforms or observables: this is a statement about coordinates on stationary Kerr.

---

🔗 [Back to the weekly digest](../2026-11-24)
