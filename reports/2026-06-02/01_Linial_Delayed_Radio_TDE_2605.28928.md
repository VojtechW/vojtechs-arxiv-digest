# ☄️ Delayed Radio Flares in TDEs from Star-Disk Collision Outflows

**arXiv:** [2605.28928](https://arxiv.org/abs/2605.28928)
**Authors:** Itai Linial, Brian D. Metzger, Andrei M. Beloborodov
**Categories:** astro-ph.HE
**Quality:** 7/10 — **Relevance:** Very High — **Tier:** Must-Read

## Summary

Proposes that delayed radio flares observed years after TDEs arise from a pre-existing stellar EMRI (P_orb ~ hours-days) being struck by the viscously spreading TDE disk. The same star-disk collision machinery the authors developed for QPEs is repurposed to power radio outflows, with mass ejection from both the disk surface and the orbiting star via ablation.

## Key claims

- Some delayed TDE radio flares (e.g. WTP14adeqka) require ≥0.1 M☉ ejecta — a serious problem for conventional disk-wind/jet models because the TDE disk simply does not have that mass available at late times (Fig. 1).
- A time-dependent 1D viscous diffusion model (Crank-Nicolson) with a sink term at the EMRI semi-major axis yields ejecta masses 10⁻³–1 M☉, wind velocities 0.02–0.1c, and kinetic energies up to 10⁵¹ erg, peaking on years timescales — matching the observed delayed-radio sample.
- Concrete falsifiable prediction: AT 2019qiz should rebrighten in radio years post-2024 QPE detection (F_ν ~ 7 mJy at 1 GHz if disk-cleared low-density cavity).
- Closed-form scaling inversion: observed (v_w, E_k, Δt) → P_orb, t_v, m_w (Eqs. 22–28).

## Strengths

- Genuinely well-posed inverse problem with closed-form scalings tied to a concrete numerical disk model.
- Connects two independent observational puzzles (delayed radio + QPEs) within one self-consistent framework with falsifiable source-by-source predictions.
- Mass-budget argument vs. conventional models (Fig. 1) is a real tension, not a strawman.
- Uses Yao+2025 simulation-calibrated ablation prescription rather than pure parametrization.
- Honest about regime breaks (ablation efficiency calibration range; survivability of EMRI star).

## Weaknesses

- ~5 free dimensionless efficiencies (f_ub^star, f_ub^d, k, ξ_w, η) spanning orders of magnitude. With this many knobs the "agreement" with data is a weak constraint.
- No collision hydrodynamics — explicitly punted. The asserted v_ej ≈ √2 v_k is plausible but not derived for the relevant Σ_d/H_d regime.
- η = 0.03 ablation efficiency extrapolated outside the calibration range.
- Constant-viscosity disk toy model; full Σ ∝ Σ^{2/7} structure flagged but not used.
- The ~10% QPE-TDE rate vs ~40% delayed-radio rate discrepancy is hand-waved away ("not all EMRIs make QPEs").
- Competing Wu et al. 2026 disk-state-transition model is acknowledged to fit the same data; no decisive discriminator proposed beyond the joint QPE-radio coincidence.

## Skeptic's strongest objection

With ~5 free dimensionless efficiencies and a viscous time normalized to fit, this risks being curve-fitting dressed as a physical model. The model's range can accommodate almost anything in the (M_ej, v_w) plane.

## Relevance to Vojtěch

Directly hits the EMRI/QPE/TDE/circum-SMBH-environment intersection. Eq. (3) τ_GW scaling, the Hills-mechanism EMRI supply, and EMRI survivability constraints for GSN 069 / eRO-QPE2 are squarely in scope. The AT 2019qiz prediction is concrete and testable in the near future.

## Verdict

Must-Read for the QPE-EMRI thread. The framework is incomplete but the gestalt — same star-disk collision machinery powering both QPEs and delayed radio — is a meaningful unifying picture.
