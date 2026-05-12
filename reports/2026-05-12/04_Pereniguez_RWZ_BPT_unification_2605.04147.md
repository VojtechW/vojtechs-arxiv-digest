# 〰️ Unifying the Regge-Wheeler-Zerilli and Bardeen-Press-Teukolsky formalisms on spherical backgrounds

**Authors:** David Pereñíguez
**arXiv:** [2605.04147](https://arxiv.org/abs/2605.04147) [gr-qc, hep-th]
**Date:** 5 May 2026
**Categories:** gr-qc, hep-th

---

## Summary

Pereñíguez derives a formulation of perturbation theory on spherically symmetric backgrounds in which the Regge-Wheeler-Zerilli (RWZ) metric-perturbation equations and the Bardeen-Press-Teukolsky (BPT) curvature-perturbation equations arise as different *projections of a single tensorial curvature equation*, written in terms of self-dual curvature variables and expanded in spherical harmonics. Both formalisms have been used in parallel since the 1970s with each having its own advantages: RWZ exposes the metric directly and makes parity and isospectrality structure visible; BPT/Teukolsky decouples cleanly and is the standard tool for radiation extraction. The unification proposed here keeps both advantages by exposing them as different components of one master equation.

Concrete payoffs reported: (i) quasi-normal-mode isospectrality between axial and polar parity sectors is made *manifest* (no longer requiring the case-by-case algebraic identities of the RWZ–Zerilli construction); (ii) the metric can be reconstructed *algebraically* from any of the proposed master functions and their derivatives, at least in the frequency domain — possible time-domain obstructions are flagged; (iii) the formulation is presented for a general energy-momentum source before specialising to vacuum GR + matter. An xAct-based Mathematica notebook implementing the formalism is released with the paper.

## Strengths

- **Genuine structural insight.** Isospectrality of RWZ axial and polar modes is a phenomenon that has been understood, but not derived from manifestly invariant structure — the standard route is via Chandrasekhar-style transformations. Making it manifest via self-dual variables is the kind of structural cleanup that pays off downstream.
- **Algebraic metric reconstruction.** Algebraic reconstruction in the frequency domain is the right structural counterpart of the CCK / Wald / Aksteiner-Andersson reconstruction story on Kerr. Spherical is the natural starting point.
- **Released computational tool.** An xAct notebook lets the community check the construction directly. Reproducibility is a meaningful signal of seriousness.
- **Right framing.** Self-dual variables and spherical harmonics together are the natural setting for separating perturbations on a spherical background; the paper does not invent new technology, it deploys existing technology in the right combination.

## Weaknesses

- **Spherical only.** The big prize is, of course, Kerr: a Teukolsky-RWZ unification on Kerr would be genuinely important since Kerr-RWZ-style metric equations remain notoriously absent and reconstruction is still an active area. The spherical case is structurally well-understood; the value of this paper depends on how naturally the construction will lift to Kerr (or to algebraically special Petrov-D more generally). The abstract does not commit to this.
- **Astrophysical relevance is indirect.** Pure spherical perturbations are no longer a frontier in their own right; the practical use is downstream — in EMRI self-force formalisms, in scalar-cloud calculations, in EFT matching.
- **No new physical computation.** The paper is structural; it does not produce, e.g., a new QNM spectrum or a new self-force coefficient. The payoff is framework-level, which can be undervalued if the formalism is not adopted.
- **Time-domain obstructions are mentioned but not solved.** The frequency-domain algebraic reconstruction is clean, but for many applications (time-domain self-force, mode evolution) one needs the time-domain story.

## Relevance to Vojtěch

**Moderate-high (7/10).** Direct relevance via BHPT structure: Vojtěch works on Teukolsky-equation flux computation and self-force, where reconstruction and isospectrality structure are foundational. A unified formalism that exposes isospectrality manifestly is the kind of thing that may eventually fold into the post-adiabatic self-force toolkit. The Kerr extension, if and when it arrives, would push relevance to 9. For now, an Axis-2 structural paper worth following.

## Quality / Verdict

- **Quality:** 8/10
- **Relevance:** 7/10
- **Survives critical review:** **Yes.** Structurally clean unification with concrete payoffs (manifest isospectrality, algebraic reconstruction) and a released tool.

A skeptic notes: structural-unification papers are valuable only if their downstream applications are realised; the paper does not perform any of those applications itself, and the spherical setting is conceptually well-understood. If the Kerr extension turns out to be hard, this paper risks becoming a curiosity. A defender notes: structural insight is what produces the next generation of computational tools, and exposing isospectrality manifestly is a real piece of mathematical clarity that prior literature had not achieved.
