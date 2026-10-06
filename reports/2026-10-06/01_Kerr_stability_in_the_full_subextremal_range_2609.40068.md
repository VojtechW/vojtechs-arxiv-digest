# ∞ Kerr stability in the full subextremal range

🌠 **Should-Read** · 🔬 Quality 8/10 · 🎯 Relevance 5/10

📎 **Citation:** Jérémie Szeftel, *Kerr stability in the full subextremal range*, arXiv:[2609.40068](https://arxiv.org/abs/2609.40068) [math.AP, gr-qc, math-ph], submitted 30 Sep 2026.

> 💡 A mathematical proof that every rotating black hole spinning slower than the theoretical maximum is stable: if slightly disturbed by a broad, loosely constrained class of perturbations, it settles down to a nearby rotating black hole.

## 🔍 Executive Summary

The paper completes the Klainerman-Szeftel programme for nonlinear stability of Kerr, removing the slow-rotation assumption |a| << m and covering all |a| < m for initial perturbations decaying only like r^{-3/2-delta}, with no structure required in that decay. The author argues that the earlier slow-rotation proof (GCM spheres and hypersurfaces, the PG/PT gauges, Ricci-coefficient estimates) already holds for all subextremal spins. On that reading, smallness of a was used in only two places: decay of the Teukolsky scalars (Theorems M1/M2) and high-order curvature energy estimates (Theorem M8). The first is handled by importing the Ma-Szeftel energy-Morawetz estimates for Teukolsky wave/transport systems on perturbed Kerr, adapted to a bootstrap region that ends at a spacelike boundary Sigma_*. The second needs two new arguments: an R-hat-squared commutation of the coupled wave equation for the renormalized curvature component P, and a second type of Hodge estimate in the non-integrable formalism that avoids the smallness of a by using prior control of null derivatives of A, B, B-bar and A-bar.

## 📣 Claimed Contribution

Extension of the slowly rotating Kerr stability theorem (Klainerman-Szeftel, Giorgi-Klainerman-Szeftel, Shen) to the full subextremal range |a|<m, 'thereby completing the proof of the Kerr stability conjecture' for general asymptotically flat data with r^{-3/2-delta} decay. New ingredients: adapting the Ma-Szeftel Teukolsky energy-Morawetz estimates to the bootstrap spacetime, including new coordinates, complex 1-forms and a regular triplet for scalarization; an energy-Morawetz estimate for the renormalized curvature component P-check that does not use smallness of a; and Hodge estimates in the non-integrable formalism that hold for all subextremal a.

## ✅ Strengths

- Addresses the central open problem of mathematical black-hole physics: nonlinear stability of Kerr for all subextremal spins, in a framework that tolerates rough data decaying only like r^{-3/2-delta}.
- The introduction states precisely where smallness of a entered the earlier proof (Theorems M1, M2 and the curvature part of M8 in GKS22). The reduction to fixing exactly those steps is clearly structured and can be checked against the earlier volumes.
- Brings in genuinely new arguments where the old proof needed small a: the old proof absorbed the term Im(W) = O(m a r^{-4}) in the P-check wave equation, while the new proof uses an R-hat-squared commutation and the identity linking angular derivatives of P-check to Teukolsky scalars. It also adds a second type of Hodge estimate in the non-integrable formalism that uses prior e_3/e_4 control.
- The comparison with the competing Hintz proof is explicit and concrete about the data classes (finite polyhomogeneous expansion plus O(r^{-3-delta}) remainder, versus structureless O(r^{-3/2-delta})).

## ⚠️ Weaknesses

- The paper is not self-contained. The analytic heart, energy-Morawetz estimates for Teukolsky equations in the full subextremal range, sits in Ma-Szeftel (arXiv:2410.02341, 2603.23437), and both the Teukolsky wave-transport derivation and the proof of the key Teukolsky estimate (Theorem 'MaSz26' adapted to the bootstrap region) are deferred to a companion paper (arXiv:2609.40315) posted the same week. As far as I can tell, none of these is refereed yet.
- The full proof spans thousands of pages across GCM1, GCM2, KS:Kerr, GKS22 (a book-length work), Shen and the new papers. Calling it 'completing the proof' rests on the claim that all other steps already hold for |a|<m, which the paper asserts rather than re-verifies here.
- The novelty framing towards Hintz's June 2026 proof (arXiv:2606.28253) is polemical. Hintz's data allow slowly decaying terms r^{-z}(log r)^k with z>1, slower than r^{-3/2}, provided they come as a finite expansion. Szeftel's argument that such data are 'not stable under perturbations' and amount only to 'well-prepared data' is a fair point about genericity, but it is not a neutral description of a competing full-subextremal result posted three months earlier.
- The decay information obtained is the bootstrap-level statement (for example tau^{-1-delta} decay of A), weaker and less explicit than the t^{-2-epsilon} rate in compact regions and the gravitational-wave tail asymptotics in Hintz's approach, so physics applications get less out of it.
- As with the earlier volumes, the presentation is extremely technical (the iteration over J derivatives, norms like R_{J+1} and S_{J+1}). Without the earlier volumes at hand it cannot be checked in reasonable time.

## 🤔 Skeptic's Cross-Examination

The headline result is mostly an assembly: the hardest new analysis (large-a Teukolsky energy-Morawetz estimates near trapping and superradiance) lives in unrefereed companion papers, one of them posted the same week. The claim that every other step of a multi-thousand-page proof 'already holds for |a|<m' is asserted, not re-proved. Meanwhile, the framing that the competing Hintz result covers only 'well-prepared' data is a choice of topology on initial data, which is precisely where the two camps disagree.

## 🆕 Novelty in Context

The paper presents itself as the conclusion of the Klainerman-Szeftel / Giorgi-Klainerman-Szeftel / Shen programme (slow rotation, |a| << m), with the large-|a| analytic input supplied by Ma-Szeftel 2024 (scalar wave, arXiv:2410.02341) and 2026 (Teukolsky, arXiv:2603.23437). The Ma-Szeftel 2026 abstract explicitly frames that work as the essential step towards this extension, so much of the analytic novelty for large a is already in that preprint. The new content here is the integration into the bootstrap, plus new P-check and Hodge-estimate arguments for the curvature energy estimates. The literature check shows the 'completing the Kerr stability conjecture' claim has a direct competitor. Häfner-Hintz-Vasy proved linear stability for all subextremal spins (arXiv:2506.21183), and Hintz posted 'Nonlinear stability of subextremal Kerr black holes' (arXiv:2606.28253, June 2026). That paper works in a generalized wave-map gauge with a Nash-Moser scheme, and its data are a finite expansion in r^{-z}(log r)^k with z>1 plus an O(r^{-3-epsilon}) remainder. Szeftel describes the Hintz data accurately but frames them as 'well-prepared' and not an open set. The defensible novelty claim is therefore narrower than the abstract implies. This is the first full-subextremal proof for general, structureless data with r^{-3/2-delta} decay, which handles the infinite-dimensional gauge freedom of general covariance directly through GCM constructions. It is not the first nonlinear Kerr stability proof for all |a|<m.

## 🎯 Relevance to Your Research

This is a landmark mathematical-GR result rather than a direct tool for EMRI or self-force modelling. It is relevant mainly as background: it rigorously closes the stability question for the Kerr background that perturbative and self-force work assumes, and it relies on Teukolsky wave/transport systems and Teukolsky scalars on perturbed Kerr, which overlap conceptually with Teukolsky-based perturbation theory. Worth a skim of the introduction for context and for the competing-approaches landscape (curvature versus metric perturbations, and the Hintz comparison). The technical sections are of interest mainly if you follow how Teukolsky estimates work near the trapped set at large spin.

📖 **Where to start:** Section 1.1.4 (rough main theorem and the data class); Section 1.3.3 (exactly which earlier steps needed |a| << m); Section 1.3.4 (comparison with Hintz's proof and the Minkowski-stability analogy); Section 1.4.3 (proof strategy, especially the new P-check and Hodge-estimate arguments for Theorem M8). Sections 5-6 only if you need the technical details.

## Scores

- 🔬 **Quality:** 8/10
- 🎯 **Relevance:** 5/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.9/10)

## 🚧 Caveats

- This is the closing step of a very long multi-paper programme. The key Teukolsky estimates are in Ma-Szeftel and a same-week companion paper (arXiv:2609.40315), none of which appear to be refereed yet.
- Hintz posted an independent full-subextremal Kerr stability proof in June 2026 (arXiv:2606.28253) for a different class of initial data. This paper calls that result the 'well-prepared data' case; the two results cover different data classes, and whether the hard core of the conjecture has been solved by both or only by this paper is contested.
- Pure mathematical analysis: no new physical predictions, waveforms or decay tails.

---

🔗 [Back to the weekly digest](../2026-10-06)
