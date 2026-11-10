# 🕳️ Variational Approach to the Mathisson-Papapetrou-Dixon Equations of Motion for Extended Objects in General Relativity

🌠 **Should-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 6/10

📎 **Citation:** Trevor Scheopner, Felix Lichtner, *Variational Approach to the Mathisson-Papapetrou-Dixon Equations of Motion for Extended Objects in General Relativity*, arXiv:[2611.10794](https://arxiv.org/abs/2611.10794) [gr-qc, hep-th], submitted 07 Nov 2026.

> 💡 A long, modernised review rebuilds Dixon's exact theory of how a spinning, deformable body moves in curved spacetime from a single action principle, linking the classic equations directly to the effective-field-theory language used in binary calculations.

## 🔍 Executive Summary

The paper reviews the Mathisson-Papapetrou-Dixon theory of extended bodies: momentum and spin are defined as generators of approximate Poincare transformations built from Synge's world function, and the stress-energy and current densities are decomposed into Dixon's reduced multipole moments, which are not constrained by the conservation laws. It goes through the pieces in order: Newtonian gravity, flat-space electromagnetism, linearised gravity, then curved-space electromagnetism and full general relativity. It works with the gauge-invariant pairing of the stress-energy tensor with a metric perturbation throughout, so each reduced moment ends up paired with one 'multipolar Riemann tensor' (Dixon's tensor extension of the metric). The whole system is then packaged into a worldline action with a dynamical mass function, from which the moments follow as derivatives. The authors also give a fixed-point (contraction) argument, with explicit integral bounds, for when the momentum-aligned time slicing and the covariant (Tulczyjew-Dixon) spin supplementary condition can be imposed.

## 📣 Claimed Contribution

A coherent, modern-notation review of the full MPD theory that fills stated gaps in the literature: (i) precise conditions under which the momentum-direction time slicing and the covariant spin supplementary condition can be enforced, with proofs in the appendices; (ii) a derivation of Dixon's reduced moments from a manifestly gauge-invariant variational principle, which the authors say is simpler than Dixon's original route; (iii) 'for the first time', a simplified explicit distributional formula for the stress-energy tensor of a generic compact object in terms of its reduced multipole moments and a natural basis of curvature tensors conjugate to them; (iv) the relation between the worldline effective-field-theory dynamical mass function and Dixon's reduced moments.

## ✅ Strengths

- Fills a genuine pedagogical gap: Dixon's 1970-74 trilogy is notoriously hard to read, and a self-contained, modern-notation treatment that builds up from Newtonian gravity through flat-space electromagnetism and linearised gravity is useful as a reference.
- Real calculation, not hand-waving: the curved-spacetime gravitational sector is derived explicitly (metric variation of the tangentised metric, Lie-derivative terms that generate force and torque, pairing of the reduced moments with the multipolar Riemann tensors).
- Gives a clean dictionary between Dixon's reduced moments and derivatives of the dynamical mass function with respect to the multipolar Riemann tensors and field-strength extensions, which is exactly what is needed to match effective-field-theory Wilson coefficients to physical multipoles without degeneracies.
- Existence and uniqueness of the centroid satisfying the spin supplementary condition is argued with an explicit contraction-map construction and quantitative integral bounds (Appendices on time-direction and SSC integral bounds), not just asserted.
- Honest about limits: it states clearly that the MPD system does not close without a model for the higher moments, and that self-force is not treated.

## ⚠️ Weaknesses

- Mostly a review: the bulk of the material (generator definitions of momentum and spin, reduced moments, the MPD force and torque to all orders) is Dixon's, and the gauge-invariant pairing of the stress-energy tensor with a metric perturbation is essentially Dixon's 1974 functional definition of the moments, later streamlined by Harte (2012) with generalised Killing fields.
- The headline 'first' result, the explicit all-order stress-energy formula in terms of reduced moments and multipolar Riemann tensors, is also the subject of a companion short paper by the same authors (arXiv:2611.10783). The incremental content is therefore split across two papers, and this one is the long-form version.
- The existence and uniqueness of the centre-of-mass worldline under the covariant spin supplementary condition was already studied by Beiglbock (1967) and Schattner (1979, Gen. Rel. Grav. 10, 377 and 395). Schattner is not among the works cited in the sections I read, so the claimed 'gap in the literature' looks overstated. The paper's contribution is explicit bounds, not the first proof.
- The action-with-dynamical-mass-function structure (Bailey-Israel, Steinhoff, Vines et al. 2016, Levi-Steinhoff) is standard. The genuinely new piece is only the all-order identification of its derivatives with Dixon's reduced moments.
- No worked example is carried through to a new physical result: no quadrupole or octupole application in Kerr, no comparison against an explicit known stress-energy tensor such as the spin-squared stress-energy of Steinhoff-Puetzfeld or Vines et al. beyond consistency statements, and nothing numerical.
- Self-force is explicitly not treated. The self-field regularisation that Harte's work handles is only mentioned, so the 'exact, including self-force' framing in the overview depends on the body's effective moments being renormalised elsewhere.
- Very long, with heavy bespoke notation (tangentisation, tensor extensions, moment-generating functionals). The SSC appendix alone is about 60 thousand characters, so the cost of entry is high.

## 🤔 Skeptic's Cross-Examination

Strip away the re-derivation of Dixon and what remains is a change of basis: rewriting Dixon's force and torque series and his skeleton stress-energy in terms of derivatives of a mass function with respect to Dixon's own tensor extensions of the metric. That is presentation, not physics. It is also published twice (here and in arXiv:2611.10783), and its claim to fill a 'gap' on the spin supplementary condition ignores Schattner's 1979 uniqueness proofs. The paper also never uses the formalism to compute anything new, so there is no test that the simpler form actually pays off.

## 🆕 Novelty in Context

The paper positions itself as a review following Dixon's logic, with three claimed advances: a variational, gauge-invariant derivation; the conditions for the covariant spin condition; and a 'first' simplified explicit stress-energy formula. Literature check: (1) An INSPIRE search for the authors shows a same-day companion paper, arXiv:2611.10783 ('The Energy-Momentum Tensor of a Compact Object in General Relativity to all Multipole Orders'), whose abstract claims the same novel distributional formula and conjugate tensor basis. The genuinely new content is shared with that paper, and this one is its extended, review-format version. (2) Dixon's own 1974 construction already defines the reduced moments through the pairing of the stress-energy tensor with test fields, and Harte (Class. Quantum Grav. 29, 055012, 2012) simplified the force and torque derivation with generalised Killing fields. So 'derive it from the metric pairing' is a streamlining, not a new idea. (3) Vines, Kunst, Steinhoff and Hinderer (Phys. Rev. D 93, 103008, 2016) and the Steinhoff and Levi effective-field-theory papers already link actions with a dynamical mass function to Dixon's quadrupole, at low multipole order. The all-order identification here extends that. (4) Existence and uniqueness of the Tulczyjew-Dixon centroid was treated by Beiglbock (1967, cited) and Schattner (Gen. Rel. Grav. 10, 1979), which I did not find in the citations I saw. The 'gap' claim should be read as 'explicit quantitative sufficient conditions', not as the first proof. Net: a valuable, careful synthesis with a modest all-order formal addition, not a conceptual breakthrough.

## 🎯 Relevance to Your Research

Directly relevant to anyone modelling spinning or tidally deformed secondaries in extreme-mass-ratio inspirals, or matching worldline effective-field-theory operators to physical multipoles. The MPD equations are the foundation of the spinning-secondary self-force and post-Minkowskian programmes. This is a reference to consult, not a result to act on: it changes no waveform or flux and gives no new prediction. Most useful to readers who need a clean all-order statement of which curvature structure each Dixon moment couples to, or a citable set of conditions for the Tulczyjew-Dixon spin supplementary condition.

📖 **Where to start:** Start with 'Overview of the Main Results' in the Introduction and the 'Summary' section near the end (subsections on mass multipole moments, worldline and time-direction specification, and variational results); together they give the whole content compactly. 'Full General Relativity: Final Form of the Action' is where the new all-order pairing of reduced moments with multipolar Riemann tensors is derived. For the spin supplementary condition argument, read 'Selection of the Worldline' and the 'SSC Integral Bounds' appendix. 'Applications and Limitations of the MPD Equations' covers how to close the system with effective-field-theory power counting.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.0/10)

## 🚧 Caveats

- This is a review. The new result (an all-order stress-energy formula in a basis of curvature tensors, one per reduced multipole) also appears in the companion paper arXiv:2611.10783.
- Self-force is not treated. All applications are left to the test-body limit or to other work.
- The 'gap' about when the covariant spin condition can be imposed overlaps older existence and uniqueness work (Beiglbock 1967, Schattner 1979).
- No new physical calculation, waveform or flux: this is formalism and pedagogy only.
- Long and notation-heavy. Use the Summary section near the end as the entry point.

---

🔗 [Back to the weekly digest](../2026-11-10)
