# 🌀 Radiation-hydrodynamics of star–disc collisions

**Citation:** Taj Janković, Sergey Karpov, Michal Zajaček, Vladimír Karas, Marzena Śniegowska, *Radiation-hydrodynamics of star-disc collisions: From system parameters to outflows and lightcurves*, arXiv:[2607.05508](https://arxiv.org/abs/2607.05508) [astro-ph.HE, astro-ph.SR], 7 Jul 2026.

## Executive Summary
Systematic 3D radiation-hydrodynamics parameter survey of a single star–disc crossing using Phantom SPH with grey flux-limited-diffusion (κ_s = 0.34 cm² g⁻¹, 6×10⁶ particles) in a local Cartesian box. Five parameters (v⋆, Σ_d, R⋆, vertical density scale σ, local inclination i) are varied around a Linial–Metzger fiducial (M_bh=10⁶ M_⊙, P=4 h, r=95 R_g). Empirical scalings are extracted for outflow momentum, peak bolometric luminosity, and flare duration, then Monte-Carlo'd via a separable product Q = Q_f·f_v·f_Σ·f_R·f_σ·f_i to fit GSN 069. Best fit favours a ~R_⊙ star on a **retrograde** orbit hitting a **dense, vertically concentrated post-TDE disc**.

## Key Contributions
- First dedicated RHD parameter grid for the single-collision QPE scenario, giving usable scalings: L_peak ∝ v⋆², R⋆^{1.5} (forward), Σ-independent for L_peak but Δt ∝ Σ^{0.5–0.6}.
- Decomposition of asymmetry into three mechanisms: intrinsic Ė asymmetry, radiative-efficiency asymmetry from adiabatic losses in the trapped backward wake, and an oblique-collision shock-breakout spike.
- Concrete GSN 069 fit with duty cycle 0.1, ratio 1.5, Δt_forw = 1 h at L_forw = 3.1×10⁴² erg s⁻¹ — plus the prediction that the later XMM12 epoch disfavours the low-Σ branch, supporting a post-TDE disc.
- Explicit tension noted with Huang, Linial & Jiang (2025) on the sign of the L_peak(Σ) trend.

## Strengths
- Substantial parameter coverage (25+ runs) and clean scaling extraction; useful late-time L ∝ [(t−t_p)/D+1]^{−ξ} fit form.
- Good positioning against contemporaries (Linial & Metzger 2023; Vurm et al. 2025; Yao et al. 2025; Huang et al. 2025/2026; Franchini et al.; Liu et al. 2026; Tagawa & Haiman 2023) and the earlier Prague/Suková–Zajaček–**Witzany**–Karas 2021 plasmoid line.
- Retrograde-orbit conclusion is a *testable, dynamically nontrivial* prediction — retrograde EMRI capture rates should be assessed.
- Honest limitation section.

## Weaknesses
- **Grey LTE FLD** cannot reproduce the observed kT ~ 100–200 eV of GSN 069; the authors admit photon starvation + Comptonization are missing. Bolometric matches therefore rest on a spectral treatment known to be inadequate.
- **Rigid-sphere star with elastic reflection** — no ablation, no stellar response, no radiation-pressure back-reaction. For R⋆ up to 4 R_⊙ at 95 R_g this is physically implausible (Śniegowska et al. 2026 shows retrograde ablation kills massive stars).
- No disc rotation, shear, self-gravity, or coronal medium — the local-box approximation removes exactly the physics that mediates the *repeated* collision cadence and cavity refill.
- **Separable one-parameter scaling** is admitted to ignore couplings, yet is used to Monte-Carlo the 5D fit — the two "candidate regions" are as much artefacts of this ansatz as physical solutions.
- The **opposite sign of L_peak(Σ_d)** vs Huang, Linial & Jiang (2025) is a red flag; the paper attributes it to vertical profile and opacity treatment but does not resolve the disagreement.

## Relevance to Vojtěch
Directly on-thread for the QPE/EMRI programme: plug-and-play scaling laws for star-on-disc EM signatures usable in EMRI+QPE joint studies; a **retrograde** inclination prediction that is dynamically interesting for EMRI formation channels and LISA-band waveforms; extends the Suková–Zajaček–**Witzany**–Karas 2021 transit line into full RHD. Karas and Zajaček are Tier-2 Prague/Warsaw collaborators — first author Janković is Zajaček's group.

## Scores
- **Quality:** 7/10 — solid, careful simulation work, but held back by grey LTE, rigid-star assumption, and unresolved tension with Huang+2025.
- **Relevance:** 9/10 — QPE mechanism, star–disc transit, direct Prague-network extension of prior collaborations.

## Verdict
🌠 **Should-Read.** Focus on Table 2 / power-law fits and the GSN 069 fit section; cite for QPE lightcurve morphology and retrograde-EMRI implications.

## Collaborator flag
**Karas, Zajaček** — Tier 2 (Prague network); Janković is a Zajaček student. Consider reaching out re: coupling to EMRI dynamics / retrograde capture rates.
