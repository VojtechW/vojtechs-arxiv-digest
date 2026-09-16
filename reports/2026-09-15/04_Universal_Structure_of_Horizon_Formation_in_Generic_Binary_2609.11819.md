# 🖥️ Universal Structure of Horizon Formation in Generic Binary Black Hole Mergers

🔦 **Worth-Skimming** · 🔬 Quality 6.5/10 · 🎯 Relevance 4/10

📎 **Citation:** Yu-Cun Xie, Vaishak Prasad, *Universal Structure of Horizon Formation in Generic Binary Black Hole Mergers*, arXiv:[2609.11819](https://arxiv.org/abs/2609.11819) [gr-qc], submitted 10 Sep 2026.

> 💡 When two merging black holes first acquire a single shared horizon, that horizon is born as a pair of surfaces whose separation grows as the square root of the time since birth, a law the authors derive analytically and confirm in three full binary simulations.

## 🔍 Executive Summary

The paper analyses the moment in a binary black hole merger when a common apparent horizon first appears on a given time slice. Because no common marginally outer trapped surface exists on earlier slices, the linearised expansion operator (the stability operator) must have a zero mode at that instant; outermost stability then forces that mode to be the principal one, with a strictly positive eigenfunction. A Lyapunov-Schmidt reduction turns the surface equation into a scalar fold (saddle-node) normal form, giving an outer and an inner branch that separate as (t - t_*)^{1/2} on top of a shared linear drift, with all coefficients expressible as integrals of geometric data on the formation surface. Three Einstein Toolkit simulations (equal mass, unequal mass, and an eccentric precessing unequal-mass system) reproduce the predicted surface geometry; free-exponent fits to area, integrated horizon shear and the principal eigenvalue return 0.5 to within about half a percent, and the different diagnostics agree on the formation time at the 1e-5 M level.

## 📣 Claimed Contribution

A symmetry-free local derivation of the structure of first common horizon formation: that the stability operator must lose invertibility, that the zero mode is principal and positive, and that Lyapunov-Schmidt reduction yields square-root branch separation plus a shared linear drift (a 'tilted parabola') with explicitly computable coefficients, together with the first test of this branch structure in generic three-dimensional binary black hole simulations including an eccentric, precessing, unequal-mass case.

## ✅ Strengths

- The theoretical argument is clean and genuinely assumption-light: past isolation forces a zero mode, and the Andersson-Mars-Simon spectral lemmas (real principal eigenvalue, positive adjoint principal mode) are exactly what is needed to make the Lyapunov-Schmidt splitting well posed. No symmetry is assumed anywhere.
- It goes beyond identifying the fold: coefficients B and C are given as explicit pairings of the adjoint zero mode with the second and third shape variations of the expansion and the time derivative of the operator, so the law is predictive rather than phenomenological.
- The numerical test is honest in construction: the formation surface and time are reconstructed from later converged branch pairs, and the reconstruction is then independently checked by evaluating the expansion residual and the stability spectrum on it (RMS Theta_+ ~ 1e-4/M, lambda_0 ~ 1e-6/M^2, with the next eigenvalue at ~0.65/M^2, confirming a one-dimensional kernel).
- Including the next-order term matters and is shown to matter: the principal-eigenvalue fit has a visibly biased exponent (~0.515) at leading order and comes into line (~0.49-0.50) once the correction is added, and fit-window sensitivity drops by a factor of five. That is the kind of internal consistency check that distinguishes a fit from a test.
- Useful practical byproduct: the analysis explains why Newton-based horizon finders lose conditioning at formation (singular Jacobian) and in Simulation II the reconstructed t_* falls on a slice where the finder had failed, so the fitted lag exceeds the search interval. Reconstructed surfaces could seed searches near formation.
- The predicted positivity of the zero mode H_0 is verified pointwise in all three runs, and the shape-fit residuals stay small an order of magnitude in time beyond the fitting window.

## ⚠️ Weaknesses

- The novelty is narrower than 'universal structure of horizon formation' suggests. Booth, Cox and Okpala (arXiv:2605.30458, May 2026) already classified MOTS pair creation as a saddle-node bifurcation of the stability operator; this paper cites it twice as 'concurrent work' although it appeared three and a half months earlier. The genuinely new content is the next-order (drift) term, the explicit coefficient formulae, and the generic three-dimensional numerical validation.
- Once one accepts the zero-mode-at-tangency picture, which Andersson-Mars-Simon established and Pook-Kolb et al. observed numerically, the square-root law is the textbook fold normal form. The derivation is careful but not deep; the physics content is concentrated in the coefficients, which are not evaluated from first principles anywhere, only fitted.
- The two nondegeneracy conditions c_t != 0 and c_2 != 0 are assumed, not proved, and the paper's argument that they hold is that the measured exponent is 1/2 rather than 1/3 - i.e. the conditions are inferred from the very fits they are needed to justify. This is not circular in a fatal way, but it means genericity is asserted, not established.
- The convergence appendix tests the wrong quantities. Mismatches of Psi_4 and of the shear near the horizon pole decrease with resolution, but there is no demonstration that the fitted exponent p, the formation time t_*, or the fields H_0 and H_d converge. The headline claim 'recovers 1/2 to within half a percent' therefore has no attached numerical error bar, and the resolutions are modest (finest spacing M/60 to M/90). Simulation III, the one that carries the 'generic, precessing, eccentric' claim, was run at a single resolution.
- Everything here - t_*, the branch fields, the coefficients, the very existence of the two branches on a slice - is foliation dependent. The paper says this, but the word 'universal' in the title is doing work the results do not support: what is universal is the exponent under smooth reparametrisations of a fixed time coordinate, in moving-puncture gauge.
- The abstract's closing sentence about a signature of common horizon formation in the merger waveform is unsupported speculation. No shear-news comparison is performed; the discussion explicitly defers it, and also concedes the common horizon forms inside the event horizon and sends no signal to infinity.
- The inner branch is located with AHFinderDirect, a finder designed for outermost horizons; the accuracy of inner-branch surfaces near formation (where conditioning is by the paper's own argument worst) is not separately quantified, yet the whole odd-parity signal O[Q] depends on it.

## 🤔 Skeptic's Cross-Examination

The strongest objection is that the paper proves a result whose conclusion was already anticipated and then verifies it with fits that are not error-controlled. The square-root law is the generic fold; given a positive zero mode and quadratic tangency, no other exponent was available, and the paper's 'test' of the exponent is a four-parameter fit to five branch pairs at one resolution per simulation with no demonstration that the recovered exponent is stable under refinement. A 0.5% agreement quoted without a numerical uncertainty is a claim about the fit, not about the spacetime.

## 🆕 Novelty in Context

Literature check: Andersson, Mars and Simon established the spectral properties of the MOTS stability operator and that invertibility gives a unique smooth MOTT, and Andersson-Mars-Metzger-Simon established that the outermost MOTS must jump before the individual horizons touch. Pook-Kolb, Booth, Hennigar, Krishnan and collaborators (2019-2021) showed numerically, in axisymmetry, that MOTSs appear and disappear in pairs with worldtubes turning in slice time, exactly the fold phenomenology. Most directly, Booth, Cox and Okpala, 'Black hole evolutions: Lessons from bifurcation theory' (arXiv:2605.30458, 28 May 2026), already identify MOTS pair creation/annihilation as a saddle-node bifurcation of the stability operator and classify the other possibilities (pitchfork, transcritical), with analytic and numerical examples in Reissner-Nordstrom-de Sitter and Weyl-distorted Schwarzschild. The present paper labels that work 'concurrent', which understates the overlap in the conceptual framework. What survives as new: the specific argument that past isolation plus outermost stability pins the kernel to the positive principal mode at first common horizon formation, the next-order expansion giving the shared linear drift and hence the tilted-parabola form with explicit coefficient formulae, and the demonstration in full three-dimensional binary black hole evolutions including a precessing, eccentric, unequal-mass system rather than in symmetric model spacetimes. That is a real but incremental advance, and the title's 'universal structure' oversells it.

## 🎯 Relevance to Your Research

This sits on the numerical-relativity / quasilocal-horizon side of gravitational physics rather than on small-mass-ratio dynamics, so it does not bear directly on self-force, extreme-mass-ratio inspiral or integrability work. It is worth an hour for two reasons: it is a clean worked example of bifurcation-theoretic (Lyapunov-Schmidt) reduction applied to a geometric evolution problem, a technique transferable to other tangency and branch-splitting problems in relativity; and the horizon-branch structure is the current frontier of understanding what actually happens geometrically at merger, which is the strong-field boundary condition for any waveform model. Read Section 3.3 for the reduction and Section 4.3-4.4 for what the simulations actually show.

📖 **Where to start:** Section 3.3 (Lyapunov-Schmidt reduction and the coefficients c_t, c_2, c_1t, c_3) for the core derivation; Table in Section 4.3 (verification of the reconstructed formation surface, expansion residual and stability spectrum) and Section 4.4 with its formation-time/exponent table for the actual evidence; Section 5 for the honest list of what is left undone. Appendix on convergence is worth a skeptical minute.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 4/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4.0/10)

## 🚧 Caveats

- The conceptual framing - common horizon birth as a saddle-node bifurcation of the MOTS stability operator - was published by Booth, Cox and Okpala (arXiv:2605.30458) three and a half months earlier; this paper calls it 'concurrent'. The new content is the next-order drift term, explicit coefficient formulae, and the three-dimensional numerical test.
- The convergence appendix checks Psi_4 and horizon shear mismatches, not the fitted exponent, formation time or branch fields. The '1/2 to within half a percent' claim carries no numerical error bar, and the precessing eccentric run has only one resolution.
- Formation time, branch fields and all coefficients are slicing dependent; only the exponent is invariant, and only under reparametrisation of a fixed time coordinate. 'Universal' should be read narrowly.
- The abstract's suggestion of a waveform signature of common horizon formation is speculation. No shear-versus-news comparison is done here, and the paper itself notes the event is causally hidden from infinity.
- The nondegeneracy conditions that make the exponent 1/2 rather than 1/3 are assumed and then argued for from the fits they underpin.

---

🔗 [Back to the weekly digest](../2026-09-15)
