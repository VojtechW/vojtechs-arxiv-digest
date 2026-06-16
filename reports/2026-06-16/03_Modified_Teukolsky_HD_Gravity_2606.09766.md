# 🪛 Modified Teukolsky Formalism for EMRIs in Higher-Derivative Gravity

**arXiv:** [2606.09766](https://arxiv.org/abs/2606.09766)
**Title:** *Modified Teukolsky Formalism for Extreme Mass-Ratio Inspirals in Higher-Derivative Gravity*
**Authors:** Chaoyi Yang, Neev Khera, Dongjun Li, Huan Yang (T3)
**Categories:** gr-qc
**Verdict:** Should-Read — Quality 7/10, Relevance 8/10

---

## One-line summary

First application of the modified Teukolsky formalism (MTF) of Li–Yagi–Yunes / Hussain–Zimmerman / Li to a point-particle EMRI source: horizon and null-infinity gravitational-wave fluxes are computed for circular equatorial orbits around a non-rotating black hole in parity-preserving cubic gravity.

## Strengths

- **Genuine new computation, not just formalism.** Numerical horizon and null-infinity fluxes (Fig. 1) for a circular equatorial EMRI in cubic gravity, l = 2, 3, 4 modes, with quoted ~1% accuracy. A supplementary Mathematica notebook is included.
- **Honest about scope.** Explicit O(ζ η) expansion, Schwarzschild + cubic correction H₁(r), H₃(r) of Cano et al.; non-rotating restriction clearly stated.
- **Coordinate/tetrad care.** Ingoing Eddington–Finkelstein coordinates + Hawking–Hartle tetrad to keep sources regular; regular metric-amplitude combinations constructed near horizon — non-trivial technical work.
- **Modified horizon-flux derivation.** Section VI extends Hawking–Hartle horizon-area-growth to cubic gravity, deriving how the Ψ₀ ↔ dE_H/dt relation picks up an effective stress-energy tensor (Eq. 67) and confirming the Isaacson tensor reduces to GR's at infinity (Eq. 72). Real side calculations, not plug-and-chug.
- **Striking physical result.** Cubic-gravity correction enhances the horizon flux by 1–2 orders of magnitude relative to GR (after factoring out ζ), while slightly reducing the infinity flux — concrete, testable, with a clear mechanism (background-geometry correction dominates near horizon).

## Weaknesses

- **Decoupling question dodged.** Non-rotating BHs in parity-preserving cubic gravity are Petrov type D (Ψ_{0,1,3,4}^{(1,0)} = 0 — verified in App. A). The formalism is not actually tested on the algebraically-general case here; that's the easy corner. Rotating extension is deferred to future work.
- **Repackaging concern is partly valid.** Sections IV.1 and the H₀, E₁, E₂ operator structure are essentially Li–Yagi–Yunes / Hussain–Zimmerman / Li 2023 verbatim. Novelty is the EMRI source coupling S_geo^{(1,1)} ∝ Ψ_0^{(1,0)} · h^{(0,1)} and the explicit cubic-gravity NP machinery — incremental but real.
- **No dephasing prediction.** Stops at fluxes; does not integrate to give an observable LISA phase. Flagged as future work but is the obvious next step.
- **One theory, one orbit family.** Circular equatorial + Schwarzschild + parity-preserving cubic only. No eccentric/inclined, no Kerr, no EsGB, no dCS.
- **GR side uses Lorenz-gauge Schwarzschild perturbation (Barack–Lousto / Akcay).** Works for non-rotating but the "naturally extends to Kerr" claim hinges on metric-reconstruction tools that are not actually exercised.
- **Missing tidal Love number contribution** to the secondary's response — acknowledged to enter at the same O(ζ η) and to be needed for a real waveform.

## Relevance to Vojtěch's research

Direct overlap. EMRIs, Teukolsky equation, beyond-GR — squarely in scope. The horizon-flux enhancement result is exactly the kind of physics-extractable consequence relevant for LISA tests-of-gravity. The MTF + point-particle source machinery is the right tool for self-force in modified gravity. The Eddington–Finkelstein / Hawking–Hartle regularization tricks are practically useful know-how. The non-rotating restriction limits direct contact with Carter-constant / spinning-particle work.

## Bottom line

Not a paradigm-shift, but the first concrete MTF-EMRI flux calculation, with a striking order-of-magnitude near-horizon result and a clear roadmap to Kerr. Read Sec. IV (formalism) and Sec. VI (fluxes + Fig. 1) closely; skim the source-term appendices unless reproducing.
