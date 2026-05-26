# 🌀 Spin-Hair Induced Chaos of Spinning Test Particles in Rotating Hairy Black Holes

**arxiv:** [2605.19673](https://arxiv.org/abs/2605.19673)
**Authors:** Surojit Dalui, Xian-Hui Ge
**Categories:** gr-qc, hep-th, nlin.CD

## TL;DR
MPD + Tulczyjew SSC integrated on a rotating "hairy" black hole from Ovalle's gravitational decoupling (GD) construction. Authors do ZAMO-projected finite-time Lyapunov scans over (r_p, ι) and (S, β), report non-monotonic "hot spots" at S ≃ 0.65–0.85 with β ≃ 0.2–0.7 and 1.2–1.5. Methodology is competent but entirely standard; the physics novelty rests on a background that is a contrived effective metric, and the "chaos hot spots" are a finite-time bookkeeping result that does not establish chaos in the dynamical-systems sense (no Poincaré sections, no SALI/FLI/MEGNO, no rescaled Jacobian — explicitly admitted as a limitation).

## Summary
The deformed mass function m̃(r) = M − α(r/2)exp[−r/(M−β/2)] (eqs. 6–7) is grafted onto a Kerr-like Boyer–Lindquist metric via the Contreras–Ovalle–Casadio 2021 axisymmetric GD construction. The authors integrate the full MPD spin-one-form system with Tulczyjew SSC by RK4 at Δτ = 0.05M up to τ_max = 10⁵M, ε₀ = 3×10⁻⁷, projecting deviation vectors onto the ZAMO frame. They distinguish "requested" vs "empirical" orbital parameters, find the weak-spin/geodesic family clusters together, large-S (0.5–1.0) trajectories show stronger finite-time growth, and the (S, β) heatmap has two localized enhancement islands. They explicitly note S = 0.9, 1.0 lies outside the pole-dipole validity range and is used as a "dynamical probe."

## Strengths
- 🧩 Honest about limitations: explicitly says S ≳ μ/M is outside pole-dipole validity, calls Q_seed only an inclination label (not a true Carter constant), distinguishes pre-saturation regime, and recommends Poincaré/SALI/FLI/MEGNO as needed follow-up.
- The requested-vs-empirical distinction is a sensible methodological point already made in Hartl 2003a, properly cited.
- Cites all the right people: Suzuki–Maeda, Hartl, Han, Lukes-Gerakopoulos–Seyrich, Zelenka–LG–Witzany–Kopáček, Witzany 2019, Witzany–Steinhoff–LG 2019, Piovano–Pantelidou–Mac Uilliam–Witzany 2025, Albertini–Skoupý–LG–Nagar 2025.
- ZAMO projection of the deviation norm is a reasonable choice for coordinate-artifact suppression.

## Weaknesses / Skeptic's Attack
- 🪛 **Background is not physically motivated.** The Ovalle GD "hairy" metric is an effective ansatz — the authors themselves write "we do not commit to a unique microscopic origin." The exponential mass deformation has no derived microphysical source. This is precisely the "contrived metric" category Vojtěch hard-excludes.
- 🎢 **No actual chaos diagnostic.** Finite-time Lyapunov from an unrescaled deviation vector with pre-saturation least-squares fit is a weak indicator — they admit it cannot distinguish bursts from true exponential separation, and they did NOT run Poincaré sections, SALI, FLI, MEGNO, or rotation-number diagnostics. The Zelenka–LG–Witzany–Kopáček 2020 paper they cite specifically used those tools to establish the resonance/chaos picture; this paper does not.
- The "hot spots" at S ∈ [0.65, 0.85] are entirely in the non-perturbative regime where pole-dipole MPD with Tulczyjew SSC is known to have spurious behavior (Costa–Natário, helical solutions, etc., not cited). The astrophysical relevance is null and the authors essentially concede this.
- No symplectic integrator. RK4 with Δτ = 0.05M for τ = 10⁵M with ε_tol ∼ 10⁻⁶ leaves serious doubt about whether the "non-monotonic structure" in (S, β) is dynamical or numerical drift — especially since some "hot" trajectories are exactly those that terminate via constraint violation.
- The two enhancement islands lack any analytical or perturbative explanation. No identification with resonant orbits, no comparison to known KAM-breaking mechanisms, no rotation curves. "Cooperative spin–hair effect" is a description, not a mechanism.
- No comparison with Kerr + scalar-hair (Herdeiro–Radu), where chaos in spinning-particle MPD has been studied for a physically motivated background.
- The Yuan et al. 2026 (2604.20533) reference they cite for "astrophysically realistic spins triggering chaos" is in Schwarzschild — they make no attempt to reproduce or extend that result, which would have been the genuinely interesting comparison.

## Relevance to Vojtěch's Research
Method-wise (MPD + Tulczyjew + Lyapunov) this is squarely in Vojtěch's wheelhouse — and it shows. The paper cites Witzany 2019, Witzany–Steinhoff–LG 2019, Lukes-Gerakopoulos–Seyrich, Zelenka et al., and Piovano–Pantelidou–Mac Uilliam–Witzany. But the application is to a metric Vojtěch has no reason to care about (effective GD ansatz, no astrophysical or fundamental-theory motivation), the chaos diagnostics are coarser than what Zelenka–Witzany already deployed in 2020, and there is no new structural insight (no integrability/non-integrability claim, no resonance identification, no canonical action-angle treatment). Vojtěch's HARD EXCLUSION criterion "QNM/greybody/shadow on exotic backgrounds unless physically motivated AND structurally interesting" applies by direct analogy here — chaos diagnostics on an exotic background, neither motivation nor structural insight.

## Quality Score
4 / 10

## Relevance Score
3 / 10

## Verdict
FAIL
