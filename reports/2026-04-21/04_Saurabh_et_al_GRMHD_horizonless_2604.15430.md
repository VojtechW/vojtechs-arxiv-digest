# 🕳️ GRMHD accretion beyond the black hole paradigm: Light from within the shadow

**arXiv:** [2604.15430](https://arxiv.org/abs/2604.15430)
**Authors:** Saurabh, Maciek Wielgus, Parth Bambhaniya, Elisabete M. de Gouveia Dal Pino, Andrei P. Lobanov, Pankaj S. Joshi
**Categories:** astro-ph.HE, gr-qc
**Submitted:** 2026-04-16

---

## Quality Assessment

**Quality Score:** 7/10
**Relevance Score:** 7/10
**Verdict:** PASS — Should-Read

---

## Summary

This paper presents the first 3D GRMHD simulation of sustained accretion onto a JMN-1 (Joshi-Malafarina-Narayan) horizonless null singularity, achieving a magnetically arrested disk (MAD) state with accretion rates comparable to Schwarzschild BH models. Using parameters appropriate for M87*, they generate synthetic ray-traced images at 230 GHz that are broadly consistent with EHT observations. The key observational discriminant is detectable brightness inside the "observable shadow" of JMN-1 — emission from near the central singularity that would be hidden behind a BH event horizon — potentially accessible to next-generation radio interferometry.

---

## Strengths

- **Genuine novelty**: First demonstration of efficient MAD-state accretion sustained onto a null singularity, overcoming potential barriers that plague other naked singularity models.
- **Well-motivated spacetime**: JMN-1 arises from gravitational collapse with anisotropic pressure in GR (Joshi & Malafarina), not an ad-hoc metric.
- **Rigorous numerics**: High-resolution 288×128×128 grid with MRI quality factors Q ≈ (100, 20, 20), extended to t ≈ 10,000 t_g. Full polarized radiative transfer (iPole).
- **Direct EHT relevance**: Synthetic images at 230 GHz directly comparable to M87* observations.
- **Clear redshift analysis**: g ∝ r^{1.25} for JMN-1 vs g ∝ (r−r_h)^{0.5} for Schwarzschild explains the inner emission physics.

---

## Weaknesses

- **No spinning generalization**: Astrophysical BHs are spinning. A valid spinning JMN-1 metric is not yet available, severely limiting predictive power for real sources.
- **"Light from within shadow" is fragile**: Only ~few % of peak brightness, boundary-condition-dependent, and requires next-gen EHT dynamic range. Easily masked by astrophysical uncertainties.
- **Limited parameter space**: Only one JMN-1 configuration (R_b = 2.8 r_g), one source (M87*), one initial condition. No sensitivity analysis on R_high, initial torus, or other choices.
- **No convergence study**: Resolution is adequate by standard criteria but not tested with grid doubling.
- **Comparison to other horizonless models is superficial**: No direct GRMHD comparison with Reissner-Nordström or boson stars under identical setups.

---

## Critical Cross-Examination

**Is JMN-1 physically well-motivated?** Better than most exotic metrics — it arises from collapse with anisotropic pressure. However, the physical origin of the anisotropic pressure is unspecified, and the choice R_b = 2.8 r_g (null singularity regime) is fine-tuned.

**How robust is the observational discriminant?** Not very. The inner brightness feature requires high dynamic range (>100:1), is parameter-dependent, and has not been tested against other horizonless models. Current EHT cannot detect it; next-gen EHT might.

**Is the BH vs JMN-1 accretion rate difference significant?** Marginally — BH: (4.6 ± 0.9) × 10⁻⁶ Ṁ_Edd vs JMN-1: (3.0 ± 0.5) × 10⁻⁶ Ṁ_Edd. Error bars overlap at ~1σ level.

---

## Key Conclusions

1. JMN-1 null singularity can sustain MAD accretion with rates comparable to Schwarzschild BH.
2. Synthetic 230 GHz images broadly consistent with EHT M87* observations.
3. "Light from within the shadow" as potential observational discriminant — but requires next-gen EHT and is boundary-condition-dependent.
4. No spinning generalization is a major limitation for real astrophysical applications.

---

## Relevance to Your Research

This connects to your broader interest in BH accretion environments and EHT-relevant physics. While not directly about EMRIs, the accretion-flow physics around horizonless objects could have implications for environmental effects on inspirals. The GRMHD methodology is state-of-the-art and the paper explores genuinely uncharted territory.

**Recommended sections:** Introduction (motivation), Sec. II (spacetime and numerics), Sec. III (MAD properties and images), Discussion (limitations and future directions).
