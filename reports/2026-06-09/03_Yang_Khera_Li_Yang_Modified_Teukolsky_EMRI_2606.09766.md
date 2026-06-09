# 🌀 C. Yang, Khera, Li, H. Yang — Modified Teukolsky Formalism for EMRIs in Higher-Derivative Gravity

**arXiv:** [2606.09766](https://arxiv.org/abs/2606.09766)
**Categories:** gr-qc
**Length:** 25 pages, 5 figures
**Recommendation:** Should-Read · **Quality:** 7/10

## Summary

Yang et al. apply the Hussain–Zimmerman/Li–Yang–Wagle–Yunes modified Teukolsky formalism (MTF) to a point particle on a circular equatorial orbit around a *non-rotating* black hole in parity-preserving cubic gravity, deriving inhomogeneous Teukolsky equations for Ψ₀ and Ψ₄ and numerically computing horizon and null-infinity energy fluxes. Headline finding: a ~1–2 order-of-magnitude *enhancement* of the horizon flux relative to GR, with the infinity flux slightly reduced.

## Key Results

- First MTF application with an EMRI point-particle source in a beyond-GR theory (prior MTF–EMRI work treated scalar clouds [Li+ 2507.02045, Keijzer+ 2604.11893] and matter rings [Polcar–Witzany 2507.15720]).
- Extension of the Hawking–Hartle horizon-flux formula and the Stein–Yunes infinity-flux argument to parity-preserving cubic gravity; Isaacson tensor reduces to GR at infinity at required order.
- Numerical integration uses ingoing Eddington–Finkelstein coordinates and the Hawking–Hartle tetrad to maintain regular sources; lower incomplete Γ functions regulate divergent integrals.
- For sufficient accuracy: ℓ = 2,3 at horizon (1%), ℓ = 2–4 at infinity. Horizon flux enhancement holds across the explored radial range.

## Strengths

- The formalism is genuinely solved end-to-end on a worked example: source terms, Green's functions, regularisation, numerics, fluxes.
- Identifies a physically interesting strong-field signature (horizon-flux enhancement) — concrete, not just a re-derivation.
- Honest about the missing tidal-Love-number contribution entering at the same order.
- Builds on Lorenz-gauge metric perturbation codes (Bourg, Pound et al.) rather than reinventing.

## Weaknesses

- Spin = 0. Everything is Schwarzschild. The hard parts of MTF (Petrov non-D backgrounds, mode coupling, isospectrality breaking) are largely avoided.
- No LISA observables: no dephasing, mismatch, or SNR-based bound on the cubic coupling ζ.
- Circular equatorial only; no Carter constant, no two-timescale evolution in practice.
- Cubic gravity is a convenient EFT test-bed but is itself UV-suppressed and not strongly motivated.
- Incremental relative to Li–Yang–Wagle–Yunes (MTF derivation), Hussain–Zimmerman (sourced MTF), Li+ 2507.02045 (MTF + EMRI for scalar clouds), and LaHaye+ 2510.16102 (perturbed-Schwarzschild EMRI).

## Relevance to Vojtěch

Direct overlap. Polcar–Witzany 2507.15720 is explicitly cited in §I as one of the few MTF–EMRI antecedents. The methodology — regular tetrad, Lorenz-gauge metric reconstruction feeding MTF source terms, Green's function with incomplete-Γ regularisation — runs in parallel to and extends the matter-environment programme. The EFT/modified-gravity framing also aligns with Vojtěch's structural interests.

## Honest Assessment

Competent and useful intermediate step — clearly more than a reformulation, since it yields a concrete flux ratio and an interesting near-horizon claim. But stops short of what the title and the LISA-tests framing suggest: no Kerr, no eccentricity, no waveforms, no dephasings. Whether the order-of-magnitude horizon enhancement survives the same-order tidal-Love contribution (flagged but not computed) is the next paper. Worth reading §IV (source construction in EF/HH coordinates) and §VI.1–VI.3 (horizon-flux derivation in modified gravity and the Stein–Yunes argument extension).
