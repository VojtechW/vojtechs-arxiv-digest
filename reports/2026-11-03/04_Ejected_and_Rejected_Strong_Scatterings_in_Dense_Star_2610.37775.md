# 💫 Ejected and Rejected: Strong Scatterings in Dense Star Clusters

🔦 **Worth-Skimming** · 🔬 Quality 5/10 · 🎯 Relevance 5/10

📎 **Citation:** Adam Distler, Nicholas C. Stone, *Ejected and Rejected: Strong Scatterings in Dense Star Clusters*, arXiv:[2610.37775](https://arxiv.org/abs/2610.37775) [astro-ph.GA, astro-ph.HE], submitted 27 Oct 2026.

> 💡 A closed-form calculation of how often stars near a giant black hole receive single large velocity kicks suggests that a rare close encounter can knock a would-be extreme mass ratio inspiral back off its inspiral track, which would preferentially remove the least eccentric such sources.

## 🔍 Executive Summary

The authors derive an exact two-dimensional rate distribution of velocity kicks (along and across the direction of motion) from two-body encounters in isotropic, spherical star clusters. They give its kinematic boundary and evaluate it for a King-model globular cluster and for power-law cusps around a supermassive black hole. They approximate the marginal distributions and third moments by rescaling the exactly solvable gamma = 3/2 case by density, then convert approximately to energy and angular-momentum kicks. Two applications follow. The first recovers the ejection rates of Teboul et al. and maps regimes where the 'one strong kick per orbit' assumption breaks down. The second is an order-of-magnitude estimate that proto-inspirals just inside the gravitational-wave-dominated region typically suffer one or more 'cancelling' angular-momentum kicks before they reach the LISA band.

## 📣 Claimed Contribution

An explicit, closed-form differential rate distribution of strong velocity kicks in two-dimensional velocity space. The authors present it as equivalent in content to a transition-probability operator but more tractable, and say they know of no prior strong-scattering operator in joint energy and angular-momentum space. They also give approximate kick rates in action space; identify a saturated-strong-kick regime and a broader 'diffusively saturated' regime for ejections around low-mass black holes; and introduce 'EMRI cancellation', a new effect they argue suppresses low-eccentricity loss-cone EMRIs.

## ✅ Strengths

- Clean, general derivation: the master formula reduces the kick-rate distribution for any isotropic distribution function that depends only on energy to a one-dimensional integral. It has a simple kinematic boundary that holds independently of the field-star distribution.
- Sanity checks done: the first and second moments reproduce standard diffusion coefficients to about 1-2 percent, the density-rescaling approximation for the marginals and third moments is checked against direct integration for gamma from 1 to 2, and ejection rates match Teboul et al.
- Analytic third moments for gamma = 3/2 (and a bounded ratio between them) may be useful to people building Fokker-Planck or Langevin codes with skewed kick distributions.
- Honest about limitations: single-mass isotropic distribution, no relativistic or tidal dissipation in encounters, no integration along the inspiral track, and the admission that steady-state EMRI rates may be unchanged.
- The 'cancellation' scaling is a neat analytic result: along a line t_GW = p t_AM, the expected number of cancelling kicks is independent of semimajor axis.

## ⚠️ Weaknesses

- The headline EMRI result rests on N_CE ~ Gamma(apocentre) x t_GW evaluated at the starting point, with no integration along the Peters inspiral, no Monte Carlo and no N-body check; the authors concede a proper treatment is still needed.
- The claimed observable consequence (fewer low-eccentricity EMRIs, more high-eccentricity ones) is asserted qualitatively and never computed; the paper itself says direct or Monte Carlo simulations are needed to verify it.
- The 'cancelling' kicks are not strong in the classical b < b0 sense. At apocentre of a 1-e ~ 1e-3 orbit, the required kick is comparable to the tiny apocentric speed, a few percent of the escape speed, so this is the Rutherford tail of ordinary relaxation. Whether it adds anything beyond what diffusion already does near the separatrix is not shown.
- The cut used to separate single kicks from diffusion (J_c - J > 5 diffusion steps per orbit) is ad hoc and compares against diffusion over one orbit, not over the full inspiral time t_GW. Near the N_CE = 1 contour, which sits close to the t_GW = t_AM line, cumulative diffusion over t_GW is by construction of comparable size.
- The test object is a 10 solar-mass black hole scattered by 1 solar-mass stars, with no mass segregation, resonant relaxation or Schwarzschild-barrier physics, all of which shape the angular-momentum evolution in exactly the region considered.
- The ejection section mainly reproduces known rates; the new saturation regimes are only mapped, and the paper says outright that their net effect on loss-cone shielding could go either way.
- The approximations for general gamma come from rescaling the gamma = 3/2 result by number density; this is tested only for gamma from 1 to 2 at a single radius.

## 🤔 Skeptic's Cross-Examination

'Cancellation' is just the power-law large-kick tail of two-body relaxation acting near a separatrix that is already fuzzy under diffusion. The relevant comparison is the single-kick probability against cumulative diffusive leakage over t_GW, not against one orbit's diffusion step. Without that comparison, or a Monte Carlo run with the full kick distribution, there is no evidence that the eccentricity distribution of LISA EMRIs changes at all. The authors themselves allow that steady-state rates are unchanged.

## 🆕 Novelty in Context

The kick-distribution idea itself is old (Henon 1960s, Goodman 1983, Lin and Tremaine 1980), and the paper cites it. So does the energy-space non-Gaussian, strong-encounter treatment of Bar-Or, Kupi and Alexander 2013 (arXiv:1209.4594), which already derived a non-perturbative anomalous-diffusion description of energy relaxation, checked against N-body runs. The new piece is the closed-form bivariate velocity-space form for power-law cusps, and that is a modest reformulation rather than new physics. The ejection application explicitly reproduces Teboul, Stone and Ostriker 2023 (arXiv:2211.05858) and its follow-ups; the saturation regimes are mapped, but their effect on loss-cone shielding is left for future work. 'EMRI cancellation' does seem new as a named effect: my queries found no prior paper treating single-kick ejection of proto-EMRIs from the gravitational-wave-dominated region. However, it is the large-kick tail of ordinary two-body relaxation applied to the standard Hopman and Alexander separatrix, and the supporting calculation is a rate-times-timescale estimate. The NASA ADS tool was unavailable during this check, so the search relied on InspireHEP and arXiv abstracts and may have missed astro-ph-only work.

## 🎯 Relevance to Your Research

Moderately relevant. For an EMRI and Kerr-dynamics reader, the useful bits are the claim that strong scatterings bias loss-cone EMRIs toward high eccentricity (a population-prior question) and the remark that skewed kick distributions might help with boundary problems in Carter-constant diffusion around Kerr black holes. It is stellar dynamics rather than relativity, and the EMRI claim is an order-of-magnitude estimate. Read the Canceled EMRIs subsection and its figure, plus the Conclusion; skim the master formula in Section 2.

📖 **Where to start:** Section 3.1 (Canceled EMRIs) for the new idea and its scaling argument; Section 2, up to the master formula and the kick boundary, for the formalism; the end of Section 3.2 for the remark on discrepancies in 'cliffhanger' EMRI rates between orbit-averaged and local Monte Carlo methods.

## Scores

- 🔬 **Quality:** 5/10
- 🎯 **Relevance:** 5/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4/10)

## 🚧 Caveats

- The EMRI 'cancellation' result is a rate-times-timescale estimate at a single point, not an integration along the inspiral or a simulation.
- The suppression of low-eccentricity EMRIs is a hypothesis; no eccentricity distribution is computed.
- The kicks invoked are the large-kick tail of ordinary relaxation, and they are never compared against cumulative diffusion over the inspiral time.
- Ejection rates reproduce earlier work; the new saturation regimes are only mapped, not quantified.
- Single-mass, isotropic, Newtonian point-mass encounters; no resonant relaxation or mass segregation.

---

🔗 [Back to the weekly digest](../2026-11-03)
