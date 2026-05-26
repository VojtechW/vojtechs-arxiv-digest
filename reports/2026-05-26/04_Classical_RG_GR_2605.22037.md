# 🌀 Classical Renormalization Group Equations for General Relativity

**arxiv:** [2605.22037](https://arxiv.org/abs/2605.22037)
**Authors:** F. Gutiérrez, K. Falls, A. Codello
**Categories:** gr-qc, hep-th, math-ph

## TL;DR
A short, technically clean follow-up to arXiv:2510.27676. The companion paper introduced a "classical Wetterich-style" flow equation by RG-improving the leading PM correction; that derivation was admittedly heuristic. This paper closes the gap by deriving a classical Polchinski equation for the gravitational two-body problem and showing — via a standard Legendre transform à la Morris/Wetterich — that it is dual to the heuristic flow equation of [6]. As a self-contained appendix the authors re-derive the PM expansion to 3PM from the Polchinski side. No new physical predictions; this is plumbing for a program, not an answer.

## Summary
- 🧩 **Setup.** Start from S_tot = (1/κ) S_g[g] + S_pp[g,x₁,x₂]; treat metric fluctuations h_μν around an Einstein background ḡ, introduce an IR regulator R_k on the graviton propagator Δ.
- ♾️ **Classical Polchinski.** Drop the one-loop term (h̄→0 classical limit) and obtain ∂_k 𝒮_k = -(κ/2) 𝒮_k^(1)·∂_k 𝒢_k·𝒮_k^(1), with the pure-gravity action as initial condition at k→∞. The on-shell effective action is shown to be RG-invariant.
- 🔮 **Legendre duality.** Define a Legendre-transformed pure-gravity functional S_{-1}[H]; show it does not flow and equals S_g[ḡ+H] for all k. This collapses the Polchinski equation onto the equation (4) of arXiv:2510.27676, now interpreted as a "classical Morris–Wetterich" equation for the average effective action S_k.
- 📐 **Appendix A.** PM iteration of the Polchinski equation reproduces S_{eff,-1}, S_{eff,0}, S_{eff,1}, S_{eff,2}, and S_{eff,3} in standard tree-level form involving Δ⁻¹, S_g^{abc}, S_g^{abcd}. The result coincides with what the companion paper obtains through the average-action equation.

## Strengths
- Honest about scope: paper exists *precisely because* the companion derivation was heuristic, and they do supply a rigorous duality. Legitimate mathematical bookkeeping.
- The Legendre-transform construction is correctly executed; the cancellations producing ∂_k S_{-1}=0 are nontrivial-looking but ultimately the right classical analogue of Morris–Slade reconstruction (arXiv:1507.08657, correctly cited).
- DeWitt notation is used cleanly; equations are dimensionally and combinatorially consistent through 3PM. This is not crank work.
- Conclusion section is *shorter* than the calculation section — no red flag there. Appendix A occupies roughly half the paper.

## Weaknesses / Skeptic's Attack
- **The amplitudes-person attack lands.** Modulo language, this is Wilsonian PM exactly as practiced in NRGR / Goldberger–Rothstein EFT for 20 years. The "classical Polchinski equation" is the tree-level truncation of the standard exact RG. The "average effective action" S_k is a 1PI generating functional for tree-level graphs with an IR-regulated propagator. To a Cheung–Solon-style amplituder this is repackaging, not new physics.
- **Reference list is alarming.** No Goldberger–Rothstein (NRGR), no Cheung–Solon, no Bern–Carrasco–Damour–Roiban–Solon, no Levi–Steinhoff, no Galley, no Foffa–Sturani, no Mogull/KMOC. Porto's EFT review is cited only as a "future work" hook [19]. Buonanno–Damour 1999 is cited twice as refs [2] and [17] (literally the same paper). For a paper claiming a "new approach to the two-body problem," failure to engage the modern PM/EFT literature is a serious tell.
- **No genuine non-perturbative result.** All three claimed "applications" — 1PN, 3PM, "future work PNDE" — are either (i) known to far higher order, or (ii) deferred. The selling point of exact RG is non-perturbative approximants (LPA, derivative expansion, vertex expansion); none are demonstrated here.
- **Heuristic origin admitted.** The companion's flow equation was obtained by RG-improving the lowest-order self-energy. Litim–Pawlowski (refs [10–12]) are correctly cited as showing this can fail. The Legendre-transform rescue works only because S_{-1}=S_g doesn't flow — itself a tree-level statement.
- **Possible Asymptotic-Safety bait-and-switch.** Falls and Codello are senior figures in the Reuter-school AS programme. The vocabulary (average effective action, Wetterich equation, IR regulator R_k, derivative-expansion convergence ref [22]) is imported wholesale from there. Whether a bridge to *quantum* asymptotic safety will be built or whether it dissolves at one loop is unclear.
- Typo cluster ("haver", duplicate refs, "middlebar" rendering artefacts) suggests rapid release.

## Relevance to Vojtěch's Research
- **Direct overlap: low to medium.** Vojtěch works on EMRIs, spinning particles in Kerr, self-force, structural insight into Kerr/GR. This paper is comparable-mass PM/PN with point particles in Minkowski. No black-hole background, no Teukolsky, no self-force, no spin.
- **Structural-insight angle: marginal but real.** If the formalism eventually yields a covariant ansatz with a "running metric" (future work [19] hook to Porto), there could be a conceptual cousin to canonical-transformation reorganisations used for spinning EMRIs. Speculative; nothing in this paper touches it.
- The Legendre/Polchinski duality is the kind of formal trick that occasionally repays study — a clean classical analogue of a quantum result. Worth knowing exists; unlikely to change anything operational.

## Quality Score
5 / 10
(Competent execution of a modest formal goal; severe disengagement from the PM/EFT literature; no new physics yet.)

## Relevance Score
2 / 10
(Wrong corner of GR for the user's day job; possible long-term conceptual interest only.)

## Verdict
Worth-Skimming
