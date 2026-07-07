# 🧭 Joint inference of line-of-sight acceleration and orbital eccentricity in neutron-star–black-hole binaries

**Authors:** Lorenzo Pompili, Aldo Gamboa, Alessandra Buonanno (T3)
**arXiv:** [2606.28156](https://arxiv.org/abs/2606.28156) · gr-qc, astro-ph.HE · 16 pp, 6 figures
**Submitted:** 26 Jun 2026

## Summary
Pompili, Gamboa & Buonanno implement a time-domain Doppler remap of line-of-sight acceleration (LOSA) atop SEOBNRv6EHM (eccentric, aligned-spin) and SEOBNRv5PHM (precessing, quasi-circular) inside pySEOBNR. They validate on three synthetic injections and analyse five LVK NSBH events plus four eccentric BBH candidates. The headline claim: for GW200105 the joint (Γ, e) posterior "disfavors both Γ and e being zero simultaneously at 90% credibility."

## Genuinely New?
Modest and correctly scoped. (i) Implementation-level: the time-domain remap is mathematically identical to earlier proposals (Vijaykumar, Chen, Tiwari); its advantage over mode-by-mode SPA frequency-domain implementations is computational speed. (ii) First joint (Γ, e) IMR-multipolar inference on GW200105 (Roy & Janquart used only PN inspiral pyEFPE). (iii) First LOSA constraints on GW200115, GW230518, GW230529 — but all null. The authors flag that concurrent paper arXiv:2606.25304 (Roy & Nitz) does the same time-domain remap on the full O1–O4a catalog, so priority is essentially shared.

## Strengths
- Clean formulation; single cubic-spline evaluation per polarization is genuinely efficient.
- Correctly identifies asymmetric mimicry (missing eccentricity biases LOSA more than missing precession).
- Avoids the |Γ|t_sd ≪ 1 cut of Bilby_TGR.
- Refutes an erroneous LOSA claim on GW190814 (Yang et al.).

## Weaknesses
- Injection suite is thin: three configurations, each at only two Γ values, fixed M=6.5 M☉, q=2, d_L=600 Mpc, one sky location, zero noise. No PP-plots, no mass/spin/inclination coverage, no noise realizations, no calibration systematics.
- No both-eccentric-and-precessing injection — the physically realistic case. Authors admit: "we leave this to future work."
- All real-event recoveries use SEOBNR only; no cross-waveform-family check.
- Eccentricity prior sensitivity for GW200105 acknowledged but not marginalized; a log-uniform e prior "weakens the preference for eccentricity."

## GW200105 claim — real or artifact?
Weak, not a detection. log₁₀ ℬ^{Γ≠0}_{Γ=0} ≈ −0.60 (LOSA alone is *disfavored*); prior work gives log₁₀ ℬ^{e≠0}_{e=0} ≈ 0.85. The "(0, 0) disfavored at 90%" is a 2D credible-region statement driven almost entirely by the pre-existing eccentricity hint, with no trials-factor treatment. This is a re-expression of known eccentricity marginal evidence, not new astrophysics.

## Relevance to Vojtěch
Directly on-topic for LIGO NSBH environmental effects: LOSA is exactly an environmental Doppler signature, the paper's target is NSBH, and the (Γ, e) degeneracy discussion (Secs. III.3, IV.1.1) — especially the asymmetric mimicking — is directly useful. Not EMRI-relevant. Buonanno T3 relationship makes it politically salient.

## Scores
- **Quality: 6.5/10** — competent, careful, honest, incremental; concurrent Roy & Nitz paper dilutes novelty.
- **Relevance: 7/10** — directly relevant to Vojtěch's environmental-effects axis; skim Secs. III.3 and IV.1.
- **Verdict: Worth-Skimming.** Solid LVK-methods paper, honestly hedged. GW200105 is *not* a detection of environmental acceleration — it is a 2D reframing of prior eccentricity hints.

## Collaborator flags
Alessandra Buonanno (T3).
