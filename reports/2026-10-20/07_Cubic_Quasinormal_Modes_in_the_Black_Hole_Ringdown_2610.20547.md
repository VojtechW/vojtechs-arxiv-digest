# 🎵 Cubic Quasinormal Modes in the Black-Hole Ringdown

🌠 **Should-Read** · 🔬 Quality 6/10 · 🎯 Relevance 6/10

📎 **Citation:** Neev Khera, Huan Yang, *Cubic Quasinormal Modes in the Black-Hole Ringdown*, arXiv:[2610.20547](https://arxiv.org/abs/2610.20547) [gr-qc], submitted 14 Oct 2026.

> 💡 The first calculation from Einstein's equations of how three ringing modes of a spinning black hole combine into new third-order tones; when the predictions are added to a simulated merger signal, they appear to carry a large share of the signal shortly after the peak.

## 🔍 Executive Summary

The authors extend black-hole perturbation theory around a rotating (Kerr) black hole to third order. They reconstruct the first- and second-order metric perturbations with Newman-Penrose transport equations in split light-cone gauges, then solve the sourced third-order Teukolsky equation in the frequency domain on a hyperboloidal, compactified grid along complex radial contours. The output is a table of complex coupling coefficients that fix each cubic mode amplitude as a product of three linear parent amplitudes. Applied to one numerical-relativity waveform (SXS:BBH:0305, remnant spin 0.692), the six cubic products of the (2,2) fundamental mode, its first overtone and their conjugates reduce the fit mismatch over some start times without adding free parameters, and they shift the fitted overtone amplitudes. At 3M after the peak, the summed cubic contribution is quoted as about 38% of h22.

## 📣 Claimed Contribution

A first-principles formulation and numerical solution of the nonlinear Teukolsky equations through third order in Kerr, giving spin-dependent cubic quasinormal-mode coupling coefficients. The authors also claim that these parameter-free cubic terms improve numerical-relativity ringdown fits and contribute appreciably in early ringdown.

## ✅ Strengths

- A real technical step beyond the authors' own second-order Kerr work (Khera, Ma and Yang, Phys. Rev. Lett. 134, 211404). Third order needs the second-order metric reconstructed from the curvature, which is hard. The supplement sets this out explicitly: a hierarchy of Newman-Penrose transport equations, with homogeneous solutions fixed by asymptotic flatness, residual gauge freedom, and boundary data at infinity derived from Psi_4.
- Careful numerics for imposing outgoing boundary conditions. Pairs of reflected complex radial contours keep the conjugated fields on a shared contour, the outgoing condition is imposed in the correct Stokes sector, and the two contour solutions are averaged for purely imaginary frequencies (the m=0 cubic modes).
- The cubic amplitudes have no free parameters. They are fixed by the fitted parent amplitudes and the computed couplings, so the linear-plus-cubic model has the same number of fitted amplitudes as the linear-only model.
- Gives concrete, reusable numbers: a table of complex coupling coefficients at spin 0.692085, projected onto the spherical (2,2), (3,2) and (4,2) harmonics.
- Tests the predicted angular structure in the higher harmonics h32 and h42 rather than only in h22, and reports honestly that h42 gets worse at early fit start times.

## ⚠️ Weaknesses

- The main Letter text could not be read with the available tools. Only the supplementary sections (transport equations, contours, coupling table, fitting method, higher harmonics, component plots) and the abstract were accessible. Comments on the main-text novelty framing, the convergence tests, and the exact definition of the 38% figure therefore rest on the abstract and the supplement.
- Near-degeneracy with overtones is the core identifiability problem. The cubic product I0^2 conj(I0) oscillates at the fundamental frequency's real part and decays three times as fast. At spin about 0.69 that is roughly 0.533 - 0.242i, almost on top of the linear first overtone (about 0.521 - 0.244i). Likewise I0 I1 conj(I0) sits near the second overtone. 'Shifts inferred linear-overtone amplitudes' is therefore close to automatic, and a better mismatch is weak evidence that the cubic physics is right.
- The supplement admits that the individual cubic products are larger than their coherent sum. These cancellations are 'analogous to those observed in linear overtone fits', the same signature of overfitting that has been criticised in overtone analyses. A 38% cubic share at 3M, built from cancelling terms, is a fragile headline.
- If third-order terms carry 38% of the signal, the perturbative hierarchy looks broken at that time. From what could be read, there is no discussion of the expected fourth-order size or of the quadratic contributions that could enter the m=2 harmonics.
- Everything rests on one non-precessing, nearly equal-mass simulation (SXS:BBH:0305) and on 'selected' fitting windows. There is no scan over mass ratio or spin, so the size of the effect may not generalise.
- The fits use a custom weighting built from a linear reference fit through n=4. The same scales are used for both models, but the weighting itself comes from linear-model residuals, which may favour whichever model absorbs those residuals.
- The coupling table gives six significant figures, but the supplement read here contains no convergence or error estimate for the couplings.

## 🤔 Skeptic's Cross-Examination

The leading cubic product I0^2 conj(I0) has almost the same complex frequency as the (2,2,1) overtone, and I0 I1 conj(I0) sits near the (2,2,2) overtone. Adding them with fixed amplitudes mainly redistributes power that linear overtones were already absorbing. A lower mismatch over chosen windows in one simulation, with individual cubic terms cancelling each other, does not show that a 38% cubic component is physical rather than another rearrangement of an over-complete basis of damped sinusoids at times when perturbation theory is questionable. A convincing test would check that the cubic amplitudes predicted from the parents stay stable as the fit start time varies, across many simulations.

## 🆕 Novelty in Context

Literature checks on INSPIRE (titles containing 'cubic quasinormal', third-order ringdown, nonlinear quasinormal modes) found no earlier first-principles cubic quasinormal-mode amplitude calculation in Kerr. The paper builds directly on the authors' own second-order Kerr couplings (Khera, Ma and Yang 2024, PRL 134, 211404), on the competing quadratic Kerr computations (for example Ma and Yang 2024, 2401.15516), on Lagos and Hui's Schwarzschild work, and on the second-order Teukolsky formalism (Spiers, Pound and Moxon 2023). Earlier fitting studies of numerical-relativity data (Cheung et al. 2023, 2310.04489) extracted second-order modes with free amplitudes, but that was phenomenological fitting, not cubic couplings derived from the field equations. So the 'first-principles cubic couplings in Kerr' claim appears to stand. The observational claim is smaller than the abstract suggests: it is a fit improvement on one simulation, in a regime where cubic and overtone frequencies nearly coincide. It extends the same group's GW250114 quadratic-mode programme (Wang et al. 2026, 2601.05734) rather than independently confirming it. A Schwarzschild-only third-order calculation could not be fully excluded with the queries run.

## 🎯 Relevance to Your Research

Directly relevant to Kerr perturbation theory beyond first order: metric reconstruction, sourced Teukolsky equations, hyperboloidal frequency-domain methods. The Newman-Penrose/GHP transport hierarchy and the complex-contour treatment of outgoing boundary conditions carry over to second-order self-force work. Less relevant to EMRI waveform modelling as such; the application is comparable-mass ringdown spectroscopy.

📖 **Where to start:** Supplement section 'Newman-Penrose transport equations', for the third-order metric reconstruction scheme and boundary data; 'Complex radial contours and outgoing boundary conditions', for the Stokes-sector treatment; the coupling-coefficient table; and 'Waveform components and cancellation', to judge the 38% claim. In the main Letter, the waveform-fit figures that show amplitude stability against fit start time.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.4/10)

## 🚧 Caveats

- One simulation (SXS:BBH:0305) and 'selected' fit windows; no survey over mass ratio or spin.
- The dominant cubic products sit almost on top of the linear first and second overtones in frequency, so cubic modes and overtones are hard to tell apart in fits.
- The 38% cubic share at 3M comes from cubic terms that partly cancel each other, the same overfitting signature seen in overtone fits; it also means perturbation theory is being pushed to its limit.
- h42 agreement can get worse at early start times when cubic terms are added.
- The coupling coefficients are given at a single remnant spin, with no error bars in the supplementary material.

## In Network

- 🚩 Huan Yang — notable author

---

🔗 [Back to the weekly digest](../2026-10-20)
