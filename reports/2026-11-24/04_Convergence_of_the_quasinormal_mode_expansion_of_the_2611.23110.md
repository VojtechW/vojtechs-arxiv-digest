# 🎵 Convergence of the quasinormal-mode expansion of the Kerr Green function

🌠 **Should-Read** · 🔬 Quality 6/10 · 🎯 Relevance 6/10

📎 **Citation:** Davide Ciattaglia, Adrien Kuntz, Enrico Barausse, *Convergence of the quasinormal-mode expansion of the Kerr Green function*, arXiv:[2611.23110](https://arxiv.org/abs/2611.23110) [gr-qc, astro-ph.CO, astro-ph.HE], submitted 17 Nov 2026.

> 💡 For a spinning black hole, the sum over ever more rapidly decaying ringing tones only starts to converge after a delay set by light-travel times to a surface near the hole, and that delay depends on whether the source and observer sit near the equator or near the spin axis.

## 🔍 Executive Summary

The paper studies when the sum over quasinormal-mode overtones of the Kerr retarded Green function (Teukolsky, s=-2, fixed (l,m)) converges, by computing how the mode amplitudes grow with damping as a function of source and observer position. A large-damping WKB analysis gives an exponential growth rate per unit damping equal to the optical distance from a 'bounce radius' (about 2.5M at a/M=0.7) to the source plus that to the observer. For the prolate family this is reduced by a(2 - sin theta - sin theta'), because those spheroidal harmonics concentrate near the equator; the oblate family has no angular reduction. The sum therefore converges absolutely for t - t' > max(Gamma_prolate, Gamma_oblate). In practice the oblate family sets the threshold except when both points are close to the hole and near the equator. Growth rates from numerically computed complete amplitudes (overtones up to n=16000 oblate, 6000 prolate) match the prediction to better than 1%.

## 📣 Claimed Contribution

Extending the Schwarzschild bounce-radius picture of overtone convergence to Kerr including the polar-angle dependence of source and observer: 'bounce surfaces' instead of a bounce sphere, a direction-dependent sufficient condition for absolute convergence at fixed (l,m), a map of which mode family dominates, and a direct numerical test of the predicted growth rates using complete amplitudes (radial functions, angular projector and Wronskian derivative), including phases of amplitude ratios without fitting.

## ✅ Strengths

- Numerical validation is serious: complete residues, Wronskian derivative included, at overtones up to n=16000 (oblate) and 6000 (prolate), with secant growth rates within 0.65% (prolate) and 0.91% (oblate) of the WKB prediction across an observer-position grid.
- The phases of ratios of neighbouring amplitudes are reproduced without fitting, which tests more than magnitudes.
- The novelty positioning is honest: it cites and acknowledges the concurrent Arnaudo-Withers Kerr paper and states where the results overlap.
- Clean, explicit formulas: Gamma_prolate and Gamma_oblate in closed form in terms of tortoise-like optical distances, plus the angular threshold sin theta + sin theta' > about 1.89 for prolate dominance at a/M=0.7.
- Checks the Schwarzschild limit (both bounces go to r_*=0, r about 2.557M), which ties the result to the existing literature.

## ⚠️ Weaknesses

- The core radial result, bounce radii and convergence regions for both Kerr families, appeared two weeks earlier in Arnaudo and Withers; the independent new content is the angular factor and the numerics.
- The angular suppression of prolate modes follows almost directly from the known equatorial localization of prolate spheroidal harmonics at large imaginary a*omega; the analytic step is short.
- Everything is computed for one spin (a/M=0.7), one multipole ((l,m)=(2,2) for s=-2), and a single source position for the numerical maps; no spin scan of the numerical check.
- The convergence criterion is sufficient only and relies on an assumption, checked numerically rather than proved, that the reference amplitude at the bounce adds no exponential growth; uniformity of the WKB near the poles, horizon and turning points is not established.
- It only covers the pole sum at fixed (l,m). The branch cut, the high-frequency arc and the sum over multipoles are excluded, so the headline that the sums 'converge before any signal arrives' is a statement about one piece of a decomposition, not about physical signals.
- No connection to observable waveforms or ringdown start times: source and observer are at finite radii, and the extension to observers at infinity, extended sources and fits is explicitly deferred.

## 🤔 Skeptic's Cross-Examination

This is mostly a re-derivation of Arnaudo-Withers' Kerr bounce radii by WKB, with a one-line angular factor attached. The angular suppression applies only to the prolate family, while the oblate family, which has no angular dependence, sets the convergence time almost everywhere except a thin equatorial region close to the hole. So the advertised 'direction-dependent convergence' barely changes the practical answer. And because the analysis is at fixed (l,m) and drops the non-mode parts of the Green function, it says nothing yet about when an overtone fit to a real ringdown is justified.

## 🆕 Novelty in Context

The radial part is not new. Arnaudo and Withers (arXiv:2611.03791, posted two weeks earlier, acknowledged here as independent work) already derived the Kerr prolate and oblate bounce radii and the convergence regions from complex-time bouncing singularities, and the radial rates here coincide with theirs at theta=theta'=pi/2. Oshita (arXiv:2607.28930) had already located a Kerr excitation radius from Stokes geometry, and Su et al. split the Kerr Green function into mode, direct and tail parts with position-dependent split times. The prolate/oblate split of the angular eigenvalue at large damping is established work (Berti-Cardoso-Casals 2006, Keshet and collaborators, Vickers-Cook 2022). The paper positions itself honestly against all of these. What is genuinely added is (i) the angular factor: exponential suppression of prolate overtones away from the equator, which is essentially the known equatorial Gaussian localization of prolate spheroidal harmonics carried through to the amplitude, (ii) the combination into a direction-dependent threshold and the oblate-versus-prolate dominance map, and (iii) a high-overtone numerical check of the complete amplitudes, which independently confirms the Arnaudo-Withers radial result. That is a solid but incremental companion paper, not a new picture.

## 🎯 Relevance to Your Research

Moderately relevant if you work on black-hole perturbation theory, ringdown modelling or plunge waveforms in Kerr. It supplies the position- and direction-dependent bounce criterion needed to generalise the Schwarzschild 'dynamical QNM amplitude' and plunge start-time analyses (De Amicis et al., Kuntz et al.) to rotating holes, and it independently checks the Arnaudo-Withers radial result numerically. It is not directly useful for data analysis or ringdown fits yet. Read it alongside arXiv:2611.03791 rather than on its own.

📖 **Where to start:** Sec. 2.1 for the convergence criterion setup; Sec. 3 for the radial optical distances and the prolate/oblate angular rates; Sec. 4 for the dominance map, the sufficient condition and the 'converges before causal arrival' remark; Appendix on numerics (growth-rate maps, Fig. with n up to 16000) to judge the validation. Section 5 (bounce surfaces, null fronts) is geometric interpretation and can be skimmed.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.8/10)

## 🚧 Caveats

- The Kerr bounce radii and radial convergence regions were already published two weeks earlier by Arnaudo and Withers (arXiv:2611.03791); this paper's new content is the angular dependence and the numerical checks.
- All results are for a/M=0.7, (l,m)=(2,2), s=-2 only.
- Sufficient condition for the fixed-(l,m) pole sum only: branch cut, high-frequency arc and multipole sum are not treated.
- No link yet to waveforms at infinity or to ringdown fit start times; the authors explicitly defer this.

---

🔗 [Back to the weekly digest](../2026-11-24)
