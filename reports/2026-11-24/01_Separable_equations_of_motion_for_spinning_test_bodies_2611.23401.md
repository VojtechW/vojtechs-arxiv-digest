# 🔮 Separable equations of motion for spinning test bodies in spacetimes with Killing--Yano symmetry

🌟 **Must-Read** · 🔬 Quality 6/10 · 🎯 Relevance 6/10

📎 **Citation:** Abhinove N. Seenivasan, Paul Ramond, Soichiro Isoyama, Sam R. Dolan, *Separable equations of motion for spinning test bodies in spacetimes with Killing--Yano symmetry*, arXiv:[2611.23401](https://arxiv.org/abs/2611.23401) [gr-qc], submitted 17 Nov 2026.

> 💡 To first order in its spin, a small spinning body moving in any spacetime with the same hidden symmetry as a rotating black hole behaves like a charged, non-spinning particle pushed by an effective force field built from the curvature, and its motion can be written down in closed form.

## 🔍 Executive Summary

The paper takes the worldline-shift trick that Skoupý and Witzany found for Kerr, where moving the reference worldline of a spinning test body turns its linear-in-spin motion into a geodesic with shifted constants, and rebuilds it covariantly from the Killing-Yano tensor, so that only a non-degenerate Killing-Yano tensor is assumed and no field equations. After the shift, the body follows the worldline of a fictitious spinless particle whose charge is set by the spin component along the orbital angular momentum. That particle obeys a Lorentz-force equation with an effective field strength F = f* . Ricci (the dual Killing-Yano tensor contracted with the Ricci tensor), which is shown to be closed and which vanishes in Ricci-flat spacetimes. In the general off-shell canonical metric (the Kerr-NUT-(A)dS-Newman family with arbitrary metric functions), the authors give explicitly separated first-order equations of motion, reproduce the Kerr results, and work through Kerr-de Sitter, where F = Lambda f*.

## 📣 Claimed Contribution

A covariant generalisation of the Kerr worldline shift to every four-dimensional spacetime admitting a non-degenerate Killing-Yano tensor, off-shell. The authors identify spin with an effective charge coupled to a curvature-built gauge field, and give explicitly separated equations of motion (reduction to quadratures) for linear-in-spin MPTD motion in the off-shell canonical metric. They present this as a constructive realisation of known integrability, and as providing solutions 'beyond Kerr, beyond vacuum and beyond geometries satisfying the Einstein equation', where the authors say they were previously unknown.

## ✅ Strengths

- Fully covariant construction: the shift vectors are fixed by the Killing-Yano geometry (f* and f contracted with the Marck tetrad legs) rather than by coordinate-specific guesswork, and the paper states they reduce to the Skoupý-Witzany expressions in Kerr.
- The spin-as-charge picture is a clean structural result: F = f* . Ric is shown to be antisymmetric and closed, so it is a legitimate field strength, and its source current is given explicitly. The paper also correctly notes that this is not the Maxwell field, since in Kerr-Newman it is even in the charge.
- Separated equations are given for arbitrary Delta(r) and Theta(y) in the off-shell canonical metric, and the Lorentz-force equation is checked symbolically for arbitrary metric functions, with a separate covariant proof in an appendix.
- The paper is honest that integrability was already known (Rüdiger, Compère-Druart, Ramond-Isoyama, Witzany HJ papers) and frames its contribution as a constructive realisation rather than a new integrability claim.
- The Kerr-de Sitter example is concrete and readable, and shows the charge acting as a pure gauge shift when Lambda = 0, with a genuine coupling when Lambda > 0.

## ⚠️ Weaknesses

- Separability of linear-in-spin motion in spacetimes whose geodesics and parallel transport separate (which includes every Killing-Yano spacetime) was already proven by Witzany and Skoupý (arXiv:2606.25792) through the Hamilton-Jacobi equation, and this paper cites that work. The new content is therefore the explicit worldline-shift form and the charge interpretation, not separability itself. The introduction's line that solutions outside Kerr 'are not known' overstates this.
- The astrophysical payoff for small-mass-ratio inspirals is thin. Most beyond-Kerr and modified-gravity black-hole metrics used in EMRI tests have at most a Killing tensor and no Killing-Yano tensor, and Kerr-de Sitter's Lambda is negligible on EMRI scales. The class actually covered is essentially Kerr-Newman-NUT-(A)dS and off-shell relatives.
- There is no numerical check against direct integration of the MPTD equations in a non-Ricci-flat case (for example Kerr-de Sitter), and no orbit, frequency or flux is computed. Validation is symbolic only, and the claimed usefulness for waveform pipelines is asserted rather than demonstrated.
- The shift is fixed partly by a choice ('require that F carry no dependence on v beyond Q0'), and the free parameters alpha = 3/2 and beta = 0 are chosen so that the Lorentz-force form holds. The uniqueness or naturalness of this gauge is argued, not proven.
- Small notational inconsistencies, such as X_y written with g(y) while the potential function is defined as h(y), and the charge given as q proportional to K/Q in the summary but q = s_par/sqrt(Q0) in the conclusions. These are minor but suggest the paper was edited in a hurry.
- The Schwarzschild-like (a -> 0) limit falls outside the regular domain of the canonical coordinates and is relegated to a footnote.

## 🤔 Skeptic's Cross-Examination

This is the Skoupý-Witzany Kerr trick rewritten in Killing-Yano language and applied to the off-shell Carter metric, whose separability for charged particles has been textbook material since 1968. The separability result was already established a few months earlier through the Hamilton-Jacobi route. The only physically new spacetimes reached are Kerr-(A)dS and Kerr-Newman-NUT, which are irrelevant for EMRIs because Lambda is tiny and astrophysical charge is negligible. Nothing is computed numerically, so the advertised use for waveform pipelines beyond Kerr remains a promise.

## 🆕 Novelty in Context

The paper positions itself as the covariant, off-shell generalisation of Skoupý and Witzany's 2024 PRL (arXiv:2411.16855), which found the worldline shift that maps linear-in-spin MPTD motion in Kerr onto geodesics. That positioning is accurate, and the authors state that their result reduces to Skoupý-Witzany in Kerr. Integrability of linear-in-spin motion with Killing-Yano symmetry is credited to Rüdiger, Compère-Druart, Ramond-Isoyama and Witzany. The key related work turned up by the literature check is Witzany and Skoupý, 'Separability of the motion of spinning test particles in curved space-time' (arXiv:2606.25792, June 2026). That paper proves the linear-in-spin Hamilton-Jacobi equation separates whenever geodesic motion and parallel transport both separate, which holds in all Killing-Yano spacetimes (Marck/Kamran; Connell-Frolov-Kubizňák). It is cited here (as Witzany:2026eqc). Separability in this class is therefore not new. The genuine additions are (i) the explicit covariant worldline shift, (ii) the identification of an effective curvature-built gauge field F = f* . Ric with a Lorentz-force law for the shifted worldline, and (iii) explicit separated first-order equations in the off-shell canonical metric. The sentence saying linear-in-spin solutions outside Kerr 'are not known' is inflated given 2606.25792. Kubizňák-Cariglia (2011), cited, treated integrability for a pseudo-classical spinning-particle model in higher dimensions, which is related but not the same as MPTD with the Tulczyjew condition.

## 🎯 Relevance to Your Research

Directly relevant to anyone working on secondary-spin effects in EMRIs/IMRIs, on the integrability of spinning-particle dynamics, or on hidden symmetries (Killing-Yano tensors, principal tensors) in black-hole spacetimes. It is an incremental but tidy structural generalisation of the Skoupý-Witzany Kerr solution and fits naturally next to the Ramond-Isoyama integrability programme. For practical Kerr EMRI modelling it adds nothing beyond Skoupý-Witzany. Its value is conceptual (spin as charge, the role of Ricci curvature) and for non-vacuum Killing-Yano spacetimes.

📖 **Where to start:** Section 1.3 (summary of results, self-contained); Section 3.1 (how the shift is fixed by the Killing-Yano tensor); Section 4.1 (the effective gauge field F = f* . Ric and its properties); Section 4.3 (Kerr-de Sitter worked example). Skip the long Appendix C unless you want to check the covariant proof of the Lorentz-force equation.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 6/10
- 🌟 **Reading priority:** Must-Read (weighted score 6/10)

## 🚧 Caveats

- Separability itself was already proven by Witzany and Skoupý (2026) through the Hamilton-Jacobi equation; what is new here is the explicit worldline shift and the spin-as-charge picture.
- Applies only to spacetimes with a full Killing-Yano tensor, which excludes most of the beyond-Kerr metrics used in EMRI tests of general relativity.
- Validation is symbolic only: there is no comparison with direct numerical integration and no orbit, flux or waveform computation.
- The Schwarzschild-like limit (zero black-hole spin) lies outside the coordinate domain used and is handled only in a footnote.

## In Network

- 🚩 Soichiro Isoyama — extended-network collaborator
- 🚩 Sam Dolan — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-11-24)
