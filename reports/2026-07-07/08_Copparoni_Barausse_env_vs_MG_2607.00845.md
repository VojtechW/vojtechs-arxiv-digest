# 🌐 Environmental effects vs. modified gravity in the LISA massive black hole binary population

**Authors:** Lorenzo Copparoni, Enrico Barausse
**arXiv:** [2607.00845](https://arxiv.org/abs/2607.00845) · gr-qc · 12 pp, 5 figures
**Submitted:** 1 Jul 2026

## Summary
Copparoni & Barausse forecast LISA's ability to distinguish a scalar-tensor Ġ signal from gaseous accretion + viscous migration in the MBHB population. All three effects enter at −4PN with the same frequency dependence, so they are formally degenerate at the single-event level. Using Fisher forecasts on BACH population catalogs and hierarchical nested sampling (dynesty) over environmental hyperparameters (active fraction λ, Eddington-slope α) and a Ġ hyperparameter G₁, they conclude: (i) LISA reaches σ_G1 ∼ 10⁻⁷ yr⁻¹, orders of magnitude weaker than Solar System; (ii) even extreme environmental injections (λ=0.5, super-Eddington f_max=10) remain compatible with vacuum at population level; and (iii) environmental effects will not bias LISA's MG tests with MBHBs.

## Genuinely New?
Modest. The BCP 2014 paper already argued MBHB environments are weak; Caputo, Sberna, Toubiana et al. 2020 provided the accretion −4PN formula reused here verbatim. Their own EMRI predecessor Copparoni et al. 2025 (2502.10087) did the same hierarchical trick for EMRIs. Novelty: (a) porting the population-level hierarchical inference from EMRIs to MBHBs, (b) doing it on realistic BACH catalogs with 5 seed models, (c) quantifying that Occam penalties in the (λ, α) model suppress false-environmental claims when the data are actually Ġ. Competent extension, not a conceptual advance.

## Strengths
- Formal Bayesian population setup is clean; degeneracy is properly diagnosed via Bayes factors, not just correlation coefficients.
- Cutler–Vallisneri bias analysis is a real check, cross-validated against full residuals.
- Bounded, well-scoped question with a definite falsifiable answer.

## Weaknesses
1. **Fisher-matrix + Gaussian single-event posteriors** — the hierarchical layer relies on Fisher σ's; Fisher is notoriously optimistic for low-SNR events at −4PN where prior boundaries and non-Gaussianity matter.
2. **Circular inspirals only** — they acknowledge refs [77, 78] showing eccentricity amplifies environmental dephasing substantially; this could be the whole story and is punted.
3. **No dynamical friction, no DM spikes** — accretion + migration is one channel; the "environmental effects don't bias" conclusion is only about that channel.
4. **HS catalogs carry the constraint**; LS/PopIII catalogs contribute <10 usable events, so the "population" claim is really a heavy-seed claim.
5. **10 yr mission** — nominal LISA is 4 yr; σ_G1 degrades.
6. **ξ ∈ [1, 10] migration fudge** is treated as one number rather than marginalized.
7. The MG channel is a single ppE −4PN mode; degeneracy-breaking against dipole radiation or graviton mass isn't addressed.

## Relevance to Vojtěch
Directly overlaps his turf. The −4PN accretion + migration prescription, the Salpeter-timescale linearization, and the choice to exclude eccentricity are exactly the modeling choices Vojtěch is well-placed to critique. The EMRI predecessor (Copparoni et al. 2025) is more directly in his wheelhouse than this MBHB extension, but this paper closes the LISA-source-class loop.

## Scores
- **Quality: 6.5/10** — careful hierarchical Bayes, but ultimately a Fisher forecast dressed up with a population layer. Conclusion is real but modest.
- **Relevance: 7.5/10** — environmental-vs-MG is Vojtěch's core topic; the eccentricity omission is a natural follow-up hook.
- **Verdict: Worth-Skimming.** Skim, don't deep-read. Worth citing when writing about environmental degeneracies in LISA science; not worth reading cover-to-cover.

## Collaborator flags
None direct.
