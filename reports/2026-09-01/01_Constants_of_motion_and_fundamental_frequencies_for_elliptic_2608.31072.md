# ♻️ Constants of motion and fundamental frequencies for elliptic orbits at fourth post-Newtonian order: aligned-spin contributions

**Citation:** David Trestini, Jan Steinhoff, *Constants of motion and fundamental frequencies for elliptic orbits at fourth post-Newtonian order: aligned-spin contributions*, arXiv:[2608.31072](https://arxiv.org/abs/2608.31072) [gr-qc, hep-th], submitted 31 Aug 2026.

**In one sentence:** The relation between a binary's energy and angular momentum and its two orbital repetition rates is now known to fourth post-Newtonian accuracy for eccentric orbits with spins aligned to the orbit, including all spin terms up to fourth power in spin and the spin-induced shape distortion of neutron stars.

## Executive Summary

Starting from the known fourth post-Newtonian (4PN) aligned-spin Hamiltonian of Levi and Steinhoff, the authors build action-angle variables, compute the gauge-invariant radial action by a Sommerfeld contour integral, and invert it to get the Delaunay Hamiltonian. From this they extract the full conservative map between (E, J) and the radial and azimuthal frequencies (n, omega) at 4PN, for arbitrary eccentricity, with all spin contributions at linear, quadratic, cubic and quartic order in spin plus the spin-induced deformability (SID) parameters. Derived quantities follow: the orbit-averaged redshift and gyroscopic invariants via the first law, circular-orbit links, and the local 4PN scattering angle with all spin terms. They also observe that the Blanchet-Iyer-Favata ISCO stability criterion C(x)=0 is exactly the post-Newtonian expansion of K^{-2}(x)=0, where K is the circular-orbit periastron advance, and use this to reproduce the recently published 4PN spinning ISCO criterion.

## Claimed Contribution

Completion of the conservative gauge-invariant constants-of-motion-to-fundamental-frequencies map at 4PN for eccentric aligned-spin binaries, extending the author's earlier nonspinning result (arXiv:2511.10735) with all terms linear through quartic in spin plus spin-induced deformability; derived redshift and gyroscopic invariants and circular links; the observation that the Blanchet-Iyer-Favata ISCO criterion is equivalent to the vanishing of the inverse-squared periastron advance; and completion of the 4PN scattering angle with all spin contributions, including new 6PM linear-in-spin coefficients.

## Strengths

- The gauge-mixing problem is handled honestly and cleverly: the point-particle 4PN Hamiltonian is known in ADM coordinates while the spin sector is known in EFT coordinates, so they parametrize the unknown 3PN/4PN point-particle EFT coefficients agnostically and demonstrate explicitly that the spin sector of the radial action is independent of those parameters, justifying the splice at the level of gauge invariants.
- Unusually extensive cross-validation: agreement with the 3PN spinning quasi-Keplerian results of Henry et al., with the 3PN nonspinning and linear-in-spin scattering angle of Bini-Damour-Geralico, with the 5PM aligned-spin EOB angle of Khalil et al., with the post-Minkowskian NNLO spin results of Bautista et al. up to S^6, with Le Tiec's circular-orbit result, and an internal consistency check via the Kalin-Porto boundary-to-bound map between the scattering angle and the periastron advance.
- The ISCO observation is a genuine structural insight rather than bookkeeping: it collapses a technically painful stability analysis (which required careful treatment of the 4PN tail term in the Blanchet-Langlois-Ligout papers) into a quantity already in hand, and it explains why the criterion is exact at leading order in mass ratio for Schwarzschild but not for Kerr, suggesting a natural resummation.
- The scattering-angle result is nonperturbative in the post-Minkowskian sense (the arctangent structure survives), so it goes beyond the PM-truncated spinning amplitudes literature at the same PN order.
- Closed-form master integrals for the scattering angle are derived in an appendix rather than left implicit, and the results are being pushed into a public repository (PNpedia).

## Weaknesses

- This is a methodologically incremental extension of the first author's own nonspinning paper from ten months earlier, using an off-the-shelf Hamiltonian (Levi-Steinhoff 2016) and the standard Damour-Schaefer radial-action technique. Nothing about the pipeline is new; what is new is the substitution of a longer input and careful bookkeeping.
- The ISCO section, headlined in the abstract, mostly reproduces results published three weeks earlier by Blanchet, Langlois and Ligout (arXiv:2608.07756) including the SID terms. The novelty there is the shortcut and the reinterpretation, not the criterion itself, and the 'for the first time' phrasing applies only to importing a known self-force/EOB criterion into PN theory.
- The stated motivation - accurate eccentric aligned-spin 4PN phasing for LISA and next-generation detectors - is not delivered. That requires a 4PN quasi-Keplerian parametrization (explicitly deferred, with the tail term named as the hard part) and 4PN eccentric fluxes, neither of which exists.
- Conservative sector only. The 4PN Schott term that distinguishes the conservative map from the full dissipative one is explicitly dropped and left to a future paper, so the results cannot be used in a phasing calculation as they stand.
- Almost all of the actual new content lives in Supplemental Material: the SID contributions everywhere, the spin and SID parts of the Delaunay Hamiltonian, the frequency map itself, the SID scattering angle. The paper as printed is largely a description of results the reader cannot see.
- There is no quantification of what the new terms are worth: no dephasing estimate, no comparison against numerical relativity or self-force data, no statement of the eccentricity or spin regime where the 4PN spin corrections matter. The paper is a coefficient delivery with no accuracy assessment attached; it defers even the ISCO accuracy analysis to the Blanchet et al. papers.
- The redshift and gyroscopic invariants are obtained by assuming the first law of binary mechanics extends to eccentric, arbitrary-order-in-spin systems at 4PN (combining the Le Tiec eccentric first law with the Antonelli et al. all-orders-in-spin argument). This composite assumption is argued but not proved in the relevant regime; the redshift is not independently computed from the regularized metric.
- Aligned spin only. The precessing case, which the conclusion concedes is 'much more difficult' and where progress stops at 2PN, is where the eccentric-binary modelling problem is actually hard.

## Skeptic's Cross-Examination

Strip away the presentation and this is: take a Hamiltonian someone else derived a decade ago, run the same action-angle machinery the first author ran on the nonspinning case last year, and print several pages of rational coefficients in a supplement. Every place the result overlaps existing literature it agrees, which is reassuring but also means the genuinely unchecked new content is exactly the part nobody can independently confirm, and no independent derivation is offered. The one conceptual claim - the ISCO criterion equals the vanishing inverse-square periastron advance - is close to a definitional restatement, since the ISCO is where the radial frequency vanishes and K = omega/n; the content is only that K^{-2} is the perturbatively well-behaved packaging, which the self-force literature (Barack-Sago) already argued.

## Novelty in Context

The self-positioning is largely accurate but the abstract front-loads the weakest novelty. The nonspinning 4PN eccentric map is the first author's own arXiv:2511.10735 (now CQG 43, 095009); the aligned-spin 4PN Hamiltonian is Levi-Steinhoff 2016, with the second author supplying that input. The 4PN spinning ISCO stability criterion including SID was published by Blanchet, Langlois and Ligout (arXiv:2608.07756) on 2026-08-10, three weeks before this paper, and this work reproduces rather than establishes it - the paper says so plainly in Sec. 7, but a reader who stops at the abstract's 'we notice that the criterion is intricately related to the periastron advance' would not guess that the criterion itself is not new here. On the scattering side, the aligned-spin angle was known to 5PM (Khalil et al.) and to NNLO PM through S^6 (Bautista et al.); the paper confirms exact agreement in the overlap, so the genuinely new part is the higher-PM tail of the 4PN spin terms and the SID sector, plus eight new 6PM linear-in-spin coefficients. What is unambiguously new and useful is the complete eccentric aligned-spin 4PN frequency map, Delaunay Hamiltonian, redshift and gyroscopic invariants with SID - no prior work covers eccentric orbits at 4PN with spin beyond 3PN (Henry et al.). The real claim is therefore 'we fill in the spin sector of an existing 4PN eccentric framework', which is smaller than the abstract's framing but still a needed piece.

## Relevance to Your Research

Directly relevant to anyone working on action-angle formulations of relativistic two-body dynamics, self-force/PN comparison, or spinning-body EMRI dynamics. The redshift and gyroscopic invariants at 4PN with spin and SID are exactly the quantities used to calibrate and cross-check self-force computations, and the eccentric first-law discussion in Sec. 5.1 is a compact and careful summary of the state of the art. The ISCO section is worth reading for the observation that the PN stability criterion is the periastron advance in disguise, and for the suggested Kerr-exact resummation. The conclusion's paragraph on the unaligned/precessing case, which cites the reader's own 2PN precessing-spin action-angle work, marks precisely the frontier this paper does not cross - the non-separability of the precessing radial action - and is the natural point of contact for follow-up.

**Where to start:** Sec. 3 (action-angle construction and the ADM/EFT gauge-splice argument, including the agnostic-parametrization consistency check), Sec. 5.1 (state of the art on the first law for eccentric and spinning binaries, including the SID rescaling subtlety), Sec. 7 (the ISCO criterion as inverse-square periastron advance, plus the Kerr non-truncation remark), and the last two paragraphs of Sec. 8 (validation against the post-Minkowskian spinning-amplitude literature and the new 6PM coefficients). Skip Sec. 4 and the appendices unless you need the coefficients themselves, which are mostly in the Supplemental Material anyway.

## Scores

- **Quality:** 7.5/10
- **Relevance:** 8/10
- **Reading priority:** 🌟 Must-Read

## Caveats

- Conservative sector only: the 4PN Schott term separating the conservative from the dissipative map is dropped and must be added later.
- Aligned spins only; the precessing case remains stuck at 2PN and is explicitly deferred.
- The 4PN spinning ISCO criterion is reproduced, not derived first - Blanchet, Langlois and Ligout (arXiv:2608.07756) published it three weeks earlier.
- Most of the new results, including all spin-induced-deformability terms and the frequency map itself, are only in the Supplemental Material.
- No dephasing estimate, no numerical-relativity or self-force comparison, no statement of where these corrections actually matter.
- The redshift and gyroscopic invariants rest on assuming the first law holds for eccentric orbits to all orders in spin at 4PN, rather than on an independent regularized-metric computation.
- The authors disclose using an AI assistant for literature exploration, equation formatting, cross-checking against the literature, and part of the master-integral computation.

## In Network

- 🚩 David Trestini — extended-network collaborator
- 🚩 Jan Steinhoff — extended-network collaborator

---

[Back to the weekly digest](../2026-09-01)
