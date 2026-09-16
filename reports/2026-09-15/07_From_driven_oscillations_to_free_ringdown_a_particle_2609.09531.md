# 🎵 From driven oscillations to free ringdown: a particle plunging into Kerr

🌠 **Should-Read** · 🔬 Quality 7/10 · 🎯 Relevance 7/10

📎 **Citation:** Colin Weller, Andrew Laeuger, Fulin Li, Neil Lu, Rowina S. Nathan, Sizheng Ma, Yanbei Chen, Ling Sun, *From driven oscillations to free ringdown: a particle plunging into Kerr*, arXiv:[2609.09531](https://arxiv.org/abs/2609.09531) [gr-qc, astro-ph.HE, hep-th], submitted 08 Sep 2026.

> 💡 The wave emitted when a small body falls into a spinning black hole can already look exactly like a fixed sum of the hole's own ringing tones at a time when every one of those tones is still being actively shaken by the falling body.

## 🔍 Executive Summary

The authors build a first-principles rational (pole-and-zero) model of the Kerr response function for the dominant quadrupole wave, using the quasinormal-mode poles, their physical residues, and the zeros located at the horizon-related frequencies that govern the late-time plunge source. Driving this model with the exact Teukolsky source of a point particle plunging from the innermost stable circular orbit for black-hole spins 0.5 to 0.9, they track each pole's contribution separately and find that each one initially oscillates at the source's instantaneous complex frequency rather than at its own ringing frequency, decoupling only once the source has decayed faster than that mode. Because the response function's zeros sit exactly at the frequencies at which the late source oscillates, the source-frequency pieces cancel in the coherent sum, leaving a waveform that is well described by a fixed-coefficient superposition of ringing tones even while the individual pieces remain driven. The pole sum reproduces the exact waveform to about two parts in a thousand of the peak even before the peak, whereas using the bare physical residues without preserving the zeros misses by up to 12 percent at spin 0.5.

## 📣 Claimed Contribution

That a ringdown waveform can admit a constant-coefficient quasinormal-mode representation while its individual mode-pole contributions are still driven by the source; plus a first-principles rational approximation to the Kerr Green's function built from quasinormal poles, physical residues and horizon-frequency zeros, and the demonstration that those zeros cancel the source-frequency content of the plunge waveform.

## ✅ Strengths

- The central claim is backed by an actual frequency-domain Teukolsky calculation with a real plunge source at five spins (0.5-0.9), not by a toy model or hand-waving.
- The rational approximation is validated against the numerically computed time-domain kernel with quantified residuals: relative error below 1 percent by t = 6.3, 2.1, 1.8, 1.8, 2.2 M and below 0.1 percent by t = 20.8, 17.4, 12.6, 10.3, 7.2 M for spins 0.5 to 0.9.
- The paper tests its own construction against the obvious alternative: a supplemental section repeats the analysis with the bare physical residues (which do not preserve the horizon-frequency zeros) and quantifies the degradation (up to 12 percent of peak pre-peak at spin 0.5 versus ~2e-3 with the modified residues).
- The driven-versus-free split is made precise rather than rhetorical: an explicit adiabatic criterion eps_ad = |d(omega_src)/dt| / |omega_src - omega_n|^2 and an exact decomposition y_n = C_n exp(-i omega_n t) + y_{s,n} with a closed-form residual for an exponential source.
- Useful data product: a table of (2,2) prograde overtones to n = 13 and retrograde overtones to n <= 9, with physical residues c_n and the modified rational residues g_n, at five spins.
- Numerical hygiene is documented in unusual detail (trajectory initialization, smoothstep windows, frequency grid chosen so that 2*Omega_H does not land on a grid point at spin 0.8, zero-padding, offset subtraction), and the small apparent acausal precursor in the numerical kernel is flagged rather than hidden.

## ⚠️ Weaknesses

- The decomposition into 'driven pole contributions' is representation-dependent. The residues g_n used to define the individual mode contributions differ substantially from the physical residues at twelve paired poles: |g_n/c_n| reaches 2.8-4.3 and arg(g_n/c_n) reaches 165 degrees. Statements about what an individual mode is doing at a given time therefore depend on which rational approximant was chosen, even though the coherent sum is fixed.
- The physical setting is a test particle on a geodesic plunge with no radiation reaction, a fixed background, energy tuned to E_ISCO(1+1e-5), only the (2,2) equatorial mode, and only spins 0.5-0.9. The extrapolation to comparable-mass mergers, where the background itself is evolving and the 'source' is not a separable test-particle term, is not demonstrated here.
- The quoted agreement levels are for windowed quantities: the source is multiplied by smoothstep tapers in both the ramp-on and roll-off regions, and both the source and the response are multiplied by a Gaussian frequency window exp(-(M*omega/2)^2) that smooths the time series on a ~0.7 M scale. A 0.7 M smoothing is not negligible on the timescale of the highest overtones retained, so the accuracy claims should be read as accuracy of a smoothed comparison.
- The apparent acausal precursor in the numerically evaluated kernel is explained only heuristically (a sgn(omega) piece in the high-frequency asymptotics generating a ln|t| term) and the authors explicitly state they cannot resolve it or establish its character from their finite-frequency integral.
- The result is interpretive rather than operational: it tells you that a good constant-coefficient fit does not license the inference 'the perturbation is now source-free', but it provides no prescription for ringdown start times, no error budget for existing overtone fits, and no template-level deliverable.
- Reading limitation on my side, stated for honesty: the Letter body could not be retrieved through the section-extraction tools (the source has no sectioning commands before the bibliography), so this assessment rests on the abstract plus the complete Supplemental Material, including its methods, validation numbers and figure captions. Claims made only in the main body (in particular the detailed decoupling times and the derivation that the late source approaches the third and higher horizon frequencies) are taken at face value.

## 🤔 Skeptic's Cross-Examination

A skeptic would say the headline is bookkeeping. The waveform is a single physical object; splitting it into 'driven pole contributions' plus 'source-frequency components' requires choosing a rational approximant, and the authors' choice deliberately deforms twelve residues away from their physical values (by up to a factor 4.3 in magnitude and 165 degrees in phase) in order to enforce the zeros. Change the approximant and you change what each 'mode' is said to be doing, while the sum is unaffected. The paper's own supplemental comparison with the bare physical residues blunts this objection - the qualitative conclusion survives at the few-percent level - but it does not remove it, and it means the quantitative decoupling times attached to individual overtones should not be taken as physical observables.

## 🆕 Novelty in Context

The two ingredients are individually old. Mino and Brink (arXiv:0809.2814) already showed that the plunge radiation contains universal damped oscillations at horizon-set frequencies distinct from the free quasinormal frequencies, and the 'MB' labelling of the zeros in this paper points back to exactly that work. The picture of a quasinormal pole as a damped oscillator driven at a source frequency, with response proportional to 1/(omega_src - omega_n), is standard in the second-order and nonlinear quasinormal-mode literature and is close in spirit to treatments such as Kehagias and Riotto's adiabatic-mode framing (arXiv:2411.07980) and to resonance-driven excitation studies such as Kubota and Motohashi (arXiv:2509.06411). My own searches did not turn up a prior statement of the specific combination claimed here, namely that the horizon-frequency zeros of the Kerr response cancel the source-frequency content so that the coherent waveform is representable with constant quasinormal coefficients while the pole contributions are still driven. So the novelty claim survives, but it should be read as a reinterpretation assembled from known structures rather than a new computational capability: the Teukolsky machinery, the plunge source, the overtone spectrum and the horizon frequencies were all available. Its main value is as a corrective to a widespread inference in the overtone-fitting literature (e.g. the constant-coefficient fits catalogued by Dyer and Moore, arXiv:2510.13954), where a good early fit is often read as evidence that the ringdown has become free.

## 🎯 Relevance to Your Research

Directly in the reader's technical territory: frequency-domain Teukolsky theory, plunge from the innermost stable circular orbit in Kerr, the analytic structure of 1/(i*omega*B_in), and the meaning of quasinormal-mode fits. It bears on the transition-to-plunge and merger end of extreme-mass-ratio waveform modelling, and it sharpens what one is entitled to conclude from a good overtone fit near the peak. The tabulated overtone frequencies and residues (prograde to n = 13, retrograde to n <= 9, five spins) are reusable. Worth reading the supplemental subsections on the single-mode driven dynamics, on the physical-residue comparison, and on the time-domain kernel validation; the trajectory and windowing subsection is the place to judge how much of the quoted accuracy is real.

📖 **Where to start:** The abstract and main-text figures for the central claim; Supplemental subsection 'Dynamics of a single QNM' for the adiabatic criterion and the exact free-plus-residual decomposition; 'Driven modes with the physical residues' for the key robustness test (12 percent versus 2e-3); 'Time-domain response and its rational approximation' for the kernel validation and the precursor discussion; 'The source: trajectories and windows' to judge the numerics; and the residue table for reusable overtone data.

## Scores

- 🔬 **Quality:** 7/10
- 🎯 **Relevance:** 7/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.6/10)

## 🚧 Caveats

- Test-particle geodesic plunge in a fixed Kerr background, no radiation reaction, (2,2) mode only, spins 0.5-0.9; comparable-mass mergers are not simulated.
- The statement that individual modes are 'driven' refers to the pole contributions of a particular rational approximant whose residues differ from the physical ones by factors up to ~4 in magnitude and by large phases at twelve poles.
- All waveform comparisons are made after smoothstep time-domain windows and a Gaussian frequency window that smooths on a ~0.7 M scale.
- The small acausal precursor in the numerically computed kernel is acknowledged but unresolved.
- Conceptual result: no ringdown start-time prescription or data-analysis recipe is delivered.

---

🔗 [Back to the weekly digest](../2026-09-15)
