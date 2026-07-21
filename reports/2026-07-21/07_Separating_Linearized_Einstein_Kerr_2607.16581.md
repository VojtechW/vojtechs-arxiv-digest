# 🪄 Separating the linearized Einstein equations in Kerr

**arXiv:** [2607.16581](https://arxiv.org/abs/2607.16581)
**Authors:** Jianwei Mei (Sun Yat-sen University / TianQin)
**Category:** gr-qc
**Submitted:** 2026-07-18

## TL;DR
A single-author paper claiming, for the first time, an explicit closed-form expression for all ten Kerr metric-perturbation components in de Donder gauge in terms of two Teukolsky-type master functions f_0, f_4 — obtained by combining the Killing–Yano symmetry operator, tracelessness of the spin-2 sector, parity, and the de Donder condition. Vacuum only; obtained via a specific ansatz whose generality the author admits is not proven.

## Summary
The linearized Einstein equations δG_μν = 8πG T̃_μν in Kerr have ten coupled PDEs. Metric reconstruction (Chrzanowski/Kegeles–Cohen/Wald/Hertz-potential) recovers the metric from ψ_0 or ψ_4 but is indirect, radiation-gauge, and has known gauge-singularity problems in the presence of sources; recent explicit work by Berens–Gravely–Lupsasca (2024) and Hollands–Toomani (2024/2026) has made this cleaner but still stays in radiation gauge. Mei attacks the problem in the de Donder gauge instead.

Building on his own earlier paper (Mei 2023, arXiv:2311.18409) that constructed a fourth-order KY-derived commuting symmetry operator 𝒦₄, this paper adds three new ingredients: (i) the trace h = g^{μν}h_{μν} obeys the spin-0 (scalar) equation and can be excised, making the spin-2 sector traceless; (ii) the equations respect a parity symmetry, and one can work at fixed parity; (iii) ψ_0, ψ_4 are treated as known Teukolsky-obeying master functions and used as constraints. Combining these with the eigen-equation of 𝒦₄ and de Donder gauge, the author reduces the system to a manageable set of equations, solves an ansatz (eq. 31) for one function, and then reads off explicit closed-form expressions (equations 39–41) for every h_{μν} component as a linear combination of f_0, f_4 and their (r,x) derivatives. A byproduct: a relation between f_0 and f_4 that resembles the Teukolsky–Starobinsky identity, with the Teukolsky–Starobinsky constant Q playing the expected role (Q=0 → algebraically special).

## Strengths
- Actually attacks the direct-separation problem in a covariant gauge (de Donder) rather than radiation gauge, which is the correct thing to want if the ultimate goal is a well-behaved metric for source problems and second-order perturbation theory.
- Explicit use of the Killing–Yano tensor and a KY-derived commuting operator — this is a real hidden-symmetry construction, not window dressing.
- Recovers the Teukolsky–Starobinsky constant from the machinery internally, which is a nontrivial internal consistency check. Explicitly cross-checks against the Berens et al. (2024) and Chandrasekhar (1984) forms of the T–S constant.
- The two mode-basis solutions (f^{(0)}_{μν}, f^{(4)}_{μν}) reproduce, without ansatz, the two solutions found by ansatz in the earlier Mei (2023) paper — an independent-derivation cross-check.
- Provides algebraically special limits (Q=0) discussion consistent with Chandrasekhar 1984.

## Weaknesses
- Vacuum only, and the "outlook" openly says extending to sources is the physically interesting case. Metric-reconstruction gauge singularities in the presence of sources are the very issue that motivated the paper; without the sourced version the payoff is theoretical.
- Uses an ansatz (eq. 31) to solve a key intermediate equation (eq. 29), and the paper explicitly says: "since (29) has been solved by using an ansatz, i.e. (31), some generality might have been lost. It will be interesting to see if there is a more general solution than the one found here." So the "unique set of decoupled mode functions" phrasing in the abstract is a slight overreach.
- Physical relevance of the mode functions is asserted as "encouraging" but not established: "the properties and true physical relevance of the mode functions require more extensive study to clarify."
- No numerical demonstration: no plot, no comparison against a known mode (e.g. Kerr QNMs, or a mode reconstructed via the Berens et al. formula), no explicit sanity check that a Chrzanowski-reconstructed metric can be mapped into these formulas by a gauge transformation.
- Single-author, and the derivation is enormous DCS ("Differentiate–Cancel–Simplify") algebra whose intermediate expressions are stated to be "too complicated to be presented in a paper". A skeptic asks: is there a supplementary Mathematica notebook? The paper (as extracted) does not point to one.
- The competing modern approach — Berens, Gravely, Lupsasca 2024, and Hollands–Toomani 2024/2026 — already gives explicit metric-reconstruction formulas without Hertz potentials, in radiation gauge, and can be gauge-transformed. Whether Mei's de-Donder-gauge formulas represent a real practical advance or a parallel construction depends on how badly the radiation-gauge singularities actually hurt the target application (self-force / second-order EMRI). The paper cites both but does not benchmark against them.
- The claim that Q≠0 is necessary for the fixed-parity relation, and that dropping fixed parity allows algebraically special solutions at Q≠0, is intriguing but is presented without further verification.

## Novelty Cross-Check
Self-assessment (Section V, verbatim): *"In this work, an explicit derivation has been presented to separate the LEEs in Kerr. ... With these equations, explicit formulas have been derived, for the first time, expressing the linear order metric perturbation entirely in terms of some master functions, i.e., f_4 and f̃_4 (or, equivalently, f_0 and f̃_0). These master functions satisfy the readily separable equations, (22), (23) and their parity conjugates, all of which are variants of Teukolsky's master equation."*

Is this honest? Nuanced yes. Prior work:
- Mei (2023), arXiv:2311.18409 — same author, same programme, but explicitly did *not* reduce to a single master equation of a single unknown; the present paper's contribution is finishing that job by adding trace + parity + Weyl-scalar constraints. So the "for the first time" wording is really "first time by *this* direct-separation route".
- Berens, Gravely, Lupsasca 2024, arXiv:2403.20311 — "Reconstruction of Linearized Metric Perturbations": also gives explicit metric-perturbation formulas from ψ_0/ψ_4 modes, no Hertz potential, using T–S identities. In *radiation* gauge, but functionally covers a large part of the same practical need. Mei's novelty over this is: (a) covariant de Donder gauge, (b) obtained by direct separation of the field equations rather than by metric reconstruction from Weyl scalars.
- Hollands, Toomani 2024/2026, arXiv:2405.18604 — modern treatment of metric reconstruction including sourced cases and gauge issues.
- The KY-operator idea for spin-2 in Kerr has a long lineage (Andersson–Bäckdahl–Blue et al.; Aksteiner et al.). Mei's 𝒦₄ operator is his own construction from Mei (2023).

Net: the "first" claim is defensible but modest. This is not "we can separate Kerr LEEs and no one else can"; it is "we can express the de Donder-gauge metric perturbation as explicit algebraic combinations of two Teukolsky-mode master functions, by direct separation, using the KY symmetry".

## Relevance to Witzany
High — this is squarely in Witzany's hidden-symmetry / separability wheelhouse. It uses a Killing–Yano-derived commuting operator on the metric-perturbation equation and claims a full separation of the spin-2 sector, exactly the kind of construction Witzany has been thinking about (parallel-transported frames, spinning-particle constants of motion, KY–driven separability). The vacuum limitation is a real disappointment for EMRI applications, but the machinery is the interesting object. Witzany may want to (a) check whether the mode basis matches or extends the covariant-basis reconstructions from the Andersson–Aksteiner–Bäckdahl programme, (b) see whether the ansatz (31) can be replaced or interpreted geometrically, and (c) evaluate whether the de-Donder-gauge master expressions could be pulled into a self-force calculation to avoid radiation-gauge string singularities.

Anti-example check: the paper is *not* an "of course it's separable because it's Kerr-like" paper — the KY structure is being genuinely used to construct a symmetry operator on the perturbation equations, not just relied on as a coordinate accident. This is the genuine hidden-symmetry variety.

## Quality Score
- Overall: 6.5/10
- Direct relevance: 8/10
- Novelty: 6/10
- Technical rigor: 6/10

**Tier:** Should-Read

**Collaborator flags:** None direct. Cites Hollands & Toomani, Berens et al. (community-adjacent).
