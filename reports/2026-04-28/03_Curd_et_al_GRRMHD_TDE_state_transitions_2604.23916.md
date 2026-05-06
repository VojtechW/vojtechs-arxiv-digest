# 💥 GRRMHD State Transitions in Non-Jetted Tidal Disruption Events

**arXiv:** [2604.23916](https://arxiv.org/abs/2604.23916)
**Authors:** Brandon Curd, Safira Heridia, Aviyel Ahiyya, Richard Anantua
**Categories:** astro-ph.HE
**Quality:** 7/10 | **Relevance:** 8/10

---

## Summary

The authors run general-relativistic radiation-magnetohydrodynamic (GRRMHD) simulations of magnetized tori adapted from the late, sub-Eddington phase of the Cooling Envelope Model (CEM) for a 1 M⊙ star disrupted by a 10⁷ M⊙ SMBH. The central finding is that the late-stage tori become *thermally unstable* on a timescale of tens of days (≈17–47 days, depending on primary spin a∈[0, 0.9]), undergoing a rapid spectral state transition: a soft X-ray excess builds up before collapse, then luminosity drops by roughly two orders of magnitude. The simulated late-time spectral evolution is qualitatively consistent with the X-ray behaviour observed in the well-studied non-jetted TDE AT2021ehb at ∼270 days post-disruption.

## Strengths

- **Real observable target.** The simulations are explicitly compared to AT2021ehb (Yao 2022; subsequent NICER/Swift follow-ups), so this is not yet another isolated GRMHD parameter scan: the predicted state-transition timescale and X-ray hardening connect directly to a published light curve.
- **Late-stage CEM regime is genuinely under-explored.** Most prior GRMHD TDE simulations focus on circularization, the super-Eddington peak, or the jetted (MAD) regime. The sub-Eddington late-time tori in CEM territory are the part of TDE phenomenology most directly relevant to *post-fallback* X-ray transients and to the observational link between TDEs and QPE host environments.
- **BH spin scan.** Running a∈[0, 0.9] and showing how the thermal-instability timescale scales with primary spin is a useful first cut for SMBH characterization from late-time TDE light curves.
- **Plausible physical mechanism.** Thermal instability of radiation-pressure-supported sub-Eddington disks (Shakura–Sunyaev α-disk pathology) re-emerging in a GRRMHD simulation is the right story to tell — magnetic stress alone is apparently not sufficient to stabilize the inner disk in this regime.

## Weaknesses

- **Single (M⋆, M_BH) point.** The scan is in BH spin only; stellar mass (1 M⊙) and SMBH mass (10⁷ M⊙) are fixed. The TDE population spans 10⁶–10⁸ M⊙ and the dependence on disruption parameters is not explored.
- **Initial conditions inherited from CEM.** The tori are *adapted* from the near-Eddington phase of the analytic Metzger–Yao CEM; the sensitivity of the thermal-instability timescale to those initial conditions (and to the assumed magnetic-field topology) is not stated.
- **Radiation transport approximations.** A practical GRRMHD simulation cannot include full Compton transport at production scale. The relevant question — *what level of opacity and Comptonization is included, and how robust is the predicted soft-excess shape to those choices?* — is the kind of detail one would want before taking the AT2021ehb match too seriously.
- **No wind / outflow analysis.** Late-time non-jetted TDEs almost certainly have substantial radiative winds (cf. [Martire et al. 2025](https://arxiv.org/abs/2502.09486)). The paper appears to focus on the disk thermal evolution; the mass-loss / outflow consequences of the state transition are not (from the abstract) the headline.

## Relevance to Vojtěch

Strong, on the QPE / accretion-environment-of-EMRIs side of the research portfolio. The Cooling Envelope Model is the natural backbone of the QPE-as-EMRI scenarios that connect Pasham (close collaborator) and Suková (extended-network collaborator) work — late-time, sub-Eddington TDE-relic disks are precisely the disk states through which a putative EMRI secondary would be transiting. Predictions of large-amplitude X-ray state transitions on tens-of-days timescales are therefore directly useful as background context for the QPE phenomenology Vojtěch tracks.

**Score: Relevance 8/10, Quality 7/10.**

## Verdict

**Should-Read.** Solid, observationally grounded GRRMHD work that ties a clear physical mechanism (thermal instability of late-stage sub-Eddington tori) to a real X-ray transient. Read for the thermal-instability timescale as a function of spin and for the implied QPE-host disk-state context. Caveat the radiation-transport assumptions and the single (M⋆, M_BH) point.

## Caveats / Collaborator Flags

- No direct Tier-1/Tier-2 hits among the authors.
- Curd has a strong track record in TDE GRMHD (Curd & Narayan 2019, 2023) — this lineage continues here. Anantua brings the M87/EHT-style GRMHD experience.
