# 🌀 Second-order Teukolsky calculations for nonspinning, quasicircular binaries

🌟 **Must-Read** · 🔬 Quality 8.5/10 · 🎯 Relevance 9.5/10

📎 **Citation:** Benjamin Leather, Andrew Spiers, Adam Pound, Samuel D. Upton, Barry Wardell, Leanne Durkan, Niels Warburton, *Second-order Teukolsky calculations for nonspinning, quasicircular binaries*, arXiv:[2609.08995](https://arxiv.org/abs/2609.08995) [gr-qc], submitted 08 Sep 2026.

> 💡 The first calculation of second-order gravitational-wave emission from a small body orbiting a black hole using the curvature-based master equation rather than the metric itself, reproducing the established answer and opening a route to spinning black holes.

## 🔍 Executive Summary

The authors build and run a complete pipeline for solving the second-order Teukolsky equation for a point mass on a quasicircular inspiral in Schwarzschild, replacing the existing approach of solving the second-order Einstein equations directly in Lorenz gauge. The scheme combines a multiscale expansion, a puncture/effective-source treatment of the particle, a first-order transformation to a Bondi-Sachs gauge, fully compactified hyperboloidal slicing so that the horizon and future null infinity are grid points, multidomain Chebyshev collocation outside the worldtube, and an integrated-by-parts variation-of-parameters solve inside it. They compute the (2,1) and (2,2) second-order energy-flux coefficients at 27 radii between 7M and 20M, agreeing with the published Lorenz-gauge fluxes at the 1e-5 level for (2,1) and 2-3e-4 for (2,2), and reproducing the 4.5PN expansion in the weak field. They also analyse the infrared behaviour, finding that the hereditary/memory divergences that force extra boundary conditions in the Lorenz-gauge multiscale equations are milder in the Teukolsky variable and absent once the Bondi-Sachs gauge is used.

## 📣 Claimed Contribution

The first second-order gravitational self-force calculation performed in the Teukolsky formalism rather than by direct Lorenz-gauge solution of the second-order Einstein equations; a numerical scheme (compactified hyperboloidal slicing with the horizon and null infinity as grid points, first-order transformation to Bondi-Sachs gauge before solving at second order, mixed spectral/variation-of-parameters solver with integration by parts to move derivatives off the low-differentiability effective source) formulated so as to carry over to Kerr; and a re-examination of the second-order infrared divergences showing they are weaker for the Teukolsky variable and eliminated in Bondi-Sachs gauge.

## ✅ Strengths

- The strategic case is real and clearly argued: the existing Lorenz-gauge second-order machinery is built on complete tensor-harmonic separability of the Schwarzschild field equations, which Kerr simply does not offer, whereas the Teukolsky route survives the move to Kerr. Second-order-in-Kerr is the actual bottleneck for astrophysical extreme-mass-ratio waveforms.
- Validation is nontrivial and quantitative: mode-by-mode comparison with the published Lorenz-gauge fluxes at 22 directly-tabulated radii, plus an independent analytic check against the 4.5PN expansion, with the observation that the Teukolsky-Lorenz difference is only 3% (for (2,1)) and 24% (for (2,2)) of the residual against 4.5PN, i.e. the bulk of the post-Newtonian residual is common to both numerical codes rather than a Teukolsky-specific error.
- The numerical-methods choices are motivated by concrete pathologies rather than fashion. Compactifying so that null infinity is a grid point removes finite-radius extraction and extrapolation entirely; the integration-by-parts variation-of-parameters trick inside the worldtube is a genuinely sensible response to the fact that the effective source is only C^1 at the worldline while the Einstein-to-Teukolsky operator wants two more derivatives of it.
- The infrared analysis is careful and self-critical: the appendix identifies precisely the two modes ((l,m) = (2,0) and (0,0)) for which 'compactification plus regularity' genuinely fails and extra boundary conditions carrying a memory integral over the whole past history are unavoidable, and reconciles this with the earlier Green's-function-convergence arguments.
- The error budget appendix is unusually honest, including an explicit statement that the error bars 'summarize the measured sensitivities, not a statistical confidence interval or a complete error bound', that some source responses are interpolated between tested radii, and that the source-response tests were not repeated with the final radial settings.

## ⚠️ Weaknesses

- Only two modes, (2,1) and (2,2), are computed. There is no total flux, no l > 2, and therefore no 1PA waveform or phase from this pipeline; the paper is a method demonstration whose physical output is a subset of a result published in 2021.
- The calculation is not independent of the machinery it validates against: the first-order fields and the effective sources are converted from the existing Lorenz-gauge infrastructure of Warburton et al. and Wardell et al. The 'two largely independent calculations' framing is qualified in the text but the shared inputs mean a common error in the puncture or first-order data would cancel in the comparison.
- The (2,2) agreement is only 2-3e-4, roughly 30 times worse than (2,1), and the paper cannot identify the origin: the fixed-source radial tests are orders of magnitude tighter (below 6.5e-9), so the discrepancy sits in the source/matching data or in the Lorenz reference. The authors can only say it falls within the Lorenz-gauge reference envelope at 20M, not at all radii.
- The infrared result is framed as a highlight of this paper but is, by the authors' own words in the conclusion, 'confirming the conclusion of Ref. [Spiers, Pound, Moxon 2026]' -- a companion paper by overlapping authors three months earlier. The new content here is the compactified-regularity route to the same statement plus the Lorenz-gauge appendix, not the statement itself.
- The Kerr claim, which is the entire strategic justification, is asserted rather than demonstrated. The conclusion concedes that the source no longer separates, that the mode-mixing strategy is unresolved between two competing approaches, and that the required second-order puncture in Kerr does not yet exist ('actively in development'). Nothing in this paper tests that the scheme survives those obstacles.
- No computational cost or efficiency comparison against the Lorenz-gauge pipeline is given, despite efficiency being invoked in the introduction as one of the motivations ('opens the door to the dense coverage of parameter space').
- Minor but telling: the appendix comparing infrared analyses contains a garbled, half-uncommented sentence fragment, and the conclusion retains a large commented-out bullet-point skeleton, suggesting the manuscript was finished in haste.

## 🤔 Skeptic's Cross-Examination

Strip away the Kerr promise and what remains is a re-derivation of two flux modes that were published five years ago, using first-order data and effective sources imported from the very calculation it is being checked against, agreeing to only a few parts in ten thousand for the dominant mode with the discrepancy unexplained. Every ingredient advertised as new (hyperboloidal compactification, Bondi-Sachs, spectral collocation, second-order Teukolsky numerics) has appeared in the same group's ringdown papers or in the companion Bondi-Sachs paper. And the one thing that would settle whether the strategy was right -- that the scheme actually works in Kerr -- is deferred, with the authors conceding that the source does not separate there, that the mode-mixing treatment is undecided, and that the necessary second-order Kerr puncture does not yet exist.

## 🆕 Novelty in Context

The claim to be the first second-order self-force calculation in the Teukolsky formalism holds up: an InspireHEP search for second-order Teukolsky work returns only the formalism paper (Spiers, Pound & Moxon 2023) and this one, and all published second-order self-force numbers (Pound et al. 2020, Warburton et al. 2021, Wardell et al. 2023, Mathews et al. 2026) come from direct Lorenz-gauge solutions. The claim is narrower than it first sounds, however. The same group has already solved the second-order Teukolsky equation numerically on compactified hyperboloidal slices for quadratic quasinormal modes (Bourg, Panosso Macedo, Spiers, Leather, Bonga & Pound, PRL 2025 and PRD 2025), so the solver and the null-infinity-as-grid-point technology are not new; what is new is coupling them to a point particle, a second-order puncture and effective source, and multiscale slow-evolution terms, which is genuinely the hard part. Likewise the Bondi-Sachs/infrared statement originates in the companion paper Spiers, Pound & Moxon (arXiv:2606.24816), and this paper confirms it by an independent route rather than establishing it. The physical output -- (2,1) and (2,2) second-order fluxes -- reproduces rather than extends Warburton et al. (2021). So the honest summary is: a new and better-designed route to an old answer, whose value lies entirely in where it can go next.

## 🎯 Relevance to Your Research

This is squarely in the reader's field: second-order self-force, multiscale/two-timescale expansions, and the path to post-adiabatic waveforms on a Kerr background. It is the first serious attempt to move second-order self-force off the Schwarzschild-Lorenz-gauge track that everything has so far depended on, and the design decisions here (Bondi-Sachs at first order, compactified hyperboloidal with null infinity as a grid point, integration by parts to handle the C^1 effective source) are the ones the community will either adopt or have to argue against. The infrared discussion is directly relevant to anyone worrying about memory and slowly-evolving modes in multiscale second-order calculations.

📖 **Where to start:** Section 3 (compactification, asymptotic analysis, and the transformation to Bondi-Sachs gauge) for the conceptual core; Section 6 for the integration-by-parts variation-of-parameters construction inside the worldtube, which is the practical trick worth stealing; Section 7 for the actual numbers and the honest discussion of the (2,2) discrepancy; Appendix 10 (infrared divergences in the Lorenz-gauge field equations) and its subsection 10.3 if the memory/boundary-condition issue matters to you. Appendix 12 is worth a skim for how the error budget was actually assembled.

## Scores

- 🔬 **Quality:** 8.5/10
- 🎯 **Relevance:** 9.5/10
- 🌟 **Reading priority:** Must-Read (weighted score 8.5/10)

## 🚧 Caveats

- Only the (2,1) and (2,2) modes are computed, at 27 radii between 7M and 20M; there is no total flux and no waveform.
- First-order fields and effective sources are converted from the existing Lorenz-gauge pipeline, so the agreement with Lorenz-gauge fluxes is not a fully independent check.
- The (2,2) flux differs from the Lorenz-gauge reference by 2-3e-4 relative, and the paper cannot attribute the difference to a specific source of error.
- The error bars are explicitly described as measured sensitivities, not a complete error bound or a statistical confidence interval.
- The Kerr extension, which is the stated motivation, is argued but not demonstrated; the required second-order puncture in Kerr does not yet exist.
- The infrared/Bondi-Sachs result confirms a conclusion already reached in a companion paper by overlapping authors.

## In Network

- 🚩 Benjamin Leather — extended-network collaborator
- 🚩 Andrew Spiers — extended-network collaborator
- 🚩 Adam Pound — extended-network collaborator
- 🚩 Barry Wardell — extended-network collaborator
- 🚩 Niels Warburton — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-09-15)
