# 🎵 Tidal Excitation of Relativistic Stars

🌠 **Should-Read** · 🔬 Quality 6/10 · 🎯 Relevance 5.5/10

📎 **Citation:** Zhiqiang Miao, Junquan Su, Neev Khera, Huan Yang, *Tidal Excitation of Relativistic Stars*, arXiv:[2610.18475](https://arxiv.org/abs/2610.18475) [gr-qc, astro-ph.HE], submitted 13 Oct 2026.

> 💡 The authors split the gravitational-wave response of a non-rotating neutron star hit by an incoming wave into four parts: a prompt echo identical to a black hole's, a reflection off the stellar surface, the star's ringing modes, and a slowly decaying late-time tail, and they check the split against direct numerical simulations.

## 🔍 Executive Summary

The paper treats tidal driving of a non-rotating perfect-fluid star as a scattering problem: a wave comes in from past null infinity and the star scatters it out to future null infinity. It builds the retarded Green function of the matched interior-Schwarzschild exterior and deforms the frequency contour differently in four causal regions. This separates a prompt piece identical to that of a black hole of the same mass, a wave reflected at the stellar surface, a sum over quasinormal modes, and a late-time tail from a branch cut. A complex bilinear form on the full metric-plus-fluid Hamiltonian phase space then projects an exterior source onto each mode and onto the continuum of branch-cut states, and every amplitude obeys a first-order driven equation. Numerical checks cover mode orthogonality (off-diagonal terms at the 1e-11 to 1e-17 level), the match between the bilinear-form norm and the Green-function residue, and agreement with a time-domain evolution for a delta-like source and for a chirp that sweeps through the f-mode. The post-resonance f-mode amplitude agrees with the authors' earlier stationary-phase result.

## 📣 Claimed Contribution

To the authors' knowledge, the first causal relativistic theory of a star's response to a generic time-dependent tide that treats the direct (prompt plus surface-reflected), quasinormal-mode and tail sectors on equal footing. It is presented as the relativistic counterpart of the Newtonian normal-mode expansion, with each sector driven by an explicit first-order oscillator equation obtained from bilinear projections of the tidal source. A secondary claim, in an appendix, is the first effective-oscillator representation of Schwarzschild black-hole metric perturbations.

## ✅ Strengths

- Concrete, well-defined analytic structure: four causal regions with explicit arrival times (direct, surface-reflected, centre-return) and branch-cut and pole contributions written out in closed form.
- Strong numerical consistency checks: bilinear-form orthogonality across f, p1-p3 and w0-w3 modes at 1e-11 or better, and agreement between the bilinear norm and the Green-function residue to machine precision (Table II).
- Independent time-domain validation in all four causal regions with a full interior-plus-exterior metric-fluid evolution in a different set of variables, not just the same equations solved twice.
- Useful physical observation: the w-mode sector can exceed the f-mode contribution during off-resonance driving because w-mode excitation factors are of order one times the inverse quality factor.
- The full Hamiltonian phase space for even-parity metric-fluid perturbations (ADM plus Brown fluid action) is derived explicitly in an appendix and is reusable.

## ⚠️ Weaknesses

- The direct/mode/tail split during driving depends on an arbitrary choice: how the incident wave from past null infinity is continued into the finite-radius exterior (the power p in the radial profile). The authors admit only the total waveform is invariant. So the mode amplitudes during the inspiral, the quantities that matter for a dynamical-tide model, are not uniquely defined. The intro's 'gauge-sensitive tide' problem has been moved, not solved.
- The mode and continuum amplitudes depend on the observer's position, because the causal windows depend on the observer radius. They are coefficients of the observed field, not intrinsic oscillator coordinates of the star, which weakens the 'relativistic normal-mode expansion' analogy.
- The 'first-order driven oscillator equations' are just the time derivative of the convolution integrals. They add no dynamics beyond the Green-function convolution.
- No orbit and no backreaction: the driver is a prescribed incoming wave, there is no binary, no tidal phase shift and no energy budget for an inspiral, despite the binary-neutron-star motivation. The only physical number obtained (post-resonance f-mode amplitude) reproduces the authors' earlier result.
- The demonstration uses a single toy star (energy polytrope p = K epsilon^2, 1.4 solar masses), l = 2 only, barotropic so no g-modes, no rotation, and a sweep rate chosen for convenience.
- The quasinormal sum is truncated at 32 w-modes and 3 p-modes, and convergence near the onset of the mode region is shown only by eye in figures, without quantified residuals of the reconstructed waveform against the simulation.
- No quantitative comparison with the existing relativistic dynamical-tide frameworks (Pitre and Poisson mode-free expansion, effective-action f-mode models) that the paper says it supersedes.

## 🤔 Skeptic's Cross-Examination

This is the authors' Schwarzschild Green-function decomposition and a published bilinear form, carried over to a fluid star, with convolution integrals renamed as oscillator equations. The headline 'complete modal-nonmodal decomposition' is not unique while the source is on: change the arbitrary continuation of the incident wave and the split between direct, mode and tail pieces changes. What is unambiguous, the post-resonance f-mode amplitude, the authors had already computed in 2025. Nothing here yet feeds a binary-neutron-star waveform model.

## 🆕 Novelty in Context

Every ingredient comes from earlier work, most of it by the same group. The causal-region contour decomposition into a branch-cut direct part, quasinormal modes and tail is Su et al. 2026 (arXiv:2601.22015) for Schwarzschild. The bilinear form extends Minucci et al. 2026 and the earlier bilinear-form literature the paper cites (Leung et al., Green et al., Ma et al. 2024). The scattering picture of tidal driving, the stellar excitation factor and the post-resonance f-mode amplitude are Miao et al. 2025 (arXiv:2506.23176), and the new chirp calculation reproduces that paper's Eq. (36). What is actually new: (i) the extra causal region for a star, which separates a surface-reflected wave from waves that return from the centre (a scalar-field analogue appears in Ould El Hadj 2026, which the paper cites); (ii) a bilinear form on the full metric-fluid phase space, with numerically confirmed orthogonality of f-, p- and w-modes and the identity linking the norm to the excitation factor; (iii) rewriting the convolution integrals as driven first-order equations. The 'first causal theory' framing is defensible only in this narrow technical sense. The relativistic dynamical-tide literature (Pitre and Poisson 2023, who argue mode sums are problematic in GR and propose a mode-free expansion; Katagiri, Yagi and Cardoso 2024 on the ambiguity in splitting tide from response) is cited only in a list. The paper never compares against it, and its own extension-dependence result reproduces exactly the split ambiguity those papers identify. The black-hole appendix claim that 'the effective oscillator representation has long been absent' is overstated: time-dependent excitation coefficients from source projection are already standard in the ringdown literature the paper itself cites.

## 🎯 Relevance to Your Research

Relevant mainly as black-hole and stellar perturbation-theory machinery rather than as tidal phenomenology. It is directly in line with work on source-driven quasinormal-mode excitation, Green-function contour decompositions and bilinear-form projections, which also matter for ringdown of plunging sources and sourced Teukolsky/Zerilli problems in self-force contexts. The black-hole appendix applies the same source-projection-plus-continuum bookkeeping to a Schwarzschild perturber. It is less useful for anyone wanting a better dynamical-tide model for binary neutron star waveforms, which this paper does not provide.

📖 **Where to start:** Sec. II.B.1-2 (stellar reflection coefficient split into prompt and centre-return parts, and the four-region contour strategy); Sec. II.C (bilinear form on the metric-fluid phase space, Table I orthogonality); Sec. III.A.2 (source projections and the residue-norm identity, Table II); Sec. III.B.1 last paragraph (dependence on the choice of continuation, p). Appendix J (Schwarzschild black-hole version) if you care about sourced ringdown. Skip the Hamiltonian appendices unless you need the variables.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 5.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- The split into direct, mode and tail pieces during driving depends on an arbitrary continuation of the incoming wave; only the total waveform is unique.
- Mode amplitudes are observer-dependent coefficients, not intrinsic stellar oscillator coordinates.
- No orbit, no backreaction, no tidal phase: the only physical output (post-resonance f-mode amplitude) reproduces the authors' 2025 result.
- Single toy polytrope, l = 2, non-rotating, no g-modes.
- The 'first causal theory' claim is narrow; the ingredients are the group's own black-hole Green-function decomposition plus an existing bilinear form.

## In Network

- 🚩 Huan Yang — notable author

---

🔗 [Back to the weekly digest](../2026-10-20)
