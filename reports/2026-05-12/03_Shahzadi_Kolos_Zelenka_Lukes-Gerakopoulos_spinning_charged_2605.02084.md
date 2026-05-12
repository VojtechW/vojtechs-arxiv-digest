# 🌀 Spinning charged test particle dynamics around Schwarzschild + uniform magnetic field

**Authors:** Misbah Shahzadi, Martin Kološ, **Ondřej Zelenka**, **Georgios Lukes-Gerakopoulos**
**arXiv:** [2605.02084](https://arxiv.org/abs/2605.02084) [gr-qc, astro-ph.HE]
**Date:** 3 May 2026
**Categories:** gr-qc, astro-ph.HE

🧭 *Collaborator paper.* Lukes-Gerakopoulos is Tier 1; Zelenka is Tier 2.

---

## Summary

Shahzadi, Kološ, Zelenka & Lukes-Gerakopoulos study the dynamics of a *spinning charged* test particle in the Schwarzschild background immersed in a Wald-type uniform external magnetic field — a system that couples three previously studied subsystems: (a) geodesics, (b) non-spinning charged motion in Schwarzschild + B (Kološ–Stuchlík–Tursunov line), (c) spinning neutral particles via the Mathisson–Papapetrou–Dixon (MPD) equations (Lukes-Gerakopoulos line).

In the equatorial plane with spin orthogonal to the orbital plane the system admits enough symmetry to integrate analytically: conserved energy E and angular momentum L_z, plus closed-form expressions for the radial Ω_r and azimuthal Ω_φ frequencies as functions of the spin parameter s and the magnetic parameter B. The effective potential is constructed and the allowed motion regions delineated.

Off-equatorial motion has three effective degrees of freedom and is non-integrable. The authors deploy *four-dimensional Poincaré surfaces of section* augmented with *recurrence quantification analysis* (RQA / recurrence plots) — the standard upgrade when 2D Poincaré sections are insufficient — and identify parameter regions exhibiting chaotic motion. They compare against the spinning-neutral and non-spinning-charged limiting cases to isolate the contributions of spin-curvature coupling vs. Lorentz force to the onset of chaos.

## Strengths

- **Methodology is the right one.** 4D PSS + recurrence analysis is exactly the toolkit developed by the Zelenka–Lukes-Gerakopoulos–Witzany–Kopáček 2020 paper (1911.00414) for 3-DOF systems, and is essential here because the standard 2D Poincaré reduction available in the limiting cases fails for the full system.
- **Genuine synthesis of two lines.** The Kološ–Stuchlík–Tursunov magnetised-charged-particle program and the Lukes-Gerakopoulos spinning-particle program have run more-or-less in parallel for a decade; bringing both ingredients together in a single MPD + Lorentz framework is a real technical step.
- **Analytical backbone before numerics.** The equatorial closed-form frequencies and effective potential are exactly the sanity-check infrastructure one wants before throwing PSS at the off-equatorial regime, and they have downstream value for any future resonance / waveform application.
- **Honest scope.** The paper acknowledges that the off-equatorial 3-DOF system "can be reduced only up to" 3 DOF and uses 4D PSS rather than overclaiming integrability or under-resolving chaos.

## Weaknesses

- **Background is Schwarzschild + Wald, not Kerr.** The most interesting astrophysical setting — magnetised accretion onto rotating MBHs (Sgr A*, M87*) — is Kerr + a more realistic disc magnetic field. The Schwarzschild restriction is methodologically clean but a step away from real targets.
- **Wald uniform field is schematic.** Real plasma magnetic fields near accreting BHs are turbulent, structured, and dynamically self-consistent (GRMHD). The Wald field is a useful tractable limit but the chaos diagnostics inherit its idealisation.
- **MPD truncation and SSC.** The abstract does not flag which spin supplementary condition is used (Tulczyjew? Mathisson-Pirani?), and the recurrence-based chaos diagnostics can in principle depend on this choice. This is a perennial concern in the MPD literature.
- **No observable connection.** The paper does not propagate the dynamics to a GW or radiative observable (resonance imprint on phasing, X-ray QPO, etc.), so the consequences of the chaos remain in the abstract dynamical-systems layer. Vojtěch may find this exactly the right place to push next.
- **Incremental, not transformational.** The setup is the natural next step after a decade of papers from the same circle of authors. The conceptual novelty over Stuchlík–Kološ–Tursunov and Zelenka–Lukes-Gerakopoulos is the *combination*; nothing structurally surprising emerges.

## Relevance to Vojtěch

**High (8/10).** Directly inside Vojtěch's spinning-particle / integrability / orbital-resonance program, and from his Tier 1+2 collaborators. The methodology (4D PSS, recurrence analysis) is one he has co-developed. Even though the background is Schwarzschild + Wald rather than Kerr, the chaos structure and resonance behaviour are likely to inform the Kerr+disc-environment generalisation that is the natural next paper.

## Quality / Verdict

- **Quality:** 6.5/10
- **Relevance:** 8/10
- **Survives critical review:** **Yes.** Solid careful work by close collaborators; conceptually incremental but methodologically the right step.

A skeptic notes: this is a "combine two known frameworks and run PSS" paper; the qualitative finding (chaos in non-integrable 3-DOF system) was almost guaranteed in advance, and the practical impact depends on whether the analytical equatorial frequencies feed downstream into resonance / phasing models. A defender notes: integrability boundaries in 3-DOF spinning-charged systems were not previously mapped out; the analytical frequencies have intrinsic value; and the work positions the group to attack the Kerr + B + spin extension that is the actually astrophysically interesting problem.
