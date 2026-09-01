# ∞ Mode stability for the Klein-Gordon equation on subextremal Kerr-de Sitter spacetimes

**Citation:** Peter Hintz, *Mode stability for the Klein-Gordon equation on subextremal Kerr-de Sitter spacetimes*, arXiv:[2608.25868](https://arxiv.org/abs/2608.25868) [gr-qc, math.AP], submitted 26 Aug 2026 (v2).

**In one sentence:** A rigorous proof shows that a scalar field on a rotating black hole in an expanding universe can never grow, for every spin rate short of the extreme limit, so all such disturbances die away exponentially.

## Executive Summary

The paper proves mode stability for the scalar wave (and, in the updated version, massive Klein-Gordon) equation on Kerr-de Sitter black holes across the entire subextremal parameter range: there are no purely oscillating or exponentially growing quasinormal modes with non-negative imaginary part except the trivial constant at zero frequency. The obstacle had always been the superradiant frequency band, where the standard Wronskian argument fails and where Whiting's integral transform, the tool that settles the asymptotically flat Kerr case, has no known Kerr-de Sitter analogue. Hintz instead works entirely in configuration space: he splits the radial domain at the point where the superradiance factor q(r) vanishes, conjugates away the outgoing oscillations on each side, and constructs an energy multiplier f times a first-order operator whose current is monotone on both pieces, forcing the boundary amplitude at the cosmological horizon to vanish. Combined with Petersen-Vasy's Fredholm/quasinormal-mode expansion, this upgrades their conditional decay statement to an unconditional theorem: sufficiently regular solutions of the scalar wave equation on any subextremal Kerr-de Sitter spacetime decay exponentially to a constant.

## Claimed Contribution

First proof of mode stability for the scalar wave / Klein-Gordon equation on Kerr-de Sitter in the full subextremal parameter range (previously known only near the slow-rotation boundary, Dyatlov, and the small-Lambda-M-squared boundary, Hintz 2021), obtained by a new, elementary physical-space energy-multiplier argument that replaces Whiting's transformation in the superradiant frequency range; and, as a corollary with Petersen-Vasy, the first unconditional exponential decay-to-constants statement for scalar waves on all subextremal Kerr-de Sitter black holes.

## Strengths

- It closes a genuinely open problem that the community had only probed numerically (Yoshida-Uchikata-Futamase; Novaes-Marinho-Lencses-Casals) or partially (Casals-Teixeira da Costa covered only part of the superradiant band for Teukolsky).
- The method is new in kind, not just in scope: a positive-commutator / energy-multiplier argument in configuration space, using only integration by parts, where every previous full-range proof (Kerr) needed Whiting's non-local integral transform. Such arguments are usually more robust to perturbation of the equation than transform-based ones.
- The logical chain is clean and checkable: reduction to the radial ODE (Sec. 3), the non-superradiant Wronskian case done in half a page, the superradiant case reduced to the existence of a multiplier with two sign conditions (Prop. 4.5), then to a constrained ODE inequality for the logarithmic derivative alpha (Lemma 4.7), with the upper-half-plane case handled by a continuity argument in the black hole parameters down to Schwarzschild-de Sitter, where stability is elementary.
- Honest positioning: the paper states plainly that the spin +/-2 Teukolsky case remains open, that it obtains no information whatsoever about modes with negative imaginary part, and that extremal parameters are excluded.
- The corollary is concrete and immediately usable: Petersen-Vasy's conditional decay result becomes unconditional for the scalar field on all subextremal Kerr-de Sitter.

## Weaknesses

- The result is for spin 0 only. The stated motivation is unconditional nonlinear stability of Kerr-de Sitter in the full subextremal range (Hintz-Petersen-Vasy 2025), which requires mode stability for the ungauged linearized Einstein equation; the paper explicitly does not address that, and the scalar case is historically the easiest rung of that ladder. The advertised payoff is therefore a first step, not the step.
- The 'algebraic miracle' at the heart of the construction is a set of polynomial positivity statements verified by Mathematica via Bernstein expansions (Lemma 4.9's A_1, the N_1 polynomial of degree 6 in s, and w*E_0 + E_1). Bernstein non-negativity is a legitimate positivity certificate, but the proof is machine-dependent in practice: no human-readable verification is offered, and the paper itself notes the argument is 'very sensitive to the precise form of the lower bound' used for the angular eigenvalue, which signals fine-tuning rather than structural insight.
- The multiplier is built by cases (an explicit f_+ = r_0/r on the cosmological side; on the event-horizon side either an explicit solution or a piecewise 'saturate the constraint then integrate the equality' construction, split according to whether A(r_e) is above or below the angular eigenvalue L). It works, but it is not conceptually illuminating in the way Whiting's transform or the Casals-Teixeira da Costa hidden spectral symmetry is, and the paper offers no evidence that it generalizes to nonzero spin.
- The decay rate epsilon in Theorem 1.3 is qualitative and unquantified. Hintz's earlier small-black-hole work gave the optimal rate sqrt(Lambda/3) + o(1) and located shallow modes; here nothing is said about the spectral gap for general parameters, so the physically interesting quantity (how fast, and where the slowest modes sit) is untouched.
- The version I could read is v1, which treats only the massless wave equation. The Klein-Gordon mass extension to m^2 in [0, sqrt(2) Lambda], including the conformally coupled / spin-0 Teukolsky case, appears only in v2, whose text the tooling did not serve; that extension is therefore unverified in this report. Given Shlapentokh-Rothman's growing massive modes on Kerr, the precise upper endpoint of the admissible mass range deserves a careful read.
- The author declares extensive use of a large language model in the exploratory phase. That is a transparency plus, but combined with the CAS-verified inequalities it means a careful referee has real verification work to do on the polynomial algebra.

## Skeptic's Cross-Examination

Strongest objection: the paper's own framing sells it as a step toward unconditional nonlinear stability of Kerr-de Sitter, but the scalar wave equation is the case everyone already believed (numerics from 2010 and 2019 said so) and the hard obstruction for the Einstein equation is the spin-2 Teukolsky system, for which the multiplier constructed here has no known analogue. A skeptic would add that the technical core reduces to Mathematica-verified positivity of specific quartic-to-sextic polynomials in a clever set of variables, chosen after the fact so that the inequalities happen to hold; without a structural reason for that positivity, there is no reason to expect the construction to survive the passage to nonzero spin, and the method may be a one-off. The counterargument is that it is nonetheless a theorem where before there was numerical evidence, and that physical-space energy arguments have historically been the ones that survive to the nonlinear setting.

## Novelty in Context

The self-positioning checks out. Dyatlov (and Vasy's Fredholm approach) covered |a/M| small; Hintz 2112.14431 covered Lambda*M^2 small with |a/M| bounded away from 1, treating Kerr-de Sitter as a singular perturbation of Kerr and using Whiting/Shlapentokh-Rothman as a black box; Casals-Teixeira da Costa 2105.13329 explicitly advertise only a 'partial mode stability result for Kerr-de Sitter' from their hidden spectral symmetries. I found no competing claim of full-range Kerr-de Sitter mode stability. Petersen-Vasy 2112.01355 does end with 'this reduces the question of decay for solutions to wave equations to the question of mode stability' in the full subextremal range, so the 'unconditional decay' corollary is correctly attributed and correctly conditional-free. The one place where the framing is more generous than the content is the nonlinear-stability motivation: Hintz-Petersen-Vasy 2508.06620 is conditional on mode stability for the ungauged Einstein equation, and nothing here bears on spin 2. The real novelty is thus twofold and both parts are genuine: the theorem for spin 0 in the full range, and a transform-free proof technique for the superradiant band.

## Relevance to Your Research

This sits in black hole perturbation theory rather than in extreme-mass-ratio dynamics, so it is background rather than directly usable. It matters if you care about the rigorous status of quasinormal-mode expansions and the meaning of 'no growing modes' for the separated radial equation, and it touches literature you are likely to know from the other side: Casals-Teixeira da Costa's hidden spectral symmetries and the Aminov-Grassi-Hatsuda / Painleve-Heun connection are cited here as reinterpretations of the Whiting transform, and this paper is precisely the statement that no such transform is needed. Read the Introduction for the map of what is and is not known about Kerr-de Sitter mode stability, then Sec. 4.1-4.2 for the multiplier idea; the rest of Sec. 4 is polynomial bookkeeping.

**Where to start:** Introduction (the paragraph listing Dyatlov, Hintz, Casals-Teixeira da Costa, and the proof-strategy paragraph at the end); Sec. 3 for the reduction to the radial ODE and the half-page Wronskian argument outside the superradiant band; Sec. 4.1-4.2 for the current, the multiplier f_+ = r_0/r, and Corollary 4.4; Sec. 6 for the continuity-in-parameters argument that pushes the result into the upper half plane. Sec. 4.3 onward and Appendix A are for readers who want to check the polynomial inequalities.

## Scores

- **Quality:** 8.5/10
- **Relevance:** 5/10
- **Reading priority:** 🌟 Must-Read

## Caveats

- Spin 0 only: the spin +/-2 Teukolsky case relevant to gravitational perturbations, and hence to unconditional nonlinear stability of Kerr-de Sitter, remains open.
- No information at all about modes with negative imaginary part, and no quantitative decay rate or spectral gap for general parameters.
- The technical core rests on polynomial positivity checks performed with computer algebra (Bernstein expansions, code in Appendix A); the author notes the argument is sensitive to the precise form of one of the bounds.
- Extremal Kerr-de Sitter parameters are excluded.
- The massive Klein-Gordon extension in the title appears in v2; the accessible v1 text covers the massless wave equation only.

---

[Back to the weekly digest](../2026-09-01)
