# ☁️ A Relativistic Newton's Third Law for Binaries in Environments

🌟 **Must-Read** · 🔬 Quality 7/10 · 🎯 Relevance 8/10

📎 **Citation:** Conor Dyson, Adam Pound, Daniel J. D'Orazio, Maarten van de Meent, Lorenz Zwick, *A Relativistic Newton's Third Law for Binaries in Environments*, arXiv:[2611.27442](https://arxiv.org/abs/2611.27442) [gr-qc, astro-ph.HE], submitted 20 Nov 2026.

> 💡 A first-principles derivation shows how the energy and angular momentum that a small body orbiting a black hole loses to surrounding gas or dark matter can be computed from the force it exerts on that matter, plus a correction from gravitational waves emitted jointly by the body and the matter, which earlier work either guessed at or got wrong.

## 🔍 Executive Summary

Working in the two-parameter (mass ratio times environment density) expansion around Kerr, the authors use conservation of the secondary's stress-energy and retarded/advanced Green's-function reciprocity to rewrite the environment-induced rate of change of the secondary's Killing charges (energy, axial angular momentum) as an integral of the matter stress-energy against the point-particle metric perturbation. The instantaneous form pairs the matter's past history with a time-localised advanced particle field; the orbit-averaged form splits into the retarded-field work done on the matter plus a cross-term gravitational-wave flux (matter x particle) at infinity and the horizon. They then give two usable versions: a leading-order (0PA) version for dynamical environments that can be fed directly from matter simulations, and an order mass-ratio-squared-times-density version for environments that are stationary and axisymmetric at leading order, which needs only the matter response, the vacuum point-particle perturbation, and the environment's leading metric perturbation. No mixed-order gravitational perturbation has to be solved for. The construction is also carried over to comparable-mass binaries in flat-space-at-leading-order settings in an appendix.

## 📣 Claimed Contribution

A first-principles relativistic analogue of Newton's Third Law for EMRIs and IMRIs in matter: (i) an instantaneous causal balance law using a time-localised advanced field, (ii) an orbit-averaged law showing that the work on the secondary equals minus the work on the environment up to the mixed matter-particle gravitational-wave flux, and (iii) ready-to-use forcing functions at 0PA for dynamical environments and at the subleading environmental order for stationary axisymmetric ones, which avoid computing any mixed-order metric perturbation. The authors claim this clarifies and corrects the ad hoc balance prescriptions in the literature (asymptotic matter fluxes, resonance work, or integrated torque on the matter), and that recent torque-based works used an acausal form that misses a radiative matter-torque term.

## ✅ Strengths

- Addresses a real and widely acknowledged gap: EMRI-environment papers have been closing the loop with assumed balance laws, and this gives a derivation from conservation of the secondary's stress-energy.
- Practical payoff is clear: the forcing functions need only the matter perturbation, the vacuum Kerr point-particle perturbation (available from public self-force codes), and the leading environment metric perturbation. No mixed-order metric perturbation solve is needed.
- Makes the physical point explicit that asymptotic matter fluxes are not equal to the local work on the secondary when the environment can store or dissipate energy (viscosity, cooling, bound states).
- Careful about which momentum is evolved beyond leading order (effective-metric versus particle-in-environment charges) and how the choice moves terms into frequency corrections. This is the kind of subtlety that later causes sign and bookkeeping errors in waveform models.
- Author team includes core second-order self-force developers, and the multiscale (fast-to-evolve) formulation is consistent with how existing EMRI waveform pipelines are built.

## ⚠️ Weaknesses

- Purely formal: as far as I could read, there is no worked example, no numerical evaluation, and no check against an existing calculation (e.g. a boson cloud or thin-disc spiral-arm result). Nothing shows how large the newly identified radiative matter-torque term is, so the practical significance of the 'correction' is unquantified.
- Covers only energy and axial angular momentum (Killing vectors). The Carter constant is not handled, so generic inclined orbits are not fully covered, as the authors admit.
- The subleading-order result assumes the matter perturbation is bounded at the particle. That excludes accretion onto the secondary, Bondi-Hoyle-type wakes and other singular near-zone matter responses, which are exactly where dynamical friction gets its Coulomb logarithm.
- The instantaneous law relies on an advanced field sourced by a non-conserved, time-localised stress-energy. The authors only 'expect' it can be computed as a vacuum solution of the relaxed equations with jump data, so the claimed practical value of the instantaneous form is untested.
- The 1PA label refers only to the order mass-ratio-squared-times-density environmental terms in the energy and angular-momentum fluxes, not a full 1PA environmental model (no Carter constant, no handling of environments without stationarity and axisymmetry at leading order, and resonance treatment only sketched for dynamical environments).
- Some rhetorical inflation ('provocative form', 'clarify the current state of the field') for what is a clean but unvalidated derivation.

## 🤔 Skeptic's Cross-Examination

This is the standard radiative/time-symmetric Green's-function flux-balance argument from self-force theory, applied to a cross-term. The headline 'correction' to earlier torque calculations comes with no estimate of its size. Until someone evaluates the radiative matter-torque term and the mixed gravitational-wave flux for a real disc or cloud, and checks them against a direct local-force calculation, you cannot tell whether earlier results change at the percent level or not at all. The key regularity assumption also quietly excludes the strongly nonlinear near-zone matter response that matters most for dynamical friction.

## 🆕 Novelty in Context

The mathematical machinery is not new: splitting retarded fields into radiative and time-symmetric parts and using Green's-function reciprocity to turn local self-force integrals into asymptotic fluxes goes back to Gal'tsov (1982), Mino and Quinn-Wald style flux-balance arguments, all cited here. What is new is applying it to the cross-term between a point particle and a generic matter stress-energy. Within the fast-growing EMRI-in-environments literature the positioning holds up. The torque-balance papers it corrects are Dyson and D'Orazio (arXiv:2601.19123), which explicitly left the link between disc torques and the force on the EMRI as an open problem, and Dittmann, Hegade and Fairbairn (arXiv:2608.17003), which derived the angular-momentum transfer from a disc Lagrangian. The flux-based papers (e.g. Keijzer et al. 2604.11893, Rahman et al., Li et al.) assume balance between asymptotic fluxes and orbital loss rather than deriving it. A parallel route, computing the environmental force directly as a self-force, has only just started (Datta, arXiv:2608.24800, flat space only). The claim to be first to derive this rigorously is plausible. 'Corrects' should be read as 'derives and adds a radiative correction term'. The paper shows no numbers on how large that term is for any realistic disc, so whether earlier torque results are quantitatively wrong is still open. Part of the 'correction' is to the lead author's own earlier paper.

## 🎯 Relevance to Your Research

Directly relevant to anyone building EMRI or IMRI evolutions in accretion discs, dark-matter spikes or boson clouds within self-force and black-hole perturbation theory. It tells you which integrals to compute in place of asymptotic matter fluxes, and that the mixed gravitational-wave flux must be included. It also bears on the multiscale/1PA bookkeeping of environmental terms and on comparable-mass binaries in gas through the post-Minkowskian appendix. Read it if you compute or use environmental forcing terms. If you only consume vacuum EMRI waveforms, it is optional.

📖 **Where to start:** Sec. 2.2 (summary of results, with the key equations in one place); Sec. 4.2 (orbit-averaged Third Law and the mixed-flux identification); Sec. 5.3.1-5.3.3 (bootstrapping to the stationary-axisymmetric subleading order, and the discussion of which earlier prescriptions are wrong and why). Sec. 4.1 only if you care about the instantaneous, causal form; Appendix on post-Minkowskian binaries if you work on gas-embedded massive black hole binaries.

## Scores

- 🔬 **Quality:** 7/10
- 🎯 **Relevance:** 8/10
- 🌟 **Reading priority:** Must-Read (weighted score 7.3/10)

## 🚧 Caveats

- Formal derivation only; no numerical example and no estimate of how big the new correction terms are.
- Energy and axial angular momentum only; Carter constant not covered, so inclined orbits are incomplete.
- Subleading-order result assumes the matter perturbation stays finite at the small body, which excludes accretion and singular wakes.
- The 'corrected' torque prescription includes the lead author's own earlier paper.

## In Network

- 🚩 Adam Pound — extended-network collaborator
- 🚩 Maarten van de Meent — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-11-24)
