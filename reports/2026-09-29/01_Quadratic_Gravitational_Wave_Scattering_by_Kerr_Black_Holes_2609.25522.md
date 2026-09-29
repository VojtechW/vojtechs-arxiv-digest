# 🎵 Quadratic Gravitational-Wave Scattering by Kerr Black Holes

🌠 **Should-Read** · 🔬 Quality 5.5/10 · 🎯 Relevance 6/10

📎 **Citation:** Lennox S. Keeble, Hengrui Zhu, Lawrence E. Kidder, Harald P. Pfeiffer, Mark A. Scheel, *Quadratic Gravitational-Wave Scattering by Kerr Black Holes*, arXiv:[2609.25522](https://arxiv.org/abs/2609.25522) [gr-qc], submitted 22 Sep 2026.

> 💡 Full numerical-relativity simulations show how strongly a spinning black hole converts an incoming gravitational wave into an outgoing wave at twice its frequency, and that this nonlinear response is not fixed by frequency alone, so it cannot be read off from the known couplings between the hole's ringing modes.

## 🔍 Executive Summary

The authors send nearly single-frequency quadrupolar (l=2, m=+-2) gravitational wave trains onto Kerr black holes with spins up to a=0.95 in full numerical relativity. They extract the complex ratio of the outgoing (4,4) wave at twice the frequency to the square of the outgoing parent wave. At low frequency this coupling is strongly suppressed, and it depends on spin in opposite ways for co-rotating and counter-rotating waves. At higher co-rotating frequencies there is a resonance whose fitted frequency and width follow the (4,4,0) quasinormal mode. Near the (2,2,0) quasinormal mode frequency the scattering-state coupling grows with spin, while the known quadratic quasinormal-mode coupling decreases. A one-dimensional model is then fitted to the numerical data and reproduces the trends.

## 📣 Claimed Contribution

The first measurement, using numerical relativity, of the quadratic self-coupling of real-frequency scattering states (not quasinormal modes) of Kerr black holes, mapped against frequency and spin for both co-rotating and counter-rotating waves. The paper also identifies a daughter-mode resonance at the (4,4,0) mode and shows that the coupling depends on the full parent scattering state, not only on its frequency. The abstract adds a 'complementary semi-analytic second-order Teukolsky calculation' that reproduces the numerical response, and offers the results as a basis for generic homogeneous radiative perturbations of Kerr at second order.

## ✅ Strengths

- It asks a well-defined question that has had little attention: quadratic coupling of the real-frequency continuum rather than of quasinormal modes. The observable (complex ratio of the 2-omega (4,4) outgoing amplitude to the square of the parent amplitude) is clean.
- It covers a lot of parameter space: many spins from 0 to 0.95, both co-rotating and counter-rotating, and frequencies from about M|omega|=0.18 up to the (4,4,0) resonance region.
- The contrast with the quadratic quasinormal-mode coupling near the (2,2,0) frequency is a useful physical point. The coupling depends on the radial profile of the parent (in-mode versus quasinormal-mode boundary conditions), not just on its frequency.
- Waveform analysis is documented in detail and is fairly transparent. It uses retarded-time-aligned fits at five extraction radii, polynomial extrapolation in 1/R, fifteen fitting variants to build a sensitivity envelope, and explicit acceptance thresholds.
- The resonance whose frequency and width follow the (4,4,0) quasinormal mode is a sensible consistency check that the nonlinear signal is physical and not an artefact.

## ⚠️ Weaknesses

- I could not read the main body of the letter with the available tools. Only the End Matter and the Supplemental Material were accessible. This assessment of the central claims therefore rests on the abstract and the supplement.
- The 'semi-analytic second-order Teukolsky calculation' in the abstract appears in the supplement as 'a scalar model for qualitative interpretation'. It has a phenomenological potential built from the geodesic radial equation with the Carter constant replaced by l(l+1), and a scalar spin-0 wave equation rather than the spin-weight -2 Teukolsky equation. Its quadratic source contains four free real coefficients, fitted by least squares to 161 numerical data points, with near-resonant points excluded. Agreement with the simulations is therefore largely by construction and is not an independent check. Unless the main text has a separate genuine second-order Teukolsky computation (the supplement documents none), the abstract overstates this component.
- Numerical convergence is weak. In the single convergence test (a=0.95, M omega=0.775), the extrapolated |Q| goes 0.118, 0.694, 1.130, 1.273 across resolutions 0 to 3, and the difference between the two finest resolutions is about 13% in the complex coupling. Only the finest resolution passes the extrapolation criteria, and no convergence order is shown. The plotted error bars cover fit and extrapolation sensitivity, not truncation error, so the true uncertainty is likely at least 10-15% near resonance.
- The initial data are not a pure first-order perturbation. The authors state that the constraint solve produces quadratic (4,4) and axisymmetric content even though the seed is purely quadrupolar, and that they 'retain these nonlinear contributions'. Any daughter content already in the initial data contaminates the attribution of the measured (4,4) signal to scattering. How this is separated is not documented in the parts I could read.
- Twenty-one runs fail the acceptance checks with the default fitting window. Their windows are chosen afterwards to minimise the diagnostics, and four still fail at least one threshold. This post-hoc selection weakens the uniformity of the dataset, especially at the lowest frequency and at the highest co-rotating frequencies for a=0.95, which are the regimes behind two headline claims.
- Only the (2,2)x(2,2) to (4,4) channel at twice the frequency is studied. The broader claim of 'a basis for generic homogeneous radiative perturbations of Kerr at second order' is aspirational given one parent mode, one daughter channel, and wave trains of finite duration.

## 🤔 Skeptic's Cross-Examination

The headline numbers come from a single highest resolution that is itself 13% away from the next resolution down. The initial data already carry nonlinear (4,4) content. The fitting windows for a fifth of the runs were chosen afterwards. The 'theory agreement' is a four-parameter fit of a scalar toy model to those same numbers. What remains robust is qualitative: the trends and the location of the resonance. Precise complex couplings usable as benchmarks at the 1% level are not established.

## 🆕 Novelty in Context

Earlier numerical-relativity and second-order perturbation work on quadratic effects in Kerr has focused on quadratic quasinormal modes. Examples are Zhu et al. 2024 (arXiv:2401.00805, scattering experiments in numerical relativity with the same group and code, extracting the quadratic quasinormal-mode coupling), Ma and Yang 2024 (2401.15516), Bourg et al. 2024-25 (2405.10270, 2503.07432), Bucciotti et al. 2024 (2405.06012), and Fransen et al. 2025 on the light-ring limit. The second-order Teukolsky formalism for Kerr exists (Spiers, Pound and Moxon 2023, 2305.19332), and nonspinning second-order Teukolsky self-force calculations have just appeared (Leather et al., 2609.08995). My INSPIRE searches found no earlier numerical-relativity measurement of quadratic coupling for monochromatic real-frequency scattering states on Kerr, so the main claim, a numerical map of the scattering-state coupling against spin and frequency, looks genuinely new. It is, however, an incremental extension of the same group's 2024 wave-packet scattering setup, moving from ringdown mode fitting to near-steady-state fitting. The 'semi-analytic second-order Teukolsky' part does not hold up as a novelty claim: what is documented is a fitted scalar toy model, not a second-order Teukolsky solution. The resonance at (4,4,0) is expected from the pole structure of the daughter Green's function and confirms known physics rather than revealing new physics.

## 🎯 Relevance to Your Research

Moderately relevant to second-order Kerr perturbation theory and second-order self-force. The homogeneous radiative sector at second order, meaning quadratic coupling of real-frequency incoming and outgoing waves, is exactly what second-order self-force and dynamical-tide calculations need, and full numerical-relativity reference values against spin are scarce. In practice, the useful output is the numerical-relativity coupling data as a benchmark for a real second-order Teukolsky code, for example one built on the Spiers-Pound-Moxon source. Do not treat the fitted scalar model as a result.

📖 **Where to start:** Main-text figures of the coupling against frequency and spin, and the comparison with the quadratic quasinormal-mode coupling (Figs. NRcoupling and qnm_coupling_comparison). Supplement section 'Numerical-relativity diagnostics', especially the resolution study and the paragraph on sample selection, to judge the error budget. Supplement section 'A scalar model for qualitative interpretation', subsection 'Numerical implementation', to see that the model's source coefficients are fitted to the numerical data. End Matter on initial data for the retained quadratic content.

## Scores

- 🔬 **Quality:** 5.5/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- The 'semi-analytic second-order Teukolsky calculation' is, in the supplement, a phenomenological scalar toy model with four source coefficients fitted to the numerical data, so its agreement with the simulations is not a prediction.
- The two finest resolutions differ by about 13% in the coupling for the one case tested, and the plotted error bars do not include truncation error.
- The initial data themselves contain quadratic (4,4) content from the constraint solve, which the authors keep.
- Only one channel is studied, (2,2)x(2,2) to (4,4) at twice the frequency; the 'generic basis' framing is ahead of the results.
- This review could access only the End Matter and the Supplemental Material, not the main letter text.

## In Network

- 🚩 Harald Pfeiffer — notable author

---

🔗 [Back to the weekly digest](../2026-09-29)
