# 🛡 Survival of Dark Matter Spikes around Sgr A*

**arXiv:** [2606.13761](https://arxiv.org/abs/2606.13761)
**Title:** *On the survival of dark matter spikes: Stellar and compact-object perturbations*
**Authors:** Theophanes K. Karydas, Francesca Scarcella, Bradley J. Kavanagh, Gianfranco Bertone
**Categories:** astro-ph.GA, astro-ph.HE, gr-qc, hep-ph
**Verdict:** Should-Read — Quality 8/10, Relevance 8/10

> ⚠ Disambiguation: **Bradley J. Kavanagh** (Cantabria/IFCA, dark-matter phenomenology) is NOT the same person as the Tier-2 GR collaborator Chris Kavanagh. This is not a collaborator paper.

---

## One-line summary

Using a 2D anisotropic Fokker–Planck/Monte Carlo treatment plus a HaloFeedback master-equation framework, the authors argue that the DM spike around Sgr A* survives gravitational perturbations from the nuclear star cluster, S-cluster stars (S2, S38), and ~270 past EMRIs over 10 Gyr — at r ~ 10⁻⁵ pc (the LISA-relevant region) the density is retained at ~82% of its initial value.

## Strengths

- **Clean radial partition.** The problem is broken into three regimes by perturber and the right tool deployed in each: anisotropic Fokker–Planck in (E, R) with stochastic Itô SDE realization for the NSC mean field; HaloFeedback master equation (full jump statistics, not truncated diffusion moments) for individual S-stars and past EMRIs.
- **Galactic-Center-anchored inputs.** NSC properties (ρ_* ∝ r^−1.4, tangential anisotropy β = −0.3, IMFs of Salpeter / Kroupa / Lu / single-mass) are tied to observations, making the case study testable rather than parametric.
- **Physical insight worth remembering.** The system develops a broken power law with the inner spike essentially intact, contradicting the textbook ρ ∝ r^{−3/2} isotropized Fokker–Planck steady state of Merritt — because both E and L diffusion are tracked, and the inner spike is in the regime where the mean-field NSC representation breaks down.
- **Direct engagement with Sharpe et al. (2026).** The Sharpe team claimed much stronger EMRI-driven depletion. Karydas et al. argue the error lies in treating the per-cycle ejection probability as constant (yielding ρ̇ ∝ p_ej ρ, exponential decay) rather than tracking phase-space redistribution, and support this with NbodyIMRI N-body simulations showing slower-than-exponential depletion transitioning to a power law.
- **Conservative choices throughout** (fixed S2/S38 orbits; isotropic β = 0 for NSC inner stars; ignoring stirring effects that would further weaken depletion).

## Weaknesses

- **The 18% headline depends on bookkeeping assumptions:** 270 EMRIs of 10 M⊙ each, Hopman & Alexander eccentricity distribution, no major mergers (q > 0.1). Major mergers — where the spike could be disrupted — are punted.
- **"Consecutive, non-overlapping" EMRI modeling** ignores coincident inspirals and inter-event refill (would favor survival, but still simplistic).
- **IMF sensitivity is non-trivial.** Depletion scales as ⟨m²⟩/⟨m⟩, so a more top-heavy IMF (plausible for the GC) pushes depletion higher than the Salpeter benchmark.
- **Formation-history handwaved.** The claim that ×5 adiabatic BH growth would erase any non-adiabatic history is asserted via Caiozzo et al. 2025, not demonstrated.
- **Disagreement with Sharpe et al. argued cogently but not fully resolved** at the level of independent reproduction in identical setups.
- **GC-specific.** Extrapolation to lower-mass MBHs (10⁴–10⁶ M⊙ in less star-rich environments) is not done — that would likely *strengthen* survival, but is missing.

## Relevance to Vojtěch's research

Directly relevant. This is the up-to-date answer to the central worry: *are DM-spike-induced dephasing forecasts in the EMRI literature (Eda+, Kavanagh+, Coogan+, Karydas+ 2025 series) realistic, or is the spike erased by the time LISA observes?* The answer here is robustly affirmative for the GC analog: spikes survive, so DM-dephasing constraints from LISA EMRIs are not automatically nullified by stellar/EMRI back-reaction. The explicit refutation of Sharpe et al. is the key takeaway — Sharpe's exponential-depletion result, if it had stood, would have largely invalidated environmental-dephasing forecasts.

For Vojtěch's accretion-and-environmental-effects line: this is the reference point on the prior distribution of DM density profiles at the time of EMRI observation.

## Bottom line

Read for: (i) the broken-power-law / cavity-not-erased argument; (ii) the Karydas–Sharpe head-to-head on EMRI depletion; (iii) the NbodyIMRI N-body validation; (iv) a defensible prior for any future Bayesian inference involving DM-spike parameters.
