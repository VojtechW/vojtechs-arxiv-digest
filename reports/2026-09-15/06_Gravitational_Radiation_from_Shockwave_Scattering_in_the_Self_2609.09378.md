# 🌀 Gravitational Radiation from Shockwave Scattering in the Self-Force EFT

🔦 **Worth-Skimming** · 🔬 Quality 6.5/10 · 🎯 Relevance 4.5/10

📎 **Citation:** Emanuele Rosi, *Gravitational Radiation from Shockwave Scattering in the Self-Force EFT*, arXiv:[2609.09378](https://arxiv.org/abs/2609.09378) [gr-qc, hep-th], submitted 08 Sep 2026.

> 💡 Treating a collision of two very fast, very light particles as a small perturbation of the gravitational shock wave of the faster one, this paper computes the emitted gravitational wave without expanding in the strength of gravity, and shows that the energy radiated at high frequencies close to the direction of the fast particle is finite rather than divergent.

## 🔍 Executive Summary

The paper adapts the self-force effective field theory of Cheung et al. to a background that is not a Schwarzschild or Kerr black hole but an Aichelburg-Sexl gravitational shock wave sourced by an ultrarelativistic massless particle of energy E1, with a second, much lighter probe (massless with E2 much less than E1, or massive with m2 much less than E1) providing the perturbation. Two technical steps are added: the self-force EFT action is extended to the Schwinger-Keldysh (in-in) path integral at order q^2 so that radiative observables can be computed, and a light-cone gauge aligned with the shock-wave Killing vector is chosen, in which the 1SF and 2SF recoil operators vanish identically (conjectured to all self-force orders). The exact retarded graviton propagator on the shock wave is obtained by resumming an exponentiating ladder, reproducing the Weinberg infrared phase and a Coulomb-like phase, and it is used to build the 1SF waveform for massless-massless scattering to all orders in Newton's constant. In the strong-field limit W = 2 G E1 (xi.k) much greater than 1 a saddle-point evaluation shows a cancellation between the free and interacting pieces of the waveform, leaving O(W^-2), which makes the angular energy spectrum in the high-frequency region collinear with the primary shock wave convergent.

## 📣 Claimed Contribution

First extension of the self-force EFT to the in-in (Schwinger-Keldysh) formalism at 1SF; a light-cone gauge in which the shock-wave recoil operators vanish at 1SF and 2SF (conjectured to all orders); the exact graviton propagator and classical Compton/response amplitude on the shock-wave background derived as an exponentiating Born series; the 1SF on-shell waveform for massless-massless collisions to all post-Minkowskian orders with a soft expansion; and a proof that the resummed waveform vanishes at leading order in the trans-Planckian limit, implying ultraviolet finiteness of the angular radiated-energy spectrum in the collinear region.

## ✅ Strengths

- Real, explicit computation throughout: an all-loop Born series is summed in a mixed momentum/transverse-position representation, the exponentiation is demonstrated rather than asserted, and the light-cone ultraviolet regulator is handled carefully.
- The claimed vanishing of the recoil operator in light-cone gauge is a genuine simplification relative to the parallel worldline-quantum-field-theory treatment, which carries an extra 'remainder' term; it is verified explicitly at 1SF and 2SF.
- Two independent validation checks are attempted rather than one: the leading post-Minkowskian waveform reproduces the tree-level KMOC result, and the soft expansion reproduces the classical soft-graviton theorems at 1/omega (linear memory) and log-omega order, the latter non-perturbatively in Newton's constant.
- The propagator agrees with two independent prior derivations (Raj-Venugopalan's eikonal-approximation result and the worldline response-theory computation of Bohnenblust et al.), and the paper is explicit that its role there is confirmatory.
- The physical payoff is non-trivial and not visible order by order: each piece of the waveform falls only as 1/W, and only their cancellation gives W^-2 and hence a convergent high-frequency energy integral. Truncated post-Minkowskian series instead grow like W^n.
- Honest about the limitations of the self-force organising principle here, stating plainly that q rescales under collinear boosts and that the whole expansion is frame-dependent.

## ⚠️ Weaknesses

- The soft-theorem check fails at the omega log^2 omega order by an overall factor of two against Laddha-Saha-Sahoo-Sen, and this is left unresolved. Worse, the appendix presenting the matching reads as if agreement were obtained; only the conclusions admit the mismatch. A failed check at the first order beyond the previously-known ones is exactly where an error in the new all-orders waveform would show up.
- The headline finiteness result is much narrower than the abstract's framing. It covers one angular region (theta close to pi, collinear with the primary shock wave), at leading self-force order only, in a non-covariant frame; the complementary collinear region, the multi-Regge region and the angular integration are all deferred to future work. The long-standing logarithmic divergence of the total radiated energy is therefore not resolved, only 'partially' addressed, as the paper itself says.
- The propagator, advertised prominently, is not new: it reproduces Raj-Venugopalan (2024) and coincides with the independently published Bohnenblust et al. (JHEP 2026) result. The paper's own contribution there is a cleaner derivation and the observation that the earlier eikonal result is exact, which Bohnenblust et al. also established.
- The all-orders waveform is not actually resummed in closed form: it is expressed through a family of integrals S_{alpha1,alpha2} with no known closed-form solution, given only as parametric representations plus a soft series. The strong-field statement rests on a leading-order steepest-descent evaluation with no quantified control over subleading corrections.
- The all-self-force-order vanishing of the recoil operators is a conjecture supported by two orders, and it is doing structural work in the argument.
- Frame dependence undercuts the comparison to the literature: the radiated energy computed here differs by a boost from the centre-of-mass results of Ciafaloni et al. and Gruzinov, so the convergence statement cannot be directly set against the known divergence claims.
- The manuscript is visibly unpolished (repeated typographical errors such as 'perurbative', 'throught', 'fourty', 'secondarty', 'To obtaining'), and one cited comparison ('n8compton') is to unpublished forthcoming work.

## 🤔 Skeptic's Cross-Examination

The one genuinely new physical claim, that the angular energy spectrum converges at high frequency, rests on a cancellation extracted from a leading-order saddle point of a waveform whose own soft expansion fails a known consistency check at the first order the author could test beyond previously-established terms. If the omega log^2 omega factor of two signals an error in the interacting waveform rather than in the matching conventions, the delicate cancellation between the free and interacting pieces, which is what upgrades 1/W to 1/W^2, is exactly the kind of thing that would not survive. Add that the statement is frame-dependent, restricted to theta close to pi, and at leading self-force order, and the connection to the long-standing trans-Planckian radiated-energy divergence is suggestive rather than established.

## 🆕 Novelty in Context

The paper's self-positioning is mostly fair but the abstract oversells. Checking the citations: Bohnenblust, Eriksen, Hoogeveen, Jakobsen and Plefka (arXiv:2604.22009, JHEP 08 (2026) 064) already computed the exact-in-G off-shell graviton scattering off the Aichelburg-Sexl shock wave in worldline quantum field theory, explicitly framing it as the ingredient for 'future 1SF computations of observables such as the impulse and waveform'. That is precisely the gap this paper fills, and it does so independently and with a cleaner gauge, but the propagator itself is not new; Raj-Venugopalan's earlier eikonal result was already the same object. Blackstad, Raj and Venugopalan (arXiv:2608.27585) treat the same dilute-dense shock-wave radiation problem a month earlier, though order by order in the heavy source rather than resummed. What is genuinely new here is therefore narrower than 'gravitational radiation from shockwave scattering in the self-force EFT' suggests: the in-in extension of the self-force EFT, the recoil-operator-killing light-cone gauge, the all-orders 1SF waveform in momentum space, and the collinear-region energy-spectrum convergence. A skeptic will also note that the resummation pattern found (an exponentiating s-channel ladder producing the Weinberg phase) is the eikonal exponentiation known since 't Hooft and Amati-Ciafaloni-Veneziano, here recovered in a different formalism rather than discovered.

## 🎯 Relevance to Your Research

This sits at the amplitudes/hep-th end of the self-force programme rather than the EMRI-phenomenology end, but the formal content is transferable. The extension of the Cheung-Solon self-force EFT to the in-in path integral at order q^2 is the piece of general methodological value for anyone computing radiative (as opposed to conservative) 1SF observables in an effective-field-theory language, and the demonstration that a well-chosen gauge can kill the recoil operator is a structural lesson that may or may not have analogues on Schwarzschild and Kerr. The physical application, trans-Planckian massless-massless scattering, has no bearing on LISA-band EMRI waveforms. Read Section 2 (self-force EFT plus Schwinger-Keldysh, and the light-cone gauge choice) and Section 4.2 (the cancellation and the collinear energy spectrum); Section 3 can be skimmed since its result is already in the literature twice.

📖 **Where to start:** Section 2 (self-force EFT extended to Schwinger-Keldysh at O(q^2), the shock-wave background, and the light-cone gauge that kills the recoil operator); Section 4.2 (the W >> 1 cancellation and the collinear energy spectrum); the Conclusions, which are unusually candid about the frame dependence and the unresolved soft-theorem mismatch. Appendix on soft matching if you want to judge the factor-of-two issue yourself.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 4.5/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4.2/10)

## 🚧 Caveats

- The graviton propagator on the shock wave is a confirmation of two earlier results (Raj-Venugopalan 2024; Bohnenblust et al., JHEP 2026), not a new result.
- The soft-expansion cross-check disagrees with the established classical soft-graviton theorem at omega log^2 omega by a factor of two; this is unresolved, and the appendix is less forthcoming about it than the conclusions.
- The finiteness claim holds in one collinear angular region, at leading self-force order, in a frame-dependent setup. The total-radiated-energy divergence problem is not settled.
- The all-orders waveform is not in closed form; it is expressed via integrals with no known evaluation, and the strong-field falloff comes from a leading-order saddle point without error control.
- The vanishing of recoil operators beyond 2SF is conjectured, not proved.

---

🔗 [Back to the weekly digest](../2026-09-15)
