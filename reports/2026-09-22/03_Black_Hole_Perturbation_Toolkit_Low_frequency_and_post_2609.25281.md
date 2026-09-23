# 🌀 Black Hole Perturbation Toolkit: Low frequency and post-Newtonian expansions

🌟 **Must-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 8/10

📎 **Citation:** Jakob Neef, Chris Kavanagh, Adrian Ottewill, *Black Hole Perturbation Toolkit: Low frequency and post-Newtonian expansions*, arXiv:[2609.25281](https://arxiv.org/abs/2609.25281) [gr-qc, hep-th], submitted 21 Sep 2026.

> 💡 A free, documented software package now computes weak-field analytic solutions of the equation governing waves around a spinning black hole, automating a step that until now most groups did with private, hand-tuned code.

## 🔍 Executive Summary

This is the companion paper to version 1.2 of the Teukolsky package and version 1.1 of the SpinWeightedSpheroidalHarmonics package in the Black Hole Perturbation Toolkit. It documents new functionality that solves the radial Teukolsky equation analytically in the Mano-Suzuki-Takasugi representation as a low-frequency (post-Minkowskian) or post-Newtonian series: the series coefficients, the renormalised angular momentum, all the standard asymptotic amplitudes, the tidal response ratio, the scattering phase shift, the homogeneous radial functions, and, for circular orbits in Kerr, the inhomogeneous solution and the energy and angular-momentum fluxes at infinity and the horizon. Everything works for generic spin weight and generic harmonic indices as well as for fixed ones, and the authors document the awkward technical part in detail: the places where the three-term recurrence degenerates (beta coefficients vanishing at n = -l, -l-1, -2l-1) and the leading orders of the series coefficients must be determined by an order-balancing argument case by case. Validation is against the toolkit's own numerics, against the stored post-Newtonian self-force data (agreement in Kerr fluxes to 7PN) and against the independent package of Markovic and Ivanov, with quoted timings of roughly four minutes for a 7PN radial function on a laptop and a doubling of cost per additional order.

## 📣 Claimed Contribution

The first open-source, end-to-end package for post-Newtonian self-force computations: an automated, fast implementation of MST low-frequency and post-Newtonian expansions of the radial Teukolsky equation inside the Black Hole Perturbation Toolkit, covering MST coefficients, renormalised angular momentum, amplitudes, phase shift, homogeneous and inhomogeneous radial solutions and fluxes, for specific and generic s, l, m, plus an extended analytic SpinWeightedSpheroidalHarmonics package and a suite of Mathematica SeriesData utilities.

## ✅ Strengths

- It fills a real gap: high-order analytic MST work has been done for fifteen years with private, largely undocumented Mathematica notebooks, and the barrier to entry has been correspondingly high. Making this public and documented is worth more to the field than another single analytic result.
- Not vapourware. The code in earlier form already underlies eight cited publications (Cunningham, Castillo et al., Bjerrum-Bohr et al., Khalaf et al., Casals et al., Brunello et al.), so it has been exercised on real problems before the paper appeared.
- Section 5 is genuinely useful technical documentation, not filler. The degenerate cases of the MST recurrence (beta_{n,0} = 0 at n = -l, -l-1, -2l-1) and the resulting order-balancing for the leading coefficients are practitioner folklore that is rarely written down anywhere; having it laid out spin by spin, including the ma = 0 subcase, is a service.
- Three independent validation channels: numerical Teukolsky solutions across the (a, omega, r) plane with residuals showing the expected power-law convergence, the PostNewtonianSelfForce data repository (Kerr fluxes agreeing to 7PN), and the independent Markovic-Ivanov package (3PM phase shift).
- Honest about the competitor. They disclose the concurrently published Markovic-Ivanov package, report agreement, and report where the intermediate results disagreed and why (their truncation of the a_n series), rather than quietly omitting it.
- Practical engineering detail that will actually save users time: the auxiliary power-counting parameter gamma to keep log(omega) out of SeriesData coefficients, gamma/polygamma canonicalisation to a fixed argument offset, and double application of the Euler reflection formula to recover cancellations in the K ratio.

## ⚠️ Weaknesses

- No new physics. This is a manual, and it should be read as one; the physics content is entirely inherited from MST and from the existing post-Newtonian self-force literature.
- The advertised new results are advertised rather than delivered. The abstract and introduction say they compute the scattering phase shift 'beyond what to our knowledge has been presented in the literature' (9PM versus the 3PM of Markovic-Ivanov), but what the paper actually shows for 9PM is a timing plot; the coefficients are not tabulated in the text, so the claim cannot be checked or cited.
- 'End-to-end post-Newtonian self-force' is a stretch given what is in the box. Inhomogeneous solutions exist only for circular orbits in Kerr; eccentric, spherical and inclined orbits are future work; KerrGeodesics has no PN implementation; and the conclusions concede that no metric-reconstruction package exists, so a user wanting an actual local self-force rather than a flux still needs private code for the last step.
- The strongest available cross-check is not reported. Schwarzschild circular-orbit fluxes are known analytically to 22PN (Fujita 2012, cited in the introduction); the flux validation stops at 7PN in Kerr. A 22PN Schwarzschild reproduction would have been the decisive test of the high-order machinery and its absence is conspicuous.
- 'State of the art precision on regular laptops' is oversold. The quoted scaling is a doubling of runtime per order, 7PN takes about four minutes for radial functions, and reaching 15PN required a cluster. Exponential scaling with a four-minute anchor at 7PN means the laptop ceiling is roughly 10PN, below the Schwarzschild state of the art.
- Generic-s and generic-l functionality, one of the headline new features, is acknowledged to hit a bottleneck at higher orders because of expression swell, and no quantitative statement is given about where that ceiling actually is.
- Error control is presented graphically (relative-error maps and residual plots) rather than as quantified bounds; the paper does not state, for a given truncation order, what accuracy a user should expect at a given (a, omega, r), beyond 'build intuition on where the analytical approximations behave well'.
- Deliberately thin on the user-facing interface: the authors explicitly decline to document options, inputs and outputs, deferring to the in-package Mathematica documentation. That is defensible but means the paper is not self-contained as a reference.

## 🤔 Skeptic's Cross-Examination

A skeptic would say the paper claims a first that a paper it itself cites already achieved, and then quantifies the difference with a single benchmark (3PM phase shift, 5 s versus 200 s) run on the authors' own machine, with the competitor's manual-intervention time excluded by fiat. Push harder and the same skeptic would attack the validation: every high-order check is against data the toolkit already ships (PostNewtonianSelfForce to 7PN) or against the authors' own numerics, both of which share assumptions with the new code; the one genuinely external analytic benchmark, Fujita's 22PN Schwarzschild flux, is cited in the introduction and never used. The headline 'beyond the literature' phase shift is then presented without coefficients. The honest reading is that the code is very probably correct at the orders checked, and untested where it matters most.

## 🆕 Novelty in Context

The 'first open-source package' claim needs one qualification and survives it, but only just. Markovic and Ivanov (arXiv:2511.04765, Phys. Rev. D 114, 024002) published a public analytic MST package for gravitational scattering amplitudes roughly ten months earlier; this paper says it became aware of that work while preparing the manuscript and compares against it. So this is not the first public analytic MST code in absolute terms. The defensible version of the claim, and the one the authors can support, is different in two ways: (i) the functionality here was merged into the toolkit as Teukolsky v1.1 in early 2025, predating the Markovic-Ivanov release, and had already been used in publications; (ii) the scope is much wider (post-Newtonian rather than purely post-Minkowskian, plus homogeneous radial functions, inhomogeneous circular-orbit modes, fluxes, and the angular package), it is fully automated where the competitor needs manual intervention, and it is about forty times faster on the shared 3PM benchmark. What is genuinely not new is the physics or the method: MST is thirty years old, and high-order analytic PN self-force results (Fujita to 22PN in Schwarzschild, Kavanagh et al., Bini-Damour, Munna-Evans, Sago et al.) have been produced for over a decade with private implementations, one of which belongs to an author of this paper. The contribution is openness, automation and speed, not capability that did not exist. Note also that the toolkit's own PostNewtonianSelfForce package already distributed the resulting data; what was missing was the generator, which is exactly what this supplies.

## 🎯 Relevance to Your Research

Directly usable infrastructure for anyone doing Kerr perturbation theory, self-force or EMRI waveform work. If you have ever needed a PN-expanded homogeneous Teukolsky solution, an asymptotic amplitude, the renormalised angular momentum to high order, or a weak-field cross-check on a numerical flux calculation, this replaces a private notebook you would otherwise have had to write or beg for. The generic-s, generic-l functionality is the part most likely to matter for structural or formal work, and the analytic SpinWeightedSpheroidalHarmonics upgrades (symbolic theta derivatives, recursion identities, automatic conjugation) are independently handy for mode-coupling calculations. Treat it as a tool announcement to be bookmarked and used, not as a result to be absorbed.

📖 **Where to start:** Section 3 ('Features at a glance') to decide in two minutes whether the package does what you need. Section 4.3 for the eta and gamma power-counting conventions, which you must get right before trusting any output and which differ from some conventions in the literature. Section 5.2-5.3 if you care how the degenerate MST recurrences are handled, or if you plan to extend the code. Section 9 for what has and has not actually been validated, and for realistic timings. Skip sections 6-8 unless you are using those specific functions.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 8/10
- 🌟 **Reading priority:** Must-Read (weighted score 7.2/10)

## 🚧 Caveats

- A software manual, not a physics result. No new physical content.
- Not the first public analytic MST code: Markovic and Ivanov (arXiv:2511.04765) got there first in print. The real claims are wider scope, full automation and roughly forty times the speed.
- The 9PM scattering phase shift billed as beyond the literature is shown only as a timing, not as coefficients you can use or check.
- 'End-to-end self-force' means circular orbits in Kerr only, and stops short of metric reconstruction; eccentric and inclined orbits are future work.
- Highest external analytic cross-check is 7PN Kerr fluxes against the toolkit's own stored data. The obvious 22PN Schwarzschild benchmark is cited but never used.
- Runtime doubles per PN order; 15PN needed a cluster, so the laptop ceiling is nearer 10PN than the abstract implies.

## In Network

- 🚩 Chris Kavanagh — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-09-22)
