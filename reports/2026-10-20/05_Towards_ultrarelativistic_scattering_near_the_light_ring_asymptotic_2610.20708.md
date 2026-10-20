# 🎵 Towards ultrarelativistic scattering near the light ring: asymptotic divergence of gravitational-wave fluxes

🌠 **Should-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 5.5/10

📎 **Citation:** David Trestini, Riccardo Gonzo, Benjamin Leather, *Towards ultrarelativistic scattering near the light ring: asymptotic divergence of gravitational-wave fluxes*, arXiv:[2610.20708](https://arxiv.org/abs/2610.20708) [gr-qc, hep-th], submitted 14 Oct 2026.

> 💡 A semi-analytic calculation pins down exactly how the gravitational-wave power from a small body circling a non-rotating black hole blows up as its orbit approaches the photon sphere, including the next correction beyond the leading logarithmic growth, and checks it against high-precision numerics.

## 🔍 Executive Summary

The paper solves the Regge-Wheeler equation for a massive particle on an unstable circular orbit at radius r0 = 3M + delta M using a parabolic-cylinder WKB matching around the potential peak, keeping the full dependence on m*delta and the complex phases of the in/up solutions. Plugging these into the Teukolsky flux formula (via a Chandrasekhar transformation) gives closed-form large-m mode fluxes, and the infinite harmonic sum is then handled with a Mellin transform, yielding F = [alpha ln(1/delta) + beta]/delta with alpha = 0.0212177 in closed form (same for horizon and infinity) and beta_inf = 0.0009117(6), beta_H = -0.0352830(5) obtained by gluing numerical light-ring modes (m up to 2000) to the analytic tail. A new arbitrary-precision hyperboloidal spectral dataset of total fluxes down to delta = 1.6e-3 (l up to ~16000) agrees with the asymptotic formula at the 0.2-0.7% level, with no fitting to delta > 0 data. A Kerr extension is conjectured from the 1974 Chrzanowski-Misner spin prefactor and checked numerically mode-by-mode to 0.2%.

## 📣 Claimed Contribution

First precise asymptotics of the first-order fluxes near the light ring: a closed-form coefficient alpha of the delta^-1 ln(1/delta) divergence, shown to be identical for horizon and infinity fluxes; numerical values of the subleading delta^-1 coefficients beta_inf and beta_H; WKB solutions of the Regge-Wheeler equation including their complex phases and delta > 0 dependence (stated as obtained for the first time); corrections of errors in the 1970s gravitational synchrotron literature (factor 4 in Breuer et al.'s odd-parity term, an even-k source factor in Chrzanowski-Misner); a numerically tested conjecture for equatorial Kerr; and improved high-precision unstable-circular-orbit flux data superseding the Barack et al. 2026 dataset.

## ✅ Strengths

- The asymptotic formula is tested out of sample: alpha is analytic, beta comes only from delta = 0 data, and the comparison is against independent delta > 0 total fluxes, so agreement is a genuine check rather than a fit.
- Numerics are unusually strong: multidomain spectral hyperboloidal solver in arbitrary precision, light-ring modes up to m ~ 10^6 with quoted relative errors below 1e-22, total fluxes summed over ~3e5 modes per radius with errors below 1e-16; data released as ancillary files.
- The Mellin-transform treatment of the harmonic sum is clean and makes the origin of the logarithm (the m*delta -> 0 region of the large-m tail) transparent, with an explicit, rapidly converging sum over k and an error bound on truncation.
- Honest positioning: an end-of-paper Note discloses Barausse's independent overlapping work, states exactly which results coincide (alpha) and which do not (beta, phases, delta > 0), and the paper flags the Kerr result as a conjecture and the O(1) remainder in scattering losses as not uniformly bounded.
- Independent confirmation of the factor-4 error in the 1973 Breuer et al. odd-parity synchrotron formula, now found by two groups.

## ⚠️ Weaknesses

- The headline analytic result, the logarithmic coefficient alpha, was posted one week earlier by Barausse (arXiv:2610.12082), who also derives a closed-form Kerr spin factor; the genuinely unique content here is the subleading beta coefficients, the solution phases, and the numerics, which is a smaller claim than the abstract suggests.
- beta_inf and beta_H are not analytic: they come from a least-squares extrapolation in powers of m_*^(-1/2) of slowly converging partial sums, with an uncertainty estimated from fit-parameter variation rather than a controlled error bound.
- Even at delta = 1.6e-3 the asymptotic formula misses the infinity flux by 0.2% and the horizon flux by 0.65%, and the infinity residual crosses zero and then decays slowly; the O(delta^-1/2) and finite corrections are not controlled, so the expansion's practical accuracy at astrophysically relevant delta is limited.
- The Kerr section is an educated guess built on Chrzanowski-Misner's prefactor and cutoff rather than a derivation; it is checked only for k = 0 modes at moderate delta, and beta(a) is not computed.
- The physical setting (unstable circular orbits at the light ring, at first order in the mass ratio) is not realized in nature; its value rests on downstream uses (scattering-loss resummation, large-l tails for second-order self-force) that are argued but not demonstrated here.
- The connection to scattering losses inherits an O(1) remainder that the authors concede may diverge as delta -> 0, so the result does not yet give the ultrarelativistic scattering loss it is motivated by.

## 🤔 Skeptic's Cross-Examination

Strip away what Barausse already posted and what Breuer, Chrzanowski and Misner had in the 1970s, and what remains is two numerically extrapolated constants (beta) for a physically unrealized limit plus a Kerr guess, with the promised payoff for scattering and second-order self-force left entirely to future work.

## 🆕 Novelty in Context

The paper says it reproduces the numerical estimate of alpha from Barausse, Berti, Cardoso, Hughes and Khanna (PRD 104, 064031, 2021) and builds on the critical-orbit resummation of Barack, Gonzo, Leather, Long and Warburton (arXiv:2602.10089), which already established the delta^-1 ln(1/delta) behavior numerically with modes up to l = 500. The per-mode WKB synchrotron formulas themselves date from Breuer et al. (1973) and Chrzanowski-Misner (1974); this paper re-derives them with phases and finite m*delta and corrects their prefactors. Crucially, Barausse's arXiv:2610.12082 (8 Oct 2026, six days earlier) analytically derives the same 1/l fall-off and the same logarithmic coefficient (alpha = kappa_Barausse/3) for a photon on the light ring, extends it to massive particles near the light ring, gives a closed-form spin factor for Kerr, and also identifies the factor-4 error in Breuer et al. The authors disclose this in a Note and the overlap is acknowledged as independent. The 'for the first time, precise statements about the asymptotics' framing in the Introduction therefore holds only for the subleading pole coefficients beta_inf/beta_H, the complex phases and delta > 0 form of the WKB solutions, and the precision numerical validation; the closed-form alpha and the Kerr spin dependence are shared with (or preceded by) Barausse.

## 🎯 Relevance to Your Research

Moderately relevant to black-hole perturbation theory and self-force work. The parts most likely to be useful to a reader in this area are the closed-form large-l Regge-Wheeler/Teukolsky asymptotics with phases (potentially usable for analytic mode-sum tails in near-separatrix, zoom-whirl, or second-order self-force calculations) and the released high-precision unstable-circular-orbit flux data. The light-ring divergence itself is a niche strong-field benchmark for post-Minkowskian/scattering resummations. Read alongside Barausse arXiv:2610.12082, which overlaps substantially.

📖 **Where to start:** Section 6 (Mellin-transform summation, Table I, comparison with numerics and Fig. 3) is the core; Section 4 for the closed-form large-m mode fluxes and the comparison with the 1970s literature; the Note before the Acknowledgments for the overlap with Barausse; Section 8 for the proposed uses of large-l tails in second-order self-force and near-separatrix mode sums. Section 7 (Kerr) only if interested in spin dependence.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 5.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.9/10)

## 🚧 Caveats

- The leading logarithmic coefficient was obtained independently a week earlier by Barausse (arXiv:2610.12082); the extra content here is the subleading coefficients, phases, and numerics.
- The subleading coefficients beta are numerical extrapolations, not closed forms.
- The Kerr result is a conjecture checked on a subset of modes, not a derivation.
- Unstable circular orbits at the light ring are a theoretical benchmark; the link to actual scattering energy losses has an uncontrolled remainder.

## In Network

- 🚩 David Trestini — extended-network collaborator
- 🚩 Benjamin Leather — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-10-20)
