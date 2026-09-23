# ♻️ A Fully Analytic Expression for the 2PN N-Body Hamiltonian

🌠 **Should-Read** · 🔬 Quality 7/10 · 🎯 Relevance 5.5/10

📎 **Citation:** Felix M. Heinze, Gerhard Schäfer, Bernd Brügmann, *A Fully Analytic Expression for the 2PN N-Body Hamiltonian*, arXiv:[2609.17510](https://arxiv.org/abs/2609.17510) [gr-qc], submitted 15 Sep 2026.

> 💡 The last integral that nobody had been able to evaluate in the second-order relativistic correction to the motion of many gravitating bodies has now been solved in closed form, so the corresponding energy function can be written down explicitly for any number of point masses.

## 🔍 Executive Summary

At second post-Newtonian order the N-body ADM Hamiltonian contains a four-body piece of the transverse-traceless static potential that, since Ohta et al. in 1974, had resisted explicit evaluation; the authors' own earlier work had reduced it to a single unevaluated spatial integral I^ln_{ab;cd}. This paper evaluates that integral analytically, obtaining a compact expression in the six inter-particle distances plus one transcendental piece proportional to the tetrahedron volume times an arctangent of a shape angle. Inserting it gives a fully explicit, quadrature-free conservative 2PN Hamiltonian for an arbitrary number of nonspinning point masses, which the authors also write out in full. The result is validated against direct numerical evaluation of the original three-dimensional integral and of a reduced two-dimensional parameter integral for 1000 random four-particle configurations (generic, hierarchical, coplanar, collinear), with mean relative deviations of order 1e-28 to 1e-26 in quadruple precision. A long-propagated index error in one three-body kinetic term of the published 2PN Hamiltonian is also corrected.

## 📣 Claimed Contribution

Analytic evaluation of the last remaining unevaluated integral in the general N-body 2PN ADM Hamiltonian, thereby completing the four-point correlation function of the transverse-traceless static potential and yielding, for the first time, a fully closed-form conservative 2PN Hamiltonian for arbitrarily many nonspinning point particles; plus correction of an index error present in several prior references.

## ✅ Strengths

- The claim is sharp, falsifiable and actually delivered: a single explicit formula for I^ln_{ab;cd} that closes a gap open since Ohta et al. (1974) and explicitly flagged as open by Chu (2009) and by the authors' own 2026 PRD.
- The final expression is remarkably compact and geometrically transparent: everything reduces to the six inter-particle distances, a positive cubic invariant D, the tetrahedron volume Delta, and a single scale-invariant angle Phi = arctan(Delta/D). The only non-rational structure surviving in the whole 2PN Hamiltonian is Delta*Phi.
- Numerical validation is unusually careful for a formula paper: quadruple precision, Gauss-Legendre with automatic order refinement up to order 292, compensated summation, 100-digit spot checks, 1000 configurations split across generic, hierarchical, coplanar and collinear classes, and two independent integral representations (3D Cuhre and the 2D parameter integral).
- The paper is short, well organised and does not pad; the full 2PN Hamiltonian is printed so it can be used directly, and data availability is stated.
- Honest correction of an index error (m_a m_c -> m_b m_c) that has propagated through Lousto-Nakano 2008, Galaviz-Brügmann 2011, Bonetti 2016 and the authors' own earlier paper, with the provenance traced back to the correct original expressions.

## ⚠️ Weaknesses

- The derivation is described only in prose (Feynman parametrisation, integration by parts in parameter space, a divergence identity, differentiation with respect to the squared perpendicular separation H^2, matching of integration constants as H -> infinity). No intermediate expressions are given, so a reader cannot reproduce or audit the derivation from the paper; the only public evidence of correctness is numerical agreement.
- All validation stays inside the same group's ADM pipeline: the closed form is checked against the integral representation of Eq. (UTT4) that the same authors derived. There is no cross-check against an independent formalism -- e.g. Chu's field-theory Lagrangian or the contemporaneous harmonic-gauge N-body equations of Huang, Yang and Ni (2608.20193) -- via a gauge-invariant quantity for a four-body configuration. An error upstream in U^TT_(4) would not be caught.
- The scientific step relative to the authors' own Phys. Rev. D 113, 104066 (2602.06961) is modest: that paper already made the complete 2PN N-body dynamics computationally accessible by evaluating the same integral numerically. What is gained here is speed, differentiability and aesthetics, not new dynamics -- and no timing benchmark, no equations-of-motion application and no physical result quantifies that gain.
- The paper never quantifies when the four-body 2PN cross terms actually matter. The importance of PN cross terms is asserted by citing Will (2014), which concerns hierarchical triples and a dominant central mass, not the four-point TT potential evaluated here. No estimate of the magnitude of this term in, say, a dense cluster or a hierarchical quadruple is offered.
- The authors note that roundoff in evaluating the analytic expression itself contributes significantly to the residuals, but there is no analysis of catastrophic cancellation in the astrophysically interesting near-degenerate regimes (tight binary embedded in a wider system, nearly coincident particles), where the formula has denominators like r_ad r_bc and the combination D +/- corrections. Whether the closed form is numerically better conditioned than the quadrature it replaces is not established.
- The derivation was obtained with 'substantive assistance' from a large language model. The authors state that they supplied the mathematical input, verified the derivation independently, and treat the numerical check as the fully independent validation -- which is the right mitigation -- but combined with the absence of a printed derivation it leaves the human-auditable chain thinner than one would want for a result intended to be quoted and reused.

## 🤔 Skeptic's Cross-Examination

The closed form is checked only against the same authors' own integral representation, numerically, with a derivation that is not shown. Given that this very lineage of expressions has carried an undetected index error through four papers over eighteen years -- which this paper itself corrects -- a single-group, single-formalism numerical consistency check is the weakest link. An independent cross-gauge verification, or a printed derivation, would be worth more than another three digits of quadrature agreement.

## 🆕 Novelty in Context

The self-positioning holds up on the narrow claim. Ohta et al. (1974) obtained formal 2PN N-body expressions obstructed by unevaluated spatial integrals; Schäfer (1987) did the three-body TT static potential; Chu (Phys. Rev. D 79, 044031, 2009) obtained the N-body 2PN effective Lagrangian from perturbative field theory but explicitly left the four-body interaction as unevaluated integrals; the authors' own N-body 2PN Hamiltonian paper (2602.06961, Phys. Rev. D 113, 104066, 2026) reduced the obstruction to the single integral I^ln_{ab;cd} and evaluated it numerically; and Huang, Yang and Ni (2608.20193, August 2026) gave a harmonic-gauge computable formulation that likewise splits off a regularised, numerically evaluated non-closed-form piece. So the closed-form evaluation of this specific integral does appear to be new, and 'fully analytic' is the right label. What deserves qualification is the implied scale of the advance: the 2PN N-body dynamics was already computable, in two independent gauges, before this paper. The contribution is the removal of the last quadrature -- a real and satisfying completion of a fifty-year-old loose end, but a step in tractability and elegance rather than in physical content. The paper's own text is reasonably careful about this ('a fully explicit closed-form expression remained unavailable'), so the inflation is mild and mostly in the framing.

## 🎯 Relevance to Your Research

Relevant if you care about relativistic dynamics of few- and many-body systems near a massive black hole, or about Hamiltonian formulations of PN dynamics generally: this is the ingredient one needs to put consistent 2PN cross-body interactions into cluster or hierarchical-multiple integrators without per-step numerical quadrature, and the explicit Hamiltonian makes canonical/secular analysis and symplectic integration straightforward. It is not self-force, EMRI or waveform work, and it contains no dynamics or astrophysics. Read Sec. II for the closed form of I^ln_{ab;cd} and the printed 2PN Hamiltonian (Eq. 2PN_hamiltonian), including the index-error correction at the end of the section; Sec. III for how the validation was done; Sec. IV for what remains open at 3PN.

📖 **Where to start:** Sec. II (closed form of I^ln_{ab;cd}, the geometric invariants D, Delta, Phi, the compact four-point potential, the full 2PN Hamiltonian, and the corrected index error); Sec. III (numerical validation); Sec. IV (open 3PN problem).

## Scores

- 🔬 **Quality:** 7/10
- 🎯 **Relevance:** 5.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.8/10)

## 🚧 Caveats

- The derivation is only sketched in prose; no intermediate steps are printed, so the formula cannot be re-derived from the paper.
- Validation is numerical and internal -- the closed form is compared to the same group's own integral representation, not to an independent formalism or gauge.
- The step beyond the authors' own 2026 PRD is tractability, not physics: the 2PN N-body dynamics was already computable numerically. No timing benchmark or application is given.
- The derivation was obtained with substantive large-language-model assistance (disclosed in Sec. II); the authors' stated safeguard is independent verification plus the numerical check.
- No estimate is given of when the four-body 2PN terms are actually large enough to matter astrophysically, and no conditioning analysis for near-degenerate (tight-binary-in-a-cluster) configurations.

---

🔗 [Back to the weekly digest](../2026-09-22)
